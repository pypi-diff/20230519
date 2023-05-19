# Comparing `tmp/nsdotpy-1.3.0.tar.gz` & `tmp/nsdotpy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.3.0.tar", max compression
+gzip compressed data, was "nsdotpy-1.3.1.tar", max compression
```

## Comparing `nsdotpy-1.3.0.tar` & `nsdotpy-1.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-19 00:19:03.509539 nsdotpy-1.3.0/LICENSE.md
--rw-r--r--   0        0        0     2440 2023-05-19 00:19:03.509539 nsdotpy-1.3.0/README.md
--rw-r--r--   0        0        0      790 2023-05-19 00:19:03.521539 nsdotpy-1.3.0/nsdotpy/__init__.py
--rw-r--r--   0        0        0    44794 2023-05-19 00:19:03.521539 nsdotpy-1.3.0/nsdotpy/session.py
--rw-r--r--   0        0        0     4963 2023-05-19 00:19:03.521539 nsdotpy-1.3.0/nsdotpy/valid.py
--rw-r--r--   0        0        0      719 2023-05-19 00:19:03.521539 nsdotpy-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-19 00:22:40.519294 nsdotpy-1.3.1/LICENSE.md
+-rw-r--r--   0        0        0     2440 2023-05-19 00:22:40.519294 nsdotpy-1.3.1/README.md
+-rw-r--r--   0        0        0      790 2023-05-19 00:22:40.535294 nsdotpy-1.3.1/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    44770 2023-05-19 00:22:40.535294 nsdotpy-1.3.1/nsdotpy/session.py
+-rw-r--r--   0        0        0     4963 2023-05-19 00:22:40.535294 nsdotpy-1.3.1/nsdotpy/valid.py
+-rw-r--r--   0        0        0      719 2023-05-19 00:22:40.535294 nsdotpy-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.1/PKG-INFO
```

### Comparing `nsdotpy-1.3.0/LICENSE.md` & `nsdotpy-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.0/README.md` & `nsdotpy-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.0/nsdotpy/__init__.py` & `nsdotpy-1.3.1/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.0/nsdotpy/session.py` & `nsdotpy-1.3.1/nsdotpy/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.3.0"
+        self.VERSION = "1.3.1"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -639,26 +639,26 @@
             nations (list[str]): List of nations to add
 
         Returns:
             bool: Whether it was successful or not
         """
 
         self.logger.info(f"Adding {nations} to dossier on {self.nation}")
-        url = "https://www.nationstates.net/template-overall=none/page=dossier"
+        url = "https://www.nationstates.net/dossier.cgi"
         data = {
             "currentnation": canonicalize(self.nation),
             "action_append": "Upload Nation Dossier File",
         }
         files = {
             "file": ("dossier.txt", "\n".join(nations), "text/plain"),
         }
         response = self.request(url, data, files=files)
 
         self._refresh_auth_values()
-        return "appended=1" in response.headers["location"]
+        return "appended=" in response.headers["location"]
 
     def wa_vote(self, council: str, vote: str) -> bool:
         """Votes on the current WA resolution.
 
         Args:
             council (str): Must be "ga" for general assembly, "sc" for security council.
             vote (str): Must be "for" or "against".
```

### Comparing `nsdotpy-1.3.0/nsdotpy/valid.py` & `nsdotpy-1.3.1/nsdotpy/valid.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.0/pyproject.toml` & `nsdotpy-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.3.0"
+version = "1.3.1"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.3.0/PKG-INFO` & `nsdotpy-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

