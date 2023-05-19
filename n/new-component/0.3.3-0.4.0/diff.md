# Comparing `tmp/new-component-0.3.3.tar.gz` & `tmp/new-component-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new-component-0.3.3.tar", last modified: Fri May 19 04:44:04 2023, max compression
+gzip compressed data, was "new-component-0.4.0.tar", last modified: Fri May 19 21:18:43 2023, max compression
```

## Comparing `new-component-0.3.3.tar` & `new-component-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-05-19 04:43:41.857266 new-component-0.3.3/LICENSE
--rw-r--r--   0        0        0     4705 2023-05-19 04:43:41.857266 new-component-0.3.3/README.md
--rw-r--r--   0        0        0     1595 2023-05-19 04:43:41.861266 new-component-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6187 2023-05-19 04:43:41.861266 new-component-0.3.3/tests/test_new_component.py
--rw-r--r--   0        0        0      491 2023-05-19 04:43:41.861266 new-component-0.3.3/tests/test_version.py
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 new-component-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 21:18:20.306099 new-component-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4705 2023-05-19 21:18:20.306099 new-component-0.4.0/README.md
+-rw-r--r--   0        0        0     1595 2023-05-19 21:18:20.306099 new-component-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6187 2023-05-19 21:18:20.306099 new-component-0.4.0/tests/test_new_component.py
+-rw-r--r--   0        0        0      491 2023-05-19 21:18:20.306099 new-component-0.4.0/tests/test_version.py
+-rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 new-component-0.4.0/PKG-INFO
```

### Comparing `new-component-0.3.3/LICENSE` & `new-component-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `new-component-0.3.3/README.md` & `new-component-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `new-component-0.3.3/pyproject.toml` & `new-component-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "new-component"
-version = "0.3.3"
+version = "0.4.0"
 description = "Quickly create opinionated Styled Components for React Projects"
 authors = [
     { name = "Ian Cleary", email = "github@iancleary.me" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = [
```

### Comparing `new-component-0.3.3/tests/test_new_component.py` & `new-component-0.4.0/tests/test_new_component.py`

 * *Files identical despite different names*

### Comparing `new-component-0.3.3/PKG-INFO` & `new-component-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new-component
-Version: 0.3.3
+Version: 0.4.0
 Summary: Quickly create opinionated Styled Components for React Projects
 License: MIT
 Author-email: Ian Cleary <github@iancleary.me>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # new-component
```

