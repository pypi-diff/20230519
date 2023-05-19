# Comparing `tmp/start_time_estimator-1.10.7.tar.gz` & `tmp/start_time_estimator-1.10.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_time_estimator-1.10.7.tar", max compression
+gzip compressed data, was "start_time_estimator-1.10.8.tar", max compression
```

## Comparing `start_time_estimator-1.10.7.tar` & `start_time_estimator-1.10.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11349 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/LICENSE
--rw-r--r--   0        0        0     7299 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/README.md
--rw-r--r--   0        0        0      548 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/pyproject.toml
--rw-r--r--   0        0        0       81 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/src/start_time_estimator/__init__.py
--rw-r--r--   0        0        0    15710 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/src/start_time_estimator/concurrency_oracle.py
--rw-r--r--   0        0        0     4429 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/src/start_time_estimator/config.py
--rw-r--r--   0        0        0     8683 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/src/start_time_estimator/estimator.py
--rw-r--r--   0        0        0     4846 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/src/start_time_estimator/resource_availability.py
--rw-r--r--   0        0        0      165 2023-05-17 14:15:08.992555 start_time_estimator-1.10.7/src/start_time_estimator/utils.py
--rw-r--r--   0        0        0     7941 1970-01-01 00:00:00.000000 start_time_estimator-1.10.7/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/LICENSE
+-rw-r--r--   0        0        0     7299 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/README.md
+-rw-r--r--   0        0        0      548 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/pyproject.toml
+-rw-r--r--   0        0        0       81 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/src/start_time_estimator/__init__.py
+-rw-r--r--   0        0        0    15710 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/src/start_time_estimator/concurrency_oracle.py
+-rw-r--r--   0        0        0     4429 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/src/start_time_estimator/config.py
+-rw-r--r--   0        0        0     8683 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/src/start_time_estimator/estimator.py
+-rw-r--r--   0        0        0     4841 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/src/start_time_estimator/resource_availability.py
+-rw-r--r--   0        0        0      165 2023-05-19 13:37:51.811784 start_time_estimator-1.10.8/src/start_time_estimator/utils.py
+-rw-r--r--   0        0        0     7941 1970-01-01 00:00:00.000000 start_time_estimator-1.10.8/PKG-INFO
```

### Comparing `start_time_estimator-1.10.7/LICENSE` & `start_time_estimator-1.10.8/LICENSE`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.7/README.md` & `start_time_estimator-1.10.8/README.md`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.7/pyproject.toml` & `start_time_estimator-1.10.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "start-time-estimator"
-version = "1.10.7"
+version = "1.10.8"
 description = "Python package to estimate the enabled time, enabling activity, and resource availability time of each activity instance in an event log."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pandas = "^2.0"
```

### Comparing `start_time_estimator-1.10.7/src/start_time_estimator/concurrency_oracle.py` & `start_time_estimator-1.10.8/src/start_time_estimator/concurrency_oracle.py`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.7/src/start_time_estimator/config.py` & `start_time_estimator-1.10.8/src/start_time_estimator/config.py`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.7/src/start_time_estimator/estimator.py` & `start_time_estimator-1.10.8/src/start_time_estimator/estimator.py`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.7/src/start_time_estimator/resource_availability.py` & `start_time_estimator-1.10.8/src/start_time_estimator/resource_availability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 import pandas as pd
+from pix_framework.calendar.availability import get_last_available_timestamp
 
 from start_time_estimator.config import Configuration
-from pix_framework.calendar.resource_calendar import get_last_available_timestamp
 
 
 class ResourceAvailability:
     def __init__(self, performed_events: dict, working_schedules: dict, config: Configuration):
         # Store dictionary with the resources as key and all its events as value
         self.performed_events = performed_events
         # Store dictionary with the resources as key and all its events as value
```

### Comparing `start_time_estimator-1.10.7/PKG-INFO` & `start_time_estimator-1.10.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: start-time-estimator
-Version: 1.10.7
+Version: 1.10.8
 Summary: Python package to estimate the enabled time, enabling activity, and resource availability time of each activity instance in an event log.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

