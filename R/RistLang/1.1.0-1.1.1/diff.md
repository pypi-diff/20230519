# Comparing `tmp/RistLang-1.1.0.tar.gz` & `tmp/RistLang-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RistLang-1.1.0.tar", last modified: Mon Jan  2 04:44:16 2023, max compression
+gzip compressed data, was "RistLang-1.1.1.tar", last modified: Fri May 19 10:37:52 2023, max compression
```

## Comparing `RistLang-1.1.0.tar` & `RistLang-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 04:44:16.445976 RistLang-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-02 04:44:00.000000 RistLang-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-01-02 04:44:16.445976 RistLang-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-01-02 04:44:00.000000 RistLang-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 04:44:16.445976 RistLang-1.1.0/RistLang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-01-02 04:44:16.000000 RistLang-1.1.0/RistLang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-02 04:44:16.000000 RistLang-1.1.0/RistLang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 04:44:16.000000 RistLang-1.1.0/RistLang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-02 04:44:16.000000 RistLang-1.1.0/RistLang.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-02 04:44:16.000000 RistLang-1.1.0/RistLang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-02 04:44:16.000000 RistLang-1.1.0/RistLang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 04:44:16.445976 RistLang-1.1.0/ristpy/
--rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-01-02 04:44:00.000000 RistLang-1.1.0/ristpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-01-02 04:44:00.000000 RistLang-1.1.0/ristpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-01-02 04:44:00.000000 RistLang-1.1.0/ristpy/walkers.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-02 04:44:16.445976 RistLang-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-01-02 04:44:00.000000 RistLang-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:37:52.216957 RistLang-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-19 10:37:31.000000 RistLang-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-19 10:37:52.216957 RistLang-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-19 10:37:31.000000 RistLang-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:37:52.216957 RistLang-1.1.1/RistLang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:37:52.216957 RistLang-1.1.1/ristpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-19 10:37:31.000000 RistLang-1.1.1/ristpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-19 10:37:31.000000 RistLang-1.1.1/ristpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-19 10:37:31.000000 RistLang-1.1.1/ristpy/walkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:37:52.216957 RistLang-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-19 10:37:31.000000 RistLang-1.1.1/setup.py
```

### Comparing `RistLang-1.1.0/LICENSE` & `RistLang-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RistLang-1.1.0/PKG-INFO` & `RistLang-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RistLang
-Version: 1.1.0
+Version: 1.1.1
 Summary: A module for compiling RistLang
 Home-page: https://github.com/RistPy/PyRist
 License: MIT
 Project-URL: Issue tracker, https://github.com/RistPy/PyRist/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `RistLang-1.1.0/README.md` & `RistLang-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `RistLang-1.1.0/RistLang.egg-info/PKG-INFO` & `RistLang-1.1.1/RistLang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RistLang
-Version: 1.1.0
+Version: 1.1.1
 Summary: A module for compiling RistLang
 Home-page: https://github.com/RistPy/PyRist
 License: MIT
 Project-URL: Issue tracker, https://github.com/RistPy/PyRist/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `RistLang-1.1.0/ristpy/__init__.py` & `RistLang-1.1.1/ristpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,22 +365,23 @@
       return self
 
     def update_locals(self, other: dict):
       self.locals.update(other)
       return self
 
   __CODE = """
-  def _runner_func({{0}}):
-      import asyncio, aiohttp
-      from importlib import import_module as {0}
+# indent: 4 spaces
+def _runner_func({{0}}):
+    import asyncio, aiohttp
+    from importlib import import_module as {0}
 
-      try:
-          pass
-      finally:
-          _executor.scope.globals.update(locals())
+    try:
+        pass
+    finally:
+        _executor.scope.globals.update(locals())
   """.format(_iex.constants.IMPORTER)
 
   def _wrap_code(code: str, args: str = '', f=None) -> ast.Module:
     user_code = _iex.parse(code, f, mode='exec')
     mod = _iex.parse(__CODE.format(args), f, mode='exec')
     definition = mod.body[-1]
     assert isinstance(definition, ast.FunctionDef)
```

### Comparing `RistLang-1.1.0/ristpy/__main__.py` & `RistLang-1.1.1/ristpy/__main__.py`

 * *Files identical despite different names*

### Comparing `RistLang-1.1.0/ristpy/walkers.py` & `RistLang-1.1.1/ristpy/walkers.py`

 * *Files identical despite different names*

### Comparing `RistLang-1.1.0/setup.py` & `RistLang-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-version = "1.1.0"
+version = "1.1.1"
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 if version.endswith(('a', 'b', 'rc')):
   # append version identifier based on commit count
   try:
```

