# Comparing `tmp/find_old_large_files-0.2.4.tar.gz` & `tmp/find_old_large_files-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.2.4.tar", last modified: Fri May 19 11:38:27 2023, max compression
+gzip compressed data, was "find_old_large_files-0.2.5.tar", last modified: Fri May 19 16:12:40 2023, max compression
```

## Comparing `find_old_large_files-0.2.4.tar` & `find_old_large_files-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:38:27.666715 find_old_large_files-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 11:38:02.000000 find_old_large_files-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-19 11:38:27.666715 find_old_large_files-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-19 11:38:02.000000 find_old_large_files-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:38:27.662715 find_old_large_files-0.2.4/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 11:38:02.000000 find_old_large_files-0.2.4/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-19 11:38:02.000000 find_old_large_files-0.2.4/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:38:27.666715 find_old_large_files-0.2.4/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-19 11:38:27.000000 find_old_large_files-0.2.4/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 11:38:27.000000 find_old_large_files-0.2.4/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:38:27.000000 find_old_large_files-0.2.4/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 11:38:27.000000 find_old_large_files-0.2.4/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:38:27.000000 find_old_large_files-0.2.4/find_old_large_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 11:38:27.000000 find_old_large_files-0.2.4/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:38:27.666715 find_old_large_files-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 11:38:02.000000 find_old_large_files-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:40.877810 find_old_large_files-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 16:12:40.877810 find_old_large_files-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:40.873810 find_old_large_files-0.2.5/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:40.877810 find_old_large_files-0.2.5/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:12:40.000000 find_old_large_files-0.2.5/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:12:40.877810 find_old_large_files-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 16:12:21.000000 find_old_large_files-0.2.5/setup.py
```

### Comparing `find_old_large_files-0.2.4/LICENSE` & `find_old_large_files-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.2.4/find_old_large_files/find_old_large_files.py` & `find_old_large_files-0.2.5/find_old_large_files/find_old_large_files.py`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.2.4/setup.py` & `find_old_large_files-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.2.4",  # Increment the version here
+    version="0.2.5",  # Increment the version here
     packages=find_packages(),
     install_requires=["tqdm"],
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
```

