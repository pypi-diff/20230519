# Comparing `tmp/ezyquant-execution-0.0.5.tar.gz` & `tmp/ezyquant-execution-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-execution-0.0.5.tar", last modified: Mon May 15 04:02:17 2023, max compression
+gzip compressed data, was "ezyquant-execution-0.0.6.tar", last modified: Fri May 19 03:08:07 2023, max compression
```

## Comparing `ezyquant-execution-0.0.5.tar` & `ezyquant-execution-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:02:17.561529 ezyquant-execution-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 04:02:17.561529 ezyquant-execution-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:02:17.557529 ezyquant-execution-0.0.5/ezyquant_execution/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/ezyquant_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/ezyquant_execution/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/ezyquant_execution/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/ezyquant_execution/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/ezyquant_execution/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/ezyquant_execution/executing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/ezyquant_execution/realtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/ezyquant_execution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:02:17.561529 ezyquant-execution-0.0.5/ezyquant_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 04:02:17.000000 ezyquant-execution-0.0.5/ezyquant_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 04:02:17.000000 ezyquant-execution-0.0.5/ezyquant_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:02:17.000000 ezyquant-execution-0.0.5/ezyquant_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-15 04:02:17.000000 ezyquant-execution-0.0.5/ezyquant_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 04:02:17.000000 ezyquant-execution-0.0.5/ezyquant_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 04:02:17.561529 ezyquant-execution-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-15 04:02:03.000000 ezyquant-execution-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:08:07.292397 ezyquant-execution-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 03:08:07.292397 ezyquant-execution-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:08:07.292397 ezyquant-execution-0.0.6/ezyquant_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/ezyquant_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/ezyquant_execution/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/ezyquant_execution/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/ezyquant_execution/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/ezyquant_execution/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/ezyquant_execution/executing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/ezyquant_execution/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/ezyquant_execution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:08:07.292397 ezyquant-execution-0.0.6/ezyquant_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 03:08:07.000000 ezyquant-execution-0.0.6/ezyquant_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-19 03:08:07.000000 ezyquant-execution-0.0.6/ezyquant_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 03:08:07.000000 ezyquant-execution-0.0.6/ezyquant_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 03:08:07.000000 ezyquant-execution-0.0.6/ezyquant_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 03:08:07.000000 ezyquant-execution-0.0.6/ezyquant_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-19 03:08:07.292397 ezyquant-execution-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-19 03:07:52.000000 ezyquant-execution-0.0.6/setup.py
```

### Comparing `ezyquant-execution-0.0.5/LICENSE.txt` & `ezyquant-execution-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.5/PKG-INFO` & `ezyquant-execution-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.0.5
+Version: 0.0.6
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.0.5/ezyquant_execution/constant.py` & `ezyquant-execution-0.0.6/ezyquant_execution/constant.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.5/ezyquant_execution/context.py` & `ezyquant-execution-0.0.6/ezyquant_execution/context.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.5/ezyquant_execution/entity.py` & `ezyquant-execution-0.0.6/ezyquant_execution/entity.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.5/ezyquant_execution/executing.py` & `ezyquant-execution-0.0.6/ezyquant_execution/executing.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.5/ezyquant_execution/realtime.py` & `ezyquant-execution-0.0.6/ezyquant_execution/realtime.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from threading import Event
+from threading import Event, Timer
 from typing import Callable, Optional
 
 from settrade_v2.realtime import RealtimeDataConnection, Subscriber
 
 from .entity import BidOffer, PriceInfo
 
 
@@ -17,14 +17,18 @@
 
         self._event: Event = Event()
 
         self._subscriber = self.function(
             on_message=self._on_message, *self.args, **self.kwargs
         )
         self._subscriber.start()
+        # Stop after 12 hours
+        timer = Timer(12 * 60 * 60, self._subscriber.stop)
+        timer.daemon = True
+        timer.start()
 
         # wait for first data to be received
         if not self._event.wait(timeout=30):
             raise ConnectionError("No data received yet")
 
     @property
     def data(self) -> dict:
```

### Comparing `ezyquant-execution-0.0.5/ezyquant_execution/utils.py` & `ezyquant-execution-0.0.6/ezyquant_execution/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.5/ezyquant_execution.egg-info/PKG-INFO` & `ezyquant-execution-0.0.6/ezyquant_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.0.5
+Version: 0.0.6
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.0.5/setup.py` & `ezyquant-execution-0.0.6/setup.py`

 * *Files identical despite different names*

