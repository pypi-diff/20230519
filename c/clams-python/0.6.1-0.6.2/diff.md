# Comparing `tmp/clams-python-0.6.1.tar.gz` & `tmp/clams-python-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-0.6.1.tar", last modified: Fri May 19 12:56:04 2023, max compression
+gzip compressed data, was "clams-python-0.6.2.tar", last modified: Fri May 19 20:53:50 2023, max compression
```

## Comparing `clams-python-0.6.1.tar` & `clams-python-0.6.2.tar`

### file list

```diff
@@ -1,45 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.832249 clams-python-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-19 12:55:41.000000 clams-python-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 12:55:41.000000 clams-python-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 12:56:04.832249 clams-python-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-19 12:55:41.000000 clams-python-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 12:55:41.000000 clams-python-0.6.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16524 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.824250 clams-python-0.6.1/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/CLAMS-generic-readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/develop/templates/github/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/github/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.832249 clams-python-0.6.1/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 12:55:41.000000 clams-python-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:56:04.832249 clams-python-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-19 12:55:41.000000 clams-python-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.372418 clams-python-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-19 20:53:25.000000 clams-python-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 20:53:25.000000 clams-python-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-19 20:53:50.372418 clams-python-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-19 20:53:25.000000 clams-python-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 20:53:25.000000 clams-python-0.6.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16524 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.364417 clams-python-0.6.2/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/CLAMS-generic-readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/app/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/develop/templates/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/develop/templates/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/workflows/issue-apps-project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/workflows/issue-assign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/workflows/issue-close.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/develop/templates/github/workflows/publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-05-19 20:53:25.000000 clams-python-0.6.2/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.368418 clams-python-0.6.2/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 20:53:50.000000 clams-python-0.6.2/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 20:53:25.000000 clams-python-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:53:50.372418 clams-python-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-19 20:53:25.000000 clams-python-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:50.372418 clams-python-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-05-19 20:53:25.000000 clams-python-0.6.2/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-19 20:53:25.000000 clams-python-0.6.2/tests/test_clamscli.py
```

### Comparing `clams-python-0.6.1/LICENSE` & `clams-python-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/PKG-INFO` & `clams-python-0.6.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.6.1
+Version: 0.6.2
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
-License: UNKNOWN
-Description: ## CLAMS project
-        [CLAMS project](https://clams.ai) aims at free and open-source software platform for computational analysis and metadata generation applications for multimedia material. We believe free and open AI-based multimedia processing platform can bring many benefits of technical advancement to libraries, archives, and museums. To achieve interoperability between various computational applications developed be different vendors, which is absolutely necessary for using applications together supported by user-friendly workflow engines, we are also developing JSON-based MultiMedia Interchange Format ([MMIF](https://mmif.clams.ai))
-        
-        ## clams-python
-        `clams-python` is a Python implementation of the CLAMS SDK. `clams-python` provides CLAMS app developers with the following assistance ; 
-        
-        1. handling MMIF files for input and output specification for CLAMS apps
-        1. a base Python class to start developing a CLAMS app
-        1. a flask-based wrapper to run a Python CLAMS app as an HTTP web app
-        1. cookie-cutter shell command that sets up everything and starts a new CLAMS app project
-        
-        ### Start now from [Getting Started](introduction.html)!
-        
-        ## For more ...
-        For user manuals and Python API documentation, take a look at [Python modules](https://clams.ai/clams-python/modules.html).
-        
-        For MMIF-specific Python API documentation, take a look at the [mmif-python website](https://clams.ai/mmif-python).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## CLAMS project
+[CLAMS project](https://clams.ai) aims at free and open-source software platform for computational analysis and metadata generation applications for multimedia material. We believe free and open AI-based multimedia processing platform can bring many benefits of technical advancement to libraries, archives, and museums. To achieve interoperability between various computational applications developed be different vendors, which is absolutely necessary for using applications together supported by user-friendly workflow engines, we are also developing JSON-based MultiMedia Interchange Format ([MMIF](https://mmif.clams.ai))
+
+## clams-python
+`clams-python` is a Python implementation of the CLAMS SDK. `clams-python` provides CLAMS app developers with the following assistance ; 
+
+1. handling MMIF files for input and output specification for CLAMS apps
+1. a base Python class to start developing a CLAMS app
+1. a flask-based wrapper to run a Python CLAMS app as an HTTP web app
+1. cookie-cutter shell command that sets up everything and starts a new CLAMS app project
+
+### Start now from [Getting Started](introduction.html)!
+
+## For more ...
+For user manuals and Python API documentation, take a look at [Python modules](https://clams.ai/clams-python/modules.html).
+
+For MMIF-specific Python API documentation, take a look at the [mmif-python website](https://clams.ai/mmif-python).
```

### Comparing `clams-python-0.6.1/README.md` & `clams-python-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/__init__.py` & `clams-python-0.6.2/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/app/__init__.py` & `clams-python-0.6.2/clams/app/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/appmetadata/__init__.py` & `clams-python-0.6.2/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/develop/__init__.py` & `clams-python-0.6.2/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/develop/templates/app/.gitignore` & `clams-python-0.6.2/clams/develop/templates/app/.gitignore`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/develop/templates/app/CLAMS-generic-readme.md` & `clams-python-0.6.2/clams/develop/templates/app/CLAMS-generic-readme.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/develop/templates/app/Containerfile` & `clams-python-0.6.2/clams/develop/templates/app/Containerfile`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/develop/templates/app/README.md` & `clams-python-0.6.2/clams/develop/templates/app/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/develop/templates/app/app.py` & `clams-python-0.6.2/clams/develop/templates/app/app.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/develop/templates/app/metadata.py` & `clams-python-0.6.2/clams/develop/templates/app/metadata.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/develop/templates/github/README.md` & `clams-python-0.6.2/clams/develop/templates/github/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/restify/__init__.py` & `clams-python-0.6.2/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams/source/__init__.py` & `clams-python-0.6.2/clams/source/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.1/clams_python.egg-info/PKG-INFO` & `clams-python-0.6.2/clams_python.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.6.1
+Version: 0.6.2
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
-License: UNKNOWN
-Description: ## CLAMS project
-        [CLAMS project](https://clams.ai) aims at free and open-source software platform for computational analysis and metadata generation applications for multimedia material. We believe free and open AI-based multimedia processing platform can bring many benefits of technical advancement to libraries, archives, and museums. To achieve interoperability between various computational applications developed be different vendors, which is absolutely necessary for using applications together supported by user-friendly workflow engines, we are also developing JSON-based MultiMedia Interchange Format ([MMIF](https://mmif.clams.ai))
-        
-        ## clams-python
-        `clams-python` is a Python implementation of the CLAMS SDK. `clams-python` provides CLAMS app developers with the following assistance ; 
-        
-        1. handling MMIF files for input and output specification for CLAMS apps
-        1. a base Python class to start developing a CLAMS app
-        1. a flask-based wrapper to run a Python CLAMS app as an HTTP web app
-        1. cookie-cutter shell command that sets up everything and starts a new CLAMS app project
-        
-        ### Start now from [Getting Started](introduction.html)!
-        
-        ## For more ...
-        For user manuals and Python API documentation, take a look at [Python modules](https://clams.ai/clams-python/modules.html).
-        
-        For MMIF-specific Python API documentation, take a look at the [mmif-python website](https://clams.ai/mmif-python).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## CLAMS project
+[CLAMS project](https://clams.ai) aims at free and open-source software platform for computational analysis and metadata generation applications for multimedia material. We believe free and open AI-based multimedia processing platform can bring many benefits of technical advancement to libraries, archives, and museums. To achieve interoperability between various computational applications developed be different vendors, which is absolutely necessary for using applications together supported by user-friendly workflow engines, we are also developing JSON-based MultiMedia Interchange Format ([MMIF](https://mmif.clams.ai))
+
+## clams-python
+`clams-python` is a Python implementation of the CLAMS SDK. `clams-python` provides CLAMS app developers with the following assistance ; 
+
+1. handling MMIF files for input and output specification for CLAMS apps
+1. a base Python class to start developing a CLAMS app
+1. a flask-based wrapper to run a Python CLAMS app as an HTTP web app
+1. cookie-cutter shell command that sets up everything and starts a new CLAMS app project
+
+### Start now from [Getting Started](introduction.html)!
+
+## For more ...
+For user manuals and Python API documentation, take a look at [Python modules](https://clams.ai/clams-python/modules.html).
+
+For MMIF-specific Python API documentation, take a look at the [mmif-python website](https://clams.ai/mmif-python).
```

### Comparing `clams-python-0.6.1/clams_python.egg-info/SOURCES.txt` & `clams-python-0.6.2/clams_python.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -14,17 +14,23 @@
 clams/develop/templates/app/Containerfile
 clams/develop/templates/app/LICENSE
 clams/develop/templates/app/README.md
 clams/develop/templates/app/app.py
 clams/develop/templates/app/metadata.py
 clams/develop/templates/app/requirements.txt
 clams/develop/templates/github/README.md
+clams/develop/templates/github/workflows/issue-apps-project.yml
+clams/develop/templates/github/workflows/issue-assign.yml
+clams/develop/templates/github/workflows/issue-close.yml
+clams/develop/templates/github/workflows/publish.yml
 clams/restify/__init__.py
 clams/serve/__init__.py
 clams/source/__init__.py
 clams/ver/__init__.py
 clams_python.egg-info/PKG-INFO
 clams_python.egg-info/SOURCES.txt
 clams_python.egg-info/dependency_links.txt
 clams_python.egg-info/entry_points.txt
 clams_python.egg-info/requires.txt
-clams_python.egg-info/top_level.txt
+clams_python.egg-info/top_level.txt
+tests/test_clamsapp.py
+tests/test_clamscli.py
```

### Comparing `clams-python-0.6.1/setup.py` & `clams-python-0.6.2/setup.py`

 * *Files identical despite different names*

