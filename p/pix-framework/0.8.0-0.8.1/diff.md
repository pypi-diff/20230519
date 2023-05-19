# Comparing `tmp/pix_framework-0.8.0.tar.gz` & `tmp/pix_framework-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix_framework-0.8.0.tar", max compression
+gzip compressed data, was "pix_framework-0.8.1.tar", max compression
```

## Comparing `pix_framework-0.8.0.tar` & `pix_framework-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-05-17 13:40:44.215619 pix_framework-0.8.0/LICENSE
--rw-r--r--   0        0        0      549 2023-05-17 13:40:44.215619 pix_framework-0.8.0/README.md
--rw-r--r--   0        0        0      744 2023-05-17 13:40:44.215619 pix_framework-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       57 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/__init__.py
--rw-r--r--   0        0        0       32 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/calendar/__init__.py
--rw-r--r--   0        0        0    11236 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/calendar/resource_calendar.py
--rw-r--r--   0        0        0        0 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/discovery/__init__.py
--rw-r--r--   0        0        0     4903 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/discovery/gateway_probabilities.py
--rw-r--r--   0        0        0        0 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/enhancement/__init__.py
--rw-r--r--   0        0        0     5444 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/enhancement/multitasking.py
--rw-r--r--   0        0        0       27 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/filesystem/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/filesystem/file_manager.py
--rw-r--r--   0        0        0     2498 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/input.py
--rw-r--r--   0        0        0        0 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/io/__init__.py
--rw-r--r--   0        0        0    38314 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/io/bpm_graph.py
--rw-r--r--   0        0        0     2058 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/log_ids.py
--rw-r--r--   0        0        0        0 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/log_split/__init__.py
--rw-r--r--   0        0        0     4414 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/log_split/log_split.py
--rw-r--r--   0        0        0       27 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/statistics/__init__.py
--rw-r--r--   0        0        0    13047 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/statistics/distribution.py
--rw-r--r--   0        0        0      970 2023-05-17 13:40:44.215619 pix_framework-0.8.0/src/pix_framework/statistics/utils.py
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 pix_framework-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 12:09:12.696756 pix_framework-0.8.1/LICENSE
+-rw-r--r--   0        0        0      549 2023-05-19 12:09:12.696756 pix_framework-0.8.1/README.md
+-rw-r--r--   0        0        0      761 2023-05-19 12:09:12.696756 pix_framework-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/calendar/__init__.py
+-rw-r--r--   0        0        0     7524 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/calendar/availability.py
+-rw-r--r--   0        0        0    30167 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/calendar/prosimos_calendar.py
+-rw-r--r--   0        0        0        0 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/discovery/__init__.py
+-rw-r--r--   0        0        0     5874 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/discovery/calendar_factory.py
+-rw-r--r--   0        0        0     7014 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/discovery/case_arrival.py
+-rw-r--r--   0        0        0     4903 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/discovery/gateway_probabilities.py
+-rw-r--r--   0        0        0        0 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/enhancement/__init__.py
+-rw-r--r--   0        0        0     5444 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/enhancement/multitasking.py
+-rw-r--r--   0        0        0       27 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/filesystem/file_manager.py
+-rw-r--r--   0        0        0     2498 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/input.py
+-rw-r--r--   0        0        0        0 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/io/__init__.py
+-rw-r--r--   0        0        0    38314 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/io/bpm_graph.py
+-rw-r--r--   0        0        0     2058 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/log_ids.py
+-rw-r--r--   0        0        0        0 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/log_split/__init__.py
+-rw-r--r--   0        0        0     4414 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/log_split/log_split.py
+-rw-r--r--   0        0        0       27 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/statistics/__init__.py
+-rw-r--r--   0        0        0    13047 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/statistics/distribution.py
+-rw-r--r--   0        0        0      970 2023-05-19 12:09:12.696756 pix_framework-0.8.1/src/pix_framework/statistics/utils.py
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 pix_framework-0.8.1/PKG-INFO
```

### Comparing `pix_framework-0.8.0/LICENSE` & `pix_framework-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/README.md` & `pix_framework-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/pyproject.toml` & `pix_framework-0.8.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pix-framework"
-version = "0.8.0"
+version = "0.8.1"
 description = "Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>", "Ihar Suvorau <ihar.suvorau@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "pix_framework", from = "src" },
 ]
 
@@ -12,14 +12,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pandas = "^2.0.1"
 scipy = "^1.10.1"
+pytz = "^2023.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 markers = [
```

### Comparing `pix_framework-0.8.0/src/pix_framework/discovery/gateway_probabilities.py` & `pix_framework-0.8.1/src/pix_framework/discovery/gateway_probabilities.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/src/pix_framework/enhancement/multitasking.py` & `pix_framework-0.8.1/src/pix_framework/enhancement/multitasking.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/src/pix_framework/filesystem/file_manager.py` & `pix_framework-0.8.1/src/pix_framework/filesystem/file_manager.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/src/pix_framework/input.py` & `pix_framework-0.8.1/src/pix_framework/input.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/src/pix_framework/io/bpm_graph.py` & `pix_framework-0.8.1/src/pix_framework/io/bpm_graph.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/src/pix_framework/log_ids.py` & `pix_framework-0.8.1/src/pix_framework/log_ids.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/src/pix_framework/log_split/log_split.py` & `pix_framework-0.8.1/src/pix_framework/log_split/log_split.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/src/pix_framework/statistics/distribution.py` & `pix_framework-0.8.1/src/pix_framework/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/src/pix_framework/statistics/utils.py` & `pix_framework-0.8.1/src/pix_framework/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.0/PKG-INFO` & `pix_framework-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pix-framework
-Version: 0.8.0
+Version: 0.8.1
 Summary: Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PIX Framework
 
 ![pix-framework](https://github.com/AutomatedProcessImprovement/pix-framework/actions/workflows/build.yaml/badge.svg)
 ![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/pix-framework)
```

