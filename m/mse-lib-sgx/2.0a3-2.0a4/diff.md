# Comparing `tmp/mse_lib_sgx-2.0a3.tar.gz` & `tmp/mse_lib_sgx-2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_sgx-2.0a3.tar", last modified: Fri May 19 12:08:23 2023, max compression
+gzip compressed data, was "mse_lib_sgx-2.0a4.tar", last modified: Fri May 19 14:07:54 2023, max compression
```

## Comparing `mse_lib_sgx-2.0a3.tar` & `mse_lib_sgx-2.0a4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 12:08:23.008125 mse_lib_sgx-2.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/import_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 12:08:23.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.894920 mse_lib_sgx-2.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/import_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-2.0a3/PKG-INFO` & `mse_lib_sgx-2.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_lib_sgx
-Version: 2.0a3
+Version: 2.0a4
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a3/README.md` & `mse_lib_sgx-2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/setup.py` & `mse_lib_sgx-2.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx/base64url.py` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx/base64url.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx/certificate.py` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx/certificate.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx/cli.py` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx/cli.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx/globs.py` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx/globs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """mse_lib_sgx.global module."""
 
 import os
 import threading
 from pathlib import Path
 from typing import Optional
+from uuid import UUID
 
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 
 CODE_SECRET_KEY: Optional[bytes] = None
 
 EXIT_EVENT: threading.Event = threading.Event()
 
-ID: Optional[str] = None
+ID: Optional[UUID] = None
 
 SSL_PRIVATE_KEY: Optional[str] = None
 NEED_SSL_PRIVATE_KEY: bool = False
 PLAINCODE: bool = False
 
 HOME_DIR_PATH: Path = Path(os.getenv("HOME", "/root"))
 KEY_DIR_PATH: Path = Path(os.getenv("KEY_PATH", "/key"))
```

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx/http_server.py` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx/http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import logging
 import ssl
 import threading
 import time
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from typing import Optional
+from uuid import UUID
 
 from mse_lib_crypto.seal_box import unseal
 
 from mse_lib_sgx import globs
 from mse_lib_sgx.base64url import base64url_decode
 from mse_lib_sgx.certificate import Certificate
 from mse_lib_sgx.error import CryptoError
@@ -59,15 +60,15 @@
                             )
                         )
                     ).encode("utf-8")
                 )
 
             # Do not process queries which have not the `uuid` data field
             # Probably a robot
-            if data["uuid"] != globs.ID:
+            if UUID(data["uuid"]) != globs.ID:
                 self.send_response_only(401)
                 self.end_headers()
                 return
 
             if globs.NEED_SSL_PRIVATE_KEY:
                 globs.SSL_PRIVATE_KEY = data["ssl_private_key"]
 
@@ -88,15 +89,15 @@
         globs.EXIT_EVENT.set()
 
 
 def serve(
     hostname: str,
     port: int,
     certificate: Certificate,
-    app_id: str,
+    app_id: UUID,
     need_ssl_private_key: bool,
     timeout: Optional[int],
 ):
     """Serve simple SGX HTTP server."""
     globs.NEED_SSL_PRIVATE_KEY = need_ssl_private_key
     globs.ID = app_id
```

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx/import_hook.py` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx/import_hook.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/key.py` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/key.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/quote.py` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/quote.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 2.0a3
+Version: 2.0a4
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/tests/test_cert_utils.py` & `mse_lib_sgx-2.0a4/tests/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a3/tests/test_conf_server.py` & `mse_lib_sgx-2.0a4/tests/test_conf_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     assert conf_server.is_alive()
 
     uuid = "64260dd9-57dd-47a1-8fd4-9992b4d12213"
     req = urllib.request.Request(
         url=f"https://{host}:{port}", headers={"Content-Type": "application/json"}
     )
     data: bytes = json.dumps(
-        {"uuid": uuid, "code_secret_key": code_secret_key.hex()}
+        {"uuid": str(uuid), "code_secret_key": code_secret_key.hex()}
     ).encode("utf-8")
     req.add_header("Content-Length", str(len(data)))
     ctx = ssl.create_default_context()
     ctx.check_hostname = False
     ctx.verify_mode = ssl.CERT_NONE
 
     with pytest.raises(urllib.error.HTTPError):
@@ -42,15 +42,15 @@
     conf_server,
 ):
     assert conf_server.is_alive()
 
     req = urllib.request.Request(
         url=f"https://{host}:{port}", headers={"Content-Type": "application/json"}
     )
-    data: bytes = json.dumps({"uuid": uuid}).encode("utf-8")
+    data: bytes = json.dumps({"uuid": str(uuid)}).encode("utf-8")
     req.add_header("Content-Length", str(len(data)))
     ctx = ssl.create_default_context()
     ctx.check_hostname = False
     ctx.verify_mode = ssl.CERT_NONE
 
     with pytest.raises(urllib.error.HTTPError):
         urllib.request.urlopen(req, data, context=ctx)
@@ -89,15 +89,15 @@
     uuid,
     conf_server,
 ):
     req = urllib.request.Request(
         url=f"https://{host}:{port}", headers={"Content-Type": "application/json"}
     )
     data: bytes = json.dumps(
-        {"uuid": uuid, "code_secret_key": code_secret_key.hex()}
+        {"uuid": str(uuid), "code_secret_key": code_secret_key.hex()}
     ).encode("utf-8")
     req.add_header("Content-Length", str(len(data)))
     ctx = ssl.create_default_context()
     ctx.check_hostname = False
     ctx.verify_mode = ssl.CERT_NONE
 
     assert conf_server.is_alive()
```

