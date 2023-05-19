# Comparing `tmp/flask-httpx-request-converted-to-flask-test-client-request-0.1.4.tar.gz` & `tmp/flask-httpx-request-converted-to-flask-test-client-request-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-httpx-request-converted-to-flask-test-client-request-0.1.4.tar", last modified: Tue May 16 12:07:04 2023, max compression
+gzip compressed data, was "flask-httpx-request-converted-to-flask-test-client-request-0.1.5.tar", last modified: Fri May 19 12:28:38 2023, max compression
```

## Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.4.tar` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request/
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-16 12:07:04.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-16 12:07:04.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:07:04.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 12:07:04.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:38.768113 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-19 12:28:25.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-19 12:28:38.768113 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-19 12:28:25.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:38.768113 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request/
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-19 12:28:25.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:28:38.768113 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-19 12:28:38.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-19 12:28:38.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:28:38.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 12:28:38.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-19 12:28:25.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:28:38.768113 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-19 12:28:25.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.5/setup.py
```

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/LICENSE` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/PKG-INFO` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-httpx-request-converted-to-flask-test-client-request
-Version: 0.1.4
+Version: 0.1.5
 Summary: Unittest Tool: This is a `flask.test_client_class` I wrote to making the libraries created by `openapi-python-client` work with `flask.test_client()`
 Home-page: https://github.com/dvaerum/flask-httpx-request-converted-to-flask-test-client-requests
 Author: Dennis Vestergaard Værum
 Author-email: convert_httpx_2_flask_test_client@varum.dk
 License: 0BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/README.md` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request/__init__.py` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 import json
 from typing import Any, Dict, TYPE_CHECKING
 from unittest.mock import patch
 
 from urllib3.util import parse_url
 from flask.testing import FlaskClient
@@ -12,21 +12,23 @@
 class ConvertHttpx2FlaskTestClient(FlaskClient):
     def __init__(self, *args: Any,
                  base_url: str = "http://localhost",
                  headers: Dict[str, str] = None,
                  cookies: Dict[str, Any] = None,
                  timeout: float = 10.0,
                  verify_ssl: bool = True,
+                 raise_on_unexpected_status: bool = False,
                  follow_redirects: bool = False,
                  **kwargs: Any):
         self.base_url = base_url
         self._headers = headers if headers else {}
         self._cookies = cookies if cookies else {}
         self._timeout = timeout
         self.verify_ssl = verify_ssl
+        self.raise_on_unexpected_status = raise_on_unexpected_status
         self.follow_redirects = follow_redirects
 
         self.mock_httpx_request = patch("httpx.Client.request",
                                         side_effect=self._convert_httpx_request_2_flask_client_open)
 
         super().__init__(*args, **kwargs)
```

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/PKG-INFO` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.5/flask_httpx_request_converted_to_flask_test_client_request.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-httpx-request-converted-to-flask-test-client-request
-Version: 0.1.4
+Version: 0.1.5
 Summary: Unittest Tool: This is a `flask.test_client_class` I wrote to making the libraries created by `openapi-python-client` work with `flask.test_client()`
 Home-page: https://github.com/dvaerum/flask-httpx-request-converted-to-flask-test-client-requests
 Author: Dennis Vestergaard Værum
 Author-email: convert_httpx_2_flask_test_client@varum.dk
 License: 0BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/setup.py` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.5/setup.py`

 * *Files identical despite different names*

