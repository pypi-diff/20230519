# Comparing `tmp/fabcohort-0.1.0.tar.gz` & `tmp/fabcohort-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabcohort-0.1.0.tar", last modified: Thu May 18 20:30:21 2023, max compression
+gzip compressed data, was "fabcohort-0.1.1.tar", last modified: Fri May 19 14:09:34 2023, max compression
```

## Comparing `fabcohort-0.1.0.tar` & `fabcohort-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-18 20:30:21.354352 fabcohort-0.1.0/
--rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-18 20:30:21.354184 fabcohort-0.1.0/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)      337 2023-05-18 20:13:13.000000 fabcohort-0.1.0/README.md
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-18 20:30:21.353128 fabcohort-0.1.0/fab_cohort/
--rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.1.0/fab_cohort/__init__.py
--rw-r--r--   0 linliding   (501) staff       (20)     1801 2023-05-18 18:09:51.000000 fabcohort-0.1.0/fab_cohort/cohort.py
-drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-18 20:30:21.353991 fabcohort-0.1.0/fabcohort.egg-info/
--rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-18 20:30:20.000000 fabcohort-0.1.0/fabcohort.egg-info/PKG-INFO
--rw-r--r--   0 linliding   (501) staff       (20)      226 2023-05-18 20:30:21.000000 fabcohort-0.1.0/fabcohort.egg-info/SOURCES.txt
--rw-r--r--   0 linliding   (501) staff       (20)        1 2023-05-18 20:30:21.000000 fabcohort-0.1.0/fabcohort.egg-info/dependency_links.txt
--rw-r--r--   0 linliding   (501) staff       (20)        7 2023-05-18 20:30:21.000000 fabcohort-0.1.0/fabcohort.egg-info/requires.txt
--rw-r--r--   0 linliding   (501) staff       (20)       11 2023-05-18 20:30:21.000000 fabcohort-0.1.0/fabcohort.egg-info/top_level.txt
--rw-r--r--   0 linliding   (501) staff       (20)       38 2023-05-18 20:30:21.354405 fabcohort-0.1.0/setup.cfg
--rw-r--r--   0 linliding   (501) staff       (20)     1284 2023-05-18 20:27:04.000000 fabcohort-0.1.0/setup.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:09:34.958796 fabcohort-0.1.1/
+-rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-19 14:09:34.958633 fabcohort-0.1.1/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)      337 2023-05-18 20:13:13.000000 fabcohort-0.1.1/README.md
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:09:34.957681 fabcohort-0.1.1/fab_cohort/
+-rw-r--r--   0 linliding   (501) staff       (20)       36 2023-05-18 20:24:44.000000 fabcohort-0.1.1/fab_cohort/__init__.py
+-rw-r--r--   0 linliding   (501) staff       (20)     5113 2023-05-19 13:35:30.000000 fabcohort-0.1.1/fab_cohort/cohort.py
+drwxr-xr-x   0 linliding   (501) staff       (20)        0 2023-05-19 14:09:34.958438 fabcohort-0.1.1/fabcohort.egg-info/
+-rw-r--r--   0 linliding   (501) staff       (20)     1028 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/PKG-INFO
+-rw-r--r--   0 linliding   (501) staff       (20)      226 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/SOURCES.txt
+-rw-r--r--   0 linliding   (501) staff       (20)        1 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/dependency_links.txt
+-rw-r--r--   0 linliding   (501) staff       (20)        7 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/requires.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       11 2023-05-19 14:09:34.000000 fabcohort-0.1.1/fabcohort.egg-info/top_level.txt
+-rw-r--r--   0 linliding   (501) staff       (20)       38 2023-05-19 14:09:34.958855 fabcohort-0.1.1/setup.cfg
+-rw-r--r--   0 linliding   (501) staff       (20)     1284 2023-05-19 11:02:52.000000 fabcohort-0.1.1/setup.py
```

### Comparing `fabcohort-0.1.0/PKG-INFO` & `fabcohort-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabcohort
-Version: 0.1.0
+Version: 0.1.1
 Summary: for cohort analysis
 Home-page: https://github.com/linliD/fabcohort/
 Author: Linli Ding
 Author-email: linli@joinbonnet.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `fabcohort-0.1.0/fabcohort.egg-info/PKG-INFO` & `fabcohort-0.1.1/fabcohort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabcohort
-Version: 0.1.0
+Version: 0.1.1
 Summary: for cohort analysis
 Home-page: https://github.com/linliD/fabcohort/
 Author: Linli Ding
 Author-email: linli@joinbonnet.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `fabcohort-0.1.0/setup.py` & `fabcohort-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="fabcohort",
-    version="0.1.0",
+    version="0.1.1",
     description="for cohort analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/linliD/fabcohort/",
     author="Linli Ding",
     author_email="linli@joinbonnet.com",
     license="MIT",
```

