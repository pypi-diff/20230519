# Comparing `tmp/pytest_when-1.0.4.tar.gz` & `tmp/pytest_when-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-1.0.4.tar", last modified: Fri May 19 17:58:54 2023, max compression
+gzip compressed data, was "pytest_when-1.0.5.tar", last modified: Fri May 19 18:46:58 2023, max compression
```

## Comparing `pytest_when-1.0.4.tar` & `pytest_when-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0    11342 2023-05-19 17:58:21.860935 pytest_when-1.0.4/LICENSE
--rw-r--r--   0        0        0     2709 2023-05-19 17:58:21.860935 pytest_when-1.0.4/README.md
--rw-r--r--   0        0        0     2776 2023-05-19 17:58:54.981792 pytest_when-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 17:58:21.860935 pytest_when-1.0.4/tests/resources/__init__.py
--rw-r--r--   0        0        0      131 2023-05-19 17:58:21.860935 pytest_when-1.0.4/tests/resources/example_module.py
--rw-r--r--   0        0        0     2492 2023-05-19 17:58:21.860935 pytest_when-1.0.4/tests/test_create_call_key.py
--rw-r--r--   0        0        0     5848 2023-05-19 17:58:21.860935 pytest_when-1.0.4/tests/test_integration.py
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 pytest_when-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-19 18:46:22.374647 pytest_when-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2709 2023-05-19 18:46:22.374647 pytest_when-1.0.5/README.md
+-rw-r--r--   0        0        0     2776 2023-05-19 18:46:58.727794 pytest_when-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 18:46:22.374647 pytest_when-1.0.5/pytest_when/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-19 18:46:22.374647 pytest_when-1.0.5/pytest_when/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:46:22.374647 pytest_when-1.0.5/pytest_when/py.typed
+-rw-r--r--   0        0        0    10667 2023-05-19 18:46:22.374647 pytest_when-1.0.5/pytest_when/when.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:46:22.374647 pytest_when-1.0.5/tests/resources/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-19 18:46:22.374647 pytest_when-1.0.5/tests/resources/example_module.py
+-rw-r--r--   0        0        0     2492 2023-05-19 18:46:22.374647 pytest_when-1.0.5/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     5848 2023-05-19 18:46:22.374647 pytest_when-1.0.5/tests/test_integration.py
+-rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 pytest_when-1.0.5/PKG-INFO
```

### Comparing `pytest_when-1.0.4/LICENSE` & `pytest_when-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.4/README.md` & `pytest_when-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.4/pyproject.toml` & `pytest_when-1.0.5/pyproject.toml`

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
-version = "1.0.4"
+version = "1.0.5"
 
 [project.entry-points.pytest11]
 pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
```

### Comparing `pytest_when-1.0.4/tests/test_create_call_key.py` & `pytest_when-1.0.5/tests/test_create_call_key.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.4/tests/test_integration.py` & `pytest_when-1.0.5/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.4/PKG-INFO` & `pytest_when-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-when
-Version: 1.0.4
+Version: 1.0.5
 Summary: Utility which makes mocking more readable and controllable
 Author-Email: zhukovgreen <iam+pytest-when@zhukovgreen.pro>
 Project-URL: Repository, https://github.com/zhukovgreen/pytest-when
 Requires-Python: >=3.8
 Requires-Dist: environs>=9.5.0
 Requires-Dist: pip>=23.1.2
 Description-Content-Type: text/markdown
```

