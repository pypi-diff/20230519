# Comparing `tmp/pytest_hot_reloading-0.1.0a4.tar.gz` & `tmp/pytest_hot_reloading-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hot_reloading-0.1.0a4.tar", max compression
+gzip compressed data, was "pytest_hot_reloading-0.1.0a5.tar", max compression
```

## Comparing `pytest_hot_reloading-0.1.0a4.tar` & `pytest_hot_reloading-0.1.0a5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-05-18 21:22:49.726174 pytest_hot_reloading-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     2442 2023-05-18 21:22:49.726174 pytest_hot_reloading-0.1.0a4/README.md
--rw-r--r--   0        0        0      676 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/__init__.py
--rw-r--r--   0        0        0     1969 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/client.py
--rw-r--r--   0        0        0     7638 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/daemon.py
--rw-r--r--   0        0        0     8221 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/plugin.py
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     2442 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/README.md
+-rw-r--r--   0        0        0      676 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/__init__.py
+-rw-r--r--   0        0        0     1969 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/client.py
+-rw-r--r--   0        0        0     9556 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/daemon.py
+-rw-r--r--   0        0        0     8221 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/plugin.py
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a5/PKG-INFO
```

### Comparing `pytest_hot_reloading-0.1.0a4/LICENSE` & `pytest_hot_reloading-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a4/README.md` & `pytest_hot_reloading-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a4/pyproject.toml` & `pytest_hot_reloading-0.1.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 98
 
 [tool.black]
 line-length = 98
 
 [tool.poetry]
 name = "pytest-hot-reloading"
-version = "0.1.0-alpha.4"
+version = "0.1.0-alpha.5"
 description = ""
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 packages = [{ include = "pytest_hot_reloading" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/client.py` & `pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/client.py`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/daemon.py` & `pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/daemon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import os
 import re
 import socket
 import subprocess
 import sys
 import time
+from typing import Counter
 from xmlrpc.server import SimpleXMLRPCServer
 
 import pytest
 from cachetools import TTLCache
 
 
 class PytestDaemon:
@@ -152,21 +153,64 @@
         return re.sub(r"\x1b(\[.*?[@-~]|\].*?(\x07|\x1b\\))", "", s, flags=re.MULTILINE)
 
     def _workaround_library_issues(self, args: list[str]) -> None:
         # load modules that workaround library issues, as needed
         pass
 
 
-session_cache = TTLCache(16, 500)
+session_item_cache = TTLCache(16, 500)
+# hack: keeping a session cache since pytest has session references
+#       littered everywhere on objects
+prior_sessions = set()
+
+
+def _manage_prior_session_garbage(session: pytest.Session) -> None:
+    """
+    Pytest creates a bunch of objects and nodes and assigns the session
+    to them. This creates a lot of dangling references to sessions that
+    can come up later due to reuse. To work around this, all prior
+    sessions have their dicts updated to point to the latest session.
+
+    To avoid accumulating too many sessions and taking up memory as well
+    as runtime, this cleans out all the sessions that appear to be redundant.
+
+    This isn't quite perfect but should maybe be enough. There's likely some
+    corner cases where the session with the fewest references doesn't meet the
+    count requirement. There may also be cases where the smallest session
+    has something important on it and we don't want to clean it up, but it
+    gets cleaned up anyways.
+
+    The use case that drew attention to this problem was an autouse session
+    fixture. The fixture's request object was referencing the session that
+    used the fixture, which at some point in the flow creates a problem
+    because that old session is not properly set up anymore.
+    """
+    ref_counts = {
+        prior_session: sys.getrefcount(prior_session) for prior_session in prior_sessions
+    }
+    counts = Counter(ref_counts.values())
+    min_count = min(counts.keys()) if ref_counts else 0
+
+    for prior_session in list(prior_sessions):
+        if (
+            len(prior_sessions) > 5
+            and counts[min_count] > 3
+            and ref_counts[prior_session] <= min_count
+        ):
+            prior_sessions.remove(prior_session)
+        else:
+            prior_session.__dict__ = session.__dict__
 
 
 def _pytest_main(config: pytest.Config, session: pytest.Session):
     """
     A monkey patched version of _pytest._main that caches test collection
     """
+    _manage_prior_session_garbage(session)
+
     import _pytest.capture
 
     _pytest.capture.CaptureManager.stop_global_capturing = lambda self: None
     start_global_capturing = _pytest.capture.CaptureManager.start_global_capturing
     resume_global_capture = _pytest.capture.CaptureManager.resume_global_capture
 
     def start_global_capture_if_needed(self: _pytest.capture.CaptureManager):
@@ -199,32 +243,33 @@
                     item_copy.__dict__[k] = best_effort_copy(v, depth_remaining - 1)
         return item_copy
 
     # here config.args becomes basically the tests to run. Other arguments are omitted
     # not 100% sure this is always the case
     session_key = tuple(config.args)
     try:
-        items = session_cache[session_key]
+        items = session_item_cache[session_key]
     except KeyError:
         # not in the cache, do test collection
         start = time.time()
         config.hook.pytest_collection(session=session)
         print(f"Pytest Daemon: Collection took {(time.time() - start):0.3f} seconds")
-        session_cache[session_key] = tuple(best_effort_copy(x) for x in session.items)
+        session_item_cache[session_key] = tuple(best_effort_copy(x) for x in session.items)
     else:
         print("Pytest Daemon: Using cached collection")
         # Assign the prior test items (tests to run) and config to the current session
         session.items = items
         session.config = config
         for i in items:
             # Items have references to the config and the session
             i.config = config
             i.session = session
             if i._request:
                 i._request._pyfuncitem = i
     config.hook.pytest_runtestloop(session=session)
+    prior_sessions.add(session)
 
     if session.testsfailed:
         return pytest.ExitCode.TESTS_FAILED
     elif session.testscollected == 0:
         return pytest.ExitCode.NO_TESTS_COLLECTED
     return None
```

### Comparing `pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/plugin.py` & `pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a4/PKG-INFO` & `pytest_hot_reloading-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-hot-reloading
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: 
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

