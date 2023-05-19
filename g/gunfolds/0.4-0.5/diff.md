# Comparing `tmp/gunfolds-0.4.tar.gz` & `tmp/gunfolds-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunfolds-0.4.tar", last modified: Fri May 19 06:18:13 2023, max compression
+gzip compressed data, was "gunfolds-0.5.tar", last modified: Fri May 19 19:20:52 2023, max compression
```

## Comparing `gunfolds-0.4.tar` & `gunfolds-0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:18:13.902558 gunfolds-0.4/
--rw-r--r--   0 gm         (501) staff       (20)    35121 2023-05-18 18:49:59.000000 gunfolds-0.4/LICENSE
--rw-r--r--   0 gm         (501) staff       (20)       50 2023-05-18 18:49:59.000000 gunfolds-0.4/MANIFEST.in
--rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 06:18:13.902352 gunfolds-0.4/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)      293 2023-05-18 18:49:59.000000 gunfolds-0.4/README.md
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:18:13.878524 gunfolds-0.4/gunfolds/
--rw-r--r--   0 gm         (501) staff       (20)      401 2023-05-19 06:17:01.000000 gunfolds-0.4/gunfolds/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)    23098 2023-05-18 18:49:59.000000 gunfolds-0.4/gunfolds/conversions.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:18:13.899272 gunfolds-0.4/gunfolds/data/
--rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-05-18 18:49:59.000000 gunfolds-0.4/gunfolds/data/allloops.zkl
--rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-05-18 18:49:59.000000 gunfolds-0.4/gunfolds/data/circular_p.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3987 2023-05-18 18:49:59.000000 gunfolds-0.4/gunfolds/data/colors.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3691 2023-05-18 18:49:59.000000 gunfolds-0.4/gunfolds/data/testgraphs.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:18:13.901162 gunfolds-0.4/gunfolds/figures/
--rw-r--r--   0 gm         (501) staff       (20)     2976 2023-05-18 18:49:59.000000 gunfolds-0.4/gunfolds/figures/shipfig.tex
--rw-r--r--   0 gm         (501) staff       (20)     1412 2023-05-18 18:49:59.000000 gunfolds-0.4/gunfolds/figures/shippage.sty
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:18:13.879914 gunfolds-0.4/gunfolds.egg-info/
--rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 06:18:13.000000 gunfolds-0.4/gunfolds.egg-info/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)      456 2023-05-19 06:18:13.000000 gunfolds-0.4/gunfolds.egg-info/SOURCES.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 06:18:13.000000 gunfolds-0.4/gunfolds.egg-info/dependency_links.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 06:18:13.000000 gunfolds-0.4/gunfolds.egg-info/not-zip-safe
--rw-r--r--   0 gm         (501) staff       (20)       95 2023-05-19 06:18:13.000000 gunfolds-0.4/gunfolds.egg-info/requires.txt
--rw-r--r--   0 gm         (501) staff       (20)        9 2023-05-19 06:18:13.000000 gunfolds-0.4/gunfolds.egg-info/top_level.txt
--rw-r--r--   0 gm         (501) staff       (20)       38 2023-05-19 06:18:13.902629 gunfolds-0.4/setup.cfg
--rw-r--r--   0 gm         (501) staff       (20)     1239 2023-05-19 06:17:16.000000 gunfolds-0.4/setup.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:18:13.901497 gunfolds-0.4/tests/
--rw-r--r--   0 gm         (501) staff       (20)    20222 2023-05-18 18:49:59.000000 gunfolds-0.4/tests/tests.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:20:52.118277 gunfolds-0.5/
+-rw-r--r--   0 gm         (501) staff       (20)    35121 2023-05-18 18:49:59.000000 gunfolds-0.5/LICENSE
+-rw-r--r--   0 gm         (501) staff       (20)       50 2023-05-18 18:49:59.000000 gunfolds-0.5/MANIFEST.in
+-rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 19:20:52.118057 gunfolds-0.5/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)      293 2023-05-18 18:49:59.000000 gunfolds-0.5/README.md
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:20:52.100488 gunfolds-0.5/gunfolds/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-05-19 19:17:57.000000 gunfolds-0.5/gunfolds/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    23098 2023-05-18 18:49:59.000000 gunfolds-0.5/gunfolds/conversions.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:20:52.116378 gunfolds-0.5/gunfolds/data/
+-rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-05-18 18:49:59.000000 gunfolds-0.5/gunfolds/data/allloops.zkl
+-rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-05-18 18:49:59.000000 gunfolds-0.5/gunfolds/data/circular_p.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3987 2023-05-18 18:49:59.000000 gunfolds-0.5/gunfolds/data/colors.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3691 2023-05-18 18:49:59.000000 gunfolds-0.5/gunfolds/data/testgraphs.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:20:52.117186 gunfolds-0.5/gunfolds/figures/
+-rw-r--r--   0 gm         (501) staff       (20)     2976 2023-05-18 18:49:59.000000 gunfolds-0.5/gunfolds/figures/shipfig.tex
+-rw-r--r--   0 gm         (501) staff       (20)     1412 2023-05-18 18:49:59.000000 gunfolds-0.5/gunfolds/figures/shippage.sty
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:20:52.102061 gunfolds-0.5/gunfolds.egg-info/
+-rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 19:20:52.000000 gunfolds-0.5/gunfolds.egg-info/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)      456 2023-05-19 19:20:52.000000 gunfolds-0.5/gunfolds.egg-info/SOURCES.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:20:52.000000 gunfolds-0.5/gunfolds.egg-info/dependency_links.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:20:52.000000 gunfolds-0.5/gunfolds.egg-info/not-zip-safe
+-rw-r--r--   0 gm         (501) staff       (20)       95 2023-05-19 19:20:52.000000 gunfolds-0.5/gunfolds.egg-info/requires.txt
+-rw-r--r--   0 gm         (501) staff       (20)        9 2023-05-19 19:20:52.000000 gunfolds-0.5/gunfolds.egg-info/top_level.txt
+-rw-r--r--   0 gm         (501) staff       (20)       38 2023-05-19 19:20:52.118451 gunfolds-0.5/setup.cfg
+-rw-r--r--   0 gm         (501) staff       (20)     1239 2023-05-19 19:18:05.000000 gunfolds-0.5/setup.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:20:52.117431 gunfolds-0.5/tests/
+-rw-r--r--   0 gm         (501) staff       (20)    20222 2023-05-18 18:49:59.000000 gunfolds-0.5/tests/tests.py
```

### Comparing `gunfolds-0.4/LICENSE` & `gunfolds-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gunfolds-0.4/PKG-INFO` & `gunfolds-0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.4
+Version: 0.5
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.4/gunfolds/conversions.py` & `gunfolds-0.5/gunfolds/conversions.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.4/gunfolds/data/allloops.zkl` & `gunfolds-0.5/gunfolds/data/allloops.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.4/gunfolds/data/circular_p.zkl` & `gunfolds-0.5/gunfolds/data/circular_p.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.4/gunfolds/data/colors.zkl` & `gunfolds-0.5/gunfolds/data/colors.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.4/gunfolds/data/testgraphs.py` & `gunfolds-0.5/gunfolds/data/testgraphs.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.4/gunfolds/figures/shipfig.tex` & `gunfolds-0.5/gunfolds/figures/shipfig.tex`

 * *Files identical despite different names*

### Comparing `gunfolds-0.4/gunfolds/figures/shippage.sty` & `gunfolds-0.5/gunfolds/figures/shippage.sty`

 * *Files identical despite different names*

### Comparing `gunfolds-0.4/gunfolds.egg-info/PKG-INFO` & `gunfolds-0.5/gunfolds.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.4
+Version: 0.5
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.4/setup.py` & `gunfolds-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 tests_require = install_requires
 
 setup(
     name='gunfolds',
     description='Tools to explore dynamic causal graphs in the case of undersampled data',
     long_description_content_type="text/markdown",
-    version=0.4,
+    version=0.5,
     author='Sergey Plis, Cynthia Freeman, Ian Beaver',
     author_email='splis@mrn.org',
     license='GPL',
     long_description=description,
     include_package_data=True, # Include files listed in MANIFEST.in
     packages=['gunfolds'], # Sub-packages must be explicitly listed.
     #entry_points=epoints,
```

### Comparing `gunfolds-0.4/tests/tests.py` & `gunfolds-0.5/tests/tests.py`

 * *Files identical despite different names*

