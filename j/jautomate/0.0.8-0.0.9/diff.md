# Comparing `tmp/jautomate-0.0.8.tar.gz` & `tmp/jautomate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jautomate-0.0.8.tar", last modified: Wed May 17 19:26:33 2023, max compression
+gzip compressed data, was "jautomate-0.0.9.tar", last modified: Thu May 18 14:17:37 2023, max compression
```

## Comparing `jautomate-0.0.8.tar` & `jautomate-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.042077 jautomate-0.0.8/
--rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-17 19:26:33.042173 jautomate-0.0.8/PKG-INFO
--rw-r--r--   0 yoxall     (503) staff       (20)     2372 2023-05-16 18:24:54.000000 jautomate-0.0.8/README.md
--rw-r--r--   0 yoxall     (503) staff       (20)      140 2023-05-05 12:20:37.000000 jautomate-0.0.8/pyproject.toml
--rw-r--r--   0 yoxall     (503) staff       (20)      805 2023-05-17 19:26:33.042527 jautomate-0.0.8/setup.cfg
--rw-r--r--   0 yoxall     (503) staff       (20)       79 2023-05-05 12:20:37.000000 jautomate-0.0.8/setup.py
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.037235 jautomate-0.0.8/src/
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.040117 jautomate-0.0.8/src/jautomate/
--rw-r--r--   0 yoxall     (503) staff       (20)      113 2023-05-17 19:26:23.000000 jautomate-0.0.8/src/jautomate/__init__.py
--rw-r--r--   0 yoxall     (503) staff       (20)      279 2023-05-05 12:20:37.000000 jautomate-0.0.8/src/jautomate/__main__.py
--rw-r--r--   0 yoxall     (503) staff       (20)     8320 2023-05-17 15:53:41.000000 jautomate-0.0.8/src/jautomate/actions.py
--rw-r--r--   0 yoxall     (503) staff       (20)      460 2023-05-05 12:20:37.000000 jautomate-0.0.8/src/jautomate/api.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1768 2023-05-16 12:57:26.000000 jautomate-0.0.8/src/jautomate/assets.py
--rw-r--r--   0 yoxall     (503) staff       (20)     6023 2023-05-17 15:49:16.000000 jautomate-0.0.8/src/jautomate/cli.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1138 2023-05-05 12:20:37.000000 jautomate-0.0.8/src/jautomate/logger.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1824 2023-05-05 12:20:37.000000 jautomate-0.0.8/src/jautomate/utils.py
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.041452 jautomate-0.0.8/src/jautomate.egg-info/
--rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/PKG-INFO
--rw-r--r--   0 yoxall     (503) staff       (20)      559 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/SOURCES.txt
--rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/dependency_links.txt
--rw-r--r--   0 yoxall     (503) staff       (20)       54 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/entry_points.txt
--rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-15 18:37:15.000000 jautomate-0.0.8/src/jautomate.egg-info/not-zip-safe
--rw-r--r--   0 yoxall     (503) staff       (20)       36 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/requires.txt
--rw-r--r--   0 yoxall     (503) staff       (20)       10 2023-05-17 19:26:33.000000 jautomate-0.0.8/src/jautomate.egg-info/top_level.txt
-drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-17 19:26:33.041906 jautomate-0.0.8/tests/
--rw-r--r--   0 yoxall     (503) staff       (20)       58 2023-05-05 12:20:37.000000 jautomate-0.0.8/tests/test_actions.py
--rw-r--r--   0 yoxall     (503) staff       (20)      308 2023-05-05 12:20:37.000000 jautomate-0.0.8/tests/test_jautomate.py
--rw-r--r--   0 yoxall     (503) staff       (20)     1583 2023-05-05 12:20:37.000000 jautomate-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-18 14:17:37.759308 jautomate-0.0.9/
+-rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-18 14:17:37.759384 jautomate-0.0.9/PKG-INFO
+-rw-r--r--   0 yoxall     (503) staff       (20)     2372 2023-05-18 14:16:36.000000 jautomate-0.0.9/README.md
+-rw-r--r--   0 yoxall     (503) staff       (20)      140 2023-05-05 12:20:37.000000 jautomate-0.0.9/pyproject.toml
+-rw-r--r--   0 yoxall     (503) staff       (20)      805 2023-05-18 14:17:37.759691 jautomate-0.0.9/setup.cfg
+-rw-r--r--   0 yoxall     (503) staff       (20)       79 2023-05-05 12:20:37.000000 jautomate-0.0.9/setup.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-18 14:17:37.754733 jautomate-0.0.9/src/
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-18 14:17:37.757268 jautomate-0.0.9/src/jautomate/
+-rw-r--r--   0 yoxall     (503) staff       (20)      113 2023-05-18 14:17:12.000000 jautomate-0.0.9/src/jautomate/__init__.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      279 2023-05-05 12:20:37.000000 jautomate-0.0.9/src/jautomate/__main__.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     8264 2023-05-18 14:16:36.000000 jautomate-0.0.9/src/jautomate/actions.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      460 2023-05-05 12:20:37.000000 jautomate-0.0.9/src/jautomate/api.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1768 2023-05-18 14:16:36.000000 jautomate-0.0.9/src/jautomate/assets.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     6023 2023-05-18 14:16:36.000000 jautomate-0.0.9/src/jautomate/cli.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1138 2023-05-05 12:20:37.000000 jautomate-0.0.9/src/jautomate/logger.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1824 2023-05-05 12:20:37.000000 jautomate-0.0.9/src/jautomate/utils.py
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-18 14:17:37.758649 jautomate-0.0.9/src/jautomate.egg-info/
+-rw-r--r--   0 yoxall     (503) staff       (20)     2731 2023-05-18 14:17:37.000000 jautomate-0.0.9/src/jautomate.egg-info/PKG-INFO
+-rw-r--r--   0 yoxall     (503) staff       (20)      559 2023-05-18 14:17:37.000000 jautomate-0.0.9/src/jautomate.egg-info/SOURCES.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-05-18 14:17:37.000000 jautomate-0.0.9/src/jautomate.egg-info/dependency_links.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)       54 2023-05-18 14:17:37.000000 jautomate-0.0.9/src/jautomate.egg-info/entry_points.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)        1 2023-03-15 18:37:15.000000 jautomate-0.0.9/src/jautomate.egg-info/not-zip-safe
+-rw-r--r--   0 yoxall     (503) staff       (20)       36 2023-05-18 14:17:37.000000 jautomate-0.0.9/src/jautomate.egg-info/requires.txt
+-rw-r--r--   0 yoxall     (503) staff       (20)       10 2023-05-18 14:17:37.000000 jautomate-0.0.9/src/jautomate.egg-info/top_level.txt
+drwxr-xr-x   0 yoxall     (503) staff       (20)        0 2023-05-18 14:17:37.759144 jautomate-0.0.9/tests/
+-rw-r--r--   0 yoxall     (503) staff       (20)       58 2023-05-05 12:20:37.000000 jautomate-0.0.9/tests/test_actions.py
+-rw-r--r--   0 yoxall     (503) staff       (20)      308 2023-05-05 12:20:37.000000 jautomate-0.0.9/tests/test_jautomate.py
+-rw-r--r--   0 yoxall     (503) staff       (20)     1583 2023-05-05 12:20:37.000000 jautomate-0.0.9/tests/test_utils.py
```

### Comparing `jautomate-0.0.8/PKG-INFO` & `jautomate-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jautomate
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automates MDM tasks using the Jamf APIs
 Author: Dustin Yoxall
 Author-email: yoxall.dustin@ccpsstaff.org
 License: MIT
 Keywords: python,jamf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jautomate-0.0.8/README.md` & `jautomate-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.8/setup.cfg` & `jautomate-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.8/src/jautomate/actions.py` & `jautomate-0.0.9/src/jautomate/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,38 +181,36 @@
             }
             jamf_p.update_mobile_device(payload, asset.jamf_id)
             j_logger.debug("Asset: %s Ok", asset.asset_tag)
 
         # Process for computers
         if asset.device_type == 'computer':
             payload = {
-                "general": {
+                "userAndLocation": {
+                    "realname": asset.student_name,
+                    "email": asset.email_address,
+                    "position": asset.position,
+                    "buildingId": get_building_id(asset.building),
+                    "room": asset.homeroom,
                     "extensionAttributes": [
                         {
                             "definitionId": "4",
                             "name": "Grade",
                             "values": [
-                                f"{asset.student_grade:02}"
+                                asset.student_grade
                             ]
                         },
                         {
                             "definitionId": "3",
                             "name": "GradYear",
                             "values": [
                                 asset.grad_year
                             ]
                         }
                     ]
-                },
-                "userAndLocation": {
-                    "realname": asset.student_name,
-                    "email": asset.email_address,
-                    "position": asset.position,
-                    "buildingId": get_building_id(asset.building),
-                    "room": asset.homeroom,
                 }
             }
             jamf_p.update_computer_inventory(payload, asset.jamf_id)
             j_logger.debug("Asset: %s Ok", asset.asset_tag)
 
 
 def get_single_computer_record_by_asset_tag(asset_tag: str):
```

### Comparing `jautomate-0.0.8/src/jautomate/assets.py` & `jautomate-0.0.9/src/jautomate/assets.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.8/src/jautomate/cli.py` & `jautomate-0.0.9/src/jautomate/cli.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.8/src/jautomate/logger.py` & `jautomate-0.0.9/src/jautomate/logger.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.8/src/jautomate/utils.py` & `jautomate-0.0.9/src/jautomate/utils.py`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.8/src/jautomate.egg-info/PKG-INFO` & `jautomate-0.0.9/src/jautomate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jautomate
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automates MDM tasks using the Jamf APIs
 Author: Dustin Yoxall
 Author-email: yoxall.dustin@ccpsstaff.org
 License: MIT
 Keywords: python,jamf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jautomate-0.0.8/src/jautomate.egg-info/SOURCES.txt` & `jautomate-0.0.9/src/jautomate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jautomate-0.0.8/tests/test_utils.py` & `jautomate-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

