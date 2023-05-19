# Comparing `tmp/caft-0.1.1.tar.gz` & `tmp/caft-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caft-0.1.1.tar", last modified: Thu May 18 19:38:29 2023, max compression
+gzip compressed data, was "caft-0.1.6.tar", last modified: Fri May 19 09:13:51 2023, max compression
```

## Comparing `caft-0.1.1.tar` & `caft-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.633545 caft-0.1.1/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1068 2023-05-05 11:28:23.000000 caft-0.1.1/LICENSE
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)      129 2023-05-18 19:27:10.000000 caft-0.1.1/MANIFEST.in
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     4313 2023-05-18 19:38:29.633653 caft-0.1.1/PKG-INFO
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     3253 2023-05-18 18:47:12.000000 caft-0.1.1/README.md
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.629586 caft-0.1.1/caft/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)       22 2023-05-18 19:31:17.000000 caft-0.1.1/caft/__init__.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1609 2023-05-17 21:50:03.000000 caft-0.1.1/caft/affine.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     7340 2023-05-17 09:20:27.000000 caft-0.1.1/caft/equation.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     3885 2023-05-17 20:49:12.000000 caft-0.1.1/caft/npoc.py
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.631045 caft-0.1.1/caft.egg-info/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     4313 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/PKG-INFO
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)      466 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/SOURCES.txt
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)        1 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/dependency_links.txt
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)       70 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/requires.txt
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)       11 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/top_level.txt
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.631460 caft-0.1.1/img/
--rw-------   0 Josh.Dunn   (504) staff       (20)    42606 2023-05-18 18:39:36.000000 caft-0.1.1/img/affine_transformed_scatter.png
--rw-------   0 Josh.Dunn   (504) staff       (20)    22050 2023-05-18 18:34:12.000000 caft-0.1.1/img/fx_scatter_plot.png
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)       98 2023-05-05 11:28:23.000000 caft-0.1.1/pyproject.toml
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)      107 2023-05-18 19:38:29.633954 caft-0.1.1/setup.cfg
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1941 2023-05-17 22:31:58.000000 caft-0.1.1/setup.py
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.632084 caft-0.1.1/tests/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)        0 2023-05-05 11:28:23.000000 caft-0.1.1/tests/__init__.py
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.633189 caft-0.1.1/tests/tests_caft/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)        0 2023-05-16 22:01:44.000000 caft-0.1.1/tests/tests_caft/__init__.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)      912 2023-05-17 21:37:54.000000 caft-0.1.1/tests/tests_caft/test_affine.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1627 2023-05-18 18:27:26.000000 caft-0.1.1/tests/tests_caft/test_equation.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1528 2023-05-17 20:25:03.000000 caft-0.1.1/tests/tests_caft/test_npoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:13:51.251978 caft-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 09:13:37.000000 caft-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-19 09:13:37.000000 caft-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-19 09:13:51.251978 caft-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-19 09:13:37.000000 caft-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:13:51.251978 caft-0.1.6/caft/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 09:13:37.000000 caft-0.1.6/caft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-19 09:13:37.000000 caft-0.1.6/caft/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-05-19 09:13:37.000000 caft-0.1.6/caft/equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-19 09:13:37.000000 caft-0.1.6/caft/npoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:13:51.251978 caft-0.1.6/caft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-19 09:13:51.000000 caft-0.1.6/caft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-19 09:13:51.000000 caft-0.1.6/caft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:13:51.000000 caft-0.1.6/caft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 09:13:51.000000 caft-0.1.6/caft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 09:13:51.000000 caft-0.1.6/caft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:13:51.251978 caft-0.1.6/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-05-19 09:13:37.000000 caft-0.1.6/img/affine_transformed_scatter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-05-19 09:13:37.000000 caft-0.1.6/img/fx_scatter_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 09:13:37.000000 caft-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 09:13:51.251978 caft-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 09:13:37.000000 caft-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:13:51.251978 caft-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:13:37.000000 caft-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:13:51.251978 caft-0.1.6/tests/tests_caft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:13:37.000000 caft-0.1.6/tests/tests_caft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-19 09:13:37.000000 caft-0.1.6/tests/tests_caft/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-19 09:13:37.000000 caft-0.1.6/tests/tests_caft/test_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-19 09:13:37.000000 caft-0.1.6/tests/tests_caft/test_npoc.py
```

### Comparing `caft-0.1.1/LICENSE` & `caft-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/PKG-INFO` & `caft-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caft
-Version: 0.1.1
+Version: 0.1.6
 Summary: Continuous Affine Feature Transformations for feature mapping.
 Home-page: https://github.com/joshdunnlime/caft
 Author: Joshua Dunn
 Author-email: joshua.t.dunn@hotmail.co.uk
 Project-URL: Documentation, https://github.com/joshdunnlime/caft
 Project-URL: Bug Reports, https://github.com/joshdunnlime/caft/issues
 Project-URL: Source Code, https://github.com/joshdunnlime/caft
```

### Comparing `caft-0.1.1/README.md` & `caft-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/caft/affine.py` & `caft-0.1.6/caft/affine.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/caft/equation.py` & `caft-0.1.6/caft/equation.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/caft/npoc.py` & `caft-0.1.6/caft/npoc.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/caft.egg-info/PKG-INFO` & `caft-0.1.6/caft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caft
-Version: 0.1.1
+Version: 0.1.6
 Summary: Continuous Affine Feature Transformations for feature mapping.
 Home-page: https://github.com/joshdunnlime/caft
 Author: Joshua Dunn
 Author-email: joshua.t.dunn@hotmail.co.uk
 Project-URL: Documentation, https://github.com/joshdunnlime/caft
 Project-URL: Bug Reports, https://github.com/joshdunnlime/caft/issues
 Project-URL: Source Code, https://github.com/joshdunnlime/caft
```

### Comparing `caft-0.1.1/img/affine_transformed_scatter.png` & `caft-0.1.6/img/affine_transformed_scatter.png`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/img/fx_scatter_plot.png` & `caft-0.1.6/img/fx_scatter_plot.png`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/setup.py` & `caft-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/tests/tests_caft/test_affine.py` & `caft-0.1.6/tests/tests_caft/test_affine.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/tests/tests_caft/test_equation.py` & `caft-0.1.6/tests/tests_caft/test_equation.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.1/tests/tests_caft/test_npoc.py` & `caft-0.1.6/tests/tests_caft/test_npoc.py`

 * *Files identical despite different names*

