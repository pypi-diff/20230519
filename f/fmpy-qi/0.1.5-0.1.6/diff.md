# Comparing `tmp/fmpy_qi-0.1.5.tar.gz` & `tmp/fmpy_qi-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmpy_qi-0.1.5.tar", last modified: Sun May 14 21:11:49 2023, max compression
+gzip compressed data, was "fmpy_qi-0.1.6.tar", last modified: Fri May 19 15:35:04 2023, max compression
```

## Comparing `fmpy_qi-0.1.5.tar` & `fmpy_qi-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-14 21:11:49.339775 fmpy_qi-0.1.5/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.5/LICENSE
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-14 21:11:49.339362 fmpy_qi-0.1.5/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2219 2023-05-14 19:24:52.000000 fmpy_qi-0.1.5/README.md
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-14 21:11:31.000000 fmpy_qi-0.1.5/pyproject.toml
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-14 21:11:49.339897 fmpy_qi-0.1.5/setup.cfg
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-14 21:11:49.333339 fmpy_qi-0.1.5/src/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.5/src/__init__.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-14 21:11:49.335641 fmpy_qi-0.1.5/src/fmpy/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.5/src/fmpy/__init__.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)    33683 2023-05-14 21:10:57.000000 fmpy_qi-0.1.5/src/fmpy/client.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)    12275 2023-05-14 20:08:21.000000 fmpy_qi-0.1.5/src/fmpy/urls.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      526 2023-05-14 19:02:44.000000 fmpy_qi-0.1.5/src/fmpy/utils.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-14 21:11:49.338753 fmpy_qi-0.1.5/src/fmpy_qi.egg-info/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-14 21:11:49.000000 fmpy_qi-0.1.5/src/fmpy_qi.egg-info/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-14 21:11:49.000000 fmpy_qi-0.1.5/src/fmpy_qi.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-14 21:11:49.000000 fmpy_qi-0.1.5/src/fmpy_qi.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-14 21:11:49.000000 fmpy_qi-0.1.5/src/fmpy_qi.egg-info/requires.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-14 21:11:49.000000 fmpy_qi-0.1.5/src/fmpy_qi.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-19 15:35:04.209633 fmpy_qi-0.1.6/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.6/LICENSE
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-19 15:35:04.209276 fmpy_qi-0.1.6/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2219 2023-05-14 19:24:52.000000 fmpy_qi-0.1.6/README.md
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-19 15:33:06.000000 fmpy_qi-0.1.6/pyproject.toml
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-19 15:35:04.209746 fmpy_qi-0.1.6/setup.cfg
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-19 15:35:04.204294 fmpy_qi-0.1.6/src/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.6/src/__init__.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-19 15:35:04.205575 fmpy_qi-0.1.6/src/fmpy/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.6/src/fmpy/__init__.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)    51492 2023-05-19 15:30:39.000000 fmpy_qi-0.1.6/src/fmpy/client.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)    12276 2023-05-19 13:07:09.000000 fmpy_qi-0.1.6/src/fmpy/urls.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      526 2023-05-14 19:02:44.000000 fmpy_qi-0.1.6/src/fmpy/utils.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-19 15:35:04.208793 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/requires.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/top_level.txt
```

### Comparing `fmpy_qi-0.1.5/LICENSE` & `fmpy_qi-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.5/PKG-INFO` & `fmpy_qi-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpy_qi
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fmpy_qi-0.1.5/README.md` & `fmpy_qi-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.5/pyproject.toml` & `fmpy_qi-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fmpy_qi"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Nicolas THIERY", email="nicles.thiery@gmail.com" },
 ]
 description = "A python wrapper for the Financial Modeling Prep API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `fmpy_qi-0.1.5/src/fmpy/urls.py` & `fmpy_qi-0.1.6/src/fmpy/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 GENERAL_NEWS = f'{API_V4_URL}/general_news'
 PRESS_RELEASES = f'{API_V3_URL}/press-releases'
 
 # MARKET PERFORMANCE
 SECTOR_PRICE_EARNING_RATIO = f'{API_V4_URL}/sector_price_earning_ratio'
 INDUSTRY_PRICE_EARNING_RATIO = f'{API_V4_URL}/industry_price_earning_ratio'
 SECTOR_PERFORMANCE = f'{API_V3_URL}/sector-performance'
-HISTORICAL_SECTOR_PERFORMANCE = f'{API_V3_URL}/historical-sector-performance'
+HISTORICAL_SECTOR_PERFORMANCE = f'{API_V3_URL}/historical-sectors-performance'
 MOST_GAINER_STOCK = f'{API_V3_URL}/stock_market/gainers'
 MOST_LOSER_STOCK = f'{API_V3_URL}/stock_market/losers'
 MOST_ACTIVE_STOCK = f'{API_V3_URL}/stock_market/actives'
 
 # ADVANCED DATA
 STANDARD_INDUSTRIAL_CLASSIFICATION = f'{API_V4_URL}/standard_industrial_classification'
 ALL_STANDARD_INDUSTRIAL_CLASSIFICATION = f'{API_V4_URL}/standard_industrial_classification/all'
```

### Comparing `fmpy_qi-0.1.5/src/fmpy/utils.py` & `fmpy_qi-0.1.6/src/fmpy/utils.py`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.5/src/fmpy_qi.egg-info/PKG-INFO` & `fmpy_qi-0.1.6/src/fmpy_qi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpy-qi
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

