# Comparing `tmp/sunsynk-0.3.5.tar.gz` & `tmp/sunsynk-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunsynk-0.3.5.tar", last modified: Thu May 18 10:27:12 2023, max compression
+gzip compressed data, was "sunsynk-0.3.6.tar", last modified: Fri May 19 13:27:21 2023, max compression
```

## Comparing `sunsynk-0.3.5.tar` & `sunsynk-0.3.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 10:27:02.000000 sunsynk-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 10:27:02.000000 sunsynk-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-18 10:27:12.956032 sunsynk-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-18 10:27:02.000000 sunsynk-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 10:27:12.956032 sunsynk-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 10:27:02.000000 sunsynk-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11686 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/pysunsynk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8030 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/usunsynk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/sunsynk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass-addon-sunsynk-dev.zip
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass-addon-sunsynk.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/tests/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_pysunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.837749 sunsynk-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-19 13:27:10.000000 sunsynk-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 13:27:10.000000 sunsynk-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-19 13:27:21.837749 sunsynk-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-19 13:27:10.000000 sunsynk-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-19 13:27:21.837749 sunsynk-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-19 13:27:10.000000 sunsynk-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.833749 sunsynk-0.3.6/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11717 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/pysunsynk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8147 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.833749 sunsynk-0.3.6/sunsynk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.833749 sunsynk-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass-addon-sunsynk-dev.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass-addon-sunsynk.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.833749 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.837749 sunsynk-0.3.6/tests/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_pysunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_usunsynk.py
```

### Comparing `sunsynk-0.3.5/LICENSE` & `sunsynk-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/PKG-INFO` & `sunsynk-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.5
+Version: 0.3.6
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.5/README.md` & `sunsynk-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/setup.cfg` & `sunsynk-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/sunsynk/definitions.py` & `sunsynk-0.3.6/sunsynk/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,21 +210,22 @@
     BATTERY_LOW_VOLT,
 )
 
 #################
 # System program
 #################
 SENSORS += (
-    SelectRWSensor(243, "Priority Mode", options={0: "Battery first", 1: "Load first"}),
+    # 0: "Battery first", 1: "Load first"
+    SwitchRWSensor(243, "Priority Load"),
     SelectRWSensor(
         244,
         "Load Limit",
         options={0: "Allow Export", 1: "Essentials", 2: "Zero Export"},
     ),
-    SwitchRWSensor(248, "Use Timer", on=1, bitmask=1),
+    SwitchRWSensor(248, "Use Timer", bitmask=1),
 )
 
 PROG1_TIME = TimeRWSensor(250, "Prog1 Time")
 PROG2_TIME = TimeRWSensor(251, "Prog2 Time", min=PROG1_TIME)
 PROG3_TIME = TimeRWSensor(252, "Prog3 Time", min=PROG2_TIME)
 PROG4_TIME = TimeRWSensor(253, "Prog4 Time", min=PROG3_TIME)
 PROG5_TIME = TimeRWSensor(254, "Prog5 Time", min=PROG4_TIME)
@@ -312,33 +313,34 @@
 
 
 #############
 # Deprecated
 #############
 SENSORS.deprecated.update(
     {
+        "absorption_voltage": "battery_absorption_voltage",
         "aux_load": "aux_power",
-        "temp_battery": "battery_temperature",
-        "temp_dc_transformer": "dc_transformer_temperature",
-        "temp_environment": "environment_temperature",
         "battery_grid_charge": "grid_charge_battery_current",
+        "day_active_power": "day_active_energy",
+        "day_load_power": "day_load_energy",
+        "day_reactive_power": "day_reactive_energy",
+        "equalization_voltage": "battery_equalization_voltage",
         "grid_ct_load": "grid_ct_power",
         "grid_l1_load": "grid_ld_power",
         "grid_l2_load": "grid_l2_power",
         "grid_load": "grid_power",
         "inverter_output": "inverter_power",
+        "month_grid_power": "month_grid_energy",
+        "month_load_power": "month_load_energy",
+        "month_pv_power": "month_pv_energy",
+        "priority_mode": "priority_load",
+        "temp_battery": "battery_temperature",
+        "temp_dc_transformer": "dc_transformer_temperature",
+        "temp_environment": "environment_temperature",
         "temp_radiator": "radiator_temperature",
-        "day_active_power": "day_active_energy",
-        "day_reactive_power": "day_reactive_energy",
         "total_active_power": "total_active_energy",
-        "month_pv_power": "month_pv_energy",
-        "month_load_power": "month_load_energy",
-        "month_grid_power": "month_grid_energy",
-        "year_pv_power": "year_pv_energy",
-        "day_load_power": "day_load_energy",
         "total_load_power": "total_load_energy",
-        "year_load_power": "year_load_energy",
         "total_pv_power": "total_pv_energy",
-        "equalization_voltage": "battery_equalization_voltage",
-        "absorption_voltage": "battery_absorption_voltage",
+        "year_load_power": "year_load_energy",
+        "year_pv_power": "year_pv_energy",
     }
 )
