# Comparing `tmp/find_old_large_files-0.2.2.tar.gz` & `tmp/find_old_large_files-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.2.2.tar", last modified: Wed May 17 21:38:17 2023, max compression
+gzip compressed data, was "find_old_large_files-0.2.3.tar", last modified: Fri May 19 11:31:45 2023, max compression
```

## Comparing `find_old_large_files-0.2.2.tar` & `find_old_large_files-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:38:17.445464 find_old_large_files-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 21:38:17.445464 find_old_large_files-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:38:17.441464 find_old_large_files-0.2.2/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:38:17.445464 find_old_large_files-0.2.2/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:38:17.445464 find_old_large_files-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:45.282659 find_old_large_files-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 11:31:16.000000 find_old_large_files-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-19 11:31:45.282659 find_old_large_files-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-19 11:31:16.000000 find_old_large_files-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:45.278659 find_old_large_files-0.2.3/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 11:31:16.000000 find_old_large_files-0.2.3/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-19 11:31:16.000000 find_old_large_files-0.2.3/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:45.278659 find_old_large_files-0.2.3/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-19 11:31:45.000000 find_old_large_files-0.2.3/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 11:31:45.000000 find_old_large_files-0.2.3/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:31:45.000000 find_old_large_files-0.2.3/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 11:31:45.000000 find_old_large_files-0.2.3/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:31:45.000000 find_old_large_files-0.2.3/find_old_large_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 11:31:45.000000 find_old_large_files-0.2.3/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:31:45.282659 find_old_large_files-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 11:31:16.000000 find_old_large_files-0.2.3/setup.py
```

### Comparing `find_old_large_files-0.2.2/LICENSE` & `find_old_large_files-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.2.2/PKG-INFO` & `find_old_large_files-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find_old_large_files
-Version: 0.2.2
+Version: 0.2.3
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.2.2/README.md` & `find_old_large_files-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.2.2/find_old_large_files.egg-info/PKG-INFO` & `find_old_large_files-0.2.3/find_old_large_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find-old-large-files
-Version: 0.2.2
+Version: 0.2.3
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.2.2/setup.py` & `find_old_large_files-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.2.2",  # Increment the version here
+    version="0.2.3",  # Increment the version here
     packages=find_packages(),
     install_requires=["tqdm"],
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
```

