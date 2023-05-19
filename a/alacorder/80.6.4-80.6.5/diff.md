# Comparing `tmp/alacorder-80.6.4.tar.gz` & `tmp/alacorder-80.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.4.tar", max compression
+gzip compressed data, was "alacorder-80.6.5.tar", max compression
```

## Comparing `alacorder-80.6.4.tar` & `alacorder-80.6.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.4/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.4/README.md
--rw-r--r--   0        0        0      746 2023-05-18 17:49:14.768333 alacorder-80.6.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-18 17:49:24.483501 alacorder-80.6.4/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.4/src/alacorder/__init__.py
--rw-r--r--   0        0        0   234228 2023-05-18 17:48:17.428661 alacorder-80.6.4/src/alacorder/__main__.py
--rw-r--r--   0        0        0   234228 2023-05-18 17:48:12.889832 alacorder-80.6.4/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.5/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.5/README.md
+-rw-r--r--   0        0        0      746 2023-05-18 23:59:01.770650 alacorder-80.6.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-18 17:49:24.483501 alacorder-80.6.5/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.5/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:45.082490 alacorder-80.6.5/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.6.5/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.5/PKG-INFO
```

### Comparing `alacorder-80.6.4/LICENSE` & `alacorder-80.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.4/README.md` & `alacorder-80.6.5/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.4/pyproject.toml` & `alacorder-80.6.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.4"
+version = "80.6.5"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.4/src/alacorder/.DS_Store` & `alacorder-80.6.5/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.4/src/alacorder/__main__.py` & `alacorder-80.6.5/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.4"
+version = "80.6.5"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2417,14 +2417,21 @@
             .alias("ID"),
             pl.col("Description")
             .str.replace(r'^\.\d?\s','')
             .str.replace(r'\s[ASC]\s', " ")
             .str.replace(r'^[ASC]\s', "")
         ]
     )
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Charges").str.contains("WILLFUL FAILURE TO RETURN TO P"))
+            .then("")
+            .otherwise(pl.col("ID"))
+            .alias("ID")
+        ])
     charges = charges.fill_null('')
     charges = charges.with_columns(
         [
             pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
             pl.col("Category").cast(pl.Categorical),
             pl.col("TypeDescription").cast(pl.Categorical),
             pl.col("CourtAction").cast(pl.Categorical),
```

### Comparing `alacorder-80.6.4/src/alacorder/alac.py` & `alacorder-80.6.5/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.4"
+version = "80.6.5"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2417,14 +2417,21 @@
             .alias("ID"),
             pl.col("Description")
             .str.replace(r'^\.\d?\s','')
             .str.replace(r'\s[ASC]\s', " ")
             .str.replace(r'^[ASC]\s', "")
         ]
     )
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Charges").str.contains("WILLFUL FAILURE TO RETURN TO P"))
+            .then("")
+            .otherwise(pl.col("ID"))
+            .alias("ID")
+        ])
     charges = charges.fill_null('')
     charges = charges.with_columns(
         [
             pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
             pl.col("Category").cast(pl.Categorical),
             pl.col("TypeDescription").cast(pl.Categorical),
             pl.col("CourtAction").cast(pl.Categorical),
```

### Comparing `alacorder-80.6.4/PKG-INFO` & `alacorder-80.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.4
+Version: 80.6.5
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

