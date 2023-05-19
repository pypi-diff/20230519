# Comparing `tmp/reactpy_jupyter-0.9.4.tar.gz` & `tmp/reactpy_jupyter-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_jupyter-0.9.4.tar", last modified: Fri May 19 02:27:48 2023, max compression
+gzip compressed data, was "reactpy_jupyter-0.9.5.tar", last modified: Fri May 19 02:51:53 2023, max compression
```

## Comparing `reactpy_jupyter-0.9.4.tar` & `reactpy_jupyter-0.9.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:27:48.854013 reactpy_jupyter-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-19 02:27:48.854013 reactpy_jupyter-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:27:48.846013 reactpy_jupyter-0.9.4/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:27:48.850013 reactpy_jupyter-0.9.4/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/jupyter-config/jupyter_server_config.d/reactpy-jupyter.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:27:48.854013 reactpy_jupyter-0.9.4/reactpy_jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/reactpy_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/reactpy_jupyter/import_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/reactpy_jupyter/jupyter_server_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/reactpy_jupyter/layout_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/reactpy_jupyter/monkey_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:27:48.854013 reactpy_jupyter-0.9.4/reactpy_jupyter/static/
--rw-r--r--   0 runner    (1001) docker     (123)    55659 2023-05-19 02:27:48.000000 reactpy_jupyter-0.9.4/reactpy_jupyter/static/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/reactpy_jupyter/widget_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:27:48.854013 reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-19 02:27:48.000000 reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-19 02:27:48.000000 reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:27:48.000000 reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:27:40.000000 reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 02:27:48.000000 reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 02:27:48.000000 reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-19 02:27:48.854013 reactpy_jupyter-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-19 02:27:21.000000 reactpy_jupyter-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:51:53.687016 reactpy_jupyter-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-19 02:51:53.687016 reactpy_jupyter-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:51:53.675016 reactpy_jupyter-0.9.5/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:51:53.683016 reactpy_jupyter-0.9.5/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/jupyter-config/jupyter_server_config.d/reactpy-jupyter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:51:53.683016 reactpy_jupyter-0.9.5/reactpy_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/reactpy_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/reactpy_jupyter/import_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/reactpy_jupyter/jupyter_server_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/reactpy_jupyter/layout_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/reactpy_jupyter/monkey_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:51:53.687016 reactpy_jupyter-0.9.5/reactpy_jupyter/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    55659 2023-05-19 02:51:52.000000 reactpy_jupyter-0.9.5/reactpy_jupyter/static/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/reactpy_jupyter/widget_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:51:53.687016 reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-19 02:51:53.000000 reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-19 02:51:53.000000 reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:51:53.000000 reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:51:34.000000 reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 02:51:53.000000 reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 02:51:53.000000 reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/reactpy_jupyter.pth
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-19 02:51:53.687016 reactpy_jupyter-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-19 02:51:05.000000 reactpy_jupyter-0.9.5/setup.py
```

### Comparing `reactpy_jupyter-0.9.4/LICENSE` & `reactpy_jupyter-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/PKG-INFO` & `reactpy_jupyter-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy_jupyter
-Version: 0.9.4
+Version: 0.9.5
 Summary: It's React, but in Python
 Home-page: https://github.com/reactive-python/reactpy
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
```

### Comparing `reactpy_jupyter-0.9.4/README.md` & `reactpy_jupyter-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter/__init__.py` & `reactpy_jupyter-0.9.5/reactpy_jupyter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from . import jupyter_server_extension
 from .import_resources import setup_import_resources
 from .layout_widget import run, set_import_source_base_url, to_widget
 from .monkey_patch import execute_patch
 from .widget_component import from_widget
 
-__version__ = "0.9.4"  # DO NOT MODIFY
+__version__ = "0.9.5"  # DO NOT MODIFY
 
 __all__ = (
     "from_widget",
     "load_ipython_extension",
     "unload_ipython_extension",
     "to_widget",
     "run",
```

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter/import_resources.py` & `reactpy_jupyter-0.9.5/reactpy_jupyter/import_resources.py`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter/jupyter_server_extension.py` & `reactpy_jupyter-0.9.5/reactpy_jupyter/jupyter_server_extension.py`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter/layout_widget.py` & `reactpy_jupyter-0.9.5/reactpy_jupyter/layout_widget.py`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter/monkey_patch.py` & `reactpy_jupyter-0.9.5/reactpy_jupyter/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter/static/index.js` & `reactpy_jupyter-0.9.5/reactpy_jupyter/static/index.js`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter/widget_component.py` & `reactpy_jupyter-0.9.5/reactpy_jupyter/widget_component.py`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/PKG-INFO` & `reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-jupyter
-Version: 0.9.4
+Version: 0.9.5
 Summary: It's React, but in Python
 Home-page: https://github.com/reactive-python/reactpy
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
```

### Comparing `reactpy_jupyter-0.9.4/reactpy_jupyter.egg-info/SOURCES.txt` & `reactpy_jupyter-0.9.5/reactpy_jupyter.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+reactpy_jupyter.pth
 setup.cfg
 setup.py
 jupyter-config/jupyter_server_config.d/reactpy-jupyter.json
 reactpy_jupyter/__init__.py
 reactpy_jupyter/import_resources.py
 reactpy_jupyter/jupyter_server_extension.py
 reactpy_jupyter/layout_widget.py
```

### Comparing `reactpy_jupyter-0.9.4/setup.cfg` & `reactpy_jupyter-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `reactpy_jupyter-0.9.4/setup.py` & `reactpy_jupyter-0.9.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,17 +158,26 @@
         log.error(traceback.format_exc())
         raise
     else:
         log.info("Successfully installed Javascript")
 
 
 def build_with_pth_file(cmd: Command):
+    build_lib = getattr(cmd, "build_lib", None) or getattr(cmd, "dist_dir", None)
+    if build_lib is None:
+        raise ValueError("Cannot find build_lib or dist_dir")
+
     pth_filename = f"{NAME}.pth"
     source_pth_file = ROOT_DIR / pth_filename
-    cmd.copy_file(str(source_pth_file), pth_filename)
+
+    build_lib = Path(build_lib)
+    build_lib.mkdir(parents=True, exist_ok=True)
+    target_pth_file = build_lib / pth_filename
+
+    cmd.copy_file(str(source_pth_file), str(target_pth_file))
 
 
 def add_to_cmd(cls: Command, functions: list[Callable[[Command], None]]) -> Command:
     class Command(cls):
         def run(self):
             for f in functions:
                 f(self)
```

