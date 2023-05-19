# Comparing `tmp/configzen-0.1.18.tar.gz` & `tmp/configzen-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.18.tar", max compression
+gzip compressed data, was "configzen-0.1.19.tar", max compression
```

## Comparing `configzen-0.1.18.tar` & `configzen-0.1.19.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.18/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.18/configzen/__main__.py
--rw-r--r--   0        0        0    52546 2023-05-19 16:53:18.824977 configzen-0.1.18/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.18/configzen/errors.py
--rw-r--r--   0        0        0    18753 2023-05-19 16:49:35.820189 configzen-0.1.18/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.18/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.18/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.18/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-19 16:50:39.334651 configzen-0.1.18/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 16:08:27.014931 configzen-0.1.18/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.18/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.19/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.19/configzen/__main__.py
+-rw-r--r--   0        0        0    52553 2023-05-19 17:19:05.319257 configzen-0.1.19/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.19/configzen/errors.py
+-rw-r--r--   0        0        0    18753 2023-05-19 16:49:35.820189 configzen-0.1.19/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.19/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.19/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.19/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-19 17:26:42.174262 configzen-0.1.19/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 16:08:27.014931 configzen-0.1.19/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.19/PKG-INFO
```

### Comparing `configzen-0.1.18/configzen/__main__.py` & `configzen-0.1.19/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.18/configzen/config.py` & `configzen-0.1.19/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,15 +876,15 @@
 
         Returns
         -------
         The configuration loader.
         """
         args: list[Any] = []
         kwargs: dict[str, Any] = {}
-        if isinstance(ctx.snippet, str):
+        if isinstance(ctx.snippet, (str, int)):
             args.append(ctx.snippet)
         elif is_dict_like(ctx.snippet):
             kwargs |= ctx.snippet
         elif is_list_like(ctx.snippet):
             args += list(ctx.snippet)
         else:
             msg = (
```

### Comparing `configzen-0.1.18/configzen/errors.py` & `configzen-0.1.19/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.18/configzen/processor.py` & `configzen-0.1.19/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.18/configzen/typedefs.py` & `configzen-0.1.19/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.18/LICENSE` & `configzen-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.18/pyproject.toml` & `configzen-0.1.19/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.18"
+version = "0.1.19"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.18/README.md` & `configzen-0.1.19/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.18/PKG-INFO` & `configzen-0.1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.18
+Version: 0.1.19
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

