# Comparing `tmp/flet_pyodide-0.8.0.dev1441.tar.gz` & `tmp/flet_pyodide-0.8.0.dev1443.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.8.0.dev1441.tar", max compression
+gzip compressed data, was "flet_pyodide-0.8.0.dev1443.tar", max compression
```

## Comparing `flet_pyodide-0.8.0.dev1441.tar` & `flet_pyodide-0.8.0.dev1443.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2023-05-18 17:42:33.355650 flet_pyodide-0.8.0.dev1441/README.md
--rw-r--r--   0        0        0      644 2023-05-18 17:43:09.872013 flet_pyodide-0.8.0.dev1441/pyproject.toml
--rw-r--r--   0        0        0      144 2023-05-18 17:42:33.355650 flet_pyodide-0.8.0.dev1441/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2023-05-18 17:42:33.355650 flet_pyodide-0.8.0.dev1441/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2406 2023-05-18 17:42:33.355650 flet_pyodide-0.8.0.dev1441/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-05-18 17:42:33.355650 flet_pyodide-0.8.0.dev1441/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-05-18 17:42:33.355650 flet_pyodide-0.8.0.dev1441/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3851 2023-05-18 17:42:33.355650 flet_pyodide-0.8.0.dev1441/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2023-05-18 17:43:09.260007 flet_pyodide-0.8.0.dev1441/src/flet/version.py
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.8.0.dev1441/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-05-18 23:59:12.910078 flet_pyodide-0.8.0.dev1443/README.md
+-rw-r--r--   0        0        0      644 2023-05-18 23:59:46.546532 flet_pyodide-0.8.0.dev1443/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-05-18 23:59:12.910078 flet_pyodide-0.8.0.dev1443/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-18 23:59:12.910078 flet_pyodide-0.8.0.dev1443/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2501 2023-05-18 23:59:12.910078 flet_pyodide-0.8.0.dev1443/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-05-18 23:59:12.910078 flet_pyodide-0.8.0.dev1443/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-05-18 23:59:12.910078 flet_pyodide-0.8.0.dev1443/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3851 2023-05-18 23:59:12.910078 flet_pyodide-0.8.0.dev1443/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-05-18 23:59:46.010557 flet_pyodide-0.8.0.dev1443/src/flet/version.py
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.8.0.dev1443/PKG-INFO
```

### Comparing `flet_pyodide-0.8.0.dev1441/README.md` & `flet_pyodide-0.8.0.dev1443/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.8.0.dev1441/pyproject.toml` & `flet_pyodide-0.8.0.dev1443/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.8.0.dev1441"
+version = "0.8.0.dev1443"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.8.0.dev1441"
+flet-core = "0.8.0.dev1443"
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `flet_pyodide-0.8.0.dev1441/src/flet/flet.py` & `flet_pyodide-0.8.0.dev1443/src/flet/flet.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,40 +26,43 @@
     name="",
     host=None,
     port=0,
     view=None,
     assets_dir=None,
     upload_dir=None,
     web_renderer=None,
+    use_color_emoji=False,
     route_url_strategy=None,
     auth_token=None,
 ):
     app_async(
         target=target,
         name=name,
         host=host,
         port=port,
         view=view,
         assets_dir=assets_dir,
         upload_dir=upload_dir,
         web_renderer=web_renderer,
+        use_color_emoji=use_color_emoji,
         route_url_strategy=route_url_strategy,
         auth_token=auth_token,
     )
 
 
 def app_async(
     target,
     name="",
     host=None,
     port=0,
     view=None,
     assets_dir=None,
     upload_dir=None,
     web_renderer=None,
+    use_color_emoji=False,
     route_url_strategy=None,
     auth_token=None,
 ):
     async def on_event(e):
         if e.sessionID in conn.sessions:
             await conn.sessions[e.sessionID].on_event_async(
                 Event(e.eventTarget, e.eventName, e.eventData)
```

### Comparing `flet_pyodide-0.8.0.dev1441/src/flet/pyodide_connection.py` & `flet_pyodide-0.8.0.dev1443/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.8.0.dev1441/PKG-INFO` & `flet_pyodide-0.8.0.dev1443/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.8.0.dev1441
+Version: 0.8.0.dev1443
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.8.0.dev1441)
+Requires-Dist: flet-core (==0.8.0.dev1443)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

