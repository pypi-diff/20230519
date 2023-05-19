# Comparing `tmp/pylipd-1.3.2.tar.gz` & `tmp/pylipd-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.3.2.tar", last modified: Thu May  4 15:21:37 2023, max compression
+gzip compressed data, was "pylipd-1.3.3.tar", last modified: Tue May  9 06:29:52 2023, max compression
```

## Comparing `pylipd-1.3.2.tar` & `pylipd-1.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.676397 pylipd-1.3.2/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.3.2/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-05-04 15:21:37.676469 pylipd-1.3.2/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.3.2/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.673875 pylipd-1.3.2/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-21 04:14:36.000000 pylipd-1.3.2/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.674850 pylipd-1.3.2/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.3.2/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      436 2023-04-20 09:57:39.000000 pylipd-1.3.2/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)     7417 2023-05-04 15:18:49.000000 pylipd-1.3.2/pylipd/globals/queries.py
--rw-r--r--   0 varun      (502) staff       (20)    15000 2023-04-21 04:08:45.000000 pylipd-1.3.2/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.3.2/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.3.2/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    29337 2023-05-04 15:18:49.000000 pylipd-1.3.2/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)     3349 2023-04-20 10:37:20.000000 pylipd-1.3.2/pylipd/lipd_series.py
--rw-r--r--   0 varun      (502) staff       (20)    43566 2023-04-20 10:00:23.000000 pylipd-1.3.2/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     3089 2023-05-04 14:42:24.000000 pylipd-1.3.2/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)     9324 2023-04-20 10:34:40.000000 pylipd-1.3.2/pylipd/rdf_graph.py
--rw-r--r--   0 varun      (502) staff       (20)    22181 2023-04-20 09:57:04.000000 pylipd-1.3.2/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.675215 pylipd-1.3.2/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.3.2/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.3.2/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.3.2/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     6073 2023-04-21 04:13:57.000000 pylipd-1.3.2/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     1095 2023-05-04 14:37:41.000000 pylipd-1.3.2/pylipd/usage_parallel.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.3.2/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-04 15:21:37.676292 pylipd-1.3.2/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      689 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.3.2/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       40 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-05-04 15:21:37.000000 pylipd-1.3.2/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.3.2/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      699 2023-05-04 15:21:37.676756 pylipd-1.3.2/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      989 2023-04-21 04:14:43.000000 pylipd-1.3.2/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-09 06:29:52.578456 pylipd-1.3.3/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.3.3/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-05-09 06:29:52.578513 pylipd-1.3.3/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.3.3/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-09 06:29:52.575974 pylipd-1.3.3/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-05-09 06:27:33.000000 pylipd-1.3.3/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-09 06:29:52.577012 pylipd-1.3.3/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.3.3/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      436 2023-04-20 09:57:39.000000 pylipd-1.3.3/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)     7417 2023-05-04 15:18:49.000000 pylipd-1.3.3/pylipd/globals/queries.py
+-rw-r--r--   0 varun      (502) staff       (20)    15000 2023-04-21 04:08:45.000000 pylipd-1.3.3/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.3.3/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15895 2023-04-11 02:38:59.000000 pylipd-1.3.3/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    29337 2023-05-09 06:26:49.000000 pylipd-1.3.3/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)     3349 2023-04-20 10:37:20.000000 pylipd-1.3.3/pylipd/lipd_series.py
+-rw-r--r--   0 varun      (502) staff       (20)    43566 2023-04-20 10:00:23.000000 pylipd-1.3.3/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     3089 2023-05-04 14:42:24.000000 pylipd-1.3.3/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)     9324 2023-04-20 10:34:40.000000 pylipd-1.3.3/pylipd/rdf_graph.py
+-rw-r--r--   0 varun      (502) staff       (20)    22181 2023-05-09 06:27:02.000000 pylipd-1.3.3/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-09 06:29:52.577333 pylipd-1.3.3/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.3.3/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.3.3/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2259 2023-04-11 05:52:03.000000 pylipd-1.3.3/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     6073 2023-05-09 06:28:06.000000 pylipd-1.3.3/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     1095 2023-05-04 14:37:41.000000 pylipd-1.3.3/pylipd/usage_parallel.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.3.3/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-05-09 06:29:52.578354 pylipd-1.3.3/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-05-09 06:29:52.000000 pylipd-1.3.3/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      689 2023-05-09 06:29:52.000000 pylipd-1.3.3/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-05-09 06:29:52.000000 pylipd-1.3.3/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.3.3/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       40 2023-05-09 06:29:52.000000 pylipd-1.3.3/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-05-09 06:29:52.000000 pylipd-1.3.3/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.3.3/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      699 2023-05-09 06:29:52.578779 pylipd-1.3.3/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      989 2023-05-09 06:27:43.000000 pylipd-1.3.3/setup.py
```

### Comparing `pylipd-1.3.2/LICENSE` & `pylipd-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/PKG-INFO` & `pylipd-1.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.2
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.3
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.3.2/README.md` & `pylipd-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/globals/queries.py` & `pylipd-1.3.3/pylipd/globals/queries.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/globals/schema.py` & `pylipd-1.3.3/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/legacy_utils.py` & `pylipd-1.3.3/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/lipd.py` & `pylipd-1.3.3/pylipd/lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/lipd_series.py` & `pylipd-1.3.3/pylipd/lipd_series.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/lipd_to_rdf.py` & `pylipd-1.3.3/pylipd/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/multi_processing.py` & `pylipd-1.3.3/pylipd/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/rdf_graph.py` & `pylipd-1.3.3/pylipd/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/rdf_to_lipd.py` & `pylipd-1.3.3/pylipd/rdf_to_lipd.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     The RDFToLiPD class helps in converting an RDF Graph to a LiPD file.
     It uses the SCHEMA dictionary (from globals/schema.py) to do the conversion
     """    
     def __init__(self, graph):
         self.graph = graph
         self.lipd_csvs = {}
         self.graphurl = NSURL
-        self.namespace = NSURL + "#"
+        self.namespace = NSURL + "/"
 
     def convert(self, dsname, lipdfile):
         '''Convert RDF graph to a LiPD file
 
         Parameters
         ----------
```

### Comparing `pylipd-1.3.2/pylipd/series/regexes.py` & `pylipd-1.3.3/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/test.py` & `pylipd-1.3.3/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/usage.py` & `pylipd-1.3.3/pylipd/usage.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/usage_parallel.py` & `pylipd-1.3.3/pylipd/usage_parallel.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd/utils.py` & `pylipd-1.3.3/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/pylipd.egg-info/PKG-INFO` & `pylipd-1.3.3/pylipd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.2
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.3
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.3.2/pylipd.egg-info/SOURCES.txt` & `pylipd-1.3.3/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.2/setup.cfg` & `pylipd-1.3.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.3.2
+version = 1.3.3
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.3.2/setup.py` & `pylipd-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.3.2'
+version = '1.3.3'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

