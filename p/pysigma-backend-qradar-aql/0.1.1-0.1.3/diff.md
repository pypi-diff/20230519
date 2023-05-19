# Comparing `tmp/pysigma_backend_qradar_aql-0.1.1.tar.gz` & `tmp/pysigma_backend_qradar_aql-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_qradar_aql-0.1.1.tar", max compression
+gzip compressed data, was "pysigma_backend_qradar_aql-0.1.3.tar", max compression
```

## Comparing `pysigma_backend_qradar_aql-0.1.1.tar` & `pysigma_backend_qradar_aql-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2023-05-11 10:26:27.440460 pysigma_backend_qradar_aql-0.1.1/LICENSE
--rw-r--r--   0        0        0    26783 2023-05-15 06:32:47.289519 pysigma_backend_qradar_aql-0.1.1/README.md
--rw-r--r--   0        0        0      539 2023-05-15 11:49:39.931911 pysigma_backend_qradar_aql-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    18776 2023-05-14 09:29:21.546257 pysigma_backend_qradar_aql-0.1.1/sigma/backends/QRadarAQL/QRadarAQL.py
--rw-r--r--   0        0        0      247 2023-05-15 06:54:27.240323 pysigma_backend_qradar_aql-0.1.1/sigma/backends/QRadarAQL/__init__.py
--rw-r--r--   0        0        0    24281 2023-05-14 09:29:21.547589 pysigma_backend_qradar_aql-0.1.1/sigma/pipelines/QRadarAQL/QRadarAQL.py
--rw-r--r--   0        0        0     1466 2023-05-10 20:46:57.641000 pysigma_backend_qradar_aql-0.1.1/sigma/pipelines/QRadarAQL/QRadarAQL_fields.py
--rw-r--r--   0        0        0     5230 2023-05-14 09:29:21.548462 pysigma_backend_qradar_aql-0.1.1/sigma/pipelines/QRadarAQL/QRadarAQL_payload.py
--rw-r--r--   0        0        0      238 2023-05-15 06:54:27.232430 pysigma_backend_qradar_aql-0.1.1/sigma/pipelines/QRadarAQL/__init__.py
--rw-r--r--   0        0        0    27495 1970-01-01 00:00:00.000000 pysigma_backend_qradar_aql-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-11 10:26:27.440460 pysigma_backend_qradar_aql-0.1.3/LICENSE
+-rw-r--r--   0        0        0    26893 2023-05-18 15:50:26.457194 pysigma_backend_qradar_aql-0.1.3/README.md
+-rw-r--r--   0        0        0      539 2023-05-19 13:59:12.906094 pysigma_backend_qradar_aql-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    18776 2023-05-14 09:29:21.546257 pysigma_backend_qradar_aql-0.1.3/sigma/backends/QRadarAQL/QRadarAQL.py
+-rw-r--r--   0        0        0      251 2023-05-18 15:03:35.537046 pysigma_backend_qradar_aql-0.1.3/sigma/backends/QRadarAQL/__init__.py
+-rw-r--r--   0        0        0    24281 2023-05-14 09:29:21.547589 pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL.py
+-rw-r--r--   0        0        0     1466 2023-05-10 20:46:57.641000 pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL_fields.py
+-rw-r--r--   0        0        0     5230 2023-05-14 09:29:21.548462 pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL_payload.py
+-rw-r--r--   0        0        0      238 2023-05-15 06:54:27.232430 pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/__init__.py
+-rw-r--r--   0        0        0    27605 1970-01-01 00:00:00.000000 pysigma_backend_qradar_aql-0.1.3/PKG-INFO
```

### Comparing `pysigma_backend_qradar_aql-0.1.1/LICENSE` & `pysigma_backend_qradar_aql-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.1/README.md` & `pysigma_backend_qradar_aql-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 Installation can be done using Sigma's plugins after installing [sigma-cli](https://github.com/SigmaHQ/sigma-cli#Installation)
 ```
 sigma plugin install QRadarAQL
 ```
 
 ## Usage
 
