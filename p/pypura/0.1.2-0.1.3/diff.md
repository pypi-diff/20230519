# Comparing `tmp/pypura-0.1.2.tar.gz` & `tmp/pypura-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypura-0.1.2.tar", max compression
+gzip compressed data, was "pypura-0.1.3.tar", max compression
```

## Comparing `pypura-0.1.2.tar` & `pypura-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-05-16 21:33:19.526089 pypura-0.1.2/LICENSE
--rw-r--r--   0        0        0       76 2023-05-16 18:55:48.661213 pypura-0.1.2/README.md
--rw-r--r--   0        0        0      631 2023-05-18 02:11:16.605364 pypura-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      251 2023-05-18 02:11:25.600975 pypura-0.1.2/pypura/__init__.py
--rw-r--r--   0        0        0     1447 2023-05-18 02:10:28.055646 pypura-0.1.2/pypura/const.py
--rw-r--r--   0        0        0      200 2023-05-16 22:52:50.516386 pypura-0.1.2/pypura/exceptions.py
--rw-r--r--   0        0        0     5620 2023-05-17 19:32:48.277789 pypura-0.1.2/pypura/pura.py
--rw-r--r--   0        0        0        0 2023-05-17 06:46:31.898658 pypura-0.1.2/pypura/py.typed
--rw-r--r--   0        0        0      717 2023-05-17 19:03:43.405261 pypura-0.1.2/pypura/utils.py
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 pypura-0.1.2/setup.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 pypura-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-19 17:38:35.855128 pypura-0.1.3/LICENSE
+-rw-r--r--   0        0        0       76 2023-05-19 17:38:35.855128 pypura-0.1.3/README.md
+-rw-r--r--   0        0        0      747 2023-05-19 17:38:53.195255 pypura-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-05-19 17:38:53.195255 pypura-0.1.3/pypura/__init__.py
+-rw-r--r--   0        0        0     1447 2023-05-19 17:38:35.855128 pypura-0.1.3/pypura/const.py
+-rw-r--r--   0        0        0      200 2023-05-19 17:38:35.855128 pypura-0.1.3/pypura/exceptions.py
+-rw-r--r--   0        0        0     6533 2023-05-19 17:38:35.855128 pypura-0.1.3/pypura/pura.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:38:35.855128 pypura-0.1.3/pypura/py.typed
+-rw-r--r--   0        0        0      717 2023-05-19 17:38:35.855128 pypura-0.1.3/pypura/utils.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 pypura-0.1.3/PKG-INFO
```

### Comparing `pypura-0.1.2/LICENSE` & `pypura-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypura-0.1.2/pyproject.toml` & `pypura-0.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypura"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python package for interacting with Pura smart fragrance diffuser"
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["pypura/py.typed"]
 
 [tool.poetry.dependencies]
@@ -19,10 +19,15 @@
 mypy = "^1.3.0"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.4"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 tox = "^4.5.1"
 
+[tool.poetry-dynamic-versioning]
+enable = true
+vcs = "git"
+style = "semver"
+
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `pypura-0.1.2/pypura/const.py` & `pypura-0.1.3/pypura/const.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.2/pypura/pura.py` & `pypura-0.1.3/pypura/pura.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Pura account."""
 from __future__ import annotations
 
 import logging
+from datetime import datetime, timedelta
 from typing import Any, Final
 from urllib.parse import urljoin
 
 import requests
 from botocore.exceptions import ClientError
 from pycognito import Cognito
 from pycognito.utils import RequestsSrpAuth, TokenType
 
 from .const import CLIENT_ID, USER_POOL_ID
-from .exceptions import PuraAuthenticationError
+from .exceptions import PuraApiException, PuraAuthenticationError
 from .utils import decode
 
 _LOGGER = logging.getLogger(__name__)
 
 BASE_URL: Final = "https://trypura.io/mobile/api/"
 
+TIMER_DURATION_DEFAULT = timedelta(hours=4)
+
 
 class Pura:
     """Pura account."""
 
     _user: Cognito | None = None
     _auth: RequestsSrpAuth | None = None
 
@@ -146,14 +149,36 @@
             "brightness": brightness,
             "color": color,
             "controller": controller,
         }
         resp = self.__post(f"devices/{device_id}/nightlight", json=json)
         return resp.get("success") is True
 
+    def set_timer(
+        self,
+        device_id: str,
+        *,
+        bay: int,
+        intensity: int,
+        start: datetime | int = datetime.now(),
+        end: datetime | timedelta | int = TIMER_DURATION_DEFAULT,
+    ) -> bool:
+        """Set timer."""
+        if isinstance(start, datetime):
+            start = int(start.timestamp())
+        if isinstance(end, datetime):
+            end = int(end.timestamp())
+        elif isinstance(end, timedelta):
+            end = start + end.seconds
+        if end <= start:
+            raise PuraApiException("Timer 'end' time must be greater than 'start' time")
+        json = {"bay": bay, "intensity": intensity, "start": start, "end": end}
+        resp = self.__post(f"devices/{device_id}/timer", json=json)
+        return resp.get("success") is True
+
     def stop_all(self, device_id: str) -> bool:
         """Stop all."""
         resp = self.__post(f"devices/{device_id}/stop-all")
         return resp.get("success") is True
 
     def __request(self, method: str, url: str, **kwargs: Any) -> Any:
         """Make a request."""
```

### Comparing `pypura-0.1.2/pypura/utils.py` & `pypura-0.1.3/pypura/utils.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.2/PKG-INFO` & `pypura-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypura
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for interacting with Pura smart fragrance diffuser
 License: MIT
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

