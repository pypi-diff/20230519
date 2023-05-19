# Comparing `tmp/starlette_async_jinja-0.1.1.tar.gz` & `tmp/starlette_async_jinja-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_async_jinja-0.1.1.tar", last modified: Wed Apr 26 17:40:13 2023, max compression
+gzip compressed data, was "starlette_async_jinja-1.2.0.tar", last modified: Fri May 19 14:47:00 2023, max compression
```

## Comparing `starlette_async_jinja-0.1.1.tar` & `starlette_async_jinja-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      282 2023-04-26 14:31:29.295695 starlette_async_jinja-0.1.1/README.md
--rw-r--r--   0        0        0     1174 2023-04-26 17:40:13.118620 starlette_async_jinja-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      420 2023-04-22 16:45:22.461705 starlette_async_jinja-0.1.1/starlette_async_jinja/__init__.py
--rw-r--r--   0        0        0     3753 2023-04-26 17:38:29.008338 starlette_async_jinja-0.1.1/starlette_async_jinja/responses.py
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 starlette_async_jinja-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      282 2023-04-26 14:31:29.295695 starlette_async_jinja-1.2.0/README.md
+-rw-r--r--   0        0        0     1169 2023-05-19 14:47:00.917189 starlette_async_jinja-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-05-19 13:51:11.189835 starlette_async_jinja-1.2.0/starlette_async_jinja/__init__.py
+-rw-r--r--   0        0        0     5994 2023-05-19 13:43:09.701695 starlette_async_jinja-1.2.0/starlette_async_jinja/responses.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 starlette_async_jinja-1.2.0/PKG-INFO
```

### Comparing `starlette_async_jinja-0.1.1/pyproject.toml` & `starlette_async_jinja-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pre-commit>=3.2.2",
-    "acb @ file:///${PROJECT_ROOT}/../acb",
     "Crackerjack @ file:///${PROJECT_ROOT}/../crackerjack",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
@@ -36,19 +35,20 @@
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "starlette-async-jinja"
-version = "0.1.1"
+version = "1.2.0"
 description = ""
 dependencies = [
     "starlette>=0.26.1",
     "jinja2>=3.1.2",
+    "jinja2-async-environment>=0.1.1",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `starlette_async_jinja-0.1.1/PKG-INFO` & `starlette_async_jinja-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: starlette-async-jinja
-Version: 0.1.1
+Version: 1.2.0
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/lesleslie/starlette-async-jinja
 Project-URL: Documentation, https://github.com/lesleslie/starlette-async-jinja
 Project-URL: Repository, https://github.com/lesleslie/starlette-async-jinja
 Requires-Python: >=3.11
 Requires-Dist: starlette>=0.26.1
 Requires-Dist: jinja2>=3.1.2
+Requires-Dist: jinja2-async-environment>=0.1.1
 Description-Content-Type: text/markdown
 
 # starlette-async-jinja
 
 ### Jinja2 is_async template support and async loaders for Starlette
 
 ## About
```

