# Comparing `tmp/jinja2_async_environment-0.1.1.tar.gz` & `tmp/jinja2_async_environment-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_async_environment-0.1.1.tar", last modified: Sat Apr 29 17:14:59 2023, max compression
+gzip compressed data, was "jinja2_async_environment-0.1.4.tar", last modified: Fri May 19 14:38:42 2023, max compression
```

## Comparing `jinja2_async_environment-0.1.1.tar` & `jinja2_async_environment-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.1.1/LICENSE
--rw-r--r--   0        0        0     6245 2023-04-29 16:12:44.541545 jinja2_async_environment-0.1.1/README.md
--rw-r--r--   0        0        0      407 2023-04-26 02:25:26.622784 jinja2_async_environment-0.1.1/jinja2_async_environment/__init__.py
--rw-r--r--   0        0        0     1342 2023-04-29 16:58:02.839049 jinja2_async_environment-0.1.1/jinja2_async_environment/bccache.py
--rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 jinja2_async_environment-0.1.1/jinja2_async_environment/compiler.py
--rw-r--r--   0        0        0     1790 2023-04-29 17:13:12.496114 jinja2_async_environment-0.1.1/jinja2_async_environment/environment.py
--rw-r--r--   0        0        0    10592 2023-04-29 17:11:35.256355 jinja2_async_environment-0.1.1/jinja2_async_environment/loaders.py
--rw-r--r--   0        0        0      902 2023-04-29 17:14:59.264970 jinja2_async_environment-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6539 1970-01-01 00:00:00.000000 jinja2_async_environment-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6245 2023-04-29 16:12:44.541545 jinja2_async_environment-0.1.4/README.md
+-rw-r--r--   0        0        0      497 2023-05-19 14:34:15.779905 jinja2_async_environment-0.1.4/jinja2_async_environment/__init__.py
+-rw-r--r--   0        0        0     1342 2023-04-29 16:58:02.839049 jinja2_async_environment-0.1.4/jinja2_async_environment/bccache.py
+-rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 jinja2_async_environment-0.1.4/jinja2_async_environment/compiler.py
+-rw-r--r--   0        0        0     1790 2023-04-29 17:13:12.496114 jinja2_async_environment-0.1.4/jinja2_async_environment/environment.py
+-rw-r--r--   0        0        0    10606 2023-05-19 14:31:50.584841 jinja2_async_environment-0.1.4/jinja2_async_environment/loaders.py
+-rw-r--r--   0        0        0      997 2023-05-19 14:38:42.808681 jinja2_async_environment-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6539 1970-01-01 00:00:00.000000 jinja2_async_environment-0.1.4/PKG-INFO
```

### Comparing `jinja2_async_environment-0.1.1/LICENSE` & `jinja2_async_environment-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.1/README.md` & `jinja2_async_environment-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.1/jinja2_async_environment/bccache.py` & `jinja2_async_environment-0.1.4/jinja2_async_environment/bccache.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.1/jinja2_async_environment/compiler.py` & `jinja2_async_environment-0.1.4/jinja2_async_environment/compiler.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.1/jinja2_async_environment/environment.py` & `jinja2_async_environment-0.1.4/jinja2_async_environment/environment.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.1/jinja2_async_environment/loaders.py` & `jinja2_async_environment-0.1.4/jinja2_async_environment/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.searchpath = searchpath
         if not isinstance(searchpath, abc.Iterable) or isinstance(searchpath, str):
             self.searchpath = [searchpath]
         self.searchpath = [AsyncPath(p) for p in searchpath]
 
     async def get_source(
         self, environment: "AsyncEnvironment", template: str | PathLike
-    ) -> [t.Tuple[str, t.Optional[str], t.Optional[t.Callable[[], bool]]], str]:
+    ) -> t.Tuple[str, t.Optional[str], t.Optional[t.Callable[[], bool]]]:  # type:ignore
         template = AsyncPath(template)
         if not self.has_source_access:
             raise RuntimeError(
                 f"{type(self).__name__} cannot provide access to the source"
             )
         raise TemplateNotFound(template.name)
 
@@ -206,15 +206,15 @@
                     "This zip import does not have the required"
                     " metadata to list templates."
                 )
             # Package is a zip file.
             prefix = self._template_root.name
             for name in self._loader._files.keys():
                 # Find names under the templates directory that aren't directories.
-                if name.startswith(prefix) and AsyncPath(name).is_file():
+                if name.startswith(prefix) and await AsyncPath(name).is_file():
                     results.append(name)
         results.sort()
         return results
 
 
 class DictLoader(AsyncBaseLoader):
     def __init__(
```

### Comparing `jinja2_async_environment-0.1.1/pyproject.toml` & `jinja2_async_environment-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "crackerjack>=0.1.7",
     "pre-commit>=3.2.2",
+    "types-redis>=4.5.5.2",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -22,28 +23,32 @@
 
 [tool.black]
 target-version = [
     "py311",
 ]
 
 [tool.mypy]
-strict = true
+strict = false
 pretty = true
+ignore_missing_imports = false
+plugins = [
+    "pydantic.mypy",
+]
 
 [tool.refurb]
 enable_all = true
 
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "jinja2-async-environment"
-version = "0.1.1"
+version = "0.1.4"
 description = ""
 dependencies = [
     "aiopath>=0.6.11",
     "jinja2>=3.1.2",
     "redis>=4.5.4",
 ]
 requires-python = ">=3.11"
```

### Comparing `jinja2_async_environment-0.1.1/PKG-INFO` & `jinja2_async_environment-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-async-environment
-Version: 0.1.1
+Version: 0.1.4
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Requires-Python: >=3.11
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: redis>=4.5.4
 Description-Content-Type: text/markdown
```

