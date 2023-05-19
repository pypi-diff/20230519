# Comparing `tmp/truesight-0.0.2a0.tar.gz` & `tmp/truesight-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truesight-0.0.2a0.tar", last modified: Fri May 19 17:16:07 2023, max compression
+gzip compressed data, was "truesight-0.0.2a2.tar", last modified: Fri May 19 19:19:03 2023, max compression
```

## Comparing `truesight-0.0.2a0.tar` & `truesight-0.0.2a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:16:07.887645 truesight-0.0.2a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-19 17:16:07.887645 truesight-0.0.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-19 17:15:44.000000 truesight-0.0.2a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 17:16:07.887645 truesight-0.0.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-19 17:15:44.000000 truesight-0.0.2a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:16:07.887645 truesight-0.0.2a0/truesight/
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-05-19 17:15:44.000000 truesight-0.0.2a0/truesight/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-19 17:15:44.000000 truesight-0.0.2a0/truesight/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-19 17:15:44.000000 truesight-0.0.2a0/truesight/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-19 17:15:44.000000 truesight-0.0.2a0/truesight/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-19 17:15:44.000000 truesight-0.0.2a0/truesight/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:16:07.887645 truesight-0.0.2a0/truesight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-19 17:16:07.000000 truesight-0.0.2a0/truesight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 17:16:07.000000 truesight-0.0.2a0/truesight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:16:07.000000 truesight-0.0.2a0/truesight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 17:16:07.000000 truesight-0.0.2a0/truesight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 17:16:07.000000 truesight-0.0.2a0/truesight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:19:03.608434 truesight-0.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-19 19:19:03.608434 truesight-0.0.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-19 19:18:46.000000 truesight-0.0.2a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 19:19:03.608434 truesight-0.0.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-19 19:18:46.000000 truesight-0.0.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:19:03.608434 truesight-0.0.2a2/truesight/
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-19 19:18:46.000000 truesight-0.0.2a2/truesight/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:19:03.608434 truesight-0.0.2a2/truesight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 19:19:03.000000 truesight-0.0.2a2/truesight.egg-info/top_level.txt
```

### Comparing `truesight-0.0.2a0/setup.py` & `truesight-0.0.2a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'truesight',
     packages = ['truesight'],
-    version = 'v0.0.2a0',
+    version = 'v0.0.2a2',
     description = 'Truesight is a python package for time series prediction using deep learning and statistical models.',
     author = 'Renan Otvin Klehm',
     author_email = 'renanotivin@hotmail.com',
     url = 'https://github.com/renanklehm/true-sight',
     download_url = 'https://github.com/renanklehm/true-sight/archive/refs/tags/v0.0.1-alpha.tar.gz',
     keywords = ['time series', 'prediction'],
     classifiers = [],
@@ -21,8 +21,8 @@
         'optuna>=2.10.1',
         'numpy>=1.23.5',
         'pandas>=1.5.3',
         'matplotlib>=3.6.3',
         'scipy>=1.10.0',
         'tqdm>=4.64.1',
     ]
-)
+)
```

### Comparing `truesight-0.0.2a0/truesight/core.py` & `truesight-0.0.2a2/truesight/core.py`

 * *Files identical despite different names*

### Comparing `truesight-0.0.2a0/truesight/metrics.py` & `truesight-0.0.2a2/truesight/metrics.py`

 * *Files identical despite different names*

### Comparing `truesight-0.0.2a0/truesight/models.py` & `truesight-0.0.2a2/truesight/models.py`

 * *Files identical despite different names*

### Comparing `truesight-0.0.2a0/truesight/preprocessing.py` & `truesight-0.0.2a2/truesight/preprocessing.py`

 * *Files identical despite different names*

### Comparing `truesight-0.0.2a0/truesight/utils.py` & `truesight-0.0.2a2/truesight/utils.py`

 * *Files identical despite different names*

