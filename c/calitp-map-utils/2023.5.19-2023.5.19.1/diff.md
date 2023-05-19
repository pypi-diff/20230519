# Comparing `tmp/calitp_map_utils-2023.5.19.tar.gz` & `tmp/calitp_map_utils-2023.5.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.5.19.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.5.19.1.tar", max compression
```

## Comparing `calitp_map_utils-2023.5.19.tar` & `calitp_map_utils-2023.5.19.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      944 2023-05-18 19:13:08.501349 calitp_map_utils-2023.5.19/README.md
--rw-r--r--   0        0        0     3744 2023-05-19 14:49:58.954976 calitp_map_utils-2023.5.19/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0      647 2023-05-19 14:49:59.217026 calitp_map_utils-2023.5.19/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0      607 2023-05-19 14:50:45.923469 calitp_map_utils-2023.5.19/pyproject.toml
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.19/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-05-18 19:13:08.501349 calitp_map_utils-2023.5.19.1/README.md
+-rw-r--r--   0        0        0     3744 2023-05-19 14:49:58.954976 calitp_map_utils-2023.5.19.1/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-19 14:49:59.217026 calitp_map_utils-2023.5.19.1/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0      609 2023-05-19 14:57:17.278748 calitp_map_utils-2023.5.19.1/pyproject.toml
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.19.1/PKG-INFO
```

### Comparing `calitp_map_utils-2023.5.19/README.md` & `calitp_map_utils-2023.5.19.1/README.md`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.19/calitp_map_utils/__init__.py` & `calitp_map_utils-2023.5.19.1/calitp_map_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.19/calitp_map_utils/__main__.py` & `calitp_map_utils-2023.5.19.1/calitp_map_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.19/pyproject.toml` & `calitp_map_utils-2023.5.19.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.5.19"
+version = "2023.5.19.1"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 pyyaml = "^6.0"
 typer = "^0.9.0"
 pydantic = "^1.10.7"
 requests = "^2.30.0"
 tqdm = "^4.65.0"
 pycurl = "^7.45.2"
 urllib3 = "^2.0.2"
 geojson-pydantic = "^0.6.1"
-calitp-data = "2023.2.15.1"
+calitp-data = "2023.2.13.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pydantic-to-typescript = "^1.0.10"
 mypy = "^1.3.0"
 types-tqdm = "^4.65.0.1"
 types-requests = "^2.30.0.0"
```

### Comparing `calitp_map_utils-2023.5.19/PKG-INFO` & `calitp_map_utils-2023.5.19.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: calitp-map-utils
-Version: 2023.5.19
+Version: 2023.5.19.1
 Summary: 
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: calitp-data (==2023.2.15.1)
+Requires-Dist: calitp-data (==2023.2.13.1)
 Requires-Dist: geojson-pydantic (>=0.6.1,<0.7.0)
 Requires-Dist: pycurl (>=7.45.2,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

