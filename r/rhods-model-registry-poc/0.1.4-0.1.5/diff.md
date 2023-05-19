# Comparing `tmp/rhods_model_registry_poc-0.1.4.tar.gz` & `tmp/rhods_model_registry_poc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhods_model_registry_poc-0.1.4.tar", max compression
+gzip compressed data, was "rhods_model_registry_poc-0.1.5.tar", max compression
```

## Comparing `rhods_model_registry_poc-0.1.4.tar` & `rhods_model_registry_poc-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      114 2023-05-17 16:42:56.567694 rhods_model_registry_poc-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-17 12:00:46.265494 rhods_model_registry_poc-0.1.4/model_registry_python_sdk/__init__.py
--rw-r--r--   0        0        0     2032 2023-05-18 14:43:12.324583 rhods_model_registry_poc-0.1.4/model_registry_python_sdk/client.py
--rw-r--r--   0        0        0      568 2023-05-18 15:31:59.190709 rhods_model_registry_poc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 rhods_model_registry_poc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-05-17 16:42:56.567694 rhods_model_registry_poc-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 12:00:46.265494 rhods_model_registry_poc-0.1.5/model_registry_python_sdk/__init__.py
+-rw-r--r--   0        0        0     2032 2023-05-18 14:43:12.324583 rhods_model_registry_poc-0.1.5/model_registry_python_sdk/client.py
+-rw-r--r--   0        0        0      568 2023-05-18 16:10:50.556233 rhods_model_registry_poc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 rhods_model_registry_poc-0.1.5/PKG-INFO
```

### Comparing `rhods_model_registry_poc-0.1.4/model_registry_python_sdk/client.py` & `rhods_model_registry_poc-0.1.5/model_registry_python_sdk/client.py`

 * *Files identical despite different names*

### Comparing `rhods_model_registry_poc-0.1.4/pyproject.toml` & `rhods_model_registry_poc-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rhods-model-registry-poc"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "README.md"
 packages = [{include = "model_registry_python_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `rhods_model_registry_poc-0.1.4/PKG-INFO` & `rhods_model_registry_poc-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhods-model-registry-poc
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

