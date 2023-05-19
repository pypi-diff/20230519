# Comparing `tmp/pyvesync-2.1.6.tar.gz` & `tmp/pyvesync-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvesync-2.1.6.tar", last modified: Fri Mar 31 13:15:03 2023, max compression
+gzip compressed data, was "pyvesync-2.1.7.tar", last modified: Fri May 19 02:06:02 2023, max compression
```

## Comparing `pyvesync-2.1.6.tar` & `pyvesync-2.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 13:15:03.894904 pyvesync-2.1.6/
--rw-rw-rw-   0        0        0     1089 2021-04-26 21:24:56.000000 pyvesync-2.1.6/LICENSE
--rw-rw-rw-   0        0        0       44 2021-04-26 21:24:56.000000 pyvesync-2.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    29785 2023-03-31 13:15:03.894904 pyvesync-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    29117 2023-03-31 13:13:29.000000 pyvesync-2.1.6/README.md
--rw-rw-rw-   0        0        0       16 2021-04-26 21:24:56.000000 pyvesync-2.1.6/requirements.txt
--rw-rw-rw-   0        0        0      342 2023-03-31 13:15:03.895905 pyvesync-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-03-31 13:13:29.000000 pyvesync-2.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 13:15:03.865904 pyvesync-2.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 13:15:03.884908 pyvesync-2.1.6/src/pyvesync/
--rw-rw-rw-   0        0        0      216 2023-03-31 13:13:29.000000 pyvesync-2.1.6/src/pyvesync/__init__.py
--rw-rw-rw-   0        0        0    14192 2023-03-31 13:13:29.000000 pyvesync-2.1.6/src/pyvesync/helpers.py
--rw-rw-rw-   0        0        0    13453 2023-03-31 13:13:29.000000 pyvesync-2.1.6/src/pyvesync/vesync.py
--rw-rw-rw-   0        0        0     5682 2023-03-31 13:13:29.000000 pyvesync-2.1.6/src/pyvesync/vesyncbasedevice.py
--rw-rw-rw-   0        0        0    44232 2023-03-31 13:13:29.000000 pyvesync-2.1.6/src/pyvesync/vesyncbulb.py
--rw-rw-rw-   0        0        0    49494 2023-03-31 13:13:29.000000 pyvesync-2.1.6/src/pyvesync/vesyncfan.py
--rw-rw-rw-   0        0        0    24285 2023-03-31 13:13:29.000000 pyvesync-2.1.6/src/pyvesync/vesynckitchen.py
--rw-rw-rw-   0        0        0    25884 2022-06-11 01:15:51.000000 pyvesync-2.1.6/src/pyvesync/vesyncoutlet.py
--rw-rw-rw-   0        0        0    13023 2023-03-31 13:13:29.000000 pyvesync-2.1.6/src/pyvesync/vesyncswitch.py
-drwxrwxrwx   0        0        0        0 2023-03-31 13:15:03.893906 pyvesync-2.1.6/src/pyvesync.egg-info/
--rw-rw-rw-   0        0        0    29785 2023-03-31 13:15:03.000000 pyvesync-2.1.6/src/pyvesync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2023-03-31 13:15:03.000000 pyvesync-2.1.6/src/pyvesync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 13:15:03.000000 pyvesync-2.1.6/src/pyvesync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-03 00:59:55.000000 pyvesync-2.1.6/src/pyvesync.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-03-31 13:15:03.000000 pyvesync-2.1.6/src/pyvesync.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-31 13:15:03.000000 pyvesync-2.1.6/src/pyvesync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 02:06:02.447202 pyvesync-2.1.7/
+-rw-rw-rw-   0        0        0     1089 2021-04-26 21:24:56.000000 pyvesync-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-04-26 21:24:56.000000 pyvesync-2.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    31937 2023-05-19 02:06:02.447202 pyvesync-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    31205 2023-05-19 01:46:13.000000 pyvesync-2.1.7/README.md
+-rw-rw-rw-   0        0        0       16 2021-04-26 21:24:56.000000 pyvesync-2.1.7/requirements.txt
+-rw-rw-rw-   0        0        0      342 2023-05-19 02:06:02.449202 pyvesync-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2023-05-19 02:02:56.000000 pyvesync-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 02:06:02.394202 pyvesync-2.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 02:06:02.432201 pyvesync-2.1.7/src/pyvesync/
+-rw-rw-rw-   0        0        0      216 2023-03-31 13:13:29.000000 pyvesync-2.1.7/src/pyvesync/__init__.py
+-rw-rw-rw-   0        0        0    20649 2023-05-19 01:42:51.000000 pyvesync-2.1.7/src/pyvesync/helpers.py
+-rw-rw-rw-   0        0        0    13951 2023-05-18 23:52:27.000000 pyvesync-2.1.7/src/pyvesync/vesync.py
+-rw-rw-rw-   0        0        0     5682 2023-03-31 13:13:29.000000 pyvesync-2.1.7/src/pyvesync/vesyncbasedevice.py
+-rw-rw-rw-   0        0        0    45082 2023-05-18 23:52:27.000000 pyvesync-2.1.7/src/pyvesync/vesyncbulb.py
+-rw-rw-rw-   0        0        0    54642 2023-05-19 00:27:27.000000 pyvesync-2.1.7/src/pyvesync/vesyncfan.py
+-rw-rw-rw-   0        0        0    24285 2023-03-31 13:13:29.000000 pyvesync-2.1.7/src/pyvesync/vesynckitchen.py
+-rw-rw-rw-   0        0        0    25884 2022-06-11 01:15:51.000000 pyvesync-2.1.7/src/pyvesync/vesyncoutlet.py
+-rw-rw-rw-   0        0        0    13023 2023-03-31 13:13:29.000000 pyvesync-2.1.7/src/pyvesync/vesyncswitch.py
+drwxrwxrwx   0        0        0        0 2023-05-19 02:06:02.446202 pyvesync-2.1.7/src/pyvesync.egg-info/
+-rw-rw-rw-   0        0        0    31937 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-11-03 00:59:55.000000 pyvesync-2.1.7/src/pyvesync.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/top_level.txt
```

### Comparing `pyvesync-2.1.6/LICENSE` & `pyvesync-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.6/PKG-INFO` & `pyvesync-2.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyvesync
-Version: 2.1.6
-Summary: pyvesync is a library to manage Etekcity                 Devices and Levoit Air Purifier
+Version: 2.1.7
+Summary: pyvesync is a library to manage Etekcity                 Devices, Cosori Air Fryers and Levoit Air                      Purifiers run on the VeSync app.
 Home-page: https://github.com/webdjoe/pyvesync
 Author: Mark Perdue, Joe Trabulsy
 Author-email: webdjoe@gmail.com
 License: MIT
 Keywords: iot,vesync,levoit,etekcity,cosori,valceno
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -58,31 +58,31 @@
     - [Humidifier Properties](#humidifier-properties)
     - [Humidifer Methods](#humidifer-methods)
     - [600S warm mist feature](#600s-warm-mist-feature)
   - [Cosori Devices](#cosori-devices)
     - [Cosori 3.7 and 5.8 Quart Air Fryer](#cosori-37-and-58-quart-air-fryer)
       - [Air Fryer Properties](#air-fryer-properties)
       - [Air Fryer Methods](#air-fryer-methods)
+  - [Timer DataClass](#timer-dataclass)
   - [JSON Output API](#json-output-api)
     - [JSON Output for All Devices](#json-output-for-all-devices)
     - [JSON Output for Outlets](#json-output-for-outlets)
     - [JSON Output for Dimmable Switch](#json-output-for-dimmable-switch)
     - [JSON Output for Dimmable Bulb](#json-output-for-dimmable-bulb)
     - [JSON Output for Tunable Bulb](#json-output-for-tunable-bulb)
     - [JSON Output for Multicolor Bulb](#json-output-for-multicolor-bulb)
     - [JSON Output for Air Purifier](#json-output-for-air-purifier)
-    - [JSON Output for 300S Humidifier](#json-output-for-300s-humidifier)
     - [JSON Output for Core200S Purifier](#json-output-for-core200s-purifier)
     - [JSON Output for 400S Purifier](#json-output-for-400s-purifier)
     - [JSON Output for 600S Purifier](#json-output-for-600s-purifier)
 - [Notes](#notes)
 - [Debug mode](#debug-mode)
+- [Redact mode](#redact-mode)
 - [Feature Requests](#feature-requests)
 
-
 ## Installation
 
 Install the latest version from pip:
 
 ```bash
 pip install pyvesync
 ```
@@ -94,14 +94,15 @@
 1. Voltson Smart WiFi Outlet- Round (7A model ESW01-USA)
 2. Voltson Smart WiFi Outlet - Round (10A model ESW01-EU)
 3. Voltson Smart Wifi Outlet - Round (10A model ESW03-USA)
 4. Voltson Smart WiFi Outlet - Rectangle (15A model ESW15-USA)
 5. Two Plug Outdoor Outlet (ESO15-TB) (Each plug is a separate `VeSyncOutlet` object, energy readings are for both plugs combined)
 
 ### Wall Switches
+
 1. Etekcity Smart WiFi Light Switch (model ESWL01)
 2. Etekcity Wifi Dimmer Switch (ESD16)
 
 ### Levoit Air Purifiers
 
 1. LV-PUR131S
 2. Core 200S
@@ -111,35 +112,39 @@
 
 ### Etekcity Bulbs
 
 1. Soft White Dimmable Smart Bulb (ESL100)
 2. Cool to Soft White Tunable Dimmable Bulb (ESL100CW)
 
 ### Valceno Bulbs
+
 1. Multicolor Bulb (XYD0001)
 
 ### Levoit Humidifiers
+
 1. Dual 200S
 2. Classic 300S
 3. LUH-D301S-WEU Dual (200S)
 4. LV600S
 5. OasisMist LUS-O415S-WUS
 
 Cosori Air Fryer
+
 1. Cosori 3.7 and 5.8 Quart Air Fryer
 
 ## Usage
 
 To start with the module:
 
 ```python
 from pyvesync import VeSync
 
-manager = VeSync("EMAIL", "PASSWORD", "TIME_ZONE", debug=False)
+manager = VeSync("EMAIL", "PASSWORD", "TIME_ZONE", debug=False, redact=True)
 manager.login()
+# debug and redact are optional arguments, the above values are their defaults
 
 # Get/Update Devices from server - populate device lists
 manager.update()
 
 my_switch = manager.outlets[0]
 # Turn on the first switch
 my_switch.turn_on()
@@ -151,14 +156,15 @@
 
 # Set bulb brightness to 75% of first bulb in the list
 my_bulb = manager.bulbs[0]
 my_bulb.set_brightness(75)
 # get its details in JSON and print
 print(my_bulb.displayJSON())
 ```
+
 Devices are stored in the respective lists in the instantiated `VeSync` class:
 
 ```python
 manager.login()
 manager.update()
 
 manager.outlets = [VeSyncOutletObjects]
@@ -175,34 +181,39 @@
 
 # Turn on switch by switch name
 switch_name = "My Switch"
 for switch in manager.switches:
   if switch.device_name == switch_name:
     switch.turn_on()
 ```
+
 ## Configuration
 
 ### Time Zones
+
 The `time_zone` argument is optional but the specified time zone must match time zone in the tz database (IANNA Time Zone Database), see this link for reference:
 [tz database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
 The time zone determines how the energy history is generated for the smart outlets, i.e. for the week starts at 12:01AM Sunday morning at the specified time zone.  If no time zone or an invalid time zone is entered the default is America/New_York
 
 ### Outlet energy data update interval
+
 If outlets are going to be continuously polled, a custom energy update interval can be set - The default is 6 hours (21600 seconds)
 
 ```python
 manager.energy_update_interval = 360 # time in seconds
 ```
 
 ## Example Usage
 
 ### Get electricity metrics of outlets
 
 Bypass the interval check to trigger outlet energy update.
+
 ```python
+
 for s in manager.outlets:
   s.update_energy(check_bypass=False) # Get energy history for each device
 ```
 
 ## API Details
 
 ### Manager API
@@ -323,14 +334,15 @@
 `VeSyncFan.manual_mode()` - Change fan mode to manual with fan level 1
 
 `VeSyncFan.sleep_mode()` - Change fan mode to sleep
 
 `VeSyncFan.change_fan_speed(speed=None)` - Change fan speed. Call without speed to toggle to next speed
 
 Compatible levels for each model:
+
 - Core 200S [1, 2, 3]
 - Core 300S/400S [1, 2, 3, 4]
 - PUR131S [1, 2, 3]
 
 #### Levoit Purifier Core200S/300S/400S Properties
 
 `VeSyncFan.child_lock` - Return the state of the child lock (True=On/False=off)
@@ -345,14 +357,19 @@
 
 `VeSyncFan.turn_on_display()` Turn display on
 
 `VeSyncFan.turn_off_display()` Turn display off
 
 `VeSyncFan.set_night_light('on'|'dim'|'off')` - Set night light brightness
 
+`VeSyncFan.get_timer()` - Get any running timers, stores Timer DataClass in `VeSyncFan.timer`
+
+`VeSyncFan.set_timer(timer_duration=3000)` - Set a timer for the device, only turns device off. Timer DataClass stored in `VeSyncFan.timer`
+
+`VeSyncFan.clear_timer()` - Cancel any running timer
 
 ### Lights API Methods & Properties
 
 #### Brightness Light Bulb Method and Properties
 
 *Compatible with all bulbs*
 `VeSyncBulb.brightness` - Return brightness in percentage (1 - 100)
@@ -368,17 +385,17 @@
 
 `VeSyncBulb.set_color_temp(color_temp)` - Set white temperature in percentage (0 - 100)
 
 #### Multicolor Light Bulb Methods and Properties
 
 *Compatible with ESL100MC & Valceno Bulbs*
 **Properties**
-`VeSyncBulb.color` - Returns a dataclass with HSV and RGB attributes that are named tuples
+`VeSyncBulb.color` - Returns a Dataclass with HSV and RGB attributes that are named tuples
 
-```
+```python
 VeSyncBulb.color.rbg = namedtuple('RGB', ['red', 'green', 'blue'])
 VeSyncBulb.color.hsv = namedtuple('HSV', ['hue', 'saturation', 'value'])
 ```
 
 `VeSyncBulb.color_hsv` - Returns a named tuple with HSV values
 
 `VeSyncBulb.color_rgb` - Returns a named tuple with RGB values
@@ -561,14 +578,15 @@
 `VeSyncAirFryer158.cook_set_temp` - Set temperature or target temperature for preheat
 
 `VeSyncAirFryer158.cook_last_time` - The last minutes remaining returned from API for cook mode
 
 `VeSyncAirFryer158.preheat_last_time` - The last minutes remaining returned from API for preheat mode
 
 `VeSyncAirFryer158.cook_status` - Status of air fryer. This can be the following states:
+
 1. `standby` - Air fryer is off and no cook or preheat is in progress
 2. `cooking` - Air fryer is actively cooking
 3. `cookStop` - Cooking is paused and can be resumed
 4. `cookEnd` - Cooking is ended and can be resumed
 5. `heating` - Air fryer is preheating
 6. `preheatStop` - Preheat is paused and can be resumed
 7. `heatEnd` - Preheat is ended and cooking mode can be started with `cook_from_preheat()` method
@@ -577,15 +595,15 @@
 
 `VeSyncAirFryer158.is_cooking` - Returns true if air fryer is cooking
 
 `VeSyncAirFryer158.is_paused` - Returns true if air fryer is paused and can be resumed
 
 `VeSyncAirFryer158.remaining_time` - Returns minutes remaining based on timestamp of last API return when air fryer is running. Returns `None` if not running
 
-`VeSyncAirFryer158.fryer_status` - Dataclass that contains the status of the air fryer. The attributes of this dataclass are directly accessible from the `VeSyncAirFryer158` properties and **should not be directly set.**
+`VeSyncAirFryer158.fryer_status` - Dataclass that contains the status of the air fryer. The attributes of this Dataclass are directly accessible from the `VeSyncAirFryer158` properties and **should not be directly set.**
 
 ##### Air Fryer Methods
 
 `VeSyncAirFryer158.update()` - Retrieve current status
 
 `VeSyncAirFryer158.cook(set_temp: int, set_time: int)` - Set air fryer cook mode based on time and temp in defined units
 
@@ -595,14 +613,51 @@
 
 `VeSyncAirFryer158.pause()` - Pause air fryer when in `cooking` or `heating` state
 
 `VeSyncAirFryer158.resume()` - Resume air fryer when in `cookStop` or `preheatStop` state
 
 `VeSyncAirFryer158.end()` - End cooking or preheating and return air fryer to `standby` state
 
+
+### Timer DataClass
+
+This is the a Timer DataClass that is used in the  `get_timer()` or `set_timer()` methods *only implemented for Levoit Core 200S and 300S Air Purifier*, will eventually integrate with remaining devices. This object is created when the device timer methods are called. **The `pause()`, `resume()` and `stop()` methods for this DataClass only impact the timer locally and do not update the API.**
+
+```python
+from pyvesync.helpers import Timer
+
+timer = Timer(timer_duration=60, id=1)
+
+# Get time remaining in seconds
+# Calculates based on timer elapsed each time property is called
+timer.remaining_time
+
+# Get status
+timer.status
+
+# Get action
+timer.action
+
+# Set status - active or done
+timer.status = 'active'
+
+# set time remaining in seconds, does not edit status
+timer.remaining_time = 120
+
+# Pause timer - Does not update API - only pauses locally
+timer.pause()
+
+# End timer -Does not update API - only ends locally
+timer.end()
+
+# Resume timer - Does not update API - only Resumes locally
+timer.start()
+```
+
+
 ### JSON Output API
 
 The `device.displayJSON()` method outputs properties and status of the device
 
 #### JSON Output for All Devices
 
 ```python
@@ -694,17 +749,17 @@
   "Fan Level": "2", # fan level 1-3
   "Air Quality": "95", # air quality in percent
   "Mode": "auto",
   "Screen Status": "on",
   "Filter Life": "99" # remaining filter life in percent
 }
 ```
-#### JSON Output for 300S Humidifier
 
 ```python
+
 {
   "Mode": "manual", # auto, manual, sleep
   "Humidity": 20, # percent
   "Mist Virtual Level": 6, # Mist level 1 - 9
   "Water Lacks": true, # True/False
   "Water Tank Lifted": true, # True/False
   "Display": true, # True/False
@@ -715,29 +770,29 @@
 }
 ```
 
 #### JSON Output for Core200S Purifier
 
 ```python
 {
-	"Device Name": "MyPurifier",
-	"Model": "Core200S",
-	"Subdevice No": "None",
-	"Status": "on",
-	"Online": "online",
-	"Type": "wifi-air",
-	"CID": "asd_sdfKIHG7IJHGwJGJ7GJ_ag5h3G55",
-	"Mode": "manual",
-	"Filter Life": "99",
-	"Fan Level": "1",
-	"Display": true,
-	"Child Lock": false,
-	"Night Light": "off",
-	"Display Config": true,
-	"Display_Forever Config": false
+  "Device Name": "MyPurifier",
+  "Model": "Core200S",
+  "Subdevice No": "None",
+  "Status": "on",
+  "Online": "online",
+  "Type": "wifi-air",
+  "CID": "asd_sdfKIHG7IJHGwJGJ7GJ_ag5h3G55",
+  "Mode": "manual",
+  "Filter Life": "99",
+  "Fan Level": "1",
+  "Display": true,
+  "Child Lock": false,
+  "Night Light": "off",
+  "Display Config": true,
+  "Display_Forever Config": false
 }
 ```
 
 #### JSON Output for 400S Purifier
 
 ```python
 {
@@ -756,14 +811,15 @@
   "Display": true,
   "Child Lock": false,
   "Night Light": "off",
   "Display Config": true,
   "Display_Forever Config": false
 }
 ```
+
 #### JSON Output for 600S Purifier
 
 ```python
 {
   "Device Name": "My 600s",
   "Model": "LAP-C601S-WUS",
   "Subdevice No": "None",
@@ -807,40 +863,59 @@
 
 manager = vs.VeSync('user', 'pass', debug=True)
 manager.login()
 manager.update()
 # Prints device list returned from Vesync
 ```
 
+## Redact mode
+
+To make it easier to post logs online , there is a `redact` argument in the `VeSync` method. This redacts any sensitive information from the logs.
+The dafault is set to True
+
+```python
+import pyvesync.vesync as vs
+
+manager = vs.VeSync('user', 'pass', debug=True, redact=True)
+manager.login()
+manager.update()
+# Prints device list returned from Vesync
+```
+
 ## Feature Requests
 
 ~~If you would like new devices to be added, you will need to capture the packets from the app. The easiest way to do this is by using [Packet Capture for Android](https://play.google.com/store/apps/details?id=app.greyshirts.sslcapture&hl=en_US&gl=US). This works without rooting the device. If you do not have an android or are concerned with adding an app that uses a custom certificate to read the traffic, you can use an Android emulator such as [Nox](https://www.bignox.com/).~~
 
-SSL pinning makes capturing packets with android not feasible anymore. Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
+SSL pinning makes capturing packets with Android ~~not feasible anymore~~ harder than before. A system-wide proxy [ProxyDroid](https://play.google.com/store/apps/details?id=org.proxydroid&hl=en) can be used if ssl pinning is disabled [TrustMeAlready](https://github.com/ViRb3/TrustMeAlready).
+
+Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
 
 When capturing packets make sure all packets are captured from the device list, along with all functions that the app contains. The captured packets are stored in text files, please do not capture with pcap format.
 
 After you capture the packets, please redact the `accountid` and `token`. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
 
 For example:
 
 Before:
-```
+
+```json
 {
-  'tk': 'abc123abc123==3rf',
-  'accountId': '123456789',
-  'cid': 'abcdef12-3gh-ij'
+  "tk": "abc123abc123==3rf",
+  "accountId": "123456789",
+  "cid": "abcdef12-3gh-ij"
 }
 ```
+
 After:
-```
+
+```json
 {
-  'tk': 'AAA111AAA111==1AA',
-  'accountId': '111111111',
-  'cid': 'AAAAAA11-1AA-AA'
+  "tk": "AAA111AAA111==1AA",
+  "accountId": "111111111",
+  "cid": "AAAAAA11-1AA-AA"
 }
 ```
 
 All [contributions](CONTRIBUTING.md) are welcome, please run `tox` before submitting a PR to ensure code is valid.
 
 Ensure new devices are integrated in tests, please review the [testing](tests/README.md) documentation for more information.
```

### Comparing `pyvesync-2.1.6/README.md` & `pyvesync-2.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,31 +40,31 @@
     - [Humidifier Properties](#humidifier-properties)
     - [Humidifer Methods](#humidifer-methods)
     - [600S warm mist feature](#600s-warm-mist-feature)
   - [Cosori Devices](#cosori-devices)
     - [Cosori 3.7 and 5.8 Quart Air Fryer](#cosori-37-and-58-quart-air-fryer)
       - [Air Fryer Properties](#air-fryer-properties)
       - [Air Fryer Methods](#air-fryer-methods)
+  - [Timer DataClass](#timer-dataclass)
   - [JSON Output API](#json-output-api)
     - [JSON Output for All Devices](#json-output-for-all-devices)
     - [JSON Output for Outlets](#json-output-for-outlets)
     - [JSON Output for Dimmable Switch](#json-output-for-dimmable-switch)
     - [JSON Output for Dimmable Bulb](#json-output-for-dimmable-bulb)
     - [JSON Output for Tunable Bulb](#json-output-for-tunable-bulb)
     - [JSON Output for Multicolor Bulb](#json-output-for-multicolor-bulb)
     - [JSON Output for Air Purifier](#json-output-for-air-purifier)
-    - [JSON Output for 300S Humidifier](#json-output-for-300s-humidifier)
     - [JSON Output for Core200S Purifier](#json-output-for-core200s-purifier)
     - [JSON Output for 400S Purifier](#json-output-for-400s-purifier)
     - [JSON Output for 600S Purifier](#json-output-for-600s-purifier)
 - [Notes](#notes)
 - [Debug mode](#debug-mode)
+- [Redact mode](#redact-mode)
 - [Feature Requests](#feature-requests)
 
-
 ## Installation
 
 Install the latest version from pip:
 
 ```bash
 pip install pyvesync
 ```
@@ -76,14 +76,15 @@
 1. Voltson Smart WiFi Outlet- Round (7A model ESW01-USA)
 2. Voltson Smart WiFi Outlet - Round (10A model ESW01-EU)
 3. Voltson Smart Wifi Outlet - Round (10A model ESW03-USA)
 4. Voltson Smart WiFi Outlet - Rectangle (15A model ESW15-USA)
 5. Two Plug Outdoor Outlet (ESO15-TB) (Each plug is a separate `VeSyncOutlet` object, energy readings are for both plugs combined)
 
 ### Wall Switches
+
 1. Etekcity Smart WiFi Light Switch (model ESWL01)
 2. Etekcity Wifi Dimmer Switch (ESD16)
 
 ### Levoit Air Purifiers
 
 1. LV-PUR131S
 2. Core 200S
@@ -93,35 +94,39 @@
 
 ### Etekcity Bulbs
 
 1. Soft White Dimmable Smart Bulb (ESL100)
 2. Cool to Soft White Tunable Dimmable Bulb (ESL100CW)
 
 ### Valceno Bulbs
+
 1. Multicolor Bulb (XYD0001)
 
 ### Levoit Humidifiers
+
 1. Dual 200S
 2. Classic 300S
 3. LUH-D301S-WEU Dual (200S)
 4. LV600S
 5. OasisMist LUS-O415S-WUS
 
 Cosori Air Fryer
+
 1. Cosori 3.7 and 5.8 Quart Air Fryer
 
 ## Usage
 
 To start with the module:
 
 ```python
 from pyvesync import VeSync
 
-manager = VeSync("EMAIL", "PASSWORD", "TIME_ZONE", debug=False)
+manager = VeSync("EMAIL", "PASSWORD", "TIME_ZONE", debug=False, redact=True)
 manager.login()
+# debug and redact are optional arguments, the above values are their defaults
 
 # Get/Update Devices from server - populate device lists
 manager.update()
 
 my_switch = manager.outlets[0]
 # Turn on the first switch
 my_switch.turn_on()
@@ -133,14 +138,15 @@
 
 # Set bulb brightness to 75% of first bulb in the list
 my_bulb = manager.bulbs[0]
 my_bulb.set_brightness(75)
 # get its details in JSON and print
 print(my_bulb.displayJSON())
 ```
+
 Devices are stored in the respective lists in the instantiated `VeSync` class:
 
 ```python
 manager.login()
 manager.update()
 
 manager.outlets = [VeSyncOutletObjects]
@@ -157,34 +163,39 @@
 
 # Turn on switch by switch name
 switch_name = "My Switch"
 for switch in manager.switches:
   if switch.device_name == switch_name:
     switch.turn_on()
 ```
+
 ## Configuration
 
 ### Time Zones
+
 The `time_zone` argument is optional but the specified time zone must match time zone in the tz database (IANNA Time Zone Database), see this link for reference:
 [tz database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
 The time zone determines how the energy history is generated for the smart outlets, i.e. for the week starts at 12:01AM Sunday morning at the specified time zone.  If no time zone or an invalid time zone is entered the default is America/New_York
 
 ### Outlet energy data update interval
+
 If outlets are going to be continuously polled, a custom energy update interval can be set - The default is 6 hours (21600 seconds)
 
 ```python
 manager.energy_update_interval = 360 # time in seconds
 ```
 
 ## Example Usage
 
 ### Get electricity metrics of outlets
 
 Bypass the interval check to trigger outlet energy update.
+
 ```python
+
 for s in manager.outlets:
   s.update_energy(check_bypass=False) # Get energy history for each device
 ```
 
 ## API Details
 
 ### Manager API
@@ -305,14 +316,15 @@
 `VeSyncFan.manual_mode()` - Change fan mode to manual with fan level 1
 
 `VeSyncFan.sleep_mode()` - Change fan mode to sleep
 
 `VeSyncFan.change_fan_speed(speed=None)` - Change fan speed. Call without speed to toggle to next speed
 
 Compatible levels for each model:
+
 - Core 200S [1, 2, 3]
 - Core 300S/400S [1, 2, 3, 4]
 - PUR131S [1, 2, 3]
 
 #### Levoit Purifier Core200S/300S/400S Properties
 
 `VeSyncFan.child_lock` - Return the state of the child lock (True=On/False=off)
@@ -327,14 +339,19 @@
 
 `VeSyncFan.turn_on_display()` Turn display on
 
 `VeSyncFan.turn_off_display()` Turn display off
 
 `VeSyncFan.set_night_light('on'|'dim'|'off')` - Set night light brightness
 
+`VeSyncFan.get_timer()` - Get any running timers, stores Timer DataClass in `VeSyncFan.timer`
+
+`VeSyncFan.set_timer(timer_duration=3000)` - Set a timer for the device, only turns device off. Timer DataClass stored in `VeSyncFan.timer`
+
+`VeSyncFan.clear_timer()` - Cancel any running timer
 
 ### Lights API Methods & Properties
 
 #### Brightness Light Bulb Method and Properties
 
 *Compatible with all bulbs*
 `VeSyncBulb.brightness` - Return brightness in percentage (1 - 100)
@@ -350,17 +367,17 @@
 
 `VeSyncBulb.set_color_temp(color_temp)` - Set white temperature in percentage (0 - 100)
 
 #### Multicolor Light Bulb Methods and Properties
 
 *Compatible with ESL100MC & Valceno Bulbs*
 **Properties**
-`VeSyncBulb.color` - Returns a dataclass with HSV and RGB attributes that are named tuples
+`VeSyncBulb.color` - Returns a Dataclass with HSV and RGB attributes that are named tuples
 
-```
+```python
 VeSyncBulb.color.rbg = namedtuple('RGB', ['red', 'green', 'blue'])
 VeSyncBulb.color.hsv = namedtuple('HSV', ['hue', 'saturation', 'value'])
 ```
 
 `VeSyncBulb.color_hsv` - Returns a named tuple with HSV values
 
 `VeSyncBulb.color_rgb` - Returns a named tuple with RGB values
@@ -543,14 +560,15 @@
 `VeSyncAirFryer158.cook_set_temp` - Set temperature or target temperature for preheat
 
 `VeSyncAirFryer158.cook_last_time` - The last minutes remaining returned from API for cook mode
 
 `VeSyncAirFryer158.preheat_last_time` - The last minutes remaining returned from API for preheat mode
 
 `VeSyncAirFryer158.cook_status` - Status of air fryer. This can be the following states:
+
 1. `standby` - Air fryer is off and no cook or preheat is in progress
 2. `cooking` - Air fryer is actively cooking
 3. `cookStop` - Cooking is paused and can be resumed
 4. `cookEnd` - Cooking is ended and can be resumed
 5. `heating` - Air fryer is preheating
 6. `preheatStop` - Preheat is paused and can be resumed
 7. `heatEnd` - Preheat is ended and cooking mode can be started with `cook_from_preheat()` method
@@ -559,15 +577,15 @@
 
 `VeSyncAirFryer158.is_cooking` - Returns true if air fryer is cooking
 
 `VeSyncAirFryer158.is_paused` - Returns true if air fryer is paused and can be resumed
 
 `VeSyncAirFryer158.remaining_time` - Returns minutes remaining based on timestamp of last API return when air fryer is running. Returns `None` if not running
 
-`VeSyncAirFryer158.fryer_status` - Dataclass that contains the status of the air fryer. The attributes of this dataclass are directly accessible from the `VeSyncAirFryer158` properties and **should not be directly set.**
+`VeSyncAirFryer158.fryer_status` - Dataclass that contains the status of the air fryer. The attributes of this Dataclass are directly accessible from the `VeSyncAirFryer158` properties and **should not be directly set.**
 
 ##### Air Fryer Methods
 
 `VeSyncAirFryer158.update()` - Retrieve current status
 
 `VeSyncAirFryer158.cook(set_temp: int, set_time: int)` - Set air fryer cook mode based on time and temp in defined units
 
@@ -577,14 +595,51 @@
 
 `VeSyncAirFryer158.pause()` - Pause air fryer when in `cooking` or `heating` state
 
 `VeSyncAirFryer158.resume()` - Resume air fryer when in `cookStop` or `preheatStop` state
 
 `VeSyncAirFryer158.end()` - End cooking or preheating and return air fryer to `standby` state
 
+
+### Timer DataClass
+
+This is the a Timer DataClass that is used in the  `get_timer()` or `set_timer()` methods *only implemented for Levoit Core 200S and 300S Air Purifier*, will eventually integrate with remaining devices. This object is created when the device timer methods are called. **The `pause()`, `resume()` and `stop()` methods for this DataClass only impact the timer locally and do not update the API.**
+
+```python
+from pyvesync.helpers import Timer
+
+timer = Timer(timer_duration=60, id=1)
+
+# Get time remaining in seconds
+# Calculates based on timer elapsed each time property is called
+timer.remaining_time
+
+# Get status
+timer.status
+
+# Get action
+timer.action
+
+# Set status - active or done
+timer.status = 'active'
+
+# set time remaining in seconds, does not edit status
+timer.remaining_time = 120
+
+# Pause timer - Does not update API - only pauses locally
+timer.pause()
+
+# End timer -Does not update API - only ends locally
+timer.end()
+
+# Resume timer - Does not update API - only Resumes locally
+timer.start()
+```
+
+
 ### JSON Output API
 
 The `device.displayJSON()` method outputs properties and status of the device
 
 #### JSON Output for All Devices
 
 ```python
@@ -676,17 +731,17 @@
   "Fan Level": "2", # fan level 1-3
   "Air Quality": "95", # air quality in percent
   "Mode": "auto",
   "Screen Status": "on",
   "Filter Life": "99" # remaining filter life in percent
 }
 ```
-#### JSON Output for 300S Humidifier
 
 ```python
+
 {
   "Mode": "manual", # auto, manual, sleep
   "Humidity": 20, # percent
   "Mist Virtual Level": 6, # Mist level 1 - 9
   "Water Lacks": true, # True/False
   "Water Tank Lifted": true, # True/False
   "Display": true, # True/False
@@ -697,29 +752,29 @@
 }
 ```
 
 #### JSON Output for Core200S Purifier
 
 ```python
 {
-	"Device Name": "MyPurifier",
-	"Model": "Core200S",
-	"Subdevice No": "None",
-	"Status": "on",
-	"Online": "online",
-	"Type": "wifi-air",
-	"CID": "asd_sdfKIHG7IJHGwJGJ7GJ_ag5h3G55",
-	"Mode": "manual",
-	"Filter Life": "99",
-	"Fan Level": "1",
-	"Display": true,
-	"Child Lock": false,
-	"Night Light": "off",
-	"Display Config": true,
-	"Display_Forever Config": false
+  "Device Name": "MyPurifier",
+  "Model": "Core200S",
+  "Subdevice No": "None",
+  "Status": "on",
+  "Online": "online",
+  "Type": "wifi-air",
+  "CID": "asd_sdfKIHG7IJHGwJGJ7GJ_ag5h3G55",
+  "Mode": "manual",
+  "Filter Life": "99",
+  "Fan Level": "1",
+  "Display": true,
+  "Child Lock": false,
+  "Night Light": "off",
+  "Display Config": true,
+  "Display_Forever Config": false
 }
 ```
 
 #### JSON Output for 400S Purifier
 
 ```python
 {
@@ -738,14 +793,15 @@
   "Display": true,
   "Child Lock": false,
   "Night Light": "off",
   "Display Config": true,
   "Display_Forever Config": false
 }
 ```
+
 #### JSON Output for 600S Purifier
 
 ```python
 {
   "Device Name": "My 600s",
   "Model": "LAP-C601S-WUS",
   "Subdevice No": "None",
@@ -789,40 +845,59 @@
 
 manager = vs.VeSync('user', 'pass', debug=True)
 manager.login()
 manager.update()
 # Prints device list returned from Vesync
 ```
 
+## Redact mode
+
+To make it easier to post logs online , there is a `redact` argument in the `VeSync` method. This redacts any sensitive information from the logs.
+The dafault is set to True
+
+```python
+import pyvesync.vesync as vs
+
+manager = vs.VeSync('user', 'pass', debug=True, redact=True)
+manager.login()
+manager.update()
+# Prints device list returned from Vesync
+```
+
 ## Feature Requests
 
 ~~If you would like new devices to be added, you will need to capture the packets from the app. The easiest way to do this is by using [Packet Capture for Android](https://play.google.com/store/apps/details?id=app.greyshirts.sslcapture&hl=en_US&gl=US). This works without rooting the device. If you do not have an android or are concerned with adding an app that uses a custom certificate to read the traffic, you can use an Android emulator such as [Nox](https://www.bignox.com/).~~
 
-SSL pinning makes capturing packets with android not feasible anymore. Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
+SSL pinning makes capturing packets with Android ~~not feasible anymore~~ harder than before. A system-wide proxy [ProxyDroid](https://play.google.com/store/apps/details?id=org.proxydroid&hl=en) can be used if ssl pinning is disabled [TrustMeAlready](https://github.com/ViRb3/TrustMeAlready).
+
+Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
 
 When capturing packets make sure all packets are captured from the device list, along with all functions that the app contains. The captured packets are stored in text files, please do not capture with pcap format.
 
 After you capture the packets, please redact the `accountid` and `token`. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
 
 For example:
 
 Before:
-```
+
+```json
 {
-  'tk': 'abc123abc123==3rf',
-  'accountId': '123456789',
-  'cid': 'abcdef12-3gh-ij'
+  "tk": "abc123abc123==3rf",
+  "accountId": "123456789",
+  "cid": "abcdef12-3gh-ij"
 }
 ```
+
 After:
-```
+
+```json
 {
-  'tk': 'AAA111AAA111==1AA',
-  'accountId': '111111111',
-  'cid': 'AAAAAA11-1AA-AA'
+  "tk": "AAA111AAA111==1AA",
+  "accountId": "111111111",
+  "cid": "AAAAAA11-1AA-AA"
 }
 ```
 
 All [contributions](CONTRIBUTING.md) are welcome, please run `tox` before submitting a PR to ensure code is valid.
 
 Ensure new devices are integrated in tests, please review the [testing](tests/README.md) documentation for more information.
```

### Comparing `pyvesync-2.1.6/setup.py` & `pyvesync-2.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyvesync',
-    version='2.1.6',
+    version='2.1.7',
     description='pyvesync is a library to manage Etekcity\
-                 Devices and Levoit Air Purifier',
+                 Devices, Cosori Air Fryers and Levoit Air \
+                     Purifiers run on the VeSync app.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/webdjoe/pyvesync',
     author='Mark Perdue, Joe Trabulsy',
     author_email='webdjoe@gmail.com',
     license='MIT',
     classifiers=[
```

### Comparing `pyvesync-2.1.6/src/pyvesync/vesync.py` & `pyvesync-2.1.7/src/pyvesync/vesync.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,25 +72,29 @@
         dev_obj = None
     return type_str, dev_obj
 
 
 class VeSync:  # pylint: disable=function-redefined
     """VeSync API functions."""
 
-    def __init__(self, username, password, time_zone=DEFAULT_TZ, debug=False):
+    def __init__(self, username, password, time_zone=DEFAULT_TZ,
+                 debug=False, redact=True):
         """Initialize VeSync class with username, password and time zone."""
         self.debug = debug
         if debug:  # pragma: no cover
             logger.setLevel(logging.DEBUG)
             bulb_mods.logger.setLevel(logging.DEBUG)
             switch_mods.logger.setLevel(logging.DEBUG)
             outlet_mods.logger.setLevel(logging.DEBUG)
             fan_mods.logger.setLevel(logging.DEBUG)
             helpermodule.logger.setLevel(logging.DEBUG)
             kitchen_mods.logger.setLevel(logging.DEBUG)
+        self._redact = redact
+        if redact:
+            self.redact = redact
         self.username = username
         self.password = password
         self.token = None
         self.account_id = None
         self.country_code = None
         self.devices = None
         self.enabled = False
@@ -147,14 +151,28 @@
         elif new_flag is False:
             logger.setLevel(logging.WARNING)
             for m in log_modules:
                 m.logger.setLevel(logging.WARNING)
         self._debug = new_flag
 
     @property
+    def redact(self) -> bool:
+        """Return debug flag."""
+        return self._redact
+
+    @redact.setter
+    def redact(self, new_flag: bool) -> None:
+        """Set debug flag."""
+        if new_flag:
+            Helpers.shouldredact = True
+        elif new_flag is False:
+            Helpers.shouldredact = False
+        self._redact = new_flag
+
+    @property
     def energy_update_interval(self) -> int:
         """Return energy update interval."""
         return self._energy_update_interval
 
     @energy_update_interval.setter
     def energy_update_interval(self, new_energy_update: int) -> None:
         """Set energy update interval in seconds."""
```

### Comparing `pyvesync-2.1.6/src/pyvesync/vesyncbasedevice.py` & `pyvesync-2.1.7/src/pyvesync/vesyncbasedevice.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.6/src/pyvesync/vesyncbulb.py` & `pyvesync-2.1.7/src/pyvesync/vesyncbulb.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,22 +467,26 @@
                    green: Optional[NUMERIC_T] = None,
                    blue: Optional[NUMERIC_T] = None) -> bool:
         """Set status of VeSync ESL100MC."""
         brightness_update = 100
         if red is not None and green is not None and blue is not None:
             new_color = self._validate_rgb(red, green, blue)
             color_mode = 'color'
-            if new_color == self._color:
+            if self.device_status == 'on' and new_color == self._color:
                 logger.debug("New color is same as current color")
                 return True
         else:
             logger.debug("RGB Values not provided")
             new_color = None
             if brightness is not None:
                 brightness_update = int(self._validate_brightness(brightness))
+                # Do nothing if brightness is passed and same as current
+                if self.device_status == 'on' and brightness_update == self._brightness:
+                    logger.debug('Brightness already set to %s', brightness)
+                    return True
                 color_mode = 'white'
             else:
                 logger.debug("Brightness and RGB values are not set")
                 return False
 
         head = helpers.bypass_header()
         body = helpers.bypass_body_v2(self.manager)
@@ -623,15 +627,19 @@
 
     def set_brightness(self, brightness: int) -> bool:
         """Set brightness of dimmable bulb."""
         if not self.dimmable_feature:
             logger.debug('%s is not dimmable', self.device_name)
             return False
         brightness_update = int(self._validate_brightness(brightness))
-
+        if self.device_status == 'on' and brightness_update == self._brightness:
+            logger.debug("Device already in requested state")
+            return True
+        if self.device_status == 'off':
+            self.toggle('on')
         body = helpers.req_body(self.manager, 'devicestatus')
         body['uuid'] = self.uuid
         body['status'] = 'on'
         body['brightNess'] = str(brightness_update)
         r, _ = helpers.call_api(
             '/SmartBulb/v1/device/updateBrightness',
             'put',
@@ -730,15 +738,16 @@
         self.device_status = 'off'
         self.connection_status = 'offline'
         return False
 
     def set_brightness(self, brightness: int) -> bool:
         """Set brightness of tunable bulb."""
         brightness_update = int(self._validate_brightness(brightness))
-        if brightness_update == self._brightness:
+        if self.device_status == 'on' and brightness_update == self._brightness:
+            logger.debug("Device already in requested state")
             return True
         body = helpers.req_body(self.manager, 'bypass')
         body['cid'] = self.cid
         body['configModule'] = self.config_module
         light_dict: Dict[str, NUMERIC_T] = {
             'brightness': brightness_update}
         if self.device_status == 'off':
@@ -761,15 +770,16 @@
         logger.debug('%s offline', self.device_name)
 
         return False
 
     def set_color_temp(self, color_temp: int) -> bool:
         """Set Color Temperature of Bulb in pct (1 - 100)."""
         color_temp_update = self._validate_color_temp(color_temp)
-        if color_temp_update == self._color_temp:
+        if self.device_status == 'on' and color_temp_update == self._color_temp:
+            logger.debug("Device already in requested state")
             return True
         body = helpers.req_body(self.manager, 'bypass')
         body['cid'] = self.cid
         body['jsonCmd'] = {'light': {}}
         body['jsonCmd']['light']['colorTempe'] = color_temp_update
         if self.device_status == 'off':
             body['jsonCmd']['light']['action'] = 'on'
@@ -840,15 +850,16 @@
                 self._color_temp = innerresult.get('colorTemp')
             if self.rgb_shift_feature:
                 self._color_mode = innerresult.get('colorMode')
                 hue = float(round(innerresult.get('hue')/27.777777, 2))
                 sat = float(innerresult.get('saturation')/100)
                 val = float(innerresult.get('value'))
                 self._color = Color(hue=hue, saturation=sat, value=val)
-        elif response.get('code') == -11300030:
+        elif (response.get('code') == -11300030 or
+              response.get('code') == -11302030):
             logger.debug('%s device request timeout', self.device_name)
             self.connection_status = 'offline'
             self.device_status = 'off'
         elif response.get('code') == -11300027:
             logger.debug('%s device offline', self.device_name)
             self.connection_status = 'offline'
             self.device_status = 'off'
@@ -997,15 +1008,15 @@
                             "saturation": self.color_saturation,
                             "brightness": self.color_value}
             same_colors = True
             for key, val in arg_dict.items():
                 if val != "":
                     if val != current_dict[key]:
                         same_colors = False
-            if same_colors:
+            if self.device_status == 'on' and same_colors:
                 logger.debug("Device already in requested state")
                 return True
         for key, val in arg_dict.items():
             if key == 'hue' and isinstance(val, float):
                 arg_dict[key] = int(round(val*27.77778, 0))
             if key == "saturation" and isinstance(val, float):
                 arg_dict[key] = int(round(val*100, 0))
@@ -1080,15 +1091,15 @@
         force_list = ['colorTemp', 'saturation', 'hue', 'colorMode', 'value']
         if brightness is not None:
             brightness_update = self._validate_brightness(brightness)
 
             if all(locals().get(k) is None for k in force_list):
 
                 # Do nothing if brightness is passed and same as current
-                if brightness_update == self._brightness:
+                if self.device_status == 'on' and brightness_update == self._brightness:
                     logger.debug('Brightness already set to %s', brightness)
                     return True
                 request_dict['force'] = 0
             request_dict['brightness'] = int(brightness_update)
         else:
             brightness_update = None
         # Set White Temperature of Bulb in pct (1 - 100).
```

### Comparing `pyvesync-2.1.6/src/pyvesync/vesyncfan.py` & `pyvesync-2.1.7/src/pyvesync/vesyncfan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """VeSync API for controling fans and purifiers."""
 
 import json
 import logging
 from typing import Dict, Tuple, Union, Optional
 from pyvesync.vesyncbasedevice import VeSyncBaseDevice
-from pyvesync.helpers import Helpers
+from pyvesync.helpers import Helpers, Timer
 
 
 humid_features: dict = {
     'Classic300S': {
         'module': 'VeSyncHumid200300S',
         'models': ['Classic300S', 'LUH-A601S-WUSB'],
         'features': ['nightlight'],
@@ -149,14 +149,15 @@
             'filter_life': 0,
             'mode': 'manual',
             'level': 0,
             'display': False,
             'child_lock': False,
             'night_light': 'off',
         }
+        self.timer: Optional[Timer] = None
         if self.air_quality_feature is True:
             self.details['air_quality'] = 0
         self.config: Dict[str, Union[str, int, float, bool]] = {
             'display': False,
             'display_forever': False
         }
 
@@ -166,15 +167,16 @@
         standard modes are: ['getPurifierStatus', 'setSwitch',
         'setNightLight',
         'setLevel', 'setPurifierMode', 'setDisplay',
         'setChildLock']
         """
         modes = ['getPurifierStatus', 'setSwitch', 'setNightLight',
                  'setLevel', 'setPurifierMode', 'setDisplay',
-                 'setChildLock', 'setIndicatorLight']
+                 'setChildLock', 'setIndicatorLight', 'getTimer',
+                 'addTimer', 'delTimer']
         if method not in modes:
             logger.debug('Invalid mode - %s', method)
             return {}, {}
         head = Helpers.bypass_header()
         body = Helpers.bypass_body_v2(self.manager)
         body['cid'] = self.cid
         body['configModule'] = self.config_module
@@ -252,14 +254,126 @@
         else:
             logger.debug('Error in purifier response')
 
     def update(self):
         """Update Purifier details."""
         self.get_details()
 
+    def get_timer(self) -> Optional[Timer]:
+        """Retrieve running timer from purifier."""
+        head, body = self.build_api_dict('getTimer')
+        body['payload']['data'] = {}
+        if not head and not body:
+            return None
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+        if not isinstance(r, dict):
+            logger.debug('Error in purifier response')
+            return None
+        if r.get('code') != 0:
+            logger.debug('Error in purifier response, code %s', r.get('code', 'unknown'))
+            return None
+        if r.get('result', {}).get('code') != 0:
+            logger.debug('Error in purifier result response, code %s',
+                         r.get('result', {}).get('code', 'unknown'))
+            return None
+        timers = r.get('result', {}).get('result', {}).get('timers', [])
+        if not isinstance(timers, list) or len(timers) < 1:
+            self.timer = None
+            logger.debug('No timer found')
+            return None
+
+        timer = timers[0]
+        if self.timer is None:
+            self.timer = Timer(timer_duration=timer.get('duration', 0),
+                               action=timer.get('action'),
+                               id=timer.get('id'),
+                               remaining=timer.get('remaining'))
+        else:
+            self.timer.update(time_remaining=timer.get('remaining'))
+        logger.debug('Timer found: %s', str(self.timer))
+        return self.timer
+
+    def set_timer(self, timer_duration: int) -> bool:
+        """Set timer for Purifier.
+
+        Arguments
+        ----------
+        timer_duration: int
+            Duration of timer in seconds
+        """
+        if self.device_status != 'on':
+            logger.debug("Can't set timer when device is off")
+        head, body = self.build_api_dict('addTimer')
+        if not head and not body:
+            return False
+
+        body['payload']['data'] = {
+            'total': timer_duration,
+            'action': 'off',
+        }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r.get('code') != 0:
+            logger.debug('Error in purifier response, code %s', r.get('code', 'unknown'))
+            return False
+        if r.get('result', {}).get('code') != 0:
+            logger.debug('Error in purifier result response, code %s',
+                         r.get('result', {}).get('code', 'unknown'))
+            return False
+        timer_id = r.get('result', {}).get('result', {}).get('id')
+        if timer_id is not None:
+            self.timer = Timer(timer_duration=timer_duration,
+                               action='off',
+                               id=timer_id)
+        else:
+            self.timer = Timer(timer_duration=timer_duration,
+                               action='off')
+        return True
+
+    def clear_timer(self) -> bool:
+        """Clear timer."""
+        self.get_timer()
+        if self.timer is None:
+            logger.debug('No timer to clear')
+            return False
+        if self.timer.id is None:
+            logger.debug("Timer doesn't have an ID, can't clear")
+        head, body = self.build_api_dict('delTimer')
+        if not head and not body:
+            return False
+
+        body['payload']['data'] = {
+            'id': self.timer.id
+        }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r.get('code') != 0:
+            logger.debug('Error in purifier response, code %s', r.get('code', 'unknown'))
+            return False
+        logger.debug("Timer cleared")
+        return True
+
     def change_fan_speed(self,
                          speed=None) -> bool:
         """Change fan speed based on levels in configuration dict."""
         speeds: list = self.config_dict.get('levels', [])
         current_speed = self.speed
 
         if speed is not None:
@@ -607,15 +721,15 @@
 class VeSyncAir131(VeSyncBaseDevice):
     """Levoit Air Purifier Class."""
 
     def __init__(self, details, manager):
         """Initilize air purifier class."""
         super().__init__(details, manager)
 
-        self.details: Dict = {}
+        self.details = {}
 
     def get_details(self) -> None:
         """Build Air Purifier details dictionary."""
         body = Helpers.req_body(self.manager, 'devicedetail')
         body['uuid'] = self.uuid
         head = Helpers.req_headers(self.manager)
 
@@ -681,14 +795,40 @@
         return self.details.get('air_quality', 'unknown')
 
     @property
     def screen_status(self) -> str:
         """Return Screen status (on/off)."""
         return self.details.get('screen_status', 'unknown')
 
+    def turn_on_display(self) -> bool:
+        """Turn display on."""
+        return self.toggle_display('on')
+
+    def turn_off_display(self) -> bool:
+        """Turn display off."""
+        return self.toggle_display('off')
+
+    def toggle_display(self, status: str) -> bool:
+        """Toggle Display of VeSync LV-PUR131."""
+        if status.lower() not in ['on', 'off']:
+            logger.debug('Invalid display status - %s', status)
+            return False
+        head = Helpers.req_headers(self.manager)
+        body = Helpers.req_body(self.manager, 'devicestatus')
+        body['status'] = status.lower()
+        r, _ = Helpers.call_api(
+            '/131airPurifier/v1/device/updateScreen', 'put',
+            json_object=body, headers=head
+        )
+        if r is not None and Helpers.code_check(r):
+            self.details['screen_status'] = status.lower()
+            return True
+        logger.debug('Error toggling display for %s', self.device_name)
+        return False
+
     def turn_on(self) -> bool:
         """Turn Air Purifier on."""
         if self.device_status != 'on':
             body = Helpers.req_body(self.manager, 'devicestatus')
             body['uuid'] = self.uuid
             body['status'] = 'on'
             head = Helpers.req_headers(self.manager)
```

### Comparing `pyvesync-2.1.6/src/pyvesync/vesynckitchen.py` & `pyvesync-2.1.7/src/pyvesync/vesynckitchen.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.6/src/pyvesync/vesyncoutlet.py` & `pyvesync-2.1.7/src/pyvesync/vesyncoutlet.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.6/src/pyvesync/vesyncswitch.py` & `pyvesync-2.1.7/src/pyvesync/vesyncswitch.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.6/src/pyvesync.egg-info/PKG-INFO` & `pyvesync-2.1.7/src/pyvesync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyvesync
-Version: 2.1.6
-Summary: pyvesync is a library to manage Etekcity                 Devices and Levoit Air Purifier
+Version: 2.1.7
+Summary: pyvesync is a library to manage Etekcity                 Devices, Cosori Air Fryers and Levoit Air                      Purifiers run on the VeSync app.
 Home-page: https://github.com/webdjoe/pyvesync
 Author: Mark Perdue, Joe Trabulsy
 Author-email: webdjoe@gmail.com
 License: MIT
 Keywords: iot,vesync,levoit,etekcity,cosori,valceno
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -58,31 +58,31 @@
     - [Humidifier Properties](#humidifier-properties)
     - [Humidifer Methods](#humidifer-methods)
     - [600S warm mist feature](#600s-warm-mist-feature)
   - [Cosori Devices](#cosori-devices)
     - [Cosori 3.7 and 5.8 Quart Air Fryer](#cosori-37-and-58-quart-air-fryer)
       - [Air Fryer Properties](#air-fryer-properties)
       - [Air Fryer Methods](#air-fryer-methods)
+  - [Timer DataClass](#timer-dataclass)
   - [JSON Output API](#json-output-api)
     - [JSON Output for All Devices](#json-output-for-all-devices)
     - [JSON Output for Outlets](#json-output-for-outlets)
     - [JSON Output for Dimmable Switch](#json-output-for-dimmable-switch)
     - [JSON Output for Dimmable Bulb](#json-output-for-dimmable-bulb)
     - [JSON Output for Tunable Bulb](#json-output-for-tunable-bulb)
     - [JSON Output for Multicolor Bulb](#json-output-for-multicolor-bulb)
     - [JSON Output for Air Purifier](#json-output-for-air-purifier)
-    - [JSON Output for 300S Humidifier](#json-output-for-300s-humidifier)
     - [JSON Output for Core200S Purifier](#json-output-for-core200s-purifier)
     - [JSON Output for 400S Purifier](#json-output-for-400s-purifier)
     - [JSON Output for 600S Purifier](#json-output-for-600s-purifier)
 - [Notes](#notes)
 - [Debug mode](#debug-mode)
+- [Redact mode](#redact-mode)
 - [Feature Requests](#feature-requests)
 
-
 ## Installation
 
 Install the latest version from pip:
 
 ```bash
 pip install pyvesync
 ```
@@ -94,14 +94,15 @@
 1. Voltson Smart WiFi Outlet- Round (7A model ESW01-USA)
 2. Voltson Smart WiFi Outlet - Round (10A model ESW01-EU)
 3. Voltson Smart Wifi Outlet - Round (10A model ESW03-USA)
 4. Voltson Smart WiFi Outlet - Rectangle (15A model ESW15-USA)
 5. Two Plug Outdoor Outlet (ESO15-TB) (Each plug is a separate `VeSyncOutlet` object, energy readings are for both plugs combined)
 
 ### Wall Switches
+
 1. Etekcity Smart WiFi Light Switch (model ESWL01)
 2. Etekcity Wifi Dimmer Switch (ESD16)
 
 ### Levoit Air Purifiers
 
 1. LV-PUR131S
 2. Core 200S
@@ -111,35 +112,39 @@
 
 ### Etekcity Bulbs
 
 1. Soft White Dimmable Smart Bulb (ESL100)
 2. Cool to Soft White Tunable Dimmable Bulb (ESL100CW)
 
 ### Valceno Bulbs
+
 1. Multicolor Bulb (XYD0001)
 
 ### Levoit Humidifiers
+
 1. Dual 200S
 2. Classic 300S
 3. LUH-D301S-WEU Dual (200S)
 4. LV600S
 5. OasisMist LUS-O415S-WUS
 
 Cosori Air Fryer
+
 1. Cosori 3.7 and 5.8 Quart Air Fryer
 
 ## Usage
 
 To start with the module:
 
 ```python
 from pyvesync import VeSync
 
-manager = VeSync("EMAIL", "PASSWORD", "TIME_ZONE", debug=False)
+manager = VeSync("EMAIL", "PASSWORD", "TIME_ZONE", debug=False, redact=True)
 manager.login()
+# debug and redact are optional arguments, the above values are their defaults
 
 # Get/Update Devices from server - populate device lists
 manager.update()
 
 my_switch = manager.outlets[0]
 # Turn on the first switch
 my_switch.turn_on()
@@ -151,14 +156,15 @@
 
 # Set bulb brightness to 75% of first bulb in the list
 my_bulb = manager.bulbs[0]
 my_bulb.set_brightness(75)
 # get its details in JSON and print
 print(my_bulb.displayJSON())
 ```
+
 Devices are stored in the respective lists in the instantiated `VeSync` class:
 
 ```python
 manager.login()
 manager.update()
 
 manager.outlets = [VeSyncOutletObjects]
@@ -175,34 +181,39 @@
 
 # Turn on switch by switch name
 switch_name = "My Switch"
 for switch in manager.switches:
   if switch.device_name == switch_name:
     switch.turn_on()
 ```
+
 ## Configuration
 
 ### Time Zones
+
 The `time_zone` argument is optional but the specified time zone must match time zone in the tz database (IANNA Time Zone Database), see this link for reference:
 [tz database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
 The time zone determines how the energy history is generated for the smart outlets, i.e. for the week starts at 12:01AM Sunday morning at the specified time zone.  If no time zone or an invalid time zone is entered the default is America/New_York
 
 ### Outlet energy data update interval
+
 If outlets are going to be continuously polled, a custom energy update interval can be set - The default is 6 hours (21600 seconds)
 
 ```python
 manager.energy_update_interval = 360 # time in seconds
 ```
 
 ## Example Usage
 
 ### Get electricity metrics of outlets
 
 Bypass the interval check to trigger outlet energy update.
+
 ```python
+
 for s in manager.outlets:
   s.update_energy(check_bypass=False) # Get energy history for each device
 ```
 
 ## API Details
 
 ### Manager API
@@ -323,14 +334,15 @@
 `VeSyncFan.manual_mode()` - Change fan mode to manual with fan level 1
 
 `VeSyncFan.sleep_mode()` - Change fan mode to sleep
 
 `VeSyncFan.change_fan_speed(speed=None)` - Change fan speed. Call without speed to toggle to next speed
 
 Compatible levels for each model:
+
 - Core 200S [1, 2, 3]
 - Core 300S/400S [1, 2, 3, 4]
 - PUR131S [1, 2, 3]
 
 #### Levoit Purifier Core200S/300S/400S Properties
 
 `VeSyncFan.child_lock` - Return the state of the child lock (True=On/False=off)
@@ -345,14 +357,19 @@
 
 `VeSyncFan.turn_on_display()` Turn display on
 
 `VeSyncFan.turn_off_display()` Turn display off
 
 `VeSyncFan.set_night_light('on'|'dim'|'off')` - Set night light brightness
 
+`VeSyncFan.get_timer()` - Get any running timers, stores Timer DataClass in `VeSyncFan.timer`
+
+`VeSyncFan.set_timer(timer_duration=3000)` - Set a timer for the device, only turns device off. Timer DataClass stored in `VeSyncFan.timer`
+
+`VeSyncFan.clear_timer()` - Cancel any running timer
 
 ### Lights API Methods & Properties
 
 #### Brightness Light Bulb Method and Properties
 
 *Compatible with all bulbs*
 `VeSyncBulb.brightness` - Return brightness in percentage (1 - 100)
@@ -368,17 +385,17 @@
 
 `VeSyncBulb.set_color_temp(color_temp)` - Set white temperature in percentage (0 - 100)
 
 #### Multicolor Light Bulb Methods and Properties
 
 *Compatible with ESL100MC & Valceno Bulbs*
 **Properties**
-`VeSyncBulb.color` - Returns a dataclass with HSV and RGB attributes that are named tuples
+`VeSyncBulb.color` - Returns a Dataclass with HSV and RGB attributes that are named tuples
 
-```
+```python
 VeSyncBulb.color.rbg = namedtuple('RGB', ['red', 'green', 'blue'])
 VeSyncBulb.color.hsv = namedtuple('HSV', ['hue', 'saturation', 'value'])
 ```
 
 `VeSyncBulb.color_hsv` - Returns a named tuple with HSV values
 
 `VeSyncBulb.color_rgb` - Returns a named tuple with RGB values
@@ -561,14 +578,15 @@
 `VeSyncAirFryer158.cook_set_temp` - Set temperature or target temperature for preheat
 
 `VeSyncAirFryer158.cook_last_time` - The last minutes remaining returned from API for cook mode
 
 `VeSyncAirFryer158.preheat_last_time` - The last minutes remaining returned from API for preheat mode
 
 `VeSyncAirFryer158.cook_status` - Status of air fryer. This can be the following states:
+
 1. `standby` - Air fryer is off and no cook or preheat is in progress
 2. `cooking` - Air fryer is actively cooking
 3. `cookStop` - Cooking is paused and can be resumed
 4. `cookEnd` - Cooking is ended and can be resumed
 5. `heating` - Air fryer is preheating
 6. `preheatStop` - Preheat is paused and can be resumed
 7. `heatEnd` - Preheat is ended and cooking mode can be started with `cook_from_preheat()` method
@@ -577,15 +595,15 @@
 
 `VeSyncAirFryer158.is_cooking` - Returns true if air fryer is cooking
 
 `VeSyncAirFryer158.is_paused` - Returns true if air fryer is paused and can be resumed
 
 `VeSyncAirFryer158.remaining_time` - Returns minutes remaining based on timestamp of last API return when air fryer is running. Returns `None` if not running
 
-`VeSyncAirFryer158.fryer_status` - Dataclass that contains the status of the air fryer. The attributes of this dataclass are directly accessible from the `VeSyncAirFryer158` properties and **should not be directly set.**
+`VeSyncAirFryer158.fryer_status` - Dataclass that contains the status of the air fryer. The attributes of this Dataclass are directly accessible from the `VeSyncAirFryer158` properties and **should not be directly set.**
 
 ##### Air Fryer Methods
 
 `VeSyncAirFryer158.update()` - Retrieve current status
 
 `VeSyncAirFryer158.cook(set_temp: int, set_time: int)` - Set air fryer cook mode based on time and temp in defined units
 
@@ -595,14 +613,51 @@
 
 `VeSyncAirFryer158.pause()` - Pause air fryer when in `cooking` or `heating` state
 
 `VeSyncAirFryer158.resume()` - Resume air fryer when in `cookStop` or `preheatStop` state
 
 `VeSyncAirFryer158.end()` - End cooking or preheating and return air fryer to `standby` state
 
+
+### Timer DataClass
+
+This is the a Timer DataClass that is used in the  `get_timer()` or `set_timer()` methods *only implemented for Levoit Core 200S and 300S Air Purifier*, will eventually integrate with remaining devices. This object is created when the device timer methods are called. **The `pause()`, `resume()` and `stop()` methods for this DataClass only impact the timer locally and do not update the API.**
+
+```python
+from pyvesync.helpers import Timer
+
+timer = Timer(timer_duration=60, id=1)
+
+# Get time remaining in seconds
+# Calculates based on timer elapsed each time property is called
+timer.remaining_time
+
+# Get status
+timer.status
+
+# Get action
+timer.action
+
+# Set status - active or done
+timer.status = 'active'
+
+# set time remaining in seconds, does not edit status
+timer.remaining_time = 120
+
+# Pause timer - Does not update API - only pauses locally
+timer.pause()
+
+# End timer -Does not update API - only ends locally
+timer.end()
+
+# Resume timer - Does not update API - only Resumes locally
+timer.start()
+```
+
+
 ### JSON Output API
 
 The `device.displayJSON()` method outputs properties and status of the device
 
 #### JSON Output for All Devices
 
 ```python
@@ -694,17 +749,17 @@
   "Fan Level": "2", # fan level 1-3
   "Air Quality": "95", # air quality in percent
   "Mode": "auto",
   "Screen Status": "on",
   "Filter Life": "99" # remaining filter life in percent
 }
 ```
-#### JSON Output for 300S Humidifier
 
 ```python
+
 {
   "Mode": "manual", # auto, manual, sleep
   "Humidity": 20, # percent
   "Mist Virtual Level": 6, # Mist level 1 - 9
   "Water Lacks": true, # True/False
   "Water Tank Lifted": true, # True/False
   "Display": true, # True/False
@@ -715,29 +770,29 @@
 }
 ```
 
 #### JSON Output for Core200S Purifier
 
 ```python
 {
-	"Device Name": "MyPurifier",
-	"Model": "Core200S",
-	"Subdevice No": "None",
-	"Status": "on",
-	"Online": "online",
-	"Type": "wifi-air",
-	"CID": "asd_sdfKIHG7IJHGwJGJ7GJ_ag5h3G55",
-	"Mode": "manual",
-	"Filter Life": "99",
-	"Fan Level": "1",
-	"Display": true,
-	"Child Lock": false,
-	"Night Light": "off",
-	"Display Config": true,
-	"Display_Forever Config": false
+  "Device Name": "MyPurifier",
+  "Model": "Core200S",
+  "Subdevice No": "None",
+  "Status": "on",
+  "Online": "online",
+  "Type": "wifi-air",
+  "CID": "asd_sdfKIHG7IJHGwJGJ7GJ_ag5h3G55",
+  "Mode": "manual",
+  "Filter Life": "99",
+  "Fan Level": "1",
+  "Display": true,
+  "Child Lock": false,
+  "Night Light": "off",
+  "Display Config": true,
+  "Display_Forever Config": false
 }
 ```
 
 #### JSON Output for 400S Purifier
 
 ```python
 {
@@ -756,14 +811,15 @@
   "Display": true,
   "Child Lock": false,
   "Night Light": "off",
   "Display Config": true,
   "Display_Forever Config": false
 }
 ```
+
 #### JSON Output for 600S Purifier
 
 ```python
 {
   "Device Name": "My 600s",
   "Model": "LAP-C601S-WUS",
   "Subdevice No": "None",
@@ -807,40 +863,59 @@
 
 manager = vs.VeSync('user', 'pass', debug=True)
 manager.login()
 manager.update()
 # Prints device list returned from Vesync
 ```
 
+## Redact mode
+
+To make it easier to post logs online , there is a `redact` argument in the `VeSync` method. This redacts any sensitive information from the logs.
+The dafault is set to True
+
+```python
+import pyvesync.vesync as vs
+
+manager = vs.VeSync('user', 'pass', debug=True, redact=True)
+manager.login()
+manager.update()
+# Prints device list returned from Vesync
+```
+
 ## Feature Requests
 
 ~~If you would like new devices to be added, you will need to capture the packets from the app. The easiest way to do this is by using [Packet Capture for Android](https://play.google.com/store/apps/details?id=app.greyshirts.sslcapture&hl=en_US&gl=US). This works without rooting the device. If you do not have an android or are concerned with adding an app that uses a custom certificate to read the traffic, you can use an Android emulator such as [Nox](https://www.bignox.com/).~~
 
-SSL pinning makes capturing packets with android not feasible anymore. Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
+SSL pinning makes capturing packets with Android ~~not feasible anymore~~ harder than before. A system-wide proxy [ProxyDroid](https://play.google.com/store/apps/details?id=org.proxydroid&hl=en) can be used if ssl pinning is disabled [TrustMeAlready](https://github.com/ViRb3/TrustMeAlready).
+
+Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
 
 When capturing packets make sure all packets are captured from the device list, along with all functions that the app contains. The captured packets are stored in text files, please do not capture with pcap format.
 
 After you capture the packets, please redact the `accountid` and `token`. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
 
 For example:
 
 Before:
-```
+
+```json
 {
-  'tk': 'abc123abc123==3rf',
-  'accountId': '123456789',
-  'cid': 'abcdef12-3gh-ij'
+  "tk": "abc123abc123==3rf",
+  "accountId": "123456789",
+  "cid": "abcdef12-3gh-ij"
 }
 ```
+
 After:
-```
+
+```json
 {
-  'tk': 'AAA111AAA111==1AA',
-  'accountId': '111111111',
-  'cid': 'AAAAAA11-1AA-AA'
+  "tk": "AAA111AAA111==1AA",
+  "accountId": "111111111",
+  "cid": "AAAAAA11-1AA-AA"
 }
 ```
 
 All [contributions](CONTRIBUTING.md) are welcome, please run `tox` before submitting a PR to ensure code is valid.
 
 Ensure new devices are integrated in tests, please review the [testing](tests/README.md) documentation for more information.
```

### Comparing `pyvesync-2.1.6/src/pyvesync.egg-info/SOURCES.txt` & `pyvesync-2.1.7/src/pyvesync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

