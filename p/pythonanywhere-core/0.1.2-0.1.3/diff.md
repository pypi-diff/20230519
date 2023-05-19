# Comparing `tmp/pythonanywhere_core-0.1.2.tar.gz` & `tmp/pythonanywhere_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonanywhere_core-0.1.2.tar", max compression
+gzip compressed data, was "pythonanywhere_core-0.1.3.tar", max compression
```

## Comparing `pythonanywhere_core-0.1.2.tar` & `pythonanywhere_core-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1080 2022-03-25 13:53:43.266580 pythonanywhere_core-0.1.2/LICENSE
--rw-r--r--   0        0        0      223 2022-03-25 13:58:27.215546 pythonanywhere_core-0.1.2/README.rst
--rw-r--r--   0        0        0     1033 2023-02-10 20:34:06.458015 pythonanywhere_core-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2022-02-06 12:11:19.224987 pythonanywhere_core-0.1.2/pythonanywhere_core/__init__.py
--rw-r--r--   0        0        0     1984 2022-02-11 16:18:15.739949 pythonanywhere_core-0.1.2/pythonanywhere_core/base.py
--rw-r--r--   0        0        0      207 2022-10-21 16:53:31.963470 pythonanywhere_core-0.1.2/pythonanywhere_core/exceptions.py
--rw-r--r--   0        0        0     7026 2023-02-10 20:26:15.861991 pythonanywhere_core-0.1.2/pythonanywhere_core/webapp.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 pythonanywhere_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-25 13:53:43.266580 pythonanywhere_core-0.1.3/LICENSE
+-rw-r--r--   0        0        0      223 2022-03-25 13:58:27.215546 pythonanywhere_core-0.1.3/README.rst
+-rw-r--r--   0        0        0     1033 2023-05-19 16:26:21.647672 pythonanywhere_core-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-02-06 12:11:19.224987 pythonanywhere_core-0.1.3/pythonanywhere_core/__init__.py
+-rw-r--r--   0        0        0     1984 2022-02-11 16:18:15.739949 pythonanywhere_core-0.1.3/pythonanywhere_core/base.py
+-rw-r--r--   0        0        0      207 2022-10-21 16:53:31.963470 pythonanywhere_core-0.1.3/pythonanywhere_core/exceptions.py
+-rw-r--r--   0        0        0     3763 2023-05-19 16:24:10.017760 pythonanywhere_core-0.1.3/pythonanywhere_core/schedule.py
+-rw-r--r--   0        0        0     7026 2023-02-10 20:26:15.861991 pythonanywhere_core-0.1.3/pythonanywhere_core/webapp.py
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 pythonanywhere_core-0.1.3/PKG-INFO
```

### Comparing `pythonanywhere_core-0.1.2/LICENSE` & `pythonanywhere_core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonanywhere_core-0.1.2/pyproject.toml` & `pythonanywhere_core-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythonanywhere-core"
-version = "0.1.2"
+version = "0.1.3"
 description = "API wrapper for programmatic management of PythonAnywhere services."
 authors = ["PythonAnywhere <developers@pythonanywhere.com>"]
 license = "MIT"
 readme = "README.rst"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -16,19 +16,19 @@
     "Programming Language :: Python :: 3.7",
 ]
 keywords = ["pythonanywhere", "api", "cloud", "web hosting"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 python-dateutil = "^2.8.2"
-requests = "^2.25.1"
-snakesay = "^0.10.1"
+requests = "^2.30.0"
+snakesay = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.0"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 responses = "^0.22.0"
 
 [tool.black]
 line-length = 120
```

### Comparing `pythonanywhere_core-0.1.2/pythonanywhere_core/base.py` & `pythonanywhere_core-0.1.3/pythonanywhere_core/base.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere_core-0.1.2/pythonanywhere_core/webapp.py` & `pythonanywhere_core-0.1.3/pythonanywhere_core/webapp.py`

 * *Files identical despite different names*

### Comparing `pythonanywhere_core-0.1.2/PKG-INFO` & `pythonanywhere_core-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonanywhere-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: API wrapper for programmatic management of PythonAnywhere services.
 License: MIT
 Keywords: pythonanywhere,api,cloud,web hosting
 Author: PythonAnywhere
 Author-email: developers@pythonanywhere.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: snakesay (>=0.10.1,<0.11.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: snakesay (>=0.10.2,<0.11.0)
 Description-Content-Type: text/x-rst
 
 API wrapper for programmatic management of PythonAnywhere services.
 
 It's an extraction and improvement of core code behind `PythonAnywhere cli tool`_.
 
 .. _PythonAnywhere cli tool: https://pypi.org/project/pythonanywhere/
```

