# Comparing `tmp/rhods_model_registry_poc-0.1.5.tar.gz` & `tmp/rhods_model_registry_poc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhods_model_registry_poc-0.1.5.tar", max compression
+gzip compressed data, was "rhods_model_registry_poc-0.1.6.tar", max compression
```

## Comparing `rhods_model_registry_poc-0.1.5.tar` & `rhods_model_registry_poc-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      114 2023-05-17 16:42:56.567694 rhods_model_registry_poc-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-17 12:00:46.265494 rhods_model_registry_poc-0.1.5/model_registry_python_sdk/__init__.py
--rw-r--r--   0        0        0     2032 2023-05-18 14:43:12.324583 rhods_model_registry_poc-0.1.5/model_registry_python_sdk/client.py
--rw-r--r--   0        0        0      568 2023-05-18 16:10:50.556233 rhods_model_registry_poc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 rhods_model_registry_poc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-05-17 16:42:56.567694 rhods_model_registry_poc-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 12:00:46.265494 rhods_model_registry_poc-0.1.6/model_registry_python_sdk/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-19 13:29:48.406716 rhods_model_registry_poc-0.1.6/model_registry_python_sdk/client.py
+-rw-r--r--   0        0        0      568 2023-05-19 13:29:55.145325 rhods_model_registry_poc-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 rhods_model_registry_poc-0.1.6/PKG-INFO
```

### Comparing `rhods_model_registry_poc-0.1.5/model_registry_python_sdk/client.py` & `rhods_model_registry_poc-0.1.6/model_registry_python_sdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from kiota_http.httpx_request_adapter import HttpxRequestAdapter
 from minio import Minio
 from apicurioregistrysdk.client.groups.item.artifacts.artifacts_request_builder import ArtifactsRequestBuilder
 from apicurioregistrysdk.client.registry_client import RegistryClient
 from apicurioregistrysdk.client.models.artifact_content import ArtifactContent
 
 REGISTRY_URL = f"https://registry-external-ref.fly.dev/apis/registry/v2"
-MINIO_URL = "registry-external-ref-minio.fly.dev:9000"
+MINIO_URL = "2a09:8280:1::37:1c21:9000"
+# MINIO_URL = "registry-external-ref-minio.fly.dev:9000"
 BUCKET = "models"
 
 class ModelRegistryClient:
   
   def __init__(self) -> None:
     self.auth_provider = AnonymousAuthenticationProvider()
     self.request_adapter = HttpxRequestAdapter(self.auth_provider)
```

### Comparing `rhods_model_registry_poc-0.1.5/pyproject.toml` & `rhods_model_registry_poc-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rhods-model-registry-poc"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "README.md"
 packages = [{include = "model_registry_python_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `rhods_model_registry_poc-0.1.5/PKG-INFO` & `rhods_model_registry_poc-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhods-model-registry-poc
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

