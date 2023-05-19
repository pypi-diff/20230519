# Comparing `tmp/nigeria_banks-0.1.3.tar.gz` & `tmp/nigeria_banks-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nigeria_banks-0.1.3.tar", last modified: Sun Apr 23 23:57:39 2023, max compression
+gzip compressed data, was "nigeria_banks-0.1.5.tar", last modified: Fri May 19 15:34:37 2023, max compression
```

## Comparing `nigeria_banks-0.1.3.tar` & `nigeria_banks-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:39.566267 nigeria_banks-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-23 23:57:39.566267 nigeria_banks-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:39.562267 nigeria_banks-0.1.3/cbn_banks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/cbn_banks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/cbn_banks/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/cbn_banks/bank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:39.562267 nigeria_banks-0.1.3/cbn_banks/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/cbn_banks/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/cbn_banks/database/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:39.562267 nigeria_banks-0.1.3/nigeria_banks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/nigeria_banks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/nigeria_banks/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/nigeria_banks/bank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:39.566267 nigeria_banks-0.1.3/nigeria_banks/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/nigeria_banks/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61777 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/nigeria_banks/database/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:57:39.566267 nigeria_banks-0.1.3/nigeria_banks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-23 23:57:39.000000 nigeria_banks-0.1.3/nigeria_banks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-23 23:57:39.000000 nigeria_banks-0.1.3/nigeria_banks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:57:39.000000 nigeria_banks-0.1.3/nigeria_banks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 23:57:39.000000 nigeria_banks-0.1.3/nigeria_banks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 23:57:39.566267 nigeria_banks-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-23 23:57:29.000000 nigeria_banks-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.821495 nigeria_banks-0.1.5/cbn_banks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/bank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/cbn_banks/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/cbn_banks/database/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/nigeria_banks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/bank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/nigeria_banks/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62044 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/nigeria_banks/database/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/nigeria_banks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 15:34:37.000000 nigeria_banks-0.1.5/nigeria_banks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-19 15:34:37.000000 nigeria_banks-0.1.5/nigeria_banks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:34:37.000000 nigeria_banks-0.1.5/nigeria_banks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 15:34:37.000000 nigeria_banks-0.1.5/nigeria_banks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:34:37.825495 nigeria_banks-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-19 15:34:24.000000 nigeria_banks-0.1.5/setup.py
```

### Comparing `nigeria_banks-0.1.3/LICENSE` & `nigeria_banks-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.3/PKG-INFO` & `nigeria_banks-0.1.5/nigeria_banks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nigeria_banks
-Version: 0.1.3
+Name: nigeria-banks
+Version: 0.1.5
 Summary: Get details of specific bank in Nigeria
 Home-page: https://github.com/Josephchinedu/nigeria_banks
 Author: Devjoseph
 Author-email: joseph4jubilant@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nigeria_banks-0.1.3/README.md` & `nigeria_banks-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.3/cbn_banks/bank.py` & `nigeria_banks-0.1.5/cbn_banks/bank.py`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.3/cbn_banks/database/db.py` & `nigeria_banks-0.1.5/cbn_banks/database/db.py`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.3/nigeria_banks/bank.py` & `nigeria_banks-0.1.5/nigeria_banks/bank.py`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.3/nigeria_banks/database/db.py` & `nigeria_banks-0.1.5/nigeria_banks/database/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,332 +1,220 @@
 def bankdb():
     data = [
         {
-            "bank_code": "110005",
-            "cbn_code": "",
-            "name": "3Line",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
-        },
-        {
-            "bank_code": "",
-            "cbn_code": "120001",
-            "name": "9mobile 9Payment Service Bank",
-            "bank_short_name": "9mobile-9payment-service-bank-ng",
-            "ussd_code": "",
-            "bank_logo": "",
-        },
-        {
-            "bank_code": "",
-            "cbn_code": "035A",
-            "name": "ALAT by WEMA",
-            "bank_short_name": "alat-by-wema",
-            "ussd_code": "",
-            "bank_logo": "",
-        },
-        {
             "bank_code": "090116",
-            "cbn_code": "",
+            "cbn_code": "993",
             "name": "AMML MFB",
-            "bank_short_name": "",
+            "bank_short_name": "amml-mfb",
             "ussd_code": "",
-            "logo": "",
-        },
-        {
-            "bank_code": "",
-            "cbn_code": "51341",
-            "name": "AMPERSAND MICROFINANCE BANK",
-            "bank_short_name": "ampersand-microfinance-bank-ng",
-            "ussd_code": "",
-            "bank_logo": "",
-        },
-        {
-            "bank_code": "090270",
-            "cbn_code": "",
-            "name": "Ab MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/amml-mfb.png",
         },
         {
             "bank_code": "070010",
             "cbn_code": "801",
             "name": "Abbey Mortgage Bank",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
+            "bank_short_name": "abbey-mortgage-bank",
+            "ussd_code": "*332#",
+            "logo": "https://nigeria-banks.onrender.com/static/images/abbey-mortgage-bank.png",
         },
         {
             "bank_code": "090260",
             "cbn_code": "51204",
             "name": "Above Only MFB",
-            "bank_short_name": "",
+            "bank_short_name": "above-only-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/above-only-mfb.png",
         },
         {
             "bank_code": "090197",
-            "cbn_code": "",
+            "cbn_code": "606",
             "name": "Abu MFB",
-            "bank_short_name": "",
+            "bank_short_name": "abu_mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/abu_mfb.png",
         },
         {
-            "bank_code": "",
-            "cbn_code": "51312",
-            "name": "Abulesoro MFB",
-            "bank_short_name": "abulesoro-mfb-ng",
-            "ussd_code": "",
-            "bank_logo": "",
+            "bank_code": "090270",
+            "cbn_code": "613",
+            "name": "Ab MFB",
+            "bank_short_name": "ab-mfb",
+            "ussd_code": "*389*755#",
+            "logo": "https://nigeria-banks.onrender.com/static/images/ab-mfb.png",
         },
         {
             "bank_code": "000014",
             "cbn_code": "063",
             "name": "Access Bank Nigeria",
             "bank_short_name": "access",
             "ussd_code": "*901#",
             "logo": "https://nigeria-banks.onrender.com/static/images/access.png",
         },
         {
             "bank_code": "100052",
-            "cbn_code": "",
+            "cbn_code": "052",
             "name": "Access Yello and Beta",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
+            "bank_short_name": "access-yello-beta",
+            "ussd_code": "*901#",
+            "logo": "https://nigeria-banks.onrender.com/static/images/access-yello-beta.png",
         },
         {
             "bank_code": "100013",
             "cbn_code": "323",
             "name": "Accessmoney",
             "bank_short_name": "access-mobile",
-            "ussd_code": "",
-            "logo": "",
+            "ussd_code": "*901#",
+            "logo": "https://nigeria-banks.onrender.com/static/images/access-mobile.png",
         },
         {
             "bank_code": "090134",
             "cbn_code": "602",
             "name": "Accion MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
+            "bank_short_name": "accion-mfb",
+            "ussd_code": "*572#",
+            "logo": "https://nigeria-banks.onrender.com/static/images/accion-mfb.png",
         },
         {
             "bank_code": "090160",
-            "cbn_code": "",
+            "cbn_code": "975",
             "name": "Addosser MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
+            "bank_short_name": "addosser-mfb",
+            "ussd_code": "*258#",
+            "logo": "https://nigeria-banks.onrender.com/static/images/addosser-mfb.png",
         },
         {
             "bank_code": "090268",
-            "cbn_code": "",
+            "cbn_code": "618",
             "name": "Adeyemi College Staff MFB",
-            "bank_short_name": "",
+            "bank_short_name": "adeyemi-college-staff-mfb",
             "ussd_code": "",
-            "logo": "",
-        },
-        {
-            "bank_code": "090292",
-            "cbn_code": "",
-            "name": "Afekhafe MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/adeyemi-college-staff-mfb.png",
         },
         {
             "bank_code": "100028",
-            "cbn_code": "",
+            "cbn_code": "028",
             "name": "Ag Mortgage Bank",
-            "bank_short_name": "",
+            "bank_short_name": "ag-mortgage-bank",
             "ussd_code": "",
-            "logo": "",
-        },
-        {
-            "bank_code": "",
-            "cbn_code": "50036",
-            "name": "Ahmadu Bello University Microfinance Bank",
-            "bank_short_name": "ahmadu-bello-university-microfinance-bank-ng",
-            "ussd_code": "",
-            "bank_logo": "",
-        },
-        {
-            "bank_code": "",
-            "cbn_code": "120004",
-            "name": "Airtel Smartcash PSB",
-            "bank_short_name": "airtel-smartcash-psb-ng",
-            "ussd_code": "",
-            "bank_logo": "",
-        },
-        {
-            "bank_code": "090133",
-            "cbn_code": "",
-            "name": "Al-Barkah MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/ag-mortgage-bank.png",
         },
         {
             "bank_code": "090277",
-            "cbn_code": "",
+            "cbn_code": "51076",
             "name": "Al-Hayat MFB",
-            "bank_short_name": "",
+            "bank_short_name": "al-hayat-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/al-hayat-mfb.png",
         },
         {
             "bank_code": "090259",
-            "cbn_code": "",
+            "cbn_code": "608",
             "name": "Alekun MFB",
-            "bank_short_name": "",
+            "bank_short_name": "alekun-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/alekun-mfb.png",
         },
         {
             "bank_code": "090297",
-            "cbn_code": "",
+            "cbn_code": "642",
             "name": "Alert MFB",
-            "bank_short_name": "",
+            "bank_short_name": "alert-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/alert-mfb.png",
         },
         {
             "bank_code": "090131",
-            "cbn_code": "",
+            "cbn_code": "040",
             "name": "Allworkers MFB",
-            "bank_short_name": "",
+            "bank_short_name": "allworkers-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/allworkers-mfb.png",
         },
         {
             "bank_code": "090169",
-            "cbn_code": "",
+            "cbn_code": "584",
             "name": "Alpha Kapital MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
+            "bank_short_name": "alpha-mfb",
+            "ussd_code": "https://nigeria-banks.onrender.com/static/images/alpha-mfb.jpg",
             "logo": "",
         },
         {
             "bank_code": "090180",
             "cbn_code": "50926",
             "name": "Amju Unique MFB",
-            "bank_short_name": "",
+            "bank_short_name": "amju-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/amju-mfb.png",
         },
         {
             "bank_code": "090143",
-            "cbn_code": "",
+            "cbn_code": "986",
             "name": "Apeks MFB",
-            "bank_short_name": "",
+            "bank_short_name": "apeks-mfb",
             "ussd_code": "",
-            "logo": "",
-        },
-        {
-            "bank_code": "",
-            "cbn_code": "50083",
-            "name": "Aramoko MFB",
-            "bank_short_name": "aramoko-mfb",
-            "ussd_code": "",
-            "bank_logo": "",
-        },
-        {
-            "bank_code": "090282",
-            "cbn_code": "",
-            "name": "Arise MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/apeks-mfb.png",
         },
         {
             "bank_code": "090001",
             "cbn_code": "401",
             "name": "Aso Savings And Loans",
             "bank_short_name": "aso-savings",
             "ussd_code": "",
             "logo": "https://nigeria-banks.onrender.com/static/images/aso-savings.png",
         },
         {
-            "bank_code": "090287",
-            "cbn_code": "",
-            "name": "Assetmatrix MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
-        },
-        {
             "bank_code": "090172",
-            "cbn_code": "MFB50094",
+            "cbn_code": "631",
             "name": "Astrapolaris MFB",
-            "bank_short_name": "",
+            "bank_short_name": "astrapolaris-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/astrapolaris-mfb.png",
         },
         {
             "bank_code": "090264",
-            "cbn_code": "",
+            "cbn_code": "612",
             "name": "Auchi MFB",
-            "bank_short_name": "",
+            "bank_short_name": "auchi-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/auchi-mfb.png",
         },
         {
             "bank_code": "090127",
-            "cbn_code": "",
+            "cbn_code": "037",
             "name": "BC Kash MFB",
-            "bank_short_name": "",
+            "bank_short_name": "bc-kash-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/bc-kash-mfb.png",
         },
         {
             "bank_code": "090188",
-            "cbn_code": "",
+            "cbn_code": "593",
             "name": "Baines Credit MFB",
-            "bank_short_name": "",
+            "bank_short_name": "baines-mfb",
             "ussd_code": "",
-            "logo": "",
-        },
-        {
-            "bank_code": "",
-            "cbn_code": "51229",
-            "name": "Bainescredit MFB",
-            "bank_short_name": "bainescredit-mfb",
-            "ussd_code": "",
-            "bank_logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/baines-mfb.png",
         },
         {
             "bank_code": "090326",
-            "cbn_code": "",
+            "cbn_code": "647",
             "name": "Balogun Gambari MFB",
-            "bank_short_name": "",
-            "ussd_code": "",
-            "logo": "",
-        },
-        {
-            "bank_code": "",
-            "cbn_code": "50117",
-            "name": "Banc Corp Microfinance Bank",
-            "bank_short_name": "banc-corp-microfinance-bank-ng",
+            "bank_short_name": "balogun-mfb",
             "ussd_code": "",
-            "bank_logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/balogun-mfb.jpg",
         },
         {
             "bank_code": "090136",
-            "cbn_code": "",
+            "cbn_code": "577",
             "name": "Baobab MFB",
-            "bank_short_name": "",
+            "bank_short_name": "baobab-mfb",
             "ussd_code": "",
-            "logo": "",
+            "logo": "https://nigeria-banks.onrender.com/static/images/baobab-mfb.png",
         },
         {
             "bank_code": "090117",
-            "cbn_code": "",
+            "cbn_code": "581",
             "name": "Boctrust MFB",
             "bank_short_name": "",
             "ussd_code": "",
             "logo": "",
         },
         {
             "bank_code": "090176",
@@ -2199,7 +2087,83 @@
             "bank_short_name": "",
             "ussd_code": "",
             "logo": "",
         },
     ]
 
     return data
+
+
+"""
+ALL DETAILS NOT AVAILABLE FOR THIS BANKS:
+
+{
+    "bank_code": "110005",
+    "cbn_code": "",
+    "name": "3Line",
+    "bank_short_name": "3Line",
+    "ussd_code": "",
+    "logo": "https://nigeria-banks.onrender.com/static/images/3Line.png",
+},
+{
+    "bank_code": "",
+    "cbn_code": "120001",
+    "name": "9mobile 9Payment Service Bank",
+    "bank_short_name": "9psb",
+    "ussd_code": "*990#",
+    "bank_logo": "https://nigeria-banks.onrender.com/static/images/9psb.png",
+},
+
+{
+    "bank_code": "",
+    "cbn_code": "51341",
+    "name": "AMPERSAND MICROFINANCE BANK",
+    "bank_short_name": "ampersand-microfinance-bank-ng",
+    "ussd_code": "",
+    "bank_logo": "",
+},
+
+{
+    "bank_code": "",
+    "cbn_code": "51312",
+    "name": "Abulesoro MFB",
+    "bank_short_name": "abulesoro-mfb-ng",
+    "ussd_code": "",
+    "bank_logo": "",
+},
+
+{
+    "bank_code": "090292",
+    "cbn_code": "",
+    "name": "Afekhafe MFB",
+    "bank_short_name": "",
+    "ussd_code": "",
+    "logo": "",
+},
+
+{
+    "bank_code": "",
+    "cbn_code": "50036",
+    "name": "Ahmadu Bello University Microfinance Bank",
+    "bank_short_name": "ahmadu-bello-university-microfinance-bank-ng",
+    "ussd_code": "",
+    "bank_logo": "",
+},
+{
+    "bank_code": "",
+    "cbn_code": "120004",
+    "name": "Airtel Smartcash PSB",
+    "bank_short_name": "airtel-smartcash-psb-ng",
+    "ussd_code": "",
+    "bank_logo": "",
+},
+
+{
+            "bank_code": "090133",
+            "cbn_code": "",
+            "name": "Al-Barkah MFB",
+            "bank_short_name": "",
+            "ussd_code": "",
+            "logo": "",
+        },
+
+"""
```

### Comparing `nigeria_banks-0.1.3/nigeria_banks.egg-info/PKG-INFO` & `nigeria_banks-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nigeria-banks
-Version: 0.1.3
+Name: nigeria_banks
+Version: 0.1.5
 Summary: Get details of specific bank in Nigeria
 Home-page: https://github.com/Josephchinedu/nigeria_banks
 Author: Devjoseph
 Author-email: joseph4jubilant@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nigeria_banks-0.1.3/setup.py` & `nigeria_banks-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 NAME = 'nigeria_banks'
 DESCRIPTION = 'Get details of specific bank in Nigeria'
 URL = 'https://github.com/Josephchinedu/nigeria_banks'
 EMAIL = 'joseph4jubilant@gmail.com'
 AUTHOR = 'Devjoseph'
 REQUIRES_PYTHON = '>=3.7.9'
-VERSION = '0.1.3'
+VERSION = '0.1.5'
 
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
 EXTRAS = {
```

