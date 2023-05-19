# Comparing `tmp/t2d2-sdk-0.0.2.tar.gz` & `tmp/t2d2-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2d2-sdk-0.0.2.tar", last modified: Fri May 19 00:21:42 2023, max compression
+gzip compressed data, was "t2d2-sdk-0.0.3.tar", last modified: Fri May 19 00:35:45 2023, max compression
```

## Comparing `t2d2-sdk-0.0.2.tar` & `t2d2-sdk-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 00:21:32.000000 t2d2-sdk-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-19 00:21:32.000000 t2d2-sdk-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-19 00:21:32.000000 t2d2-sdk-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:21:42.515743 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-19 00:21:42.000000 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 00:21:42.000000 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:21:42.000000 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 00:21:42.000000 t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:35:45.349559 t2d2-sdk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 00:35:33.000000 t2d2-sdk-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-19 00:35:45.349559 t2d2-sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-19 00:35:33.000000 t2d2-sdk-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-19 00:35:33.000000 t2d2-sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:35:45.349559 t2d2-sdk-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:35:45.345559 t2d2-sdk-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:35:45.345559 t2d2-sdk-0.0.3/src/t2d2_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-19 00:35:45.000000 t2d2-sdk-0.0.3/src/t2d2_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 00:35:45.000000 t2d2-sdk-0.0.3/src/t2d2_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:35:45.000000 t2d2-sdk-0.0.3/src/t2d2_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 00:35:45.000000 t2d2-sdk-0.0.3/src/t2d2_sdk.egg-info/top_level.txt
```

### Comparing `t2d2-sdk-0.0.2/LICENSE` & `t2d2-sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `t2d2-sdk-0.0.2/PKG-INFO` & `t2d2-sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2d2-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: T2D2 SDK
 Author-email: Badri Hiriyur <badri@t2d2.ai>
 Project-URL: Homepage, https://github.com/t2d2-ai/py-sdk
 Project-URL: Bug Tracker, https://github.com/t2d2-ai/py-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 
 T2D2 api class
 
 ```python
 T = T2D2(credentials)
 ```
 
+```text
 - users                 create, get, update, delete
 --  api_keys            create, get, update, delete
 --  notifications       create, get, update, delete
 --  tasks               create, get, update, delete
 
 - organizations         create, get, update, delete, add_user, update_user, remove_user
 --  licenses            create, get, update, delete
@@ -36,7 +37,8 @@
 --  3dmodels            create, get, update, delete, upload
 --  annotations         create, get, update, delete
 --  geotags             create, get, update, delete
 --  filters             create, get, update, delete
 --  tags                create, get, update, delete
 --  tools               create, get, update, delete
 --  labels              create, get, update, delete
+```
```

### Comparing `t2d2-sdk-0.0.2/README.md` & `t2d2-sdk-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 T2D2 api class
 
 ```python
 T = T2D2(credentials)
 ```
 
+```text
 - users                 create, get, update, delete
 --  api_keys            create, get, update, delete
 --  notifications       create, get, update, delete
 --  tasks               create, get, update, delete
 
 - organizations         create, get, update, delete, add_user, update_user, remove_user
 --  licenses            create, get, update, delete
@@ -22,7 +23,8 @@
 --  3dmodels            create, get, update, delete, upload
 --  annotations         create, get, update, delete
 --  geotags             create, get, update, delete
 --  filters             create, get, update, delete
 --  tags                create, get, update, delete
 --  tools               create, get, update, delete
 --  labels              create, get, update, delete
+```
```

### Comparing `t2d2-sdk-0.0.2/pyproject.toml` & `t2d2-sdk-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "t2d2-sdk"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Badri Hiriyur", email="badri@t2d2.ai" },
 ]
 description = "T2D2 SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `t2d2-sdk-0.0.2/src/t2d2_sdk.egg-info/PKG-INFO` & `t2d2-sdk-0.0.3/src/t2d2_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2d2-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: T2D2 SDK
 Author-email: Badri Hiriyur <badri@t2d2.ai>
 Project-URL: Homepage, https://github.com/t2d2-ai/py-sdk
 Project-URL: Bug Tracker, https://github.com/t2d2-ai/py-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 
 T2D2 api class
 
 ```python
 T = T2D2(credentials)
 ```
 
+```text
 - users                 create, get, update, delete
 --  api_keys            create, get, update, delete
 --  notifications       create, get, update, delete
 --  tasks               create, get, update, delete
 
 - organizations         create, get, update, delete, add_user, update_user, remove_user
 --  licenses            create, get, update, delete
@@ -36,7 +37,8 @@
 --  3dmodels            create, get, update, delete, upload
 --  annotations         create, get, update, delete
 --  geotags             create, get, update, delete
 --  filters             create, get, update, delete
 --  tags                create, get, update, delete
 --  tools               create, get, update, delete
 --  labels              create, get, update, delete
+```
```

