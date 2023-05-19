# Comparing `tmp/automation_anywhere-2.1.0.tar.gz` & `tmp/automation_anywhere-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_anywhere-2.1.0.tar", last modified: Fri May 19 19:11:37 2023, max compression
+gzip compressed data, was "automation_anywhere-2.1.1.tar", last modified: Fri May 19 19:50:18 2023, max compression
```

## Comparing `automation_anywhere-2.1.0.tar` & `automation_anywhere-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.0/LICENSE
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3431 2023-05-19 18:02:53.000000 automation_anywhere-2.1.0/README.md
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/automation_anywhere/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.0/automation_anywhere/__init__.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4068 2023-05-11 13:45:41.000000 automation_anywhere-2.1.0/automation_anywhere/base.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.0/automation_anywhere/errors.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)    10108 2023-05-19 18:00:11.000000 automation_anywhere-2.1.0/automation_anywhere/executor.py
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/automation_anywhere.egg-info/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-19 19:11:37.000000 automation_anywhere-2.1.0/automation_anywhere.egg-info/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-05-19 19:11:37.000000 automation_anywhere-2.1.0/automation_anywhere.egg-info/SOURCES.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-05-19 19:11:37.000000 automation_anywhere-2.1.0/automation_anywhere.egg-info/dependency_links.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-05-19 19:11:37.000000 automation_anywhere-2.1.0/automation_anywhere.egg-info/top_level.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-05-19 19:10:11.000000 automation_anywhere-2.1.0/pyproject.toml
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-05-19 19:11:37.676112 automation_anywhere-2.1.0/setup.cfg
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:50:18.067487 automation_anywhere-2.1.1/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.1/LICENSE
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-19 19:50:18.067487 automation_anywhere-2.1.1/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3431 2023-05-19 18:02:53.000000 automation_anywhere-2.1.1/README.md
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:50:18.067487 automation_anywhere-2.1.1/automation_anywhere/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.1/automation_anywhere/__init__.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4068 2023-05-11 13:45:41.000000 automation_anywhere-2.1.1/automation_anywhere/base.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.1/automation_anywhere/errors.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)    10131 2023-05-19 19:48:44.000000 automation_anywhere-2.1.1/automation_anywhere/executor.py
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:50:18.067487 automation_anywhere-2.1.1/automation_anywhere.egg-info/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-19 19:50:18.000000 automation_anywhere-2.1.1/automation_anywhere.egg-info/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-05-19 19:50:18.000000 automation_anywhere-2.1.1/automation_anywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-05-19 19:50:18.000000 automation_anywhere-2.1.1/automation_anywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-05-19 19:50:18.000000 automation_anywhere-2.1.1/automation_anywhere.egg-info/top_level.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-05-19 19:49:47.000000 automation_anywhere-2.1.1/pyproject.toml
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-05-19 19:50:18.067487 automation_anywhere-2.1.1/setup.cfg
```

### Comparing `automation_anywhere-2.1.0/LICENSE` & `automation_anywhere-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.0/PKG-INFO` & `automation_anywhere-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_anywhere
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation_anywhere-2.1.0/README.md` & `automation_anywhere-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.0/automation_anywhere/base.py` & `automation_anywhere-2.1.1/automation_anywhere/base.py`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.0/automation_anywhere/executor.py` & `automation_anywhere-2.1.1/automation_anywhere/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,9 +199,10 @@
             error = f'Bad Request - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 401:
             error = f'Authentication Error - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 404:
             error = f'Not Found - {response.json()["message"]}'
         else:
             error = f'Unknown error: {response.text}'
+        success = True
         return success, error, return_data
```

### Comparing `automation_anywhere-2.1.0/automation_anywhere.egg-info/PKG-INFO` & `automation_anywhere-2.1.1/automation_anywhere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-anywhere
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation_anywhere-2.1.0/pyproject.toml` & `automation_anywhere-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="automation_anywhere"
-version="2.1.0"
+version="2.1.1"
 authors=[{name="Mateus Interciso", email="minterciso@gmail.com"}]
 description="A Python Package to deploy tasks on Automation Anywhere 360"
 readme="README.md"
 requires-python=">=3.9"
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

