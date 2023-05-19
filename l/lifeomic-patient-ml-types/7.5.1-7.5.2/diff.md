# Comparing `tmp/lifeomic_patient_ml_types-7.5.1.tar.gz` & `tmp/lifeomic_patient_ml_types-7.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.5.1.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.5.2.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.5.1.tar` & `lifeomic_patient_ml_types-7.5.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13974 2023-05-05 09:39:38.254231 lifeomic_patient_ml_types-7.5.1/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-05-05 09:40:54.262696 lifeomic_patient_ml_types-7.5.1/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.1/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.1/PKG-INFO
+-rw-r--r--   0        0        0    14150 2023-05-19 21:47:09.063811 lifeomic_patient_ml_types-7.5.2/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-05-19 21:48:24.752074 lifeomic_patient_ml_types-7.5.2/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.2/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.2/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.5.1/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.5.2/lifeomic_patient_ml_types/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,14 +562,18 @@
     """
     Timestamp of when the run started. Expressed as milliseconds since the UTC epoch.
     """
     end: Optional[float] = None
     """
     Timestamp of when the run ended. Expressed as milliseconds since the UTC epoch.
     """
+    isArchived: Optional[bool] = None
+    """
+    True if this run has been archived. Archived runs' related artifacts are deleted, and they can no longer be deployed.
+    """
     splits: Optional[RunSplits] = None
     hyperparameters: List[Parameter]
     """
     The hyperparameters used to train the model version created by this run.
     """
     metrics: RunMetrics
     approvals: List[ApprovalDecision]
```

### Comparing `lifeomic_patient_ml_types-7.5.1/pyproject.toml` & `lifeomic_patient_ml_types-7.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.5.1"
+version = "7.5.2"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

### Comparing `lifeomic_patient_ml_types-7.5.1/setup.py` & `lifeomic_patient_ml_types-7.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '7.5.1',
+    'version': '7.5.2',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

