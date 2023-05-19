# Comparing `tmp/pix_framework-0.8.2.tar.gz` & `tmp/pix_framework-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix_framework-0.8.2.tar", max compression
+gzip compressed data, was "pix_framework-0.8.3.tar", max compression
```

## Comparing `pix_framework-0.8.2.tar` & `pix_framework-0.8.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-05-19 12:19:49.400172 pix_framework-0.8.2/LICENSE
--rw-r--r--   0        0        0      549 2023-05-19 12:19:49.400172 pix_framework-0.8.2/README.md
--rw-r--r--   0        0        0      761 2023-05-19 12:19:49.400172 pix_framework-0.8.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/__init__.py
--rw-r--r--   0        0        0       32 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/calendar/__init__.py
--rw-r--r--   0        0        0     7524 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/calendar/availability.py
--rw-r--r--   0        0        0    30167 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/calendar/prosimos_calendar.py
--rw-r--r--   0        0        0        0 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/discovery/__init__.py
--rw-r--r--   0        0        0     5874 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/discovery/calendar_factory.py
--rw-r--r--   0        0        0     7014 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/discovery/case_arrival.py
--rw-r--r--   0        0        0     4903 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/discovery/gateway_probabilities.py
--rw-r--r--   0        0        0        0 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/enhancement/__init__.py
--rw-r--r--   0        0        0     5444 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/enhancement/multitasking.py
--rw-r--r--   0        0        0       27 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/filesystem/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/filesystem/file_manager.py
--rw-r--r--   0        0        0     2498 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/input.py
--rw-r--r--   0        0        0        0 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/io/__init__.py
--rw-r--r--   0        0        0    38314 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/io/bpm_graph.py
--rw-r--r--   0        0        0     2058 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/log_ids.py
--rw-r--r--   0        0        0        0 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/log_split/__init__.py
--rw-r--r--   0        0        0     4414 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/log_split/log_split.py
--rw-r--r--   0        0        0       27 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/statistics/__init__.py
--rw-r--r--   0        0        0    13047 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/statistics/distribution.py
--rw-r--r--   0        0        0      970 2023-05-19 12:19:49.400172 pix_framework-0.8.2/src/pix_framework/statistics/utils.py
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 pix_framework-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 13:30:01.651982 pix_framework-0.8.3/LICENSE
+-rw-r--r--   0        0        0      549 2023-05-19 13:30:01.651982 pix_framework-0.8.3/README.md
+-rw-r--r--   0        0        0      761 2023-05-19 13:30:01.651982 pix_framework-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/calendar/__init__.py
+-rw-r--r--   0        0        0     7524 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/calendar/availability.py
+-rw-r--r--   0        0        0    30167 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/calendar/resource_calendar.py
+-rw-r--r--   0        0        0        0 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/discovery/__init__.py
+-rw-r--r--   0        0        0     5874 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/discovery/calendar_factory.py
+-rw-r--r--   0        0        0     7014 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/discovery/case_arrival.py
+-rw-r--r--   0        0        0     4903 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/discovery/gateway_probabilities.py
+-rw-r--r--   0        0        0        0 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/enhancement/__init__.py
+-rw-r--r--   0        0        0     5444 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/enhancement/multitasking.py
+-rw-r--r--   0        0        0       27 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/filesystem/file_manager.py
+-rw-r--r--   0        0        0     2498 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/input.py
+-rw-r--r--   0        0        0        0 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/io/__init__.py
+-rw-r--r--   0        0        0    38314 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/io/bpm_graph.py
+-rw-r--r--   0        0        0     2058 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/log_ids.py
+-rw-r--r--   0        0        0        0 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/log_split/__init__.py
+-rw-r--r--   0        0        0     4414 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/log_split/log_split.py
+-rw-r--r--   0        0        0       27 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/statistics/__init__.py
+-rw-r--r--   0        0        0    13047 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/statistics/distribution.py
+-rw-r--r--   0        0        0      970 2023-05-19 13:30:01.651982 pix_framework-0.8.3/src/pix_framework/statistics/utils.py
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 pix_framework-0.8.3/PKG-INFO
```

### Comparing `pix_framework-0.8.2/LICENSE` & `pix_framework-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/README.md` & `pix_framework-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/pyproject.toml` & `pix_framework-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pix-framework"
-version = "0.8.2"
+version = "0.8.3"
 description = "Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>", "Ihar Suvorau <ihar.suvorau@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "pix_framework", from = "src" },
 ]
```

### Comparing `pix_framework-0.8.2/src/pix_framework/calendar/availability.py` & `pix_framework-0.8.3/src/pix_framework/calendar/availability.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 (https://github.com/AutomatedProcessImprovement/Prosimos/blob/main/bpdfr_simulation_engine/resource_calendar.py).
 """
 from typing import List
 
 import pandas as pd
 import pytz
 
-from pix_framework.calendar.prosimos_calendar import RCalendar, Interval
+from pix_framework.calendar.resource_calendar import RCalendar, Interval
 
 
 def get_last_available_timestamp(
     start: pd.Timestamp, end: pd.Timestamp, schedule: RCalendar
 ) -> pd.Timestamp:
     """
     Get the timestamp [last_available] within the interval from [start] to [end] (i.e. [start] <= [last_available] <= [end]) such that
```

### Comparing `pix_framework-0.8.2/src/pix_framework/calendar/prosimos_calendar.py` & `pix_framework-0.8.3/src/pix_framework/calendar/resource_calendar.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/discovery/calendar_factory.py` & `pix_framework-0.8.3/src/pix_framework/discovery/calendar_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from typing import Dict
 
 import pytz
 
-from pix_framework.calendar.prosimos_calendar import (
+from pix_framework.calendar.resource_calendar import (
     RCalendar,
     int_week_days,
     GranuleInfo,
     CalendarKPIInfoFactory,
 )
```

### Comparing `pix_framework-0.8.2/src/pix_framework/discovery/case_arrival.py` & `pix_framework-0.8.3/src/pix_framework/discovery/case_arrival.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from dataclasses import dataclass
 from typing import List
 
 import pandas as pd
 
-from pix_framework.calendar.prosimos_calendar import RCalendar
+from pix_framework.calendar.resource_calendar import RCalendar
 from pix_framework.discovery.calendar_factory import CalendarFactory
 from pix_framework.log_ids import EventLogIDs
 from pix_framework.statistics.distribution import (
     get_best_fitting_distribution,
     get_observations_histogram,
 )
```

### Comparing `pix_framework-0.8.2/src/pix_framework/discovery/gateway_probabilities.py` & `pix_framework-0.8.3/src/pix_framework/discovery/gateway_probabilities.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/enhancement/multitasking.py` & `pix_framework-0.8.3/src/pix_framework/enhancement/multitasking.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/filesystem/file_manager.py` & `pix_framework-0.8.3/src/pix_framework/filesystem/file_manager.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/input.py` & `pix_framework-0.8.3/src/pix_framework/input.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/io/bpm_graph.py` & `pix_framework-0.8.3/src/pix_framework/io/bpm_graph.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/log_ids.py` & `pix_framework-0.8.3/src/pix_framework/log_ids.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/log_split/log_split.py` & `pix_framework-0.8.3/src/pix_framework/log_split/log_split.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/statistics/distribution.py` & `pix_framework-0.8.3/src/pix_framework/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/src/pix_framework/statistics/utils.py` & `pix_framework-0.8.3/src/pix_framework/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.2/PKG-INFO` & `pix_framework-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix-framework
-Version: 0.8.2
+Version: 0.8.3
 Summary: Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

