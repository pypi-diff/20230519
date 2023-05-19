# Comparing `tmp/fastf1-3.0.2.tar.gz` & `tmp/fastf1-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastf1-3.0.2.tar", last modified: Tue May  9 20:26:25 2023, max compression
+gzip compressed data, was "fastf1-3.0.3.tar", last modified: Fri May 19 20:53:28 2023, max compression
```

## Comparing `fastf1-3.0.2.tar` & `fastf1-3.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 20:26:14.000000 fastf1-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 20:26:14.000000 fastf1-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-09 20:26:25.394238 fastf1-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-09 20:26:14.000000 fastf1-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.390237 fastf1-3.0.2/fastf1/
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/api.py
--rw-r--r--   0 runner    (1001) docker     (123)   136190 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/ergast/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/ergast/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/livetiming/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/livetiming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/livetiming/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/livetiming/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/livetiming/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/req.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/signalr_aio/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/signalr_aio/events/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/events/_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/signalr_aio/hubs/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/hubs/_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.394238 fastf1-3.0.2/fastf1/signalr_aio/transports/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-09 20:26:14.000000 fastf1-3.0.2/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-09 20:26:15.000000 fastf1-3.0.2/fastf1/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 20:26:15.000000 fastf1-3.0.2/fastf1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:26:25.390237 fastf1-3.0.2/fastf1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 20:26:25.000000 fastf1-3.0.2/fastf1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 20:26:15.000000 fastf1-3.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-09 20:26:25.394238 fastf1-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 20:26:15.000000 fastf1-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-19 20:53:18.000000 fastf1-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 20:53:18.000000 fastf1-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-19 20:53:28.913574 fastf1-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-19 20:53:18.000000 fastf1-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.909574 fastf1-3.0.3/fastf1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136246 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/ergast/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/ergast/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/livetiming/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/livetiming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/livetiming/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/livetiming/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/livetiming/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/req.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/signalr_aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/signalr_aio/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/events/_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/signalr_aio/hubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/hubs/_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.913574 fastf1-3.0.3/fastf1/signalr_aio/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 20:53:18.000000 fastf1-3.0.3/fastf1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:53:28.909574 fastf1-3.0.3/fastf1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 20:53:28.000000 fastf1-3.0.3/fastf1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-19 20:53:18.000000 fastf1-3.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-19 20:53:28.917574 fastf1-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-19 20:53:18.000000 fastf1-3.0.3/setup.py
```

### Comparing `fastf1-3.0.2/LICENSE` & `fastf1-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/PKG-INFO` & `fastf1-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastf1
-Version: 3.0.2
+Version: 3.0.3
 Summary: Wrapper library for F1 data and telemetry API with additional data processing capabilities.
 Home-page: https://github.com/theOehrly/Fast-F1
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: # FastF1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastf1 Version: 3.0.2 Summary: Wrapper library for
+Metadata-Version: 2.1 Name: fastf1 Version: 3.0.3 Summary: Wrapper library for
 F1 data and telemetry API with additional data processing capabilities. Home-
 page: https://github.com/theOehrly/Fast-F1 Author: Oehrly Author-email:
 oehrly@mailbox.org License: MIT Description: # FastF1 FastF1 is a python
 package for accessing and analyzing Formula 1 results, schedules, timing data
 and telemetry. ![](docs/_static/readme.png "banner") ## Main Features - Access
 to F1 timing data, telemetry, sessions results and more - Full support for
 [Ergast](http://ergast.com/mrd/) to access current and historical F1 data - All
```

### Comparing `fastf1-3.0.2/README.md` & `fastf1-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/__init__.py` & `fastf1-3.0.3/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/_api.py` & `fastf1-3.0.3/fastf1/_api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/api.py` & `fastf1-3.0.3/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/core.py` & `fastf1-3.0.3/fastf1/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1607,20 +1607,22 @@
                 )
 
                 quali_results = (quali_results
                                  .merge(laps, on='DriverNumber', how='left'))
             else:
                 quali_results[session_name] = pd.NaT
 
-        quali_results = (quali_results.sort_values(by=['Q3', 'Q2', 'Q1'])
-                         .reset_index())
+        quali_results = quali_results \
+            .sort_values(by=['Q3', 'Q2', 'Q1']) \
+            .reset_index(drop=True)
         quali_results['Position'] = quali_results.index + 1
         quali_results = quali_results.set_index('DriverNumber', drop=True)
 
-        self.results.update(quali_results, overwrite=force)
+        self.results.loc[:, quali_results.columns] \
+            .update(quali_results, overwrite=force)
         self.results.sort_values(by=['Position'], inplace=True)
 
     @soft_exceptions("add track status to laps",
                      "Failed to add track status to Laps!",
                      _logger)
     def _add_track_status_to_laps(self, laps):
         # add track status information to each lap
