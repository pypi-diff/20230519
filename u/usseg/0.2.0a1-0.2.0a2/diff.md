# Comparing `tmp/usseg-0.2.0a1.tar.gz` & `tmp/usseg-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usseg-0.2.0a1.tar", max compression
+gzip compressed data, was "usseg-0.2.0a2.tar", max compression
```

## Comparing `usseg-0.2.0a1.tar` & `usseg-0.2.0a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2831 2023-05-17 14:48:09.714561 usseg-0.2.0a1/README.md
--rw-r--r--   0        0        0      665 2023-05-18 10:18:19.531200 usseg-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0    53504 2023-05-17 12:58:04.630200 usseg-0.2.0a1/usseg/General_functions.py
--rw-r--r--   0        0        0     4115 2023-05-17 14:37:14.323870 usseg-0.2.0a1/usseg/Organise_files.py
--rw-r--r--   0        0        0    11405 2023-05-17 19:40:16.094684 usseg-0.2.0a1/usseg/Refined_anon_2_html.py
--rw-r--r--   0        0        0      303 2023-05-17 12:40:36.083145 usseg-0.2.0a1/usseg/__init__.py
--rw-r--r--   0        0        0      857 2023-05-18 10:07:46.451007 usseg-0.2.0a1/usseg/main.py
--rw-r--r--   0        0        0     4914 2023-05-17 14:12:40.206489 usseg-0.2.0a1/usseg/visualisation_html.py
--rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 usseg-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-05-17 14:48:09.714561 usseg-0.2.0a2/README.md
+-rw-r--r--   0        0        0      703 2023-05-18 10:26:45.709016 usseg-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0    53504 2023-05-17 12:58:04.630200 usseg-0.2.0a2/usseg/General_functions.py
+-rw-r--r--   0        0        0     4115 2023-05-17 14:37:14.323870 usseg-0.2.0a2/usseg/Organise_files.py
+-rw-r--r--   0        0        0    11405 2023-05-17 19:40:16.094684 usseg-0.2.0a2/usseg/Refined_anon_2_html.py
+-rw-r--r--   0        0        0      303 2023-05-17 12:40:36.083145 usseg-0.2.0a2/usseg/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-18 10:07:46.451007 usseg-0.2.0a2/usseg/main.py
+-rw-r--r--   0        0        0     4914 2023-05-17 14:12:40.206489 usseg-0.2.0a2/usseg/visualisation_html.py
+-rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 usseg-0.2.0a2/PKG-INFO
```

### Comparing `usseg-0.2.0a1/README.md` & `usseg-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `usseg-0.2.0a1/pyproject.toml` & `usseg-0.2.0a2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usseg"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "Tools to segment doppler ultrasound signals from scan images."
 authors = ["Dale Kernot <874043@swansea.ac.uk>"]
 license = "GPL-v3-or-later"
 readme = "README.md"
 packages = [{include = "usseg"}]
 
 [tool.poetry.dependencies]
@@ -15,15 +15,17 @@
 numpy = "^1.24.3"
 opencv-python = "^4.7.0.72"
 nibabel = "^5.1.0"
 pandas = "^2.0.1"
 pytesseract = "^0.3.10"
 openpyxl = "^3.1.2"
 plotly = "^5.14.1"
-pytest = "^7.3.1"
 toml = "^0.10.2"
 sklearn = "^0.0.post5"
 
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `usseg-0.2.0a1/usseg/General_functions.py` & `usseg-0.2.0a2/usseg/General_functions.py`

 * *Files identical despite different names*

### Comparing `usseg-0.2.0a1/usseg/Organise_files.py` & `usseg-0.2.0a2/usseg/Organise_files.py`

 * *Files identical despite different names*

### Comparing `usseg-0.2.0a1/usseg/Refined_anon_2_html.py` & `usseg-0.2.0a2/usseg/Refined_anon_2_html.py`

 * *Files identical despite different names*

### Comparing `usseg-0.2.0a1/usseg/main.py` & `usseg-0.2.0a2/usseg/main.py`

 * *Files identical despite different names*

### Comparing `usseg-0.2.0a1/usseg/visualisation_html.py` & `usseg-0.2.0a2/usseg/visualisation_html.py`

 * *Files identical despite different names*

### Comparing `usseg-0.2.0a1/PKG-INFO` & `usseg-0.2.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usseg
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Tools to segment doppler ultrasound signals from scan images.
 License: GPL-v3-or-later
 Author: Dale Kernot
 Author-email: 874043@swansea.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,14 @@
 Requires-Dist: nibabel (>=5.1.0,<6.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sklearn (>=0.0.post5,<0.1)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Doppler Segmetnations
```

