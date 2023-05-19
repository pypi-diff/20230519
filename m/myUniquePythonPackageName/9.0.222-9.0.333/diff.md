# Comparing `tmp/myUniquePythonPackageName-9.0.222.tar.gz` & `tmp/myUniquePythonPackageName-9.0.333.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myUniquePythonPackageName-9.0.222.tar", last modified: Fri May 19 09:03:03 2023, max compression
+gzip compressed data, was "myUniquePythonPackageName-9.0.333.tar", last modified: Fri May 19 11:02:24 2023, max compression
```

## Comparing `myUniquePythonPackageName-9.0.222.tar` & `myUniquePythonPackageName-9.0.333.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:03:03.716218 myUniquePythonPackageName-9.0.222/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-19 09:03:03.716218 myUniquePythonPackageName-9.0.222/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2563 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:03:03.693218 myUniquePythonPackageName-9.0.222/apimaticcalculator/
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/apimaticcalculator_client.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:03:03.696218 myUniquePythonPackageName-9.0.222/apimaticcalculator/controllers/
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/controllers/simple_calculator_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:03:03.699218 myUniquePythonPackageName-9.0.222/apimaticcalculator/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:03:03.705218 myUniquePythonPackageName-9.0.222/apimaticcalculator/http/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:03:03.706218 myUniquePythonPackageName-9.0.222/apimaticcalculator/models/
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/models/operation_type_enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:03:03.708218 myUniquePythonPackageName-9.0.222/apimaticcalculator/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/apimaticcalculator/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:03:03.716218 myUniquePythonPackageName-9.0.222/myUniquePythonPackageName.egg-info/
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-19 09:03:03.000000 myUniquePythonPackageName-9.0.222/myUniquePythonPackageName.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-19 09:03:03.000000 myUniquePythonPackageName-9.0.222/myUniquePythonPackageName.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 09:03:03.000000 myUniquePythonPackageName-9.0.222/myUniquePythonPackageName.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-19 09:03:03.000000 myUniquePythonPackageName-9.0.222/myUniquePythonPackageName.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-19 09:03:03.000000 myUniquePythonPackageName-9.0.222/myUniquePythonPackageName.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-19 09:02:29.000000 myUniquePythonPackageName-9.0.222/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-19 09:03:03.718218 myUniquePythonPackageName-9.0.222/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:02:24.177662 myUniquePythonPackageName-9.0.333/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-05-19 11:02:24.177662 myUniquePythonPackageName-9.0.333/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2878 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:02:24.163662 myUniquePythonPackageName-9.0.333/apimaticcalculator/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/apimaticcalculator_client.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:02:24.165662 myUniquePythonPackageName-9.0.333/apimaticcalculator/controllers/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/controllers/simple_calculator_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:02:24.166662 myUniquePythonPackageName-9.0.333/apimaticcalculator/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:02:24.170662 myUniquePythonPackageName-9.0.333/apimaticcalculator/http/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:02:24.171662 myUniquePythonPackageName-9.0.333/apimaticcalculator/models/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/models/operation_type_enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:02:24.173662 myUniquePythonPackageName-9.0.333/apimaticcalculator/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/apimaticcalculator/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:02:24.177662 myUniquePythonPackageName-9.0.333/myUniquePythonPackageName.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-05-19 11:02:24.000000 myUniquePythonPackageName-9.0.333/myUniquePythonPackageName.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-19 11:02:24.000000 myUniquePythonPackageName-9.0.333/myUniquePythonPackageName.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 11:02:24.000000 myUniquePythonPackageName-9.0.333/myUniquePythonPackageName.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-19 11:02:24.000000 myUniquePythonPackageName-9.0.333/myUniquePythonPackageName.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-19 11:02:24.000000 myUniquePythonPackageName-9.0.333/myUniquePythonPackageName.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      615 2023-05-19 11:01:53.000000 myUniquePythonPackageName-9.0.333/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-19 11:02:24.178662 myUniquePythonPackageName-9.0.333/setup.cfg
```

### Comparing `myUniquePythonPackageName-9.0.222/LICENSE` & `myUniquePythonPackageName-9.0.333/LICENSE`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/api_helper.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/api_helper.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/apimaticcalculator_client.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/apimaticcalculator_client.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/configuration.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/configuration.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/controllers/base_controller.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/controllers/simple_calculator_controller.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/controllers/simple_calculator_controller.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/exceptions/api_exception.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/http/http_request.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/http/http_request.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/http/http_response.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/http/http_response.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/apimaticcalculator/models/operation_type_enum.py` & `myUniquePythonPackageName-9.0.333/apimaticcalculator/models/operation_type_enum.py`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/myUniquePythonPackageName.egg-info/SOURCES.txt` & `myUniquePythonPackageName-9.0.333/myUniquePythonPackageName.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myUniquePythonPackageName-9.0.222/pyproject.toml` & `myUniquePythonPackageName-9.0.333/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "myUniquePythonPackageName"
-description = "as"
-version = "9.0.222"
+description = "Simple calculator API hosted on APIMATIC"
+version = "9.0.333"
+readme = "README.md"
 requires-python = ">=3.7"
 keywords = []
 authors = [{name = "RandomPerson", email = "randomEmail@testing.com"}]
 urls = {}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
 [project.optional-dependencies]
```

