# Comparing `tmp/logger-local-python-package-0.0.2.tar.gz` & `tmp/logger-local-python-package-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-local-python-package-0.0.2.tar", last modified: Fri May 19 10:02:28 2023, max compression
+gzip compressed data, was "logger-local-python-package-0.0.3.tar", last modified: Fri May 19 10:17:52 2023, max compression
```

## Comparing `logger-local-python-package-0.0.2.tar` & `logger-local-python-package-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:02:28.070372 logger-local-python-package-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-19 10:02:28.070372 logger-local-python-package-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:02:28.070372 logger-local-python-package-0.0.2/logger_local_python_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-19 10:02:28.000000 logger-local-python-package-0.0.2/logger_local_python_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-19 10:02:28.000000 logger-local-python-package-0.0.2/logger_local_python_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:02:28.000000 logger-local-python-package-0.0.2/logger_local_python_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 10:02:28.000000 logger-local-python-package-0.0.2/logger_local_python_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:02:28.070372 logger-local-python-package-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:02:28.070372 logger-local-python-package-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/src/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/src/LoggerServiceSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/src/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/src/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:02:28.070372 logger-local-python-package-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-19 10:02:15.000000 logger-local-python-package-0.0.2/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-19 10:17:52.000000 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-19 10:17:52.000000 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:17:52.000000 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 10:17:52.000000 logger-local-python-package-0.0.3/logger_local_python_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/LoggerServiceSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:17:52.389367 logger-local-python-package-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-19 10:17:41.000000 logger-local-python-package-0.0.3/tests/test_writer.py
```

### Comparing `logger-local-python-package-0.0.2/LICENSE` & `logger-local-python-package-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-local-python-package-0.0.2/PKG-INFO` & `logger-local-python-package-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local-python-package
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-python-package-0.0.2/logger_local_python_package.egg-info/PKG-INFO` & `logger-local-python-package-0.0.3/logger_local_python_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local-python-package
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-python-package-0.0.2/setup.py` & `logger-local-python-package-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='logger-local-python-package',
-    version='0.0.2',
+    version='0.0.3',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Logger Python Local",
     long_description="This is a package for sharing common Logger function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles-zone/logger-local-python-package",
     packages=setuptools.find_packages(),
```

### Comparing `logger-local-python-package-0.0.2/src/LoggerService.py` & `logger-local-python-package-0.0.3/src/LoggerService.py`

 * *Files identical despite different names*

### Comparing `logger-local-python-package-0.0.2/src/Writer.py` & `logger-local-python-package-0.0.3/src/Writer.py`

 * *Files identical despite different names*

### Comparing `logger-local-python-package-0.0.2/tests/test_writer.py` & `logger-local-python-package-0.0.3/tests/test_writer.py`

 * *Files identical despite different names*

