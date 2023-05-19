# Comparing `tmp/landmarkclassifier-2.0.1.tar.gz` & `tmp/landmarkclassifier-2.0.2.tar.gz`

## Comparing `landmarkclassifier-2.0.1.tar` & `landmarkclassifier-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/environment.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/LANDMark/LANDMark.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/LANDMark/__init__.py
--rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/LANDMark/lm_base_clfs.py
--rw-r--r--   0        0        0    21923 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/LANDMark/tree.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/LANDMark/utils.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/docs/API.md
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/tests/test_landmark.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/.gitignore
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/LICENSE
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/environment.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/LANDMark.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/__init__.py
+-rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/lm_base_clfs.py
+-rw-r--r--   0        0        0    21923 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/tree.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LANDMark/utils.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/docs/API.md
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/tests/test_landmark.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/README.md
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.2/PKG-INFO
```

### Comparing `landmarkclassifier-2.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `landmarkclassifier-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `landmarkclassifier-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/.github/workflows/ci.yml` & `landmarkclassifier-2.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/.github/workflows/python-publish.yml` & `landmarkclassifier-2.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/LANDMark/LANDMark.py` & `landmarkclassifier-2.0.2/LANDMark/LANDMark.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/LANDMark/lm_base_clfs.py` & `landmarkclassifier-2.0.2/LANDMark/lm_base_clfs.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/LANDMark/tree.py` & `landmarkclassifier-2.0.2/LANDMark/tree.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/LANDMark/utils.py` & `landmarkclassifier-2.0.2/LANDMark/utils.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/docs/API.md` & `landmarkclassifier-2.0.2/docs/API.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/docs/CONTRIBUTING.md` & `landmarkclassifier-2.0.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/tests/test_landmark.py` & `landmarkclassifier-2.0.2/tests/test_landmark.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/.gitignore` & `landmarkclassifier-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/LICENSE` & `landmarkclassifier-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/README.md` & `landmarkclassifier-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.1/pyproject.toml` & `landmarkclassifier-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "LANDMarkClassifier"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Teresita M. Porter"},
     {name = "Michael Wright"},
     {name = "G. Brian Golding"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
```

### Comparing `landmarkclassifier-2.0.1/PKG-INFO` & `landmarkclassifier-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LANDMarkClassifier
-Version: 2.0.1
+Version: 2.0.2
 Summary: LANDMark: An ensemble approach to the supervised selection of biomarkers in high-throughput sequencing data
 Project-URL: Homepage, https://github.com/jrudar/LANDMark
 Project-URL: Repository, https://github.com/jrudar/LANDMark.git
 Project-URL: Bug Tracker, https://github.com/jrudar/LANDMark/issues
 Author: Teresita M. Porter, Michael Wright, G. Brian Golding
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
```

