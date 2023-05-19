# Comparing `tmp/tuneflow-devkit-py-0.8.1.tar.gz` & `tmp/tuneflow-devkit-py-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-devkit-py-0.8.1.tar", last modified: Wed May 10 04:54:39 2023, max compression
+gzip compressed data, was "tuneflow-devkit-py-0.8.2.tar", last modified: Fri May 19 14:01:04 2023, max compression
```

## Comparing `tuneflow-devkit-py-0.8.1.tar` & `tuneflow-devkit-py-0.8.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.1/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.1/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-05-10 04:53:09.000000 tuneflow-devkit-py-0.8.1/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/
--rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     7078 2023-05-10 04:50:11.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/debugger.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8042 2023-05-10 04:50:11.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/translate_utils.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/validation_utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.1/test/test_runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.1/test/test_validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 14:01:04.356059 tuneflow-devkit-py-0.8.2/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.2/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-19 14:01:04.356059 tuneflow-devkit-py-0.8.2/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.2/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-05-19 03:07:55.000000 tuneflow-devkit-py-0.8.2/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-19 14:01:04.356059 tuneflow-devkit-py-0.8.2/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 14:01:04.356059 tuneflow-devkit-py-0.8.2/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 14:01:04.356059 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     7078 2023-05-10 04:50:11.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/debugger.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8263 2023-05-19 02:57:51.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/translate_utils.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 14:01:04.356059 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-19 14:01:04.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-05-19 14:01:04.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-19 14:01:04.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-05-19 14:01:04.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-05-19 14:01:04.000000 tuneflow-devkit-py-0.8.2/src/tuneflow_devkit_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 14:01:04.356059 tuneflow-devkit-py-0.8.2/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.2/test/test_runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.2/test/test_validation_utils.py
```

### Comparing `tuneflow-devkit-py-0.8.1/LICENSE` & `tuneflow-devkit-py-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.1/PKG-INFO` & `tuneflow-devkit-py-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.1
+Version: 0.8.2
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.1/README.md` & `tuneflow-devkit-py-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.1/pyproject.toml` & `tuneflow-devkit-py-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-devkit-py"
-version = "0.8.1"
+version = "0.8.2"
 authors = [{ name = "Andantei", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     "AI",
     "music",
```

### Comparing `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/debugger.py` & `tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/debugger.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/runner.py` & `tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,15 @@
             allow_origins=cors_allowed_origins,
             allow_credentials=True,
             allow_methods=["*"],
             allow_headers=["*"],
         )
 
         async_config = config["async"] if config and "async" in config else None
+        exception_handler = config["exception"]["handler"] if config and "exception" in config and "handler" in config["exception"] else None
 
         @app.middleware("http")
         async def add_vary_origin_header(request: Request, call_next):
             response = await call_next(request)
             response.headers["Vary"] = 'Origin'
             return response
 
@@ -93,14 +94,16 @@
                 }
 
         def run_plugin_task(plugin_class: Type[TuneflowPlugin], song, params):
             try:
                 plugin_class.run(song, params)
             except Exception as e:
                 print(traceback.format_exc())
+                if exception_handler:
+                    exception_handler(e)
                 return {
                     "status": "ERROR"
                 }
             return {
                 "status": "OK",
                 "song": song.serialize_to_bytestring()
             }
```

### Comparing `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/translate_utils.py` & `tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/translate_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/validation_utils.py` & `tuneflow-devkit-py-0.8.2/src/tuneflow_devkit/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/PKG-INFO` & `tuneflow-devkit-py-0.8.2/src/tuneflow_devkit_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.1
+Version: 0.8.2
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.1/test/test_runner.py` & `tuneflow-devkit-py-0.8.2/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.1/test/test_validation_utils.py` & `tuneflow-devkit-py-0.8.2/test/test_validation_utils.py`

 * *Files identical despite different names*

