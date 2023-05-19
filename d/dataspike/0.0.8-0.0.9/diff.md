# Comparing `tmp/dataspike-0.0.8.tar.gz` & `tmp/dataspike-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspike-0.0.8.tar", last modified: Wed Apr  5 11:56:49 2023, max compression
+gzip compressed data, was "dataspike-0.0.9.tar", last modified: Fri May 19 13:25:53 2023, max compression
```

## Comparing `dataspike-0.0.8.tar` & `dataspike-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2038 2023-04-05 11:56:28.905099 dataspike-0.0.8/README.md
--rw-r--r--   0        0        0      201 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/__init__.py
--rw-r--r--   0        0        0      939 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/__version__.py
--rw-r--r--   0        0        0        0 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/aml/__init__.py
--rw-r--r--   0        0        0     1122 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/aml/aml.py
--rw-r--r--   0        0        0     8041 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/aml/model.py
--rw-r--r--   0        0        0       21 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/applicants/__init__.py
--rw-r--r--   0        0        0     3071 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/applicants/applicants.py
--rw-r--r--   0        0        0     1125 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/applicants/model.py
--rw-r--r--   0        0        0      255 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/common.py
--rw-r--r--   0        0        0     1993 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/dataspike.py
--rw-r--r--   0        0        0       21 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/documents/__init__.py
--rw-r--r--   0        0        0     3405 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/documents/documents.py
--rw-r--r--   0        0        0     1513 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/documents/model.py
--rw-r--r--   0        0        0      270 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/errors.py
--rw-r--r--   0        0        0      817 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/resource.py
--rw-r--r--   0        0        0        0 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/sdk/__init__.py
--rw-r--r--   0        0        0      683 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/sdk/sdk.py
--rw-r--r--   0        0        0     1744 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/syncapi.py
--rw-r--r--   0        0        0      902 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/utils.py
--rw-r--r--   0        0        0       21 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/verifications/__init__.py
--rw-r--r--   0        0        0     2986 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/verifications/model.py
--rw-r--r--   0        0        0     3333 2023-04-05 11:56:28.905099 dataspike-0.0.8/dataspike/verifications/verifications.py
--rw-r--r--   0        0        0     2439 2023-04-05 11:56:28.905099 dataspike-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2478 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0     2327 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/test_aml.py
--rw-r--r--   0        0        0     2895 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/test_applicants.py
--rw-r--r--   0        0        0     1625 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/test_documents.py
--rw-r--r--   0        0        0      557 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/test_json_encoder.py
--rw-r--r--   0        0        0      412 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/test_sdk.py
--rw-r--r--   0        0        0      546 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/test_sync.py
--rw-r--r--   0        0        0      631 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/test_verification_model.py
--rw-r--r--   0        0        0     2363 2023-04-05 11:56:28.905099 dataspike-0.0.8/tests/test_verifications.py
--rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 dataspike-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2038 2023-05-19 13:25:36.612684 dataspike-0.0.9/README.md
+-rw-r--r--   0        0        0      201 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/__version__.py
+-rw-r--r--   0        0        0        0 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/aml/__init__.py
+-rw-r--r--   0        0        0     1122 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/aml/aml.py
+-rw-r--r--   0        0        0     8041 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/aml/model.py
+-rw-r--r--   0        0        0       21 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/applicants/__init__.py
+-rw-r--r--   0        0        0     3071 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/applicants/applicants.py
+-rw-r--r--   0        0        0     1125 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/applicants/model.py
+-rw-r--r--   0        0        0      255 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/common.py
+-rw-r--r--   0        0        0     1993 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/dataspike.py
+-rw-r--r--   0        0        0       21 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/documents/__init__.py
+-rw-r--r--   0        0        0     3405 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/documents/documents.py
+-rw-r--r--   0        0        0     1513 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/documents/model.py
+-rw-r--r--   0        0        0      270 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/errors.py
+-rw-r--r--   0        0        0      817 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/resource.py
+-rw-r--r--   0        0        0        0 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/sdk/__init__.py
+-rw-r--r--   0        0        0      683 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/sdk/sdk.py
+-rw-r--r--   0        0        0     1744 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/syncapi.py
+-rw-r--r--   0        0        0      902 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/utils.py
+-rw-r--r--   0        0        0       21 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/verifications/__init__.py
+-rw-r--r--   0        0        0     3130 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/verifications/model.py
+-rw-r--r--   0        0        0     3333 2023-05-19 13:25:36.612684 dataspike-0.0.9/dataspike/verifications/verifications.py
+-rw-r--r--   0        0        0     2439 2023-05-19 13:25:36.612684 dataspike-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2478 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0     2327 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/test_aml.py
+-rw-r--r--   0        0        0     2895 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/test_applicants.py
+-rw-r--r--   0        0        0     1625 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/test_documents.py
+-rw-r--r--   0        0        0      557 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/test_json_encoder.py
+-rw-r--r--   0        0        0      412 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/test_sdk.py
+-rw-r--r--   0        0        0      546 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/test_sync.py
+-rw-r--r--   0        0        0      631 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/test_verification_model.py
+-rw-r--r--   0        0        0     2363 2023-05-19 13:25:36.612684 dataspike-0.0.9/tests/test_verifications.py
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 dataspike-0.0.9/PKG-INFO
```

### Comparing `dataspike-0.0.8/README.md` & `dataspike-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/__version__.py` & `dataspike-0.0.9/dataspike/__version__.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/aml/aml.py` & `dataspike-0.0.9/dataspike/aml/aml.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/aml/model.py` & `dataspike-0.0.9/dataspike/aml/model.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/applicants/applicants.py` & `dataspike-0.0.9/dataspike/applicants/applicants.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/applicants/model.py` & `dataspike-0.0.9/dataspike/applicants/model.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/dataspike.py` & `dataspike-0.0.9/dataspike/dataspike.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/documents/documents.py` & `dataspike-0.0.9/dataspike/documents/documents.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/documents/model.py` & `dataspike-0.0.9/dataspike/documents/model.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/resource.py` & `dataspike-0.0.9/dataspike/resource.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/sdk/sdk.py` & `dataspike-0.0.9/dataspike/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/syncapi.py` & `dataspike-0.0.9/dataspike/syncapi.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/utils.py` & `dataspike-0.0.9/dataspike/utils.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/dataspike/verifications/model.py` & `dataspike-0.0.9/dataspike/verifications/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     Visa = "visa"
     IdCard = "id_card"
     Liveness = "liveness_photo"
     ResidencePermit = "residence_permit"
     Selfie = "selfie"
     DriverLicense = "driver_license"
     Poa = "poa"
