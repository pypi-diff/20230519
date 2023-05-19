# Comparing `tmp/discotoolkit-1.0.8.tar.gz` & `tmp/discotoolkit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.0.8.tar", last modified: Tue May 16 06:03:22 2023, max compression
+gzip compressed data, was "discotoolkit-1.0.9.tar", last modified: Fri May 19 08:11:45 2023, max compression
```

## Comparing `discotoolkit-1.0.8.tar` & `discotoolkit-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-16 06:03:11.017838 discotoolkit-1.0.8/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.8/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-16 06:03:11.013838 discotoolkit-1.0.8/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)     2599 2023-05-16 06:01:24.000000 discotoolkit-1.0.8/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-16 06:03:10.973838 discotoolkit-1.0.8/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)    17688 2023-05-16 05:02:50.000000 discotoolkit-1.0.8/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.8/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.0.8/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     7377 2023-05-15 05:29:07.000000 discotoolkit-1.0.8/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.0.8/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.8/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      130 2023-05-16 06:01:49.000000 discotoolkit-1.0.8/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-16 06:03:11.005838 discotoolkit-1.0.8/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)      106 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-16 06:03:11.017838 discotoolkit-1.0.8/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1052 2023-05-16 06:02:14.000000 discotoolkit-1.0.8/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-19 08:11:34.229661 discotoolkit-1.0.9/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.9/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-19 08:11:34.229661 discotoolkit-1.0.9/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2618 2023-05-18 08:04:18.000000 discotoolkit-1.0.9/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-19 08:11:34.197661 discotoolkit-1.0.9/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    17688 2023-05-16 05:02:50.000000 discotoolkit-1.0.9/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.9/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.0.9/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     7361 2023-05-18 08:03:41.000000 discotoolkit-1.0.9/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     4195 2023-05-19 08:07:31.000000 discotoolkit-1.0.9/discotoolkit/GeneSearch.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.0.9/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.9/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      156 2023-05-18 08:04:40.000000 discotoolkit-1.0.9/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-19 08:11:34.221661 discotoolkit-1.0.9/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-19 08:11:33.000000 discotoolkit-1.0.9/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      431 2023-05-19 08:11:33.000000 discotoolkit-1.0.9/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-19 08:11:33.000000 discotoolkit-1.0.9/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)      122 2023-05-19 08:11:33.000000 discotoolkit-1.0.9/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-19 08:11:33.000000 discotoolkit-1.0.9/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-19 08:11:34.233661 discotoolkit-1.0.9/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1052 2023-05-18 08:05:55.000000 discotoolkit-1.0.9/setup.py
```

### Comparing `discotoolkit-1.0.8/PKG-INFO` & `discotoolkit-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.8
+Version: 1.0.9
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 Requires-Python: >=3.8.16
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.         It provides the following functions
```

### Comparing `discotoolkit-1.0.8/README.md` & `discotoolkit-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
  * @Author: Mengwei Li
  * @Date: 2023-04-16 21:20:42
  * @LastEditors: Mengwei Li
  * @LastEditTime: 2023-04-16 21:22:03
 -->
 [![Documentation Status](https://readthedocs.org/projects/discotoolkit-py/badge/?version=latest)](https://discotoolkit-py.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/discotoolkit?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/discotoolkit) [![PyPI version](https://img.shields.io/pypi/v/discotoolkit)](https://pypi.org/project/discotoolkit)
 
-# DISCOtoolkit 1.0.8
+# DISCOtoolkit 1.0.9
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). Read the documentation [DISCOtoolkit](https://discotoolkit-py.readthedocs.io/en/latest/). It provides the following functions:
 
 - Filter and download DISCO data based on sample metadata and cell type information
 - CELLiD: cell type annotation
 - scEnrichment: geneset enrichment using DISCO DEGs
 
@@ -21,17 +21,21 @@
 - Numpy >= 1.21.6
 - Pandas >= 1.4.2
 - Scanpy >= 1.9.3
 - Scipy >= 1.8.0
 - joblib >= 1.1.0
 - pandarallel >= 1.6.5
 
-## Installation guide:
+## Minimal installation:
 
-we recommend to install miniconda first and install discotoolkit in virtual env
+The DISCOtoolkit can be easily installed in the current Python environment using `pip`:
+
+```
+pip install discotoolkit
+```
 
 ## Installation guide:
 
 we recommend to install miniconda first and install discotoolkit in virtual env
 
 ```
 conda create --name disco python=3.8
@@ -41,16 +45,14 @@
 ```
 ```
 conda install ipykernel
 ```
 ```
 python -m ipykernel install --user --name disco --display-name "disco"
 ```
-
-Installation using pip:
 ``` 
 python -m pip install discotoolkit # adding -U for installing the latest version
 ```
 
 ## Basic Usage
 Example in Jupyter notebook.
```

### Comparing `discotoolkit-1.0.8/discotoolkit/CELLiD.py` & `discotoolkit-1.0.9/discotoolkit/CELLiD.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.8/discotoolkit/DiscoClass.py` & `discotoolkit-1.0.9/discotoolkit/DiscoClass.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.8/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.0.9/discotoolkit/DownloadDiscoData.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # import libraries
 import requests
 import json
 import pandas as pd
 import re
 import os
 import hashlib
-import requests
 
 # import variable and class from other script
 from .GlobalVariable import logging, prefix_disco_url
 from .DiscoClass import FilterData, Filter
 from .GetMetadata import check_in_list
 
 def download_disco_data(metadata, output_dir : str = "DISCOtmp"):
```

### Comparing `discotoolkit-1.0.8/discotoolkit/GetMetadata.py` & `discotoolkit-1.0.9/discotoolkit/GetMetadata.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.8/discotoolkit/GlobalVariable.py` & `discotoolkit-1.0.9/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.8/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.0.9/discotoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.8
+Version: 1.0.9
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 Requires-Python: >=3.8.16
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.         It provides the following functions
```

### Comparing `discotoolkit-1.0.8/setup.py` & `discotoolkit-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='discotoolkit',
-    version="1.0.8",
+    version="1.0.9",
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
     install_requires=requirements,
     python_requires = '>=3.8.16',
```

