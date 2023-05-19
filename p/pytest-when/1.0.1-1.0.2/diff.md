# Comparing `tmp/pytest_when-1.0.1.tar.gz` & `tmp/pytest_when-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-1.0.1.tar", last modified: Fri May 19 16:01:59 2023, max compression
+gzip compressed data, was "pytest_when-1.0.2.tar", last modified: Fri May 19 16:14:57 2023, max compression
```

## Comparing `pytest_when-1.0.1.tar` & `pytest_when-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11342 2023-05-19 16:01:20.781230 pytest_when-1.0.1/LICENSE
--rw-r--r--   0        0        0     1684 2023-05-19 16:01:20.781230 pytest_when-1.0.1/README.md
--rw-r--r--   0        0        0     2752 2023-05-19 16:01:59.305570 pytest_when-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 16:01:20.781230 pytest_when-1.0.1/tests/resources/__init__.py
--rw-r--r--   0        0        0      131 2023-05-19 16:01:20.781230 pytest_when-1.0.1/tests/resources/example_module.py
--rw-r--r--   0        0        0     2492 2023-05-19 16:01:20.781230 pytest_when-1.0.1/tests/test_create_call_key.py
--rw-r--r--   0        0        0     5280 2023-05-19 16:01:20.781230 pytest_when-1.0.1/tests/test_integration.py
--rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 pytest_when-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-19 16:14:05.133202 pytest_when-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2358 2023-05-19 16:14:05.133202 pytest_when-1.0.2/README.md
+-rw-r--r--   0        0        0     2752 2023-05-19 16:14:57.478490 pytest_when-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 16:14:05.137203 pytest_when-1.0.2/tests/resources/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-19 16:14:05.137203 pytest_when-1.0.2/tests/resources/example_module.py
+-rw-r--r--   0        0        0     2492 2023-05-19 16:14:05.137203 pytest_when-1.0.2/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     5848 2023-05-19 16:14:05.137203 pytest_when-1.0.2/tests/test_integration.py
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 pytest_when-1.0.2/PKG-INFO
```

### Comparing `pytest_when-1.0.1/LICENSE` & `pytest_when-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.1/README.md` & `pytest_when-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pytest-when
+Version: 1.0.2
+Summary: Utility makes mocing more readable
+Author-Email: zhukovgreen <iam+pytest-when@zhukovgreen.pro>
+Project-URL: Repository, https://github.com/zhukovgreen/pytest-when
+Requires-Python: >=3.8
+Requires-Dist: environs>=9.5.0
+Requires-Dist: pip>=23.1.2
+Description-Content-Type: text/markdown
+
 # pytest-when
 
 Pytest plugin for making mocking in python more readable.
 Inspired by <https://github.com/mockito/mockito-scala>
 
 ## Installation
 
@@ -51,14 +62,42 @@
             "not mocked param",
             1,
             kwarg1="b",
             kwarg2="c",
         )
         == "Not mocked"
     )
+
+# if you need to patch a function
+def test_patch_a_function(when):
+    when(example_module, "some_normal_function").called_with(
+        "a",
+        when.markers.any,
+        kwarg1="b",
+        kwarg2=when.markers.any,
+    ).then_return("Mocked")
+
+    assert (
+            example_module.some_normal_function(
+                "a",
+                1,
+                kwarg1="b",
+                kwarg2="c",
+            )
+            == "Mocked"
+    )
+    assert (
+            example_module.some_normal_function(
+                "not mocked param",
+                1,
+                kwarg1="b",
+                kwarg2="c",
+            )
+            == "Not mocked"
+    )
 ```
 
 It is possible to use 'when' with class methods and standalone functions
 (in this case cls parameter will become a python module).
 
 You can patch multiple times the same object with different "called_with"
 parameters in a single test.
```

### Comparing `pytest_when-1.0.1/pyproject.toml` & `pytest_when-1.0.2/pyproject.toml`

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
-version = "1.0.1"
+version = "1.0.2"
 
 [project.entry-points.pytest11]
 pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
```

### Comparing `pytest_when-1.0.1/tests/test_create_call_key.py` & `pytest_when-1.0.2/tests/test_create_call_key.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.1/tests/test_integration.py` & `pytest_when-1.0.2/tests/test_integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -172,14 +172,40 @@
             kwarg1="b",
             kwarg2="c",
         )
         == "Not mocked"
     )
 
 
+def test_should_properly_repatch(when):
+    when(Klass1, "some_method").called_with(
+        "a",
+        when.markers.any,
+        kwarg1="b",
+        kwarg2=when.markers.any,
+    ).then_return("Mocked first time")
+
+    when(Klass1, "some_method").called_with(
+        "a",
+        when.markers.any,
+        kwarg1="b",
+        kwarg2=when.markers.any,
+    ).then_return("Mocked second time")
+
+    assert (
+        Klass1().some_method(
+            "a",
+            1,
+            kwarg1="b",
+            kwarg2="c",
+        )
+        == "Mocked second time"
+    )
+
+
 def test_should_be_able_to_patch_multiple_objects(when):
     when(Klass1, "some_method").called_with(
         "a",
         when.markers.any,
         kwarg1="b",
         kwarg2=when.markers.any,
     ).then_return("Mocked Klass1")
```