```

### Comparing `sunsynk-0.3.5/sunsynk/definitions3ph.py` & `sunsynk-0.3.6/sunsynk/definitions3ph.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,17 +246,15 @@
     BATTERY_LOW_VOLTAGE,
 )
 
 #################
 # System program
 #################
 
-SENSORS += SelectRWSensor(
-    141, "Priority Mode", options={0: "Battery first", 1: "Load first"}
-)
+SENSORS += SwitchRWSensor(141, "Priority Load")
 
 SENSORS += SelectRWSensor(
     142,
     "Load Limit",
     options={0: "Allow Export", 1: "Essentials", 2: "Zero Export"},
 )
 
@@ -378,7 +376,14 @@
         "Prog6 voltage",
         VOLT,
         0.01,
         min=BATTERY_LOW_VOLTAGE,
         max=BATTERY_FLOAT_VOLTAGE,
     ),
 )
+
+
+SENSORS.deprecated.update(
+    {
+        "priority_mode": "priority_load",
+    }
+)
```

### Comparing `sunsynk-0.3.5/sunsynk/helpers.py` & `sunsynk-0.3.6/sunsynk/helpers.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/sunsynk/pysunsynk.py` & `sunsynk-0.3.6/sunsynk/pysunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/sunsynk/rwsensors.py` & `sunsynk-0.3.6/sunsynk/rwsensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import logging
 import re
 from typing import Callable, Generator, Optional, Union
 
 import attrs
+from mqtt_entity.utils import BOOL_OFF, BOOL_ON
 
 from sunsynk.helpers import NumType, RegType, SSTime, ValType, as_num
 from sunsynk.sensors import Sensor
 
 _LOGGER = logging.getLogger(__name__)
 ResolveType = Optional[Callable[[Sensor, ValType], ValType]]
 
@@ -113,24 +114,26 @@
         if res is None:
             _LOGGER.warning("%s: Unknown register value %s", self.id, regsm[0])
         return res
 
 
 @attrs.define(slots=True, eq=False)
 class SwitchRWSensor(SelectRWSensor):
-    """Sensor with a set of options to select from."""
+    """Switch Sensor."""
 
     on: int = attrs.field(default=1)  # pylint: disable=invalid-name
+    """The register value representing ON."""
     off: int = attrs.field(default=0)
+    """The register value representing OFF."""
 
     def __attrs_post_init__(self) -> None:
         """Ensure correct parameters."""
         assert not self.options
         assert self.on != self.off
-        self.options = {self.off: "OFF", self.on: "ON"}
+        self.options = {self.off: BOOL_OFF, self.on: BOOL_ON}
 
 
 @attrs.define(slots=True, eq=False)
 class SystemTimeRWSensor(RWSensor):
     """Read & write time sensor."""
 
     def value_to_reg(self, value: ValType, resolve: ResolveType) -> RegType:
```

### Comparing `sunsynk-0.3.5/sunsynk/sensors.py` & `sunsynk-0.3.6/sunsynk/sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/sunsynk/state.py` & `sunsynk-0.3.6/sunsynk/state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/sunsynk/sunsynk.py` & `sunsynk-0.3.6/sunsynk/sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/sunsynk/usunsynk.py` & `sunsynk-0.3.6/sunsynk/usunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/sunsynk.egg-info/PKG-INFO` & `sunsynk-0.3.6/sunsynk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.5
+Version: 0.3.6
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.5/sunsynk.egg-info/SOURCES.txt` & `sunsynk-0.3.6/sunsynk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/conftest.py` & `sunsynk-0.3.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/hass-addon-sunsynk-dev.zip` & `sunsynk-0.3.6/tests/hass-addon-sunsynk-dev.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/hass-addon-sunsynk.zip` & `sunsynk-0.3.6/tests/hass-addon-sunsynk.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_filter.py` & `sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_filter.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_run.py` & `sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_run.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_sensors.py` & `sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_state.py` & `sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/sunsynk/test_helpers.py` & `sunsynk-0.3.6/tests/sunsynk/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/sunsynk/test_pysunsynk.py` & `sunsynk-0.3.6/tests/sunsynk/test_pysunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/sunsynk/test_register.py` & `sunsynk-0.3.6/tests/sunsynk/test_register.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/sunsynk/test_rwsensors.py` & `sunsynk-0.3.6/tests/sunsynk/test_rwsensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/sunsynk/test_sensors.py` & `sunsynk-0.3.6/tests/sunsynk/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/sunsynk/test_sunsynk.py` & `sunsynk-0.3.6/tests/sunsynk/test_sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.5/tests/sunsynk/test_usunsynk.py` & `sunsynk-0.3.6/tests/sunsynk/test_usunsynk.py`

 * *Files identical despite different names*

