# Comparing `tmp/bifeatureanalysis-1.0.2.tar.gz` & `tmp/bifeatureanalysis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bifeatureanalysis-1.0.2.tar", last modified: Tue Jul 26 15:01:34 2022, max compression
+gzip compressed data, was "bifeatureanalysis-1.0.3.tar", last modified: Thu May 18 21:56:47 2023, max compression
```

## Comparing `bifeatureanalysis-1.0.2.tar` & `bifeatureanalysis-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-07-26 15:01:34.042812 bifeatureanalysis-1.0.2/
--rw-rw-rw-   0        0        0     1091 2022-07-25 21:48:24.000000 bifeatureanalysis-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1191 2022-07-26 15:01:34.041813 bifeatureanalysis-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      671 2022-07-25 21:55:17.000000 bifeatureanalysis-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-07-26 15:01:34.018814 bifeatureanalysis-1.0.2/bifeatureanalysis/
--rw-rw-rw-   0        0        0      273 2022-07-26 15:00:21.000000 bifeatureanalysis-1.0.2/bifeatureanalysis/__init__.py
--rw-rw-rw-   0        0        0      276 2022-07-25 21:48:24.000000 bifeatureanalysis-1.0.2/bifeatureanalysis/templateproj.py
-drwxrwxrwx   0        0        0        0 2022-07-26 15:01:34.036815 bifeatureanalysis-1.0.2/bifeatureanalysis.egg-info/
--rw-rw-rw-   0        0        0     1191 2022-07-26 15:01:33.000000 bifeatureanalysis-1.0.2/bifeatureanalysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2022-07-26 15:01:33.000000 bifeatureanalysis-1.0.2/bifeatureanalysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-26 15:01:33.000000 bifeatureanalysis-1.0.2/bifeatureanalysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-07-26 15:01:33.000000 bifeatureanalysis-1.0.2/bifeatureanalysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-07-25 21:48:24.000000 bifeatureanalysis-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-26 15:01:34.042812 bifeatureanalysis-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1132 2022-07-26 15:00:45.000000 bifeatureanalysis-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:56:47.782712 bifeatureanalysis-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-18 14:52:38.000000 bifeatureanalysis-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1195 2023-05-18 21:56:47.781204 bifeatureanalysis-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-05-18 14:54:19.000000 bifeatureanalysis-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 21:56:47.741405 bifeatureanalysis-1.0.3/bifeatureanalysis/
+-rw-rw-rw-   0        0        0     3252 2023-05-18 21:54:35.000000 bifeatureanalysis-1.0.3/bifeatureanalysis/RegressionLossFunc.py
+-rw-rw-rw-   0        0        0      494 2023-05-18 21:53:27.000000 bifeatureanalysis-1.0.3/bifeatureanalysis/__init__.py
+-rw-rw-rw-   0        0        0      350 2023-05-18 14:52:38.000000 bifeatureanalysis-1.0.3/bifeatureanalysis/aggregationfunc.py
+-rw-rw-rw-   0        0        0      346 2023-05-18 14:52:38.000000 bifeatureanalysis-1.0.3/bifeatureanalysis/templateproj.py
+drwxrwxrwx   0        0        0        0 2023-05-18 21:56:47.779214 bifeatureanalysis-1.0.3/bifeatureanalysis.egg-info/
+-rw-rw-rw-   0        0        0     1195 2023-05-18 21:56:47.000000 bifeatureanalysis-1.0.3/bifeatureanalysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-18 21:56:47.000000 bifeatureanalysis-1.0.3/bifeatureanalysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 21:56:47.000000 bifeatureanalysis-1.0.3/bifeatureanalysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-18 21:56:47.000000 bifeatureanalysis-1.0.3/bifeatureanalysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-05-18 14:52:38.000000 bifeatureanalysis-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 21:56:47.783742 bifeatureanalysis-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1409 2023-05-18 21:56:06.000000 bifeatureanalysis-1.0.3/setup.py
```

### Comparing `bifeatureanalysis-1.0.2/LICENSE` & `bifeatureanalysis-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bifeatureanalysis-1.0.2/PKG-INFO` & `bifeatureanalysis-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifeatureanalysis
-Version: 1.0.2
+Version: 1.0.3
 Summary: common usage in feature engineering analysis, make analysis more easily
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 Fast Analysis
 
 Ultimate Goal: Make Feature Engineering Analysis easy and fast as it should be.
 
 ## Installation
 
-`pip install fast-analysis`
+`pip install bifeatureanalysis`
 
 ## How to use it?
 
 Feature Engineering Analysis Common Usage Function List
 
 ## License
```

### Comparing `bifeatureanalysis-1.0.2/README.md` & `bifeatureanalysis-1.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Fast Analysis
 
 Ultimate Goal: Make Feature Engineering Analysis easy and fast as it should be.
 
 ## Installation
 
-`pip install fast-analysis`
+`pip install bifeatureanalysis`
 
 ## How to use it?
 
 Feature Engineering Analysis Common Usage Function List
 
 ## License
```

### Comparing `bifeatureanalysis-1.0.2/bifeatureanalysis.egg-info/PKG-INFO` & `bifeatureanalysis-1.0.3/bifeatureanalysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifeatureanalysis
-Version: 1.0.2
+Version: 1.0.3
 Summary: common usage in feature engineering analysis, make analysis more easily
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 Fast Analysis
 
 Ultimate Goal: Make Feature Engineering Analysis easy and fast as it should be.
 
 ## Installation
 
-`pip install fast-analysis`
+`pip install bifeatureanalysis`
 
 ## How to use it?
 
 Feature Engineering Analysis Common Usage Function List
 
 ## License
```

### Comparing `bifeatureanalysis-1.0.2/setup.py` & `bifeatureanalysis-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 '''
+Date         : 2023-05-18 10:52:38
+Author       : BDFD,bdfd2005@gmail.com
+Github       : https://github.com/bdfd
+LastEditTime : 2023-05-18 17:55:59
+LastEditors  : BDFD
+Description  : 
+FilePath     : \setup.py
+Copyright (c) 2023 by BDFD, All Rights Reserved. 
+'''
+'''
 Author:  BDFD
 Date: 2021-10-27 18:39:19
 LastEditTime: 2022-07-26 11:00:44
 LastEditors: BDFD
 Description: In User Settings Edit
 FilePath: \Section5.3-PyPi_Feature_Engineering\setup.py
 '''
+
 from setuptools import setup, find_packages
 import os
-
 here = os.path.abspath(os.path.dirname(__file__))
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'common usage in feature engineering analysis, make analysis more easily'
 PACKAGE_NAME = 'bifeatureanalysis'
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     author="BDFD",
```

