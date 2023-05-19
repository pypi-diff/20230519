# Comparing `tmp/mse_lib_sgx-2.0a4.tar.gz` & `tmp/mse_lib_sgx-2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_sgx-2.0a4.tar", last modified: Fri May 19 14:07:54 2023, max compression
+gzip compressed data, was "mse_lib_sgx-2.0a5.tar", last modified: Fri May 19 14:36:54 2023, max compression
```

## Comparing `mse_lib_sgx-2.0a4.tar` & `mse_lib_sgx-2.0a5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.894920 mse_lib_sgx-2.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/import_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 14:07:54.000000 mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:07:54.898920 mse_lib_sgx-2.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-19 14:07:06.000000 mse_lib_sgx-2.0a4/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:36:54.678262 mse_lib_sgx-2.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 14:36:54.678262 mse_lib_sgx-2.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 14:36:54.682262 mse_lib_sgx-2.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:36:54.678262 mse_lib_sgx-2.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:36:54.678262 mse_lib_sgx-2.0a5/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/import_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:36:54.678262 mse_lib_sgx-2.0a5/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:36:54.678262 mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-19 14:36:54.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 14:36:54.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:36:54.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 14:36:54.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:36:54.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 14:36:54.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 14:36:54.000000 mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:36:54.678262 mse_lib_sgx-2.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-19 14:36:10.000000 mse_lib_sgx-2.0a5/tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-2.0a4/PKG-INFO` & `mse_lib_sgx-2.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_lib_sgx
-Version: 2.0a4
+Version: 2.0a5
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a4/README.md` & `mse_lib_sgx-2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/setup.py` & `mse_lib_sgx-2.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx/base64url.py` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx/base64url.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx/certificate.py` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx/certificate.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx/cli.py` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx/cli.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx/globs.py` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx/globs.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx/http_server.py` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx/http_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,24 +112,29 @@
     httpd.socket = ctx.wrap_socket(httpd.socket, server_side=True)
 
     if timeout is not None:
         timer = threading.Timer(interval=timeout, function=kill)
         timer.start()
 
         threading.Thread(target=kill_event, args=(httpd, timer)).start()
+    else:
+        threading.Thread(target=kill_event, args=(httpd, None)).start()
 
     httpd.serve_forever()
 
 
-def kill_event(httpd: HTTPServer, timer: threading.Timer):
+def kill_event(httpd: HTTPServer, timer: Optional[threading.Timer]):
     """Kill HTTP server in a thread if `EXIT_EVENT` is set."""
     while True:
         if globs.EXIT_EVENT.is_set():
             logging.info("Stopping the configuration server...")
-            timer.cancel()
+
+            if timer:
+                timer.cancel()
+
             httpd.shutdown()
             return
 
         time.sleep(1)
 
 
 def kill():
```

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx/import_hook.py` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx/import_hook.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/key.py` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx/sgx/key.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx/sgx/quote.py` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx/sgx/quote.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 2.0a4
+Version: 2.0a5
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a4/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse_lib_sgx-2.0a5/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/tests/test_cert_utils.py` & `mse_lib_sgx-2.0a5/tests/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a4/tests/test_conf_server.py` & `mse_lib_sgx-2.0a5/tests/test_conf_server.py`

 * *Files identical despite different names*

