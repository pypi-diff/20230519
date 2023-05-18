# Comparing `tmp/SplatStats-1.6.1.tar.gz` & `tmp/SplatStats-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-1.6.1.tar", last modified: Thu May 18 17:58:01 2023, max compression
+gzip compressed data, was "SplatStats-2.0.0.tar", last modified: Thu May 18 22:55:29 2023, max compression
```

## Comparing `SplatStats-1.6.1.tar` & `SplatStats-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 17:58:01.681049 SplatStats-1.6.1/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-1.6.1/LICENSE
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-18 17:58:01.680919 SplatStats-1.6.1/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6368 2023-05-11 17:29:12.000000 SplatStats-1.6.1/README.md
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 17:58:01.680097 SplatStats-1.6.1/SplatStats/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/Battle.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/Player.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/StatInk.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/Team.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13947 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-1.6.1/SplatStats/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/files.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/parsers.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/plotsAux.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/plotsTeam.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10176 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/statInkConstants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10543 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/statInkPlots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/statInkStats.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13991 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/stats.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 17:58:01.680734 SplatStats-1.6.1/SplatStats.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-05-18 17:58:01.681095 SplatStats-1.6.1/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-1.6.1/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 22:55:29.627820 SplatStats-2.0.0/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.0.0/LICENSE
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-18 22:55:29.627689 SplatStats-2.0.0/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6368 2023-05-11 17:29:12.000000 SplatStats-2.0.0/README.md
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 22:55:29.626755 SplatStats-2.0.0/SplatStats/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/Battle.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/Player.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/StatInk.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/Team.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-05-18 22:55:29.000000 SplatStats-2.0.0/SplatStats/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13972 2023-05-18 20:39:55.000000 SplatStats-2.0.0/SplatStats/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-2.0.0/SplatStats/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/files.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/parsers.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/plotsAux.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/plotsTeam.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10176 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/statInkConstants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10543 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/statInkPlots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/statInkStats.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13991 2023-05-11 17:29:12.000000 SplatStats-2.0.0/SplatStats/stats.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 22:55:29.627510 SplatStats-2.0.0/SplatStats.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-18 22:55:29.000000 SplatStats-2.0.0/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-05-18 22:55:29.000000 SplatStats-2.0.0/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-05-18 22:55:29.000000 SplatStats-2.0.0/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-05-18 22:55:29.000000 SplatStats-2.0.0/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-05-18 22:55:29.000000 SplatStats-2.0.0/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-05-18 22:55:29.627872 SplatStats-2.0.0/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.0.0/setup.py
```

### Comparing `SplatStats-1.6.1/LICENSE` & `SplatStats-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/PKG-INFO` & `SplatStats-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 1.6.1
+Version: 2.0.0
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-1.6.1/README.md` & `SplatStats-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/Battle.py` & `SplatStats-2.0.0/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/Player.py` & `SplatStats-2.0.0/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/StatInk.py` & `SplatStats-2.0.0/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/Team.py` & `SplatStats-2.0.0/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/__init__.py` & `SplatStats-2.0.0/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/auxiliary.py` & `SplatStats-2.0.0/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/colors.py` & `SplatStats-2.0.0/SplatStats/colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,15 @@
   ('#E1772B', '#1D07AC'), ('#A714D4', '#1D07AC'),
   ('#6BFF00', '#D01D79'), ('#AEF4F0', '#D01D79'),
   ('#6B87BF', '#D01D79'), ('#E1772B', '#D01D79'),
   ('#D01D79', '#1D07AC'), ('#6BFF00', '#1D07AC'),
   ('#E1772B', '#1D07AC'), ('#A714D4', '#1D07AC'),
   ('#6BFF00', '#D01D79'), ('#AEF4F0', '#D01D79'),
   ('#6B87BF', '#D01D79'), ('#E1772B', '#D01D79'),
+  ('#D01D79', '#1D07AC')
 )
 
 ###############################################################################
 # Auxiliary Functions
 ###############################################################################
 def colorPaletteFromHexList(clist):
     c = mcolors.ColorConverter().to_rgba
```

### Comparing `SplatStats-1.6.1/SplatStats/constants.py` & `SplatStats-2.0.0/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/files.py` & `SplatStats-2.0.0/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/parsers.py` & `SplatStats-2.0.0/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/plots.py` & `SplatStats-2.0.0/SplatStats/plots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/plotsAux.py` & `SplatStats-2.0.0/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/plotsTeam.py` & `SplatStats-2.0.0/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/statInkConstants.py` & `SplatStats-2.0.0/SplatStats/statInkConstants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/statInkPlots.py` & `SplatStats-2.0.0/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/statInkStats.py` & `SplatStats-2.0.0/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats/stats.py` & `SplatStats-2.0.0/SplatStats/stats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/SplatStats.egg-info/PKG-INFO` & `SplatStats-2.0.0/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 1.6.1
+Version: 2.0.0
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-1.6.1/SplatStats.egg-info/SOURCES.txt` & `SplatStats-2.0.0/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-1.6.1/setup.py` & `SplatStats-2.0.0/setup.py`

 * *Files identical despite different names*

