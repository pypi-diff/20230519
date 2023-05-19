# Comparing `tmp/copyright_claim-0.0.1.tar.gz` & `tmp/copyright_claim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyright_claim-0.0.1.tar", max compression
+gzip compressed data, was "copyright_claim-0.0.2.tar", max compression
```

## Comparing `copyright_claim-0.0.1.tar` & `copyright_claim-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2543 2023-05-19 17:38:16.198249 copyright_claim-0.0.1/README.md
--rw-r--r--   0        0        0      114 2023-05-18 22:59:56.420566 copyright_claim-0.0.1/copyright_claim/__init__.py
--rw-r--r--   0        0        0     8128 2023-05-19 17:36:55.654300 copyright_claim-0.0.1/copyright_claim/copyright_claim.py
--rw-r--r--   0        0        0      311 2023-05-19 15:15:17.230093 copyright_claim-0.0.1/copyright_claim/dummy_copyright_claim.txt
--rw-r--r--   0        0        0      535 2023-05-18 23:08:11.343694 copyright_claim-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 copyright_claim-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2553 2023-05-19 18:02:58.062746 copyright_claim-0.0.2/README.md
+-rw-r--r--   0        0        0      114 2023-05-18 22:59:56.420566 copyright_claim-0.0.2/copyright_claim/__init__.py
+-rw-r--r--   0        0        0     8128 2023-05-19 17:36:55.654300 copyright_claim-0.0.2/copyright_claim/copyright_claim.py
+-rw-r--r--   0        0        0      311 2023-05-19 15:15:17.230093 copyright_claim-0.0.2/copyright_claim/dummy_copyright_claim.txt
+-rw-r--r--   0        0        0      535 2023-05-19 18:04:07.114981 copyright_claim-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3192 1970-01-01 00:00:00.000000 copyright_claim-0.0.2/PKG-INFO
```

### Comparing `copyright_claim-0.0.1/README.md` & `copyright_claim-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# npGUI
+# copyright-claim
 
 This very simple python package allows to add or remove copyright/license claims at
 the beginning of your  source files (single file use or whole folder use, the
 files being filtered based on their extensions).
 
  Yes it has only two functions !
```

### Comparing `copyright_claim-0.0.1/copyright_claim/copyright_claim.py` & `copyright_claim-0.0.2/copyright_claim/copyright_claim.py`

 * *Files identical despite different names*

### Comparing `copyright_claim-0.0.1/pyproject.toml` & `copyright_claim-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copyright-claim"
-version = "0.0.1"
+version = "0.0.2"
 description = "Adds and removes copyright claims at the beginning of text files."
 authors = ["Gaël Cousin <gcousin333@gmail.com>"]
 license = "BSD-2-Clause License"
 readme = "README.md"
 packages = [{include = "copyright_claim"}]
 
 [tool.poetry.dependencies]
```

### Comparing `copyright_claim-0.0.1/PKG-INFO` & `copyright_claim-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: copyright-claim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Adds and removes copyright claims at the beginning of text files.
 License: BSD-2-Clause License
 Author: Gaël Cousin
 Author-email: gcousin333@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-# npGUI
+# copyright-claim
 
 This very simple python package allows to add or remove copyright/license claims at
 the beginning of your  source files (single file use or whole folder use, the
 files being filtered based on their extensions).
 
  Yes it has only two functions !
```

