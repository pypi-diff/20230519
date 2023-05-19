# Comparing `tmp/helsing_scm-0.2.0.tar.gz` & `tmp/helsing_scm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helsing_scm-0.2.0.tar", max compression
+gzip compressed data, was "helsing_scm-0.2.1.tar", max compression
```

## Comparing `helsing_scm-0.2.0.tar` & `helsing_scm-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      998 2023-05-16 11:16:42.680037 helsing_scm-0.2.0/LICENSE
--rw-r--r--   0        0        0     3581 2023-05-17 00:36:39.323869 helsing_scm-0.2.0/README.md
--rw-r--r--   0        0        0     1675 2023-05-19 12:27:28.398825 helsing_scm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-19 12:27:28.398825 helsing_scm-0.2.0/src/helsing/scm/__init__.py
--rw-r--r--   0        0        0     2661 2023-05-19 12:25:21.926250 helsing_scm-0.2.0/src/helsing/scm/__main__.py
--rw-r--r--   0        0        0        0 2023-05-16 11:16:42.680037 helsing_scm-0.2.0/src/helsing/scm/py.typed
--rw-r--r--   0        0        0      161 2023-05-19 09:53:41.519631 helsing_scm-0.2.0/src/helsing/scm/resources/__init__.py
--rw-r--r--   0        0        0     1000 2023-05-19 12:19:18.312362 helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/AwsAccount.py
--rw-r--r--   0        0        0     3586 2023-05-19 12:19:25.152424 helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/TerraformWorkspace.py
--rw-r--r--   0        0        0      239 2023-05-19 09:53:41.559631 helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/__init__.py
--rw-r--r--   0        0        0     2070 2023-05-19 09:53:57.459709 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/__init__.py
--rw-r--r--   0        0        0      426 2023-05-19 09:53:57.475709 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/__init__.py
--rw-r--r--   0        0        0     2570 2023-05-19 09:53:57.487709 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/account_service.py
--rw-r--r--   0        0        0     2326 2023-05-19 12:24:16.217957 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/create_account.py
--rw-r--r--   0        0        0     4566 2023-05-19 12:21:07.165025 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/settings.py
--rw-r--r--   0        0        0      301 2023-05-19 09:53:57.467708 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/__init__.py
--rw-r--r--   0        0        0     1511 2023-05-19 09:53:41.519631 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/account_service.py
--rw-r--r--   0        0        0     4927 2023-05-19 12:24:28.730014 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/create_workspace.py
--rw-r--r--   0        0        0     1627 2023-05-19 12:23:49.733833 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/settings.py
--rw-r--r--   0        0        0      888 2023-05-16 13:22:02.179812 helsing_scm-0.2.0/src/helsing/scm/utils/develop.py
--rw-r--r--   0        0        0      680 2023-05-16 22:09:24.316728 helsing_scm-0.2.0/src/helsing/scm/utils/templating.py
--rw-r--r--   0        0        0      513 2023-05-16 13:57:46.413910 helsing_scm-0.2.0/src/helsing/scm/utils/types.py
--rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 helsing_scm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-05-16 11:16:42.680037 helsing_scm-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3581 2023-05-17 00:36:39.323869 helsing_scm-0.2.1/README.md
+-rw-r--r--   0        0        0     1675 2023-05-19 12:30:24.243631 helsing_scm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-19 12:30:24.243631 helsing_scm-0.2.1/src/helsing/scm/__init__.py
+-rw-r--r--   0        0        0     2661 2023-05-19 12:25:21.926250 helsing_scm-0.2.1/src/helsing/scm/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:16:42.680037 helsing_scm-0.2.1/src/helsing/scm/py.typed
+-rw-r--r--   0        0        0      161 2023-05-19 09:53:41.519631 helsing_scm-0.2.1/src/helsing/scm/resources/__init__.py
+-rw-r--r--   0        0        0     1000 2023-05-19 12:19:18.312362 helsing_scm-0.2.1/src/helsing/scm/resources/v1alpha/AwsAccount.py
+-rw-r--r--   0        0        0     3586 2023-05-19 12:19:25.152424 helsing_scm-0.2.1/src/helsing/scm/resources/v1alpha/TerraformWorkspace.py
+-rw-r--r--   0        0        0      239 2023-05-19 09:53:41.559631 helsing_scm-0.2.1/src/helsing/scm/resources/v1alpha/__init__.py
+-rw-r--r--   0        0        0     2070 2023-05-19 09:53:57.459709 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-19 09:53:57.475709 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/aws/__init__.py
+-rw-r--r--   0        0        0     2570 2023-05-19 09:53:57.487709 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/aws/account_service.py
+-rw-r--r--   0        0        0     2326 2023-05-19 12:24:16.217957 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/aws/create_account.py
+-rw-r--r--   0        0        0     4566 2023-05-19 12:21:07.165025 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/aws/settings.py
+-rw-r--r--   0        0        0      301 2023-05-19 09:53:57.467708 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/tfe/__init__.py
+-rw-r--r--   0        0        0     1511 2023-05-19 09:53:41.519631 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/tfe/account_service.py
+-rw-r--r--   0        0        0     4927 2023-05-19 12:24:28.730014 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/tfe/create_workspace.py
+-rw-r--r--   0        0        0     1627 2023-05-19 12:23:49.733833 helsing_scm-0.2.1/src/helsing/scm/tfcodegen/tfe/settings.py
+-rw-r--r--   0        0        0      888 2023-05-16 13:22:02.179812 helsing_scm-0.2.1/src/helsing/scm/utils/develop.py
+-rw-r--r--   0        0        0      680 2023-05-16 22:09:24.316728 helsing_scm-0.2.1/src/helsing/scm/utils/templating.py
+-rw-r--r--   0        0        0      513 2023-05-16 13:57:46.413910 helsing_scm-0.2.1/src/helsing/scm/utils/types.py
+-rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 helsing_scm-0.2.1/PKG-INFO
```

### Comparing `helsing_scm-0.2.0/LICENSE` & `helsing_scm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/README.md` & `helsing_scm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/pyproject.toml` & `helsing_scm-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "helsing-scm"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "helsing/scm", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `helsing_scm-0.2.0/src/helsing/scm/__main__.py` & `helsing_scm-0.2.1/src/helsing/scm/__main__.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/AwsAccount.py` & `helsing_scm-0.2.1/src/helsing/scm/resources/v1alpha/AwsAccount.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/TerraformWorkspace.py` & `helsing_scm-0.2.1/src/helsing/scm/resources/v1alpha/TerraformWorkspace.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/__init__.py` & `helsing_scm-0.2.1/src/helsing/scm/tfcodegen/__init__.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/account_service.py` & `helsing_scm-0.2.1/src/helsing/scm/tfcodegen/aws/account_service.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/create_account.py` & `helsing_scm-0.2.1/src/helsing/scm/tfcodegen/aws/create_account.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/settings.py` & `helsing_scm-0.2.1/src/helsing/scm/tfcodegen/aws/settings.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/account_service.py` & `helsing_scm-0.2.1/src/helsing/scm/tfcodegen/tfe/account_service.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/create_workspace.py` & `helsing_scm-0.2.1/src/helsing/scm/tfcodegen/tfe/create_workspace.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/settings.py` & `helsing_scm-0.2.1/src/helsing/scm/tfcodegen/tfe/settings.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/utils/develop.py` & `helsing_scm-0.2.1/src/helsing/scm/utils/develop.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/utils/templating.py` & `helsing_scm-0.2.1/src/helsing/scm/utils/templating.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/src/helsing/scm/utils/types.py` & `helsing_scm-0.2.1/src/helsing/scm/utils/types.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.2.0/PKG-INFO` & `helsing_scm-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helsing-scm
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