```

### Comparing `fastf1-3.0.2/fastf1/ergast/interface.py` & `fastf1-3.0.3/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/ergast/legacy.py` & `fastf1-3.0.3/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/ergast/sphinx.py` & `fastf1-3.0.3/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/ergast/structure.py` & `fastf1-3.0.3/fastf1/ergast/structure.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/events.py` & `fastf1-3.0.3/fastf1/events.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/legacy.py` & `fastf1-3.0.3/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/livetiming/__init__.py` & `fastf1-3.0.3/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/livetiming/__main__.py` & `fastf1-3.0.3/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/livetiming/client.py` & `fastf1-3.0.3/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/livetiming/data.py` & `fastf1-3.0.3/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/logger.py` & `fastf1-3.0.3/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/plotting.py` & `fastf1-3.0.3/fastf1/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,20 +140,20 @@
     'MAG': 'kevin magnussen', 'HUL': 'nico hulkenberg',
     'ALO': 'fernando alonso', 'STR': 'lance stroll', 'DRU': 'felipe drugovich',
     'HAM': 'lewis hamilton', 'RUS': 'george russell',
     'ALB': 'alexander albon', 'SAR': 'logan sargeant'}
 """Mapping of driver names to theirs respective abbreviations."""
 
 COMPOUND_COLORS: Dict[str, str] = {
-    "SOFT": "da291c",
-    "MEDIUM": "ffd12e",
-    "HARD": "f0f0ec",
-    "INTERMEDIATE": "43b02a",
-    "WET": "0067ad",
-    "UNKNOWN": "00ffff",
+    "SOFT": "#da291c",
+    "MEDIUM": "#ffd12e",
+    "HARD": "#f0f0ec",
+    "INTERMEDIATE": "#43b02a",
+    "WET": "#0067ad",
+    "UNKNOWN": "#00ffff",
 }
 """Mapping of tyre compound names to compound colors (hex color codes).
 (current season only)"""
 
 COLOR_PALETTE: List[str] = ['#FF79C6', '#50FA7B', '#8BE9FD', '#BD93F9',
                             '#FFB86C', '#FF5555', '#F1FA8C']
 """The default color palette for matplotlib plot lines in fastf1's color
```

### Comparing `fastf1-3.0.2/fastf1/req.py` & `fastf1-3.0.3/fastf1/req.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/signalr_aio/_connection.py` & `fastf1-3.0.3/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.0.3/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.0.3/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.0.3/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1/utils.py` & `fastf1-3.0.3/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/fastf1.egg-info/PKG-INFO` & `fastf1-3.0.3/fastf1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastf1
-Version: 3.0.2
+Version: 3.0.3
 Summary: Wrapper library for F1 data and telemetry API with additional data processing capabilities.
 Home-page: https://github.com/theOehrly/Fast-F1
 Author: Oehrly
 Author-email: oehrly@mailbox.org
 License: MIT
 Description: # FastF1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastf1 Version: 3.0.2 Summary: Wrapper library for
+Metadata-Version: 2.1 Name: fastf1 Version: 3.0.3 Summary: Wrapper library for
 F1 data and telemetry API with additional data processing capabilities. Home-
 page: https://github.com/theOehrly/Fast-F1 Author: Oehrly Author-email:
 oehrly@mailbox.org License: MIT Description: # FastF1 FastF1 is a python
 package for accessing and analyzing Formula 1 results, schedules, timing data
 and telemetry. ![](docs/_static/readme.png "banner") ## Main Features - Access
 to F1 timing data, telemetry, sessions results and more - Full support for
 [Ergast](http://ergast.com/mrd/) to access current and historical F1 data - All
```

### Comparing `fastf1-3.0.2/fastf1.egg-info/SOURCES.txt` & `fastf1-3.0.3/fastf1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.2/setup.cfg` & `fastf1-3.0.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 	fastf1.signalr_aio
 	fastf1.signalr_aio.events
 	fastf1.signalr_aio.hubs
 	fastf1.signalr_aio.transports
 python_requires = >= 3.8
 install_requires = 
 	requests-cache>=0.8.0
-	pandas>=1.2.4
-	numpy>=1.20.3
-	scipy>=1.6.3
+	pandas>=1.2.4,<3.0.0
+	numpy>=1.20.3,<2.0.0
+	scipy>=1.6.3,<2.0.0
 	thefuzz
-	matplotlib>=3.4.2
+	matplotlib>=3.4.2,<4.0.0
 	python-dateutil
 	timple>=0.1.2
 	requests>=2.28.0
 	websockets>=8.1
 
 [build_sphinx]
 project = Fast F1
```

