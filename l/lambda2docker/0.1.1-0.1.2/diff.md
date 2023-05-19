# Comparing `tmp/lambda2docker-0.1.1.tar.gz` & `tmp/lambda2docker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda2docker-0.1.1.tar", last modified: Fri May 19 11:32:29 2023, max compression
+gzip compressed data, was "lambda2docker-0.1.2.tar", last modified: Fri May 19 12:01:47 2023, max compression
```

## Comparing `lambda2docker-0.1.1.tar` & `lambda2docker-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:32:29.731902 lambda2docker-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-19 11:32:24.000000 lambda2docker-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-19 11:32:29.731902 lambda2docker-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-19 11:32:24.000000 lambda2docker-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:32:29.731902 lambda2docker-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-19 11:32:24.000000 lambda2docker-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:32:29.727902 lambda2docker-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:32:29.731902 lambda2docker-0.1.1/src/lambda2docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:32:24.000000 lambda2docker-0.1.1/src/lambda2docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-19 11:32:24.000000 lambda2docker-0.1.1/src/lambda2docker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-19 11:32:24.000000 lambda2docker-0.1.1/src/lambda2docker/lambda2docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-19 11:32:24.000000 lambda2docker-0.1.1/src/lambda2docker/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:32:29.731902 lambda2docker-0.1.1/src/lambda2docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-19 11:32:29.000000 lambda2docker-0.1.1/src/lambda2docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-19 11:32:29.000000 lambda2docker-0.1.1/src/lambda2docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:32:29.000000 lambda2docker-0.1.1/src/lambda2docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 11:32:29.000000 lambda2docker-0.1.1/src/lambda2docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:32:29.000000 lambda2docker-0.1.1/src/lambda2docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 11:32:29.000000 lambda2docker-0.1.1/src/lambda2docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 11:32:29.000000 lambda2docker-0.1.1/src/lambda2docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:01:47.620953 lambda2docker-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-19 12:01:47.616953 lambda2docker-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:01:47.620953 lambda2docker-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:01:47.616953 lambda2docker-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:01:47.616953 lambda2docker-0.1.2/src/lambda2docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/src/lambda2docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/src/lambda2docker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/src/lambda2docker/lambda2docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:01:47.616953 lambda2docker-0.1.2/src/lambda2docker/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/src/lambda2docker/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/src/lambda2docker/runtimes/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-19 12:01:42.000000 lambda2docker-0.1.2/src/lambda2docker/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:01:47.616953 lambda2docker-0.1.2/src/lambda2docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-19 12:01:47.000000 lambda2docker-0.1.2/src/lambda2docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-19 12:01:47.000000 lambda2docker-0.1.2/src/lambda2docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:01:47.000000 lambda2docker-0.1.2/src/lambda2docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 12:01:47.000000 lambda2docker-0.1.2/src/lambda2docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:01:47.000000 lambda2docker-0.1.2/src/lambda2docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 12:01:47.000000 lambda2docker-0.1.2/src/lambda2docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 12:01:47.000000 lambda2docker-0.1.2/src/lambda2docker.egg-info/top_level.txt
```

### Comparing `lambda2docker-0.1.1/LICENSE.md` & `lambda2docker-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lambda2docker-0.1.1/PKG-INFO` & `lambda2docker-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda2docker
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate a Dockerfile from a lambda function
 Home-page: https://github.com/paololazzari/lambda2docker
 Author: paololazzari
 Author-email: lazzari.paolok@gmail.com
 License: Apache License 2.0
 Keywords: aws,lambda,docker
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lambda2docker-0.1.1/README.md` & `lambda2docker-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lambda2docker-0.1.1/setup.py` & `lambda2docker-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="lambda2docker",
-    version="0.1.1",
+    version="0.1.2",
     description=("Generate a Dockerfile from a lambda function"),
     keywords="aws, lambda, docker",
     author="paololazzari",
     author_email="lazzari.paolok@gmail.com",
     url="https://github.com/paololazzari/lambda2docker",
     license="Apache License 2.0",
     package_dir={"": "src"},
```

### Comparing `lambda2docker-0.1.1/src/lambda2docker/__main__.py` & `lambda2docker-0.1.2/src/lambda2docker/__main__.py`

 * *Files identical despite different names*

### Comparing `lambda2docker-0.1.1/src/lambda2docker/lambda2docker.py` & `lambda2docker-0.1.2/src/lambda2docker/lambda2docker.py`

 * *Files identical despite different names*

### Comparing `lambda2docker-0.1.1/src/lambda2docker/validate.py` & `lambda2docker-0.1.2/src/lambda2docker/validate.py`

 * *Files identical despite different names*

### Comparing `lambda2docker-0.1.1/src/lambda2docker.egg-info/PKG-INFO` & `lambda2docker-0.1.2/src/lambda2docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda2docker
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate a Dockerfile from a lambda function
 Home-page: https://github.com/paololazzari/lambda2docker
 Author: paololazzari
 Author-email: lazzari.paolok@gmail.com
 License: Apache License 2.0
 Keywords: aws,lambda,docker
 Classifier: Development Status :: 5 - Production/Stable
```

