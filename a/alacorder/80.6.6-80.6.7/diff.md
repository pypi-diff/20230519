# Comparing `tmp/alacorder-80.6.6.tar.gz` & `tmp/alacorder-80.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.6.tar", max compression
+gzip compressed data, was "alacorder-80.6.7.tar", max compression
```

## Comparing `alacorder-80.6.6.tar` & `alacorder-80.6.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.6/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.6/README.md
--rw-r--r--   0        0        0      746 2023-05-19 14:45:01.586911 alacorder-80.6.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-19 14:45:18.802125 alacorder-80.6.6/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.6.6/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.6/src/alacorder/__init__.py
--rw-r--r--   0        0        0   234510 2023-05-19 14:44:47.423885 alacorder-80.6.6/src/alacorder/__main__.py
--rw-r--r--   0        0        0   234510 2023-05-19 14:44:52.583237 alacorder-80.6.6/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.7/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.7/README.md
+-rw-r--r--   0        0        0      746 2023-05-19 17:03:36.089471 alacorder-80.6.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-19 14:45:18.802125 alacorder-80.6.7/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.6.7/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.7/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   234772 2023-05-19 17:02:45.851868 alacorder-80.6.7/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   234772 2023-05-19 17:02:30.201314 alacorder-80.6.7/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.7/PKG-INFO
```

### Comparing `alacorder-80.6.6/LICENSE` & `alacorder-80.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.6/README.md` & `alacorder-80.6.7/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.6/pyproject.toml` & `alacorder-80.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.6"
+version = "80.6.7"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.6/src/alacorder/.DS_Store` & `alacorder-80.6.7/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.6/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.6.7/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.6/src/alacorder/__main__.py` & `alacorder-80.6.7/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.6"
+version = "80.6.7"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2419,14 +2419,22 @@
             .str.replace(r'^\.\d?\s','')
             .str.replace(r'\s[ASC]\s', " ")
             .str.replace(r'^[ASC]\s', "")
         ]
     )
     charges = charges.with_columns(
         [
+        pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
+        .then("CONSPIRACY -ROBBERY 1ST DEGREE")
+        .otherwise(pl.col("Description"))
+        .alias("Description")
+        ]
+    )
+    charges = charges.with_columns(
+        [
             pl.when(pl.col("Charges").str.contains("WILFULL FAILURE TO RETURN TO P"))
             .then("")
             .otherwise(pl.col("ID"))
             .alias("ID")
         ])
     charges = charges.fill_null('')
     charges = charges.with_columns(
```

### Comparing `alacorder-80.6.6/src/alacorder/alac.py` & `alacorder-80.6.7/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.6"
+version = "80.6.7"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2419,14 +2419,22 @@
             .str.replace(r'^\.\d?\s','')
             .str.replace(r'\s[ASC]\s', " ")
             .str.replace(r'^[ASC]\s', "")
         ]
     )
     charges = charges.with_columns(
         [
+        pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
+        .then("CONSPIRACY -ROBBERY 1ST DEGREE")
+        .otherwise(pl.col("Description"))
+        .alias("Description")
+        ]
+    )
+    charges = charges.with_columns(
+        [
             pl.when(pl.col("Charges").str.contains("WILFULL FAILURE TO RETURN TO P"))
             .then("")
             .otherwise(pl.col("ID"))
             .alias("ID")
         ])
     charges = charges.fill_null('')
     charges = charges.with_columns(
```

### Comparing `alacorder-80.6.6/PKG-INFO` & `alacorder-80.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.6
+Version: 80.6.7
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

