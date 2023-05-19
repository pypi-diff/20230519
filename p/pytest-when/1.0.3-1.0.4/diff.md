# Comparing `tmp/pytest_when-1.0.3.tar.gz` & `tmp/pytest_when-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-1.0.3.tar", last modified: Fri May 19 16:23:47 2023, max compression
+gzip compressed data, was "pytest_when-1.0.4.tar", last modified: Fri May 19 17:58:54 2023, max compression
```

## Comparing `pytest_when-1.0.3.tar` & `pytest_when-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11342 2023-05-19 16:23:14.472368 pytest_when-1.0.3/LICENSE
--rw-r--r--   0        0        0     2358 2023-05-19 16:23:14.472368 pytest_when-1.0.3/README.md
--rw-r--r--   0        0        0     2776 2023-05-19 16:23:47.572953 pytest_when-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 16:23:14.472368 pytest_when-1.0.3/tests/resources/__init__.py
--rw-r--r--   0        0        0      131 2023-05-19 16:23:14.472368 pytest_when-1.0.3/tests/resources/example_module.py
--rw-r--r--   0        0        0     2492 2023-05-19 16:23:14.476368 pytest_when-1.0.3/tests/test_create_call_key.py
--rw-r--r--   0        0        0     5848 2023-05-19 16:23:14.476368 pytest_when-1.0.3/tests/test_integration.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 pytest_when-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-19 17:58:21.860935 pytest_when-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2709 2023-05-19 17:58:21.860935 pytest_when-1.0.4/README.md
+-rw-r--r--   0        0        0     2776 2023-05-19 17:58:54.981792 pytest_when-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 17:58:21.860935 pytest_when-1.0.4/tests/resources/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-19 17:58:21.860935 pytest_when-1.0.4/tests/resources/example_module.py
+-rw-r--r--   0        0        0     2492 2023-05-19 17:58:21.860935 pytest_when-1.0.4/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     5848 2023-05-19 17:58:21.860935 pytest_when-1.0.4/tests/test_integration.py
+-rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 pytest_when-1.0.4/PKG-INFO
```

### Comparing `pytest_when-1.0.3/LICENSE` & `pytest_when-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.3/README.md` & `pytest_when-1.0.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 # pytest-when
 
-Pytest plugin for making mocking in python more readable.
+Plugin provides a `when` fixture, which enables the following way of mocking
+the python objects:
+
+```python
+(
+    when(some_object, "attribute")
+    .called_with(1, 2, when.markers.any)
+    .then_return("mocked")
+)
+```
+
+It is readable and gives you a way to enable the mock only for a specific
+argument's values. In this the attribute will be mocked, for specific
+first two arguments and any third argument.
+
 Inspired by <https://github.com/mockito/mockito-scala>
 
 ## Installation
 
 ```bash
 pip install pytest-when
 ```
```

### Comparing `pytest_when-1.0.3/pyproject.toml` & `pytest_when-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 ]
 dependencies = [
     "environs>=9.5.0",
     "pip>=23.1.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "1.0.3"
+version = "1.0.4"
 
 [project.entry-points.pytest11]
 pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
```

### Comparing `pytest_when-1.0.3/tests/test_create_call_key.py` & `pytest_when-1.0.4/tests/test_create_call_key.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.3/tests/test_integration.py` & `pytest_when-1.0.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.3/PKG-INFO` & `pytest_when-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 Metadata-Version: 2.1
 Name: pytest-when
-Version: 1.0.3
+Version: 1.0.4
 Summary: Utility which makes mocking more readable and controllable
 Author-Email: zhukovgreen <iam+pytest-when@zhukovgreen.pro>
 Project-URL: Repository, https://github.com/zhukovgreen/pytest-when
 Requires-Python: >=3.8
 Requires-Dist: environs>=9.5.0
 Requires-Dist: pip>=23.1.2
 Description-Content-Type: text/markdown
 
 # pytest-when
 
-Pytest plugin for making mocking in python more readable.
+Plugin provides a `when` fixture, which enables the following way of mocking
+the python objects:
+
+```python
+(
+    when(some_object, "attribute")
+    .called_with(1, 2, when.markers.any)
+    .then_return("mocked")
+)
+```
+
+It is readable and gives you a way to enable the mock only for a specific
+argument's values. In this the attribute will be mocked, for specific
+first two arguments and any third argument.
+
 Inspired by <https://github.com/mockito/mockito-scala>
 
 ## Installation
 
 ```bash
 pip install pytest-when
 ```
```