+    PoaUtilityBill = "poa_utility_bill"
+    PoaBankStatement = "poa_bank_statement"
+    PoaResidenceRegistration = "poa_residence_registration"
 
 
 class CheckStep(StrEnum):
     Ocr = "document_ocr"
     FaceComparison = "face_comparison"
     Liveness = "liveness"
     Mrz = "document_mrz"
```

### Comparing `dataspike-0.0.8/dataspike/verifications/verifications.py` & `dataspike-0.0.9/dataspike/verifications/verifications.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/pyproject.toml` & `dataspike-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
 ]
-version = "0.0.8"
+version = "0.0.9"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://dataspike.io"
 Repository = "https://github.com/dataspike-io/docver-sdk"
```

### Comparing `dataspike-0.0.8/tests/conftest.py` & `dataspike-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/tests/test_aml.py` & `dataspike-0.0.9/tests/test_aml.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/tests/test_applicants.py` & `dataspike-0.0.9/tests/test_applicants.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/tests/test_documents.py` & `dataspike-0.0.9/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/tests/test_json_encoder.py` & `dataspike-0.0.9/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/tests/test_sync.py` & `dataspike-0.0.9/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/tests/test_verification_model.py` & `dataspike-0.0.9/tests/test_verification_model.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/tests/test_verifications.py` & `dataspike-0.0.9/tests/test_verifications.py`

 * *Files identical despite different names*

### Comparing `dataspike-0.0.8/PKG-INFO` & `dataspike-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataspike
-Version: 0.0.8
+Version: 0.0.9
 Summary: The official wrapper for Dataspike API
 License: MIT
 Keywords: dataspike,kyc,identity
 Author-email: Sergey Rublev <sergey.rublev@dataspike.io>
 Requires-Python: >=3.8
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

