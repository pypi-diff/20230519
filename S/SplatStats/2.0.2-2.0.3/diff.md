# Comparing `tmp/SplatStats-2.0.2.tar.gz` & `tmp/SplatStats-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-2.0.2.tar", last modified: Fri May 19 00:44:03 2023, max compression
+gzip compressed data, was "SplatStats-2.0.3.tar", last modified: Fri May 19 17:13:56 2023, max compression
```

## Comparing `SplatStats-2.0.2.tar` & `SplatStats-2.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-19 00:44:03.237064 SplatStats-2.0.2/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.0.2/LICENSE
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-19 00:44:03.236927 SplatStats-2.0.2/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6368 2023-05-11 17:29:12.000000 SplatStats-2.0.2/README.md
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-19 00:44:03.235677 SplatStats-2.0.2/SplatStats/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/Battle.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/Player.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/StatInk.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/Team.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-05-19 00:44:03.000000 SplatStats-2.0.2/SplatStats/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13972 2023-05-18 20:39:55.000000 SplatStats-2.0.2/SplatStats/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-2.0.2/SplatStats/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/files.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/parsers.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/plotsAux.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/plotsTeam.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10176 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/statInkConstants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10588 2023-05-18 23:06:43.000000 SplatStats-2.0.2/SplatStats/statInkPlots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/statInkStats.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13991 2023-05-11 17:29:12.000000 SplatStats-2.0.2/SplatStats/stats.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-19 00:44:03.236722 SplatStats-2.0.2/SplatStats.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-19 00:44:03.000000 SplatStats-2.0.2/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-05-19 00:44:03.000000 SplatStats-2.0.2/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-05-19 00:44:03.000000 SplatStats-2.0.2/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-05-19 00:44:03.000000 SplatStats-2.0.2/SplatStats.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-05-19 00:44:03.000000 SplatStats-2.0.2/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-05-19 00:44:03.237121 SplatStats-2.0.2/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.0.2/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-19 17:13:56.499468 SplatStats-2.0.3/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.0.3/LICENSE
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-19 17:13:56.499333 SplatStats-2.0.3/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6368 2023-05-11 17:29:12.000000 SplatStats-2.0.3/README.md
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-19 17:13:56.498372 SplatStats-2.0.3/SplatStats/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/Battle.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/Player.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/StatInk.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/Team.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-05-19 17:13:56.000000 SplatStats-2.0.3/SplatStats/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13972 2023-05-18 20:39:55.000000 SplatStats-2.0.3/SplatStats/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-2.0.3/SplatStats/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/files.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/parsers.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/plotsAux.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/plotsTeam.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10176 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/statInkConstants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10588 2023-05-18 23:06:43.000000 SplatStats-2.0.3/SplatStats/statInkPlots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/statInkStats.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13991 2023-05-11 17:29:12.000000 SplatStats-2.0.3/SplatStats/stats.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-19 17:13:56.499145 SplatStats-2.0.3/SplatStats.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-19 17:13:56.000000 SplatStats-2.0.3/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-05-19 17:13:56.000000 SplatStats-2.0.3/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-05-19 17:13:56.000000 SplatStats-2.0.3/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-05-19 17:13:56.000000 SplatStats-2.0.3/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-05-19 17:13:56.000000 SplatStats-2.0.3/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-05-19 17:13:56.499512 SplatStats-2.0.3/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.0.3/setup.py
```

### Comparing `SplatStats-2.0.2/LICENSE` & `SplatStats-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/PKG-INFO` & `SplatStats-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.0.2
+Version: 2.0.3
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.0.2/README.md` & `SplatStats-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/Battle.py` & `SplatStats-2.0.3/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/Player.py` & `SplatStats-2.0.3/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/StatInk.py` & `SplatStats-2.0.3/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/Team.py` & `SplatStats-2.0.3/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/__init__.py` & `SplatStats-2.0.3/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/auxiliary.py` & `SplatStats-2.0.3/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/colors.py` & `SplatStats-2.0.3/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/constants.py` & `SplatStats-2.0.3/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/files.py` & `SplatStats-2.0.3/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/parsers.py` & `SplatStats-2.0.3/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/plots.py` & `SplatStats-2.0.3/SplatStats/plots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/plotsAux.py` & `SplatStats-2.0.3/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/plotsTeam.py` & `SplatStats-2.0.3/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/statInkConstants.py` & `SplatStats-2.0.3/SplatStats/statInkConstants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/statInkPlots.py` & `SplatStats-2.0.3/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/statInkStats.py` & `SplatStats-2.0.3/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats/stats.py` & `SplatStats-2.0.3/SplatStats/stats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/SplatStats.egg-info/PKG-INFO` & `SplatStats-2.0.3/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.0.2
+Version: 2.0.3
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.0.2/SplatStats.egg-info/SOURCES.txt` & `SplatStats-2.0.3/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.2/setup.py` & `SplatStats-2.0.3/setup.py`

 * *Files identical despite different names*

