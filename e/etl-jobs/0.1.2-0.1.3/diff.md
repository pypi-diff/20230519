# Comparing `tmp/etl_jobs-0.1.2.tar.gz` & `tmp/etl_jobs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_jobs-0.1.2.tar", max compression
+gzip compressed data, was "etl_jobs-0.1.3.tar", max compression
```

## Comparing `etl_jobs-0.1.2.tar` & `etl_jobs-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.2/etl_jobs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 15:06:18.864612 etl_jobs-0.1.2/etl_jobs/configuration/api_raw_data/__init__.py
--rw-r--r--   0        0        0      579 2023-05-19 15:08:39.448336 etl_jobs-0.1.2/etl_jobs/configuration/api_raw_data/apis.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.2/etl_jobs/jobs/extract/__init__.py
--rw-r--r--   0        0        0      692 2023-05-19 15:08:37.264792 etl_jobs-0.1.2/etl_jobs/jobs/extract/extract_data_api.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.2/etl_jobs/util/extract/__init__.py
--rw-r--r--   0        0        0      362 2023-05-19 15:08:39.349430 etl_jobs-0.1.2/etl_jobs/util/extract/api.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.2/etl_jobs/util/load/__init__.py
--rw-r--r--   0        0        0      305 2023-05-19 15:08:39.355246 etl_jobs-0.1.2/etl_jobs/util/load/delta_local.py
--rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.2/etl_jobs/util/transform/__init__.py
--rw-r--r--   0        0        0      444 2023-05-19 15:10:37.021525 etl_jobs-0.1.2/etl_jobs/util/transform/polar_bear.py
--rw-r--r--   0        0        0      499 2023-05-19 15:14:24.493832 etl_jobs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.2/README.md
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 etl_jobs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.3/etl_jobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:06:18.864612 etl_jobs-0.1.3/etl_jobs/configuration/api_raw_data/__init__.py
+-rw-r--r--   0        0        0      781 2023-05-19 15:58:55.374031 etl_jobs-0.1.3/etl_jobs/configuration/api_raw_data/apis.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.3/etl_jobs/jobs/extract/__init__.py
+-rw-r--r--   0        0        0      741 2023-05-19 15:59:22.196896 etl_jobs-0.1.3/etl_jobs/jobs/extract/extract_data_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.3/etl_jobs/util/extract/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-19 15:08:39.349430 etl_jobs-0.1.3/etl_jobs/util/extract/api.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.3/etl_jobs/util/load/__init__.py
+-rw-r--r--   0        0        0      305 2023-05-19 15:08:39.355246 etl_jobs-0.1.3/etl_jobs/util/load/delta_local.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:11:57.777000 etl_jobs-0.1.3/etl_jobs/util/transform/__init__.py
+-rw-r--r--   0        0        0      444 2023-05-19 15:10:37.021525 etl_jobs-0.1.3/etl_jobs/util/transform/polar_bear.py
+-rw-r--r--   0        0        0      499 2023-05-19 15:59:42.799709 etl_jobs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 15:39:00.637598 etl_jobs-0.1.3/README.md
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 etl_jobs-0.1.3/PKG-INFO
```

### Comparing `etl_jobs-0.1.2/etl_jobs/configuration/api_raw_data/apis.py` & `etl_jobs-0.1.3/etl_jobs/configuration/api_raw_data/apis.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 
 
 class restConfig(abc.ABC):
     """
     fill in
 
     """
-
-    url = "dev"
+    name = ""
+    url = ""
 
 
 @dataclass
 class MachineRestConfiguration(restConfig):
     """
     fill in
     """
-
-    url = "dev"
+    name = "bronze_maine_raw"
+    url = "https://my.api.mockaroo.com/machine.json"
 
 
 class SalesRestConfiguration(restConfig):
     """
     fill in
     """
-
-    url = "dev"
+    name = "bronze_sales"
+    url = "https://my.api.mockaroo.com/sales.json"
 
 
 class BronzeSapBsegRestConfiguration(restConfig):
     """
     fill in
     """
-
-    url = "dev"
+    name = "bronze_sap_bseg"
+    url = "https://my.api.mockaroo.com/sap_bseg.json"
 
 
 Apis = [
     MachineRestConfiguration,
     BronzeSapBsegRestConfiguration,
     SalesRestConfiguration,
 ]
```

