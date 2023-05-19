# Comparing `tmp/mse_lib_sgx-2.0a2.tar.gz` & `tmp/mse_lib_sgx-2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_sgx-2.0a2.tar", last modified: Wed May 17 14:25:19 2023, max compression
+gzip compressed data, was "mse_lib_sgx-2.0a3.tar", last modified: Fri May 19 12:08:23 2023, max compression
```

## Comparing `mse_lib_sgx-2.0a2.tar` & `mse_lib_sgx-2.0a3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/import_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 14:25:19.000000 mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:25:19.207008 mse_lib_sgx-2.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-17 14:24:31.000000 mse_lib_sgx-2.0a2/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 12:08:23.008125 mse_lib_sgx-2.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/import_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 12:08:23.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 12:08:22.000000 mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:08:23.004125 mse_lib_sgx-2.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-19 12:07:32.000000 mse_lib_sgx-2.0a3/tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-2.0a2/PKG-INFO` & `mse_lib_sgx-2.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_lib_sgx
-Version: 2.0a2
+Version: 2.0a3
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a2/README.md` & `mse_lib_sgx-2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/setup.py` & `mse_lib_sgx-2.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx/base64url.py` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx/base64url.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx/certificate.py` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx/certificate.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx/cli.py` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         # - the uuid of the app (see as an uniq token allowing to query the API)
         # - the key to decrypt the code
         # - (optional) the SSL private key if AppConnection.OWNER_CERTFICIATE
         serve_sgx_secrets(
             hostname=args.host,
             port=args.port,
             certificate=cert,
-            uuid=args.uuid,
+            app_id=args.id,
             need_ssl_private_key=ssl_app_mode == SslAppMode.CUSTOM_CERTIFICATE,
             timeout=globs.TIMEOUT,
         )
 
         if not globs.PLAINCODE and globs.CODE_SECRET_KEY is None:
             raise SecurityError("Code secret key not provided")
```

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx/globs.py` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx/globs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 
 CODE_SECRET_KEY: Optional[bytes] = None
 
 EXIT_EVENT: threading.Event = threading.Event()
 
-UUID: Optional[str] = None
+ID: Optional[str] = None
 
 SSL_PRIVATE_KEY: Optional[str] = None
 NEED_SSL_PRIVATE_KEY: bool = False
 PLAINCODE: bool = False
 
 HOME_DIR_PATH: Path = Path(os.getenv("HOME", "/root"))
 KEY_DIR_PATH: Path = Path(os.getenv("KEY_PATH", "/key"))
```

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx/http_server.py` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx/http_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,17 @@
         logging.info("Processing POST query...")
         content_length: int = int(self.headers.get("Content-Length", 0))
         body = self.rfile.read(content_length)
 
         # body is a json withthese fields:
         # - uuid
         # - (optional) ssl_private_key
-        # - code_sealed_key
+        # - (optional) app_secrets
+        # - (optional) app_sealed_secrets
+        # - code_secret_key
         try:
             data = json.loads(body.decode("utf8"))
 
             if app_secrets := data.get("app_secrets"):
                 globs.SECRETS_PATH.parent.mkdir(parents=True, exist_ok=True)
                 globs.SECRETS_PATH.write_bytes(json.dumps(app_secrets).encode("utf-8"))
 
@@ -57,15 +59,15 @@
                             )
                         )
                     ).encode("utf-8")
                 )
 
             # Do not process queries which have not the `uuid` data field
             # Probably a robot
-            if data["uuid"] != globs.UUID:
+            if data["uuid"] != globs.ID:
                 self.send_response_only(401)
                 self.end_headers()
                 return
 
             if globs.NEED_SSL_PRIVATE_KEY:
                 globs.SSL_PRIVATE_KEY = data["ssl_private_key"]
 
@@ -86,21 +88,21 @@
         globs.EXIT_EVENT.set()
 
 
 def serve(
     hostname: str,
     port: int,
     certificate: Certificate,
-    uuid: str,
+    app_id: str,
     need_ssl_private_key: bool,
     timeout: Optional[int],
 ):
     """Serve simple SGX HTTP server."""
     globs.NEED_SSL_PRIVATE_KEY = need_ssl_private_key
-    globs.UUID = uuid
+    globs.ID = app_id
 
     httpd = HTTPServer((hostname, port), SGXHTTPRequestHandler)
 
     ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
     ctx.load_cert_chain(
         certfile=str(certificate.cert_path.resolve()),
         keyfile=str(certificate.key_path.resolve()),
```

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx/import_hook.py` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx/import_hook.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/key.py` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/key.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx/sgx/quote.py` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx/sgx/quote.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 2.0a2
+Version: 2.0a3
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a2/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse_lib_sgx-2.0a3/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/tests/test_cert_utils.py` & `mse_lib_sgx-2.0a3/tests/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a2/tests/test_conf_server.py` & `mse_lib_sgx-2.0a3/tests/test_conf_server.py`

 * *Files identical despite different names*

