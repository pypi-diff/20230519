# Comparing `tmp/refractio-1.0.3.tar.gz` & `tmp/refractio-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-1.0.3.tar", last modified: Tue May  9 10:20:07 2023, max compression
+gzip compressed data, was "refractio-2.0.0.tar", last modified: Fri May 19 12:18:01 2023, max compression
```

## Comparing `refractio-1.0.3.tar` & `refractio-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-09 10:20:07.309095 refractio-1.0.3/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1124 2023-05-09 10:20:07.309095 refractio-1.0.3/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      564 2023-05-09 10:18:35.000000 refractio-1.0.3/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-09 10:20:07.308096 refractio-1.0.3/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-09 10:18:23.000000 refractio-1.0.3/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13351 2023-05-09 10:18:35.000000 refractio-1.0.3/refractio/refractio.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-09 10:20:07.308096 refractio-1.0.3/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1124 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      227 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-09 10:20:07.000000 refractio-1.0.3/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-09 10:20:07.309095 refractio-1.0.3/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     2125 2023-05-09 10:18:35.000000 refractio-1.0.3/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-19 12:18:01.303391 refractio-2.0.0/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     2356 2023-05-19 12:18:01.303391 refractio-2.0.0/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1687 2023-05-19 12:16:37.000000 refractio-2.0.0/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-19 12:18:01.301391 refractio-2.0.0/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      231 2023-05-19 12:16:37.000000 refractio-2.0.0/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4707 2023-05-19 12:16:37.000000 refractio-2.0.0/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3875 2023-05-19 12:16:37.000000 refractio-2.0.0/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-19 12:16:26.000000 refractio-2.0.0/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13446 2023-05-19 12:16:26.000000 refractio-2.0.0/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-19 12:16:37.000000 refractio-2.0.0/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-19 12:16:26.000000 refractio-2.0.0/refractio/snowflake.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-19 12:18:01.302390 refractio-2.0.0/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     2356 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      326 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-19 12:18:01.000000 refractio-2.0.0/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-19 12:18:01.303391 refractio-2.0.0/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1807 2023-05-19 12:16:37.000000 refractio-2.0.0/setup.py
```

### Comparing `refractio-1.0.3/refractio/refractio.py` & `refractio-2.0.0/refractio/refractio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #! -*- coding: utf-8 -*-
 """Library to read and write dataframes"""
 
 import os
 import requests
 import pandas as pd
 
+from .manager import validate_project_id
+
 
 def get_dataframe(ds_name, project_id=os.getenv("project_id"), row_count=-1, strategy="top", user_id="1001"):
     """
     Param:
         ds_name,
         project_id=os.getenv("project_id"),
         row_count=-1,
         strategy="top"
         user_id="1001"
     To get pandas dataframe.
     Need to install mosaic-connector-python for reading dataframe using connector backend,
     git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git@1.0.29.3
     """
     try:
+        project_id = validate_project_id(project_id)
         url = f"http://connection-manager:80/connections/api/External/v1/external/getConnConfig/" \
               f"{ds_name}/refract_user/{project_id}"    # user id hard coded, as it's not being used in API code.
         connection_details = requests.get(url, verify=False).json()
 
         if connection_details["params"]["READER"]["type"] == "RDBMS":
             if connection_details["params"]["READER"]["sub_type"] == "SNOWFLAKE":
                 data_frame = get_snowflake_df(connection_details, row_count, strategy)
```

