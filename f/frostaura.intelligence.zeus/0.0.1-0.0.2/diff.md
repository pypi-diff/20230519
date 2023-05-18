# Comparing `tmp/frostaura.intelligence.zeus-0.0.1.tar.gz` & `tmp/frostaura.intelligence.zeus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frostaura.intelligence.zeus-0.0.1.tar", last modified: Thu May 18 21:15:14 2023, max compression
+gzip compressed data, was "frostaura.intelligence.zeus-0.0.2.tar", last modified: Thu May 18 22:32:21 2023, max compression
```

## Comparing `frostaura.intelligence.zeus-0.0.1.tar` & `frostaura.intelligence.zeus-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:14.823321 frostaura.intelligence.zeus-0.0.1/frostaura/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/frostaura/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/data_access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/data_access/modalities_data_access.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/data_access/modalities_data_access__telegram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/frostaura/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/engines/asset_calculations_engine__simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/engines/subordinate_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/frostaura/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/managers/zeus_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/managers/zeus_manager__telegram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/frostaura/models/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/models/profit_calculation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/models/symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/models/valuation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/models/visualization_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/frostaura/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/resources/easy_equities_us_exclusions.json
--rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/frostaura/resources/easy_equities_us_stocks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/frostaura.intelligence.zeus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-18 21:15:14.000000 frostaura.intelligence.zeus-0.0.1/frostaura.intelligence.zeus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 21:15:14.000000 frostaura.intelligence.zeus-0.0.1/frostaura.intelligence.zeus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:15:14.000000 frostaura.intelligence.zeus-0.0.1/frostaura.intelligence.zeus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 21:15:14.000000 frostaura.intelligence.zeus-0.0.1/frostaura.intelligence.zeus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:15:14.827321 frostaura.intelligence.zeus-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-18 21:15:03.000000 frostaura.intelligence.zeus-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/frostaura/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/frostaura/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/data_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/data_access/modalities_data_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/data_access/modalities_data_access__telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/frostaura/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/engines/asset_calculations_engine__simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/engines/subordinate_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/frostaura/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/managers/zeus_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/managers/zeus_manager__telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/frostaura/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/models/profit_calculation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/models/symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/models/valuation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/models/visualization_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/frostaura/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/resources/easy_equities_us_exclusions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/frostaura/resources/easy_equities_us_stocks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/frostaura.intelligence.zeus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-18 22:32:21.000000 frostaura.intelligence.zeus-0.0.2/frostaura.intelligence.zeus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 22:32:21.000000 frostaura.intelligence.zeus-0.0.2/frostaura.intelligence.zeus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:32:21.000000 frostaura.intelligence.zeus-0.0.2/frostaura.intelligence.zeus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 22:32:21.000000 frostaura.intelligence.zeus-0.0.2/frostaura.intelligence.zeus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:32:21.182727 frostaura.intelligence.zeus-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-18 22:32:10.000000 frostaura.intelligence.zeus-0.0.2/setup.py
```

### Comparing `frostaura.intelligence.zeus-0.0.1/PKG-INFO` & `frostaura.intelligence.zeus-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frostaura.intelligence.zeus
-Version: 0.0.1
+Version: 0.0.2
 Summary: FrostAura Zeus is an autonomous general purpose, multi-modal agent.
 Home-page: https://github.com/faGH/fa.intelligence.notebooks
 Author: Dean Martin
 Author-email: dean.martin@frostaura.net
 Keywords: frostaura,deep learning,machine learning,bots,agi,ai,llm
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `frostaura.intelligence.zeus-0.0.1/frostaura/data_access/modalities_data_access.py` & `frostaura.intelligence.zeus-0.0.2/frostaura/data_access/modalities_data_access.py`

 * *Files identical despite different names*

### Comparing `frostaura.intelligence.zeus-0.0.1/frostaura/data_access/modalities_data_access__telegram.py` & `frostaura.intelligence.zeus-0.0.2/frostaura/data_access/modalities_data_access__telegram.py`

 * *Files identical despite different names*

### Comparing `frostaura.intelligence.zeus-0.0.1/frostaura/models/symbol_data.py` & `frostaura.intelligence.zeus-0.0.2/frostaura/models/symbol_data.py`

 * *Files identical despite different names*

### Comparing `frostaura.intelligence.zeus-0.0.1/frostaura/models/valuation_result.py` & `frostaura.intelligence.zeus-0.0.2/frostaura/models/valuation_result.py`

 * *Files identical despite different names*

### Comparing `frostaura.intelligence.zeus-0.0.1/frostaura/resources/easy_equities_us_stocks.json` & `frostaura.intelligence.zeus-0.0.2/frostaura/resources/easy_equities_us_stocks.json`

 * *Files identical despite different names*

### Comparing `frostaura.intelligence.zeus-0.0.1/frostaura.intelligence.zeus.egg-info/PKG-INFO` & `frostaura.intelligence.zeus-0.0.2/frostaura.intelligence.zeus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frostaura.intelligence.zeus
-Version: 0.0.1
+Version: 0.0.2
 Summary: FrostAura Zeus is an autonomous general purpose, multi-modal agent.
 Home-page: https://github.com/faGH/fa.intelligence.notebooks
 Author: Dean Martin
 Author-email: dean.martin@frostaura.net
 Keywords: frostaura,deep learning,machine learning,bots,agi,ai,llm
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `frostaura.intelligence.zeus-0.0.1/frostaura.intelligence.zeus.egg-info/SOURCES.txt` & `frostaura.intelligence.zeus-0.0.2/frostaura.intelligence.zeus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frostaura.intelligence.zeus-0.0.1/setup.py` & `frostaura.intelligence.zeus-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 ROOT_DIR = Path(__file__).parent
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'FrostAura Zeus is an autonomous general purpose, multi-modal agent.'
 LONG_DESCRIPTION = DESCRIPTION #(ROOT_DIR / '../README.md').read_text()
 
 setup(
     name='frostaura.intelligence.zeus',
     version=VERSION,
     author='Dean Martin',
```

