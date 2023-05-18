# Comparing `tmp/daimin_data-0.0.2.tar.gz` & `tmp/daimin_data-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daimin_data-0.0.2.tar", last modified: Thu May 18 21:17:03 2023, max compression
+gzip compressed data, was "daimin_data-0.0.3.tar", last modified: Thu May 18 22:22:34 2023, max compression
```

## Comparing `daimin_data-0.0.2.tar` & `daimin_data-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-18 21:17:03.937303 daimin_data-0.0.2/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 daimin_data-0.0.2/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 daimin_data-0.0.2/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1071 2023-05-18 21:17:03.937145 daimin_data-0.0.2/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      307 2023-05-18 20:16:04.000000 daimin_data-0.0.2/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-18 21:17:03.935841 daimin_data-0.0.2/daimin_data/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-05-18 20:38:37.000000 daimin_data-0.0.2/daimin_data/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1461 2023-05-18 20:38:37.000000 daimin_data-0.0.2/daimin_data/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     7031 2023-05-18 20:38:37.000000 daimin_data-0.0.2/daimin_data/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-18 21:17:03.936915 daimin_data-0.0.2/daimin_data.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1071 2023-05-18 21:17:03.000000 daimin_data-0.0.2/daimin_data.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      364 2023-05-18 21:17:03.000000 daimin_data-0.0.2/daimin_data.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-18 21:17:03.000000 daimin_data-0.0.2/daimin_data.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       65 2023-05-18 21:17:03.000000 daimin_data-0.0.2/daimin_data.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-18 20:17:01.000000 daimin_data-0.0.2/daimin_data.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       14 2023-05-18 21:17:03.000000 daimin_data-0.0.2/daimin_data.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       12 2023-05-18 21:17:03.000000 daimin_data-0.0.2/daimin_data.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      907 2023-05-18 21:16:47.000000 daimin_data-0.0.2/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-05-18 21:17:03.937351 daimin_data-0.0.2/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 daimin_data-0.0.2/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-18 22:22:34.454188 daimin_data-0.0.3/
+-rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 daimin_data-0.0.3/LICENSE
+-rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 daimin_data-0.0.3/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1071 2023-05-18 22:22:34.454022 daimin_data-0.0.3/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      307 2023-05-18 20:16:04.000000 daimin_data-0.0.3/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-18 22:22:34.452045 daimin_data-0.0.3/daimin_data/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-05-18 20:38:37.000000 daimin_data-0.0.3/daimin_data/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1461 2023-05-18 20:38:37.000000 daimin_data-0.0.3/daimin_data/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     7031 2023-05-18 20:38:37.000000 daimin_data-0.0.3/daimin_data/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-18 22:22:34.453728 daimin_data-0.0.3/daimin_data.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1071 2023-05-18 22:22:34.000000 daimin_data-0.0.3/daimin_data.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      364 2023-05-18 22:22:34.000000 daimin_data-0.0.3/daimin_data.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-18 22:22:34.000000 daimin_data-0.0.3/daimin_data.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       65 2023-05-18 22:22:34.000000 daimin_data-0.0.3/daimin_data.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-18 20:17:01.000000 daimin_data-0.0.3/daimin_data.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       23 2023-05-18 22:22:34.000000 daimin_data-0.0.3/daimin_data.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       12 2023-05-18 22:22:34.000000 daimin_data-0.0.3/daimin_data.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      916 2023-05-18 22:22:24.000000 daimin_data-0.0.3/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-05-18 22:22:34.454265 daimin_data-0.0.3/setup.cfg
+-rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 daimin_data-0.0.3/setup.py
```

### Comparing `daimin_data-0.0.2/LICENSE` & `daimin_data-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `daimin_data-0.0.2/PKG-INFO` & `daimin_data-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daimin_data
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/toyo-bunko/daimin_data
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `daimin_data-0.0.2/daimin_data/_modidx.py` & `daimin_data-0.0.3/daimin_data/_modidx.py`

 * *Files identical despite different names*

### Comparing `daimin_data-0.0.2/daimin_data/core.py` & `daimin_data-0.0.3/daimin_data/core.py`

 * *Files identical despite different names*

### Comparing `daimin_data-0.0.2/daimin_data.egg-info/PKG-INFO` & `daimin_data-0.0.3/daimin_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daimin-data
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/toyo-bunko/daimin_data
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `daimin_data-0.0.2/settings.ini` & `daimin_data-0.0.3/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = daimin_data
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = daimin_data
@@ -34,10 +34,10 @@
 description = 
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = toyo-bunko
 
 ### Optional ###
-requirements = pandas
+requirements = pandas openpyxl
 # dev_requirements = 
 # console_scripts =
```

### Comparing `daimin_data-0.0.2/setup.py` & `daimin_data-0.0.3/setup.py`

 * *Files identical despite different names*

