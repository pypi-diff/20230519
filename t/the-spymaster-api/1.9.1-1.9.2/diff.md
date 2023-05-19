# Comparing `tmp/the_spymaster_api-1.9.1.tar.gz` & `tmp/the_spymaster_api-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the_spymaster_api-1.9.1.tar", max compression
+gzip compressed data, was "the_spymaster_api-1.9.2.tar", max compression
```

## Comparing `the_spymaster_api-1.9.1.tar` & `the_spymaster_api-1.9.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      432 2023-05-12 13:26:58.187198 the_spymaster_api-1.9.1/pyproject.toml
--rw-r--r--   0        0        0       47 2022-09-25 13:05:12.295878 the_spymaster_api-1.9.1/the_spymaster_api/__init__.py
--rw-r--r--   0        0        0     2204 2023-05-12 12:11:02.909582 the_spymaster_api-1.9.1/the_spymaster_api/client.py
--rw-r--r--   0        0        0       93 2023-05-12 12:00:19.390270 the_spymaster_api-1.9.1/the_spymaster_api/structs/__init__.py
--rw-r--r--   0        0        0      789 2023-05-12 12:10:35.048752 the_spymaster_api-1.9.1/the_spymaster_api/structs/errors.py
--rw-r--r--   0        0        0      952 2022-09-27 09:51:02.090239 the_spymaster_api-1.9.1/the_spymaster_api/structs/request.py
--rw-r--r--   0        0        0     1201 2023-04-15 16:19:36.667573 the_spymaster_api-1.9.1/the_spymaster_api/structs/response.py
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 the_spymaster_api-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0      431 2023-05-19 15:05:12.689573 the_spymaster_api-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0       47 2022-09-25 13:05:12.295878 the_spymaster_api-1.9.2/the_spymaster_api/__init__.py
+-rw-r--r--   0        0        0     2204 2023-05-12 12:11:02.909582 the_spymaster_api-1.9.2/the_spymaster_api/client.py
+-rw-r--r--   0        0        0       93 2023-05-12 12:00:19.390270 the_spymaster_api-1.9.2/the_spymaster_api/structs/__init__.py
+-rw-r--r--   0        0        0      789 2023-05-12 12:10:35.048752 the_spymaster_api-1.9.2/the_spymaster_api/structs/errors.py
+-rw-r--r--   0        0        0      952 2022-09-27 09:51:02.090239 the_spymaster_api-1.9.2/the_spymaster_api/structs/request.py
+-rw-r--r--   0        0        0     1201 2023-04-15 16:19:36.667573 the_spymaster_api-1.9.2/the_spymaster_api/structs/response.py
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 the_spymaster_api-1.9.2/PKG-INFO
```

### Comparing `the_spymaster_api-1.9.1/the_spymaster_api/client.py` & `the_spymaster_api-1.9.2/the_spymaster_api/client.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_api-1.9.1/the_spymaster_api/structs/errors.py` & `the_spymaster_api-1.9.2/the_spymaster_api/structs/errors.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_api-1.9.1/the_spymaster_api/structs/request.py` & `the_spymaster_api-1.9.2/the_spymaster_api/structs/request.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_api-1.9.1/the_spymaster_api/structs/response.py` & `the_spymaster_api-1.9.2/the_spymaster_api/structs/response.py`

 * *Files identical despite different names*

### Comparing `the_spymaster_api-1.9.1/PKG-INFO` & `the_spymaster_api-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: the-spymaster-api
-Version: 1.9.1
+Version: 1.9.2
 Summary: Python client implementation for The Spymaster HTTP backend.
 Author: Asaf Kali
 Author-email: akali93@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: codenames (>=2.0,<3.0)
+Requires-Dist: codenames (>=2.2,<3.0)
 Requires-Dist: pydantic (>=1.9,<2.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: the_spymaster_solvers_client (>=1.7,<2.0)
 Requires-Dist: the_spymaster_util (>=3.0,<4.0)
```