-### Usage via [Sigma-CLI](https://github.com/SigmaHQ/sigma-cli#usage)
-Use `QRadarAQL` as backend, and one of `QRadarAQL_fields` and `QRadarAQL_payload` as pipeline.
+### Usage via Sigma-CLI
+Convert Sigma rules to AQL by using `ibm-qradar-aql` as backend, and one of `qradar-aql-fields` and `qradar-aql-payload` as pipeline:
+```
+sigma convert -t ibm-qradar-aql -p <qradar-aql-fields | qradar-aql-payload> <rule path> -o <output file name>
+```
 
 ##### Input example:
 ```
-sigma convert -t QRadarAQL -p QRadarAQL_payload rules/windows/builtin/application/win_audit_cve.yml -o output_file.txt
+sigma convert -t ibm-qradar-aql -p qradar-aql-payload rules/windows/builtin/application/win_audit_cve.yml -o output_file.txt
 ```
 
 ##### Output example:
 ```
 ["SELECT * FROM events WHERE devicetype=12 AND (LOWER(UTF8(payload)) LIKE '%microsoft-windows-audit-cve%' OR LOWER(UTF8(payload)) LIKE '%audit-cve%') AND 'Event ID'=1"]
 ```
 
@@ -50,17 +53,17 @@
 rule = SigmaCollection.from_yaml("""
    logsource:
        category: process_access
        product: windows
    detection:
        selection:
           CallTrace|startswith: 'C:\Windows\System32\ntdll.dll+'
-           GrantedAccess:
-               - '0x1028'
-               - '0x1fffff'
+          GrantedAccess:
+            - '0x1028'
+            - '0x1fffff'
        condition: selection
 """)
 print(QRadarAQLBackend(pipeline()).convert(rule))
 ```
 
 ##### Output example:
 ```
```

### Comparing `pysigma_backend_qradar_aql-0.1.1/pyproject.toml` & `pysigma_backend_qradar_aql-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-QRadar-AQL"
-version = "0.1.1"
+version = "0.1.3"
 description = "pySigma QRadarAQL backend"
 authors = ["IBM <noaakless@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/IBM/pySigma-backend-QRadar-AQL"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_qradar_aql-0.1.1/sigma/backends/QRadarAQL/QRadarAQL.py` & `pysigma_backend_qradar_aql-0.1.3/sigma/backends/QRadarAQL/QRadarAQL.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.1/sigma/pipelines/QRadarAQL/QRadarAQL.py` & `pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.1/sigma/pipelines/QRadarAQL/QRadarAQL_fields.py` & `pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL_fields.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.1/sigma/pipelines/QRadarAQL/QRadarAQL_payload.py` & `pysigma_backend_qradar_aql-0.1.3/sigma/pipelines/QRadarAQL/QRadarAQL_payload.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.1.1/PKG-INFO` & `pysigma_backend_qradar_aql-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-qradar-aql
-Version: 0.1.1
+Version: 0.1.3
 Summary: pySigma QRadarAQL backend
 Home-page: https://github.com/IBM/pySigma-backend-QRadar-AQL
 License: MIT
 Author: IBM
 Author-email: noaakless@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -41,20 +41,23 @@
 Installation can be done using Sigma's plugins after installing [sigma-cli](https://github.com/SigmaHQ/sigma-cli#Installation)
 ```
 sigma plugin install QRadarAQL
 ```
 
 ## Usage
 
-### Usage via [Sigma-CLI](https://github.com/SigmaHQ/sigma-cli#usage)
-Use `QRadarAQL` as backend, and one of `QRadarAQL_fields` and `QRadarAQL_payload` as pipeline.
+### Usage via Sigma-CLI
+Convert Sigma rules to AQL by using `ibm-qradar-aql` as backend, and one of `qradar-aql-fields` and `qradar-aql-payload` as pipeline:
+```
+sigma convert -t ibm-qradar-aql -p <qradar-aql-fields | qradar-aql-payload> <rule path> -o <output file name>
+```
 
 ##### Input example:
 ```
-sigma convert -t QRadarAQL -p QRadarAQL_payload rules/windows/builtin/application/win_audit_cve.yml -o output_file.txt
+sigma convert -t ibm-qradar-aql -p qradar-aql-payload rules/windows/builtin/application/win_audit_cve.yml -o output_file.txt
 ```
 
 ##### Output example:
 ```
 ["SELECT * FROM events WHERE devicetype=12 AND (LOWER(UTF8(payload)) LIKE '%microsoft-windows-audit-cve%' OR LOWER(UTF8(payload)) LIKE '%audit-cve%') AND 'Event ID'=1"]
 ```
 
@@ -69,17 +72,17 @@
 rule = SigmaCollection.from_yaml("""
    logsource:
        category: process_access
        product: windows
    detection:
        selection:
           CallTrace|startswith: 'C:\Windows\System32\ntdll.dll+'
-           GrantedAccess:
-               - '0x1028'
-               - '0x1fffff'
+          GrantedAccess:
+            - '0x1028'
+            - '0x1fffff'
        condition: selection
 """)
 print(QRadarAQLBackend(pipeline()).convert(rule))
 ```
 
 ##### Output example:
 ```
```

