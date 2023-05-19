# Comparing `tmp/extism-0.3.0.tar.gz` & `tmp/extism-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extism-0.3.0.tar", max compression
+gzip compressed data, was "extism-0.4.0.tar", max compression
```

## Comparing `extism-0.3.0.tar` & `extism-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1457 2023-03-15 15:37:22.708213 extism-0.3.0/LICENSE
--rw-r--r--   0        0        0      173 2023-03-15 15:37:11.496283 extism-0.3.0/README.md
--rw-r--r--   0        0        0      166 2023-03-15 15:37:11.496283 extism-0.3.0/extism/__init__.py
--rw-r--r--   0        0        0    15177 2023-03-15 15:37:11.496283 extism-0.3.0/extism/extism.py
--rw-r--r--   0        0        0      408 2023-03-15 15:37:11.496283 extism-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 extism-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1457 2023-05-19 20:29:22.383792 extism-0.4.0/LICENSE
+-rw-r--r--   0        0        0      173 2023-05-19 20:29:06.539195 extism-0.4.0/README.md
+-rw-r--r--   0        0        0      166 2023-05-19 20:29:06.539195 extism-0.4.0/extism/__init__.py
+-rw-r--r--   0        0        0    15250 2023-05-19 20:29:06.539195 extism-0.4.0/extism/extism.py
+-rw-r--r--   0        0        0      407 2023-05-19 20:29:06.539195 extism-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 extism-0.4.0/PKG-INFO
```

### Comparing `extism-0.3.0/LICENSE` & `extism-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extism-0.3.0/extism/extism.py` & `extism-0.4.0/extism/extism.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,17 @@
             Additional host functions
 
         Returns
         -------
         Plugin
             The created plugin
         """
-        return Plugin(self, manifest, wasi, config, functions)
+        return Plugin(
+            manifest, context=self, wasi=wasi, config=config, functions=functions
+        )
 
 
 class Function:
     def __init__(self, name: str, args, returns, f, *user_data):
         self.pointer = None
         args = [a.value for a in args]
         returns = [r.value for r in returns]
@@ -243,24 +245,27 @@
     Plugin is used to call WASM functions.
     Plugins can kept in a context for as long as you need
     or be freed with the `del` keyword.
     """
 
     def __init__(
         self,
-        context: Context,
         plugin: Union[str, bytes, dict],
+        context=None,
         wasi=False,
         config=None,
         functions=None,
     ):
         """
-        Construct a Plugin. Please use Context#plugin instead.
+        Construct a Plugin
         """
 
+        if context is None:
+            context = Context()
+
         wasm = _wasm(plugin)
 
         # Register plugin
         if functions is not None:
             functions = [f.pointer for f in functions]
             ptr = _ffi.new("ExtismFunction*[]", functions)
             self.plugin = _lib.extism_plugin_new(
```

### Comparing `extism-0.3.0/PKG-INFO` & `extism-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extism
-Version: 0.3.0
+Version: 0.4.0
 Summary: Extism Host SDK for python
 License: BSD-3-Clause
 Author: The Extism Authors
 Author-email: oss@extism.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

