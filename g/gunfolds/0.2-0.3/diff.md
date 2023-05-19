# Comparing `tmp/gunfolds-0.2.tar.gz` & `tmp/gunfolds-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunfolds-0.2.tar", last modified: Thu May 18 20:25:35 2023, max compression
+gzip compressed data, was "gunfolds-0.3.tar", last modified: Fri May 19 06:13:20 2023, max compression
```

## Comparing `gunfolds-0.2.tar` & `gunfolds-0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-18 20:25:35.239407 gunfolds-0.2/
--rw-r--r--   0 gm         (501) staff       (20)    35121 2023-05-18 18:49:59.000000 gunfolds-0.2/LICENSE
--rw-r--r--   0 gm         (501) staff       (20)       50 2023-05-18 18:49:59.000000 gunfolds-0.2/MANIFEST.in
--rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-18 20:25:35.239243 gunfolds-0.2/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)      293 2023-05-18 18:49:59.000000 gunfolds-0.2/README.md
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-18 20:25:35.224337 gunfolds-0.2/gunfolds/
--rw-r--r--   0 gm         (501) staff       (20)      112 2023-05-18 20:11:55.000000 gunfolds-0.2/gunfolds/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)    23098 2023-05-18 18:49:59.000000 gunfolds-0.2/gunfolds/conversions.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-18 20:25:35.236515 gunfolds-0.2/gunfolds/data/
--rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-05-18 18:49:59.000000 gunfolds-0.2/gunfolds/data/allloops.zkl
--rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-05-18 18:49:59.000000 gunfolds-0.2/gunfolds/data/circular_p.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3987 2023-05-18 18:49:59.000000 gunfolds-0.2/gunfolds/data/colors.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3691 2023-05-18 18:49:59.000000 gunfolds-0.2/gunfolds/data/testgraphs.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-18 20:25:35.237771 gunfolds-0.2/gunfolds/figures/
--rw-r--r--   0 gm         (501) staff       (20)     2976 2023-05-18 18:49:59.000000 gunfolds-0.2/gunfolds/figures/shipfig.tex
--rw-r--r--   0 gm         (501) staff       (20)     1412 2023-05-18 18:49:59.000000 gunfolds-0.2/gunfolds/figures/shippage.sty
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-18 20:25:35.225430 gunfolds-0.2/gunfolds.egg-info/
--rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-18 20:25:35.000000 gunfolds-0.2/gunfolds.egg-info/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)      456 2023-05-18 20:25:35.000000 gunfolds-0.2/gunfolds.egg-info/SOURCES.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-18 20:25:35.000000 gunfolds-0.2/gunfolds.egg-info/dependency_links.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-18 20:25:35.000000 gunfolds-0.2/gunfolds.egg-info/not-zip-safe
--rw-r--r--   0 gm         (501) staff       (20)       95 2023-05-18 20:25:35.000000 gunfolds-0.2/gunfolds.egg-info/requires.txt
--rw-r--r--   0 gm         (501) staff       (20)        9 2023-05-18 20:25:35.000000 gunfolds-0.2/gunfolds.egg-info/top_level.txt
--rw-r--r--   0 gm         (501) staff       (20)       38 2023-05-18 20:25:35.239467 gunfolds-0.2/setup.cfg
--rw-r--r--   0 gm         (501) staff       (20)     1239 2023-05-18 20:25:22.000000 gunfolds-0.2/setup.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-18 20:25:35.237939 gunfolds-0.2/tests/
--rw-r--r--   0 gm         (501) staff       (20)    20222 2023-05-18 18:49:59.000000 gunfolds-0.2/tests/tests.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:13:20.820571 gunfolds-0.3/
+-rw-r--r--   0 gm         (501) staff       (20)    35121 2023-05-18 18:49:59.000000 gunfolds-0.3/LICENSE
+-rw-r--r--   0 gm         (501) staff       (20)       50 2023-05-18 18:49:59.000000 gunfolds-0.3/MANIFEST.in
+-rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 06:13:20.820354 gunfolds-0.3/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)      293 2023-05-18 18:49:59.000000 gunfolds-0.3/README.md
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:13:20.797537 gunfolds-0.3/gunfolds/
+-rw-r--r--   0 gm         (501) staff       (20)      400 2023-05-19 06:11:26.000000 gunfolds-0.3/gunfolds/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    23098 2023-05-18 18:49:59.000000 gunfolds-0.3/gunfolds/conversions.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:13:20.816402 gunfolds-0.3/gunfolds/data/
+-rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-05-18 18:49:59.000000 gunfolds-0.3/gunfolds/data/allloops.zkl
+-rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-05-18 18:49:59.000000 gunfolds-0.3/gunfolds/data/circular_p.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3987 2023-05-18 18:49:59.000000 gunfolds-0.3/gunfolds/data/colors.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3691 2023-05-18 18:49:59.000000 gunfolds-0.3/gunfolds/data/testgraphs.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:13:20.819512 gunfolds-0.3/gunfolds/figures/
+-rw-r--r--   0 gm         (501) staff       (20)     2976 2023-05-18 18:49:59.000000 gunfolds-0.3/gunfolds/figures/shipfig.tex
+-rw-r--r--   0 gm         (501) staff       (20)     1412 2023-05-18 18:49:59.000000 gunfolds-0.3/gunfolds/figures/shippage.sty
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:13:20.798872 gunfolds-0.3/gunfolds.egg-info/
+-rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 06:13:20.000000 gunfolds-0.3/gunfolds.egg-info/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)      456 2023-05-19 06:13:20.000000 gunfolds-0.3/gunfolds.egg-info/SOURCES.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 06:13:20.000000 gunfolds-0.3/gunfolds.egg-info/dependency_links.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 06:13:20.000000 gunfolds-0.3/gunfolds.egg-info/not-zip-safe
+-rw-r--r--   0 gm         (501) staff       (20)       95 2023-05-19 06:13:20.000000 gunfolds-0.3/gunfolds.egg-info/requires.txt
+-rw-r--r--   0 gm         (501) staff       (20)        9 2023-05-19 06:13:20.000000 gunfolds-0.3/gunfolds.egg-info/top_level.txt
+-rw-r--r--   0 gm         (501) staff       (20)       38 2023-05-19 06:13:20.820643 gunfolds-0.3/setup.cfg
+-rw-r--r--   0 gm         (501) staff       (20)     1239 2023-05-19 06:12:00.000000 gunfolds-0.3/setup.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 06:13:20.819759 gunfolds-0.3/tests/
+-rw-r--r--   0 gm         (501) staff       (20)    20222 2023-05-18 18:49:59.000000 gunfolds-0.3/tests/tests.py
```

### Comparing `gunfolds-0.2/LICENSE` & `gunfolds-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gunfolds-0.2/PKG-INFO` & `gunfolds-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.2
+Version: 0.3
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.2/gunfolds/conversions.py` & `gunfolds-0.3/gunfolds/conversions.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.2/gunfolds/data/allloops.zkl` & `gunfolds-0.3/gunfolds/data/allloops.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.2/gunfolds/data/circular_p.zkl` & `gunfolds-0.3/gunfolds/data/circular_p.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.2/gunfolds/data/colors.zkl` & `gunfolds-0.3/gunfolds/data/colors.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.2/gunfolds/data/testgraphs.py` & `gunfolds-0.3/gunfolds/data/testgraphs.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.2/gunfolds/figures/shipfig.tex` & `gunfolds-0.3/gunfolds/figures/shipfig.tex`

 * *Files identical despite different names*

### Comparing `gunfolds-0.2/gunfolds/figures/shippage.sty` & `gunfolds-0.3/gunfolds/figures/shippage.sty`

 * *Files identical despite different names*

### Comparing `gunfolds-0.2/gunfolds.egg-info/PKG-INFO` & `gunfolds-0.3/gunfolds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.2
+Version: 0.3
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.2/setup.py` & `gunfolds-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 tests_require = install_requires
 
 setup(
     name='gunfolds',
     description='Tools to explore dynamic causal graphs in the case of undersampled data',
     long_description_content_type="text/markdown",
-    version=0.2,
+    version=0.3,
     author='Sergey Plis, Cynthia Freeman, Ian Beaver',
     author_email='splis@mrn.org',
     license='GPL',
     long_description=description,
     include_package_data=True, # Include files listed in MANIFEST.in
     packages=['gunfolds'], # Sub-packages must be explicitly listed.
     #entry_points=epoints,
```

### Comparing `gunfolds-0.2/tests/tests.py` & `gunfolds-0.3/tests/tests.py`

 * *Files identical despite different names*

