# Comparing `tmp/smartis_sdk-0.3.0.tar.gz` & `tmp/smartis_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartis_sdk-0.3.0.tar", max compression
+gzip compressed data, was "smartis_sdk-0.4.0.tar", max compression
```

## Comparing `smartis_sdk-0.3.0.tar` & `smartis_sdk-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0       27 2023-05-11 10:42:26.070440 smartis_sdk-0.3.0/README.md
--rw-r--r--   0        0        0     1199 2023-05-12 10:53:50.294013 smartis_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      385 2023-05-12 02:24:39.116163 smartis_sdk-0.3.0/src/smartis_sdk/__init__.py
--rw-r--r--   0        0        0     6123 2023-05-12 10:50:38.623181 smartis_sdk-0.3.0/src/smartis_sdk/client.py
--rw-r--r--   0        0        0     1303 2023-05-11 11:59:04.485496 smartis_sdk-0.3.0/src/smartis_sdk/common.py
--rw-r--r--   0        0        0     3135 2023-05-12 02:22:17.878788 smartis_sdk-0.3.0/src/smartis_sdk/entity.py
--rw-r--r--   0        0        0      279 2023-05-12 08:01:58.268061 smartis_sdk-0.3.0/src/smartis_sdk/errors.py
--rw-r--r--   0        0        0      169 2023-05-11 08:47:15.864966 smartis_sdk-0.3.0/src/smartis_sdk/utils.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 smartis_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.4.0/LICENSE
+-rw-r--r--   0        0        0       27 2023-05-11 10:42:26.070440 smartis_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0     1199 2023-05-18 14:03:34.438674 smartis_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      385 2023-05-12 02:24:39.116163 smartis_sdk-0.4.0/src/smartis_sdk/__init__.py
+-rw-r--r--   0        0        0     6123 2023-05-12 10:50:38.623181 smartis_sdk-0.4.0/src/smartis_sdk/client.py
+-rw-r--r--   0        0        0     2194 2023-05-18 14:03:06.055156 smartis_sdk-0.4.0/src/smartis_sdk/common.py
+-rw-r--r--   0        0        0     3135 2023-05-12 02:22:17.878788 smartis_sdk-0.4.0/src/smartis_sdk/entity.py
+-rw-r--r--   0        0        0      279 2023-05-12 08:01:58.268061 smartis_sdk-0.4.0/src/smartis_sdk/errors.py
+-rw-r--r--   0        0        0      169 2023-05-11 08:47:15.864966 smartis_sdk-0.4.0/src/smartis_sdk/utils.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 smartis_sdk-0.4.0/PKG-INFO
```

### Comparing `smartis_sdk-0.3.0/LICENSE` & `smartis_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.3.0/pyproject.toml` & `smartis_sdk-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartis_sdk"
-version = "0.3.0"
+version = "0.4.0"
 description = "SDK для Smartis API"
 license = "MIT"
 authors = ["viktor <vi.dave@yandex.ru>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `smartis_sdk-0.3.0/src/smartis_sdk/client.py` & `smartis_sdk-0.4.0/src/smartis_sdk/client.py`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.3.0/src/smartis_sdk/entity.py` & `smartis_sdk-0.4.0/src/smartis_sdk/entity.py`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.3.0/PKG-INFO` & `smartis_sdk-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartis-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: SDK для Smartis API
 License: MIT
 Author: viktor
 Author-email: vi.dave@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

