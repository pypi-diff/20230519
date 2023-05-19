# Comparing `tmp/gunfolds-0.6.tar.gz` & `tmp/gunfolds-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunfolds-0.6.tar", last modified: Fri May 19 19:36:36 2023, max compression
+gzip compressed data, was "gunfolds-0.7.tar", last modified: Fri May 19 19:54:55 2023, max compression
```

## Comparing `gunfolds-0.6.tar` & `gunfolds-0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:36:36.011087 gunfolds-0.6/
--rw-r--r--   0 gm         (501) staff       (20)    35121 2023-05-18 18:49:59.000000 gunfolds-0.6/LICENSE
--rw-r--r--   0 gm         (501) staff       (20)       50 2023-05-18 18:49:59.000000 gunfolds-0.6/MANIFEST.in
--rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 19:36:36.010883 gunfolds-0.6/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)      293 2023-05-18 18:49:59.000000 gunfolds-0.6/README.md
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:36:35.994198 gunfolds-0.6/gunfolds/
--rw-r--r--   0 gm         (501) staff       (20)       28 2023-05-19 19:34:12.000000 gunfolds-0.6/gunfolds/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)    23098 2023-05-18 18:49:59.000000 gunfolds-0.6/gunfolds/conversions.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:36:36.008309 gunfolds-0.6/gunfolds/data/
--rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-05-18 18:49:59.000000 gunfolds-0.6/gunfolds/data/allloops.zkl
--rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-05-18 18:49:59.000000 gunfolds-0.6/gunfolds/data/circular_p.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3987 2023-05-18 18:49:59.000000 gunfolds-0.6/gunfolds/data/colors.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3691 2023-05-18 18:49:59.000000 gunfolds-0.6/gunfolds/data/testgraphs.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:36:36.009695 gunfolds-0.6/gunfolds/figures/
--rw-r--r--   0 gm         (501) staff       (20)     2976 2023-05-18 18:49:59.000000 gunfolds-0.6/gunfolds/figures/shipfig.tex
--rw-r--r--   0 gm         (501) staff       (20)     1412 2023-05-18 18:49:59.000000 gunfolds-0.6/gunfolds/figures/shippage.sty
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:36:35.995480 gunfolds-0.6/gunfolds.egg-info/
--rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 19:36:35.000000 gunfolds-0.6/gunfolds.egg-info/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)      456 2023-05-19 19:36:35.000000 gunfolds-0.6/gunfolds.egg-info/SOURCES.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:36:35.000000 gunfolds-0.6/gunfolds.egg-info/dependency_links.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:36:35.000000 gunfolds-0.6/gunfolds.egg-info/not-zip-safe
--rw-r--r--   0 gm         (501) staff       (20)       95 2023-05-19 19:36:35.000000 gunfolds-0.6/gunfolds.egg-info/requires.txt
--rw-r--r--   0 gm         (501) staff       (20)        9 2023-05-19 19:36:35.000000 gunfolds-0.6/gunfolds.egg-info/top_level.txt
--rw-r--r--   0 gm         (501) staff       (20)       38 2023-05-19 19:36:36.011158 gunfolds-0.6/setup.cfg
--rw-r--r--   0 gm         (501) staff       (20)     1239 2023-05-19 19:34:20.000000 gunfolds-0.6/setup.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:36:36.009941 gunfolds-0.6/tests/
--rw-r--r--   0 gm         (501) staff       (20)    20222 2023-05-18 18:49:59.000000 gunfolds-0.6/tests/tests.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.350335 gunfolds-0.7/
+-rw-r--r--   0 gm         (501) staff       (20)    35121 2023-05-18 18:49:59.000000 gunfolds-0.7/LICENSE
+-rw-r--r--   0 gm         (501) staff       (20)       50 2023-05-18 18:49:59.000000 gunfolds-0.7/MANIFEST.in
+-rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 19:54:55.350117 gunfolds-0.7/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)      293 2023-05-18 18:49:59.000000 gunfolds-0.7/README.md
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.333399 gunfolds-0.7/gunfolds/
+-rw-r--r--   0 gm         (501) staff       (20)       92 2023-05-19 19:54:10.000000 gunfolds-0.7/gunfolds/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    23098 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/conversions.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.347693 gunfolds-0.7/gunfolds/data/
+-rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/data/allloops.zkl
+-rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/data/circular_p.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3987 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/data/colors.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3691 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/data/testgraphs.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.349164 gunfolds-0.7/gunfolds/figures/
+-rw-r--r--   0 gm         (501) staff       (20)     2976 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/figures/shipfig.tex
+-rw-r--r--   0 gm         (501) staff       (20)     1412 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/figures/shippage.sty
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.334698 gunfolds-0.7/gunfolds.egg-info/
+-rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)      456 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/SOURCES.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/dependency_links.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/not-zip-safe
+-rw-r--r--   0 gm         (501) staff       (20)       95 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/requires.txt
+-rw-r--r--   0 gm         (501) staff       (20)        9 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/top_level.txt
+-rw-r--r--   0 gm         (501) staff       (20)       38 2023-05-19 19:54:55.350421 gunfolds-0.7/setup.cfg
+-rw-r--r--   0 gm         (501) staff       (20)     1239 2023-05-19 19:54:21.000000 gunfolds-0.7/setup.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.349456 gunfolds-0.7/tests/
+-rw-r--r--   0 gm         (501) staff       (20)    20222 2023-05-18 18:49:59.000000 gunfolds-0.7/tests/tests.py
```

### Comparing `gunfolds-0.6/LICENSE` & `gunfolds-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gunfolds-0.6/PKG-INFO` & `gunfolds-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.6
+Version: 0.7
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.6/gunfolds/conversions.py` & `gunfolds-0.7/gunfolds/conversions.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.6/gunfolds/data/allloops.zkl` & `gunfolds-0.7/gunfolds/data/allloops.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.6/gunfolds/data/circular_p.zkl` & `gunfolds-0.7/gunfolds/data/circular_p.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.6/gunfolds/data/colors.zkl` & `gunfolds-0.7/gunfolds/data/colors.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.6/gunfolds/data/testgraphs.py` & `gunfolds-0.7/gunfolds/data/testgraphs.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.6/gunfolds/figures/shipfig.tex` & `gunfolds-0.7/gunfolds/figures/shipfig.tex`

 * *Files identical despite different names*

### Comparing `gunfolds-0.6/gunfolds/figures/shippage.sty` & `gunfolds-0.7/gunfolds/figures/shippage.sty`

 * *Files identical despite different names*

### Comparing `gunfolds-0.6/gunfolds.egg-info/PKG-INFO` & `gunfolds-0.7/gunfolds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.6
+Version: 0.7
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.6/setup.py` & `gunfolds-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 tests_require = install_requires
 
 setup(
     name='gunfolds',
     description='Tools to explore dynamic causal graphs in the case of undersampled data',
     long_description_content_type="text/markdown",
-    version=0.6,
+    version=0.7,
     author='Sergey Plis, Cynthia Freeman, Ian Beaver',
     author_email='splis@mrn.org',
     license='GPL',
     long_description=description,
     include_package_data=True, # Include files listed in MANIFEST.in
     packages=['gunfolds'], # Sub-packages must be explicitly listed.
     #entry_points=epoints,
```

### Comparing `gunfolds-0.6/tests/tests.py` & `gunfolds-0.7/tests/tests.py`

 * *Files identical despite different names*

