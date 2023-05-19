# Comparing `tmp/crosscompute-views-map-0.2.0.tar.gz` & `tmp/crosscompute-views-map-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-views-map-0.2.0.tar", last modified: Tue Apr 25 22:54:45 2023, max compression
+gzip compressed data, was "crosscompute-views-map-0.2.1.tar", last modified: Thu May 18 19:46:24 2023, max compression
```

## Comparing `crosscompute-views-map-0.2.0.tar` & `crosscompute-views-map-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.751627 crosscompute-views-map-0.2.0/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-25 22:39:14.000000 crosscompute-views-map-0.2.0/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2151 2023-04-25 22:54:45.751627 crosscompute-views-map-0.2.0/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1187 2023-04-25 22:39:54.000000 crosscompute-views-map-0.2.0/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.746627 crosscompute-views-map-0.2.0/crosscompute_views_map/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-08-23 20:11:01.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/__init__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.750627 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      221 2023-02-18 04:54:49.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/deck-screengrid-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1417 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/deck-screengrid-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)       47 2023-04-01 12:03:40.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/map.css
--rw-r--r--   0 rhh       (1000) rhh       (1000)      801 2023-02-18 04:54:49.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      772 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-location-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      114 2023-02-18 04:54:49.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-location-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      363 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-location-input.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      322 2023-02-18 04:54:49.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      607 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-output.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      131 2023-04-01 12:03:40.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      468 2023-04-01 12:03:40.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/constants.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.751627 crosscompute-views-map-0.2.0/crosscompute_views_map/routines/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-08-23 20:11:01.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/routines/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1012 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/routines/asset.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     7769 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/routines/variable.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.748627 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2151 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1079 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      259 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/entry_points.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       41 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       23 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-08-23 22:59:08.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1503 2023-04-25 22:54:45.753627 crosscompute-views-map-0.2.0/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2022-08-23 20:11:01.000000 crosscompute-views-map-0.2.0/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-18 19:46:24.345796 crosscompute-views-map-0.2.1/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2151 2023-05-18 19:46:24.345796 crosscompute-views-map-0.2.1/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1187 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-18 19:46:24.342796 crosscompute-views-map-0.2.1/crosscompute_views_map/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/__init__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-18 19:46:24.344796 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      221 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/deck-screengrid-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1417 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/deck-screengrid-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       47 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/map.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      801 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      772 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-location-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      114 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-location-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      363 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-location-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      322 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      607 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      131 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      468 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/constants.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-18 19:46:24.345796 crosscompute-views-map-0.2.1/crosscompute_views_map/routines/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/routines/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1012 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/routines/asset.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     7757 2023-05-17 09:19:19.000000 crosscompute-views-map-0.2.1/crosscompute_views_map/routines/variable.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-18 19:46:24.343796 crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2151 2023-05-18 19:46:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1079 2023-05-18 19:46:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-18 19:46:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      259 2023-05-18 19:46:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/entry_points.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       41 2023-05-18 19:46:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       23 2023-05-18 19:46:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-18 19:46:24.000000 crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1503 2023-05-18 19:46:24.346796 crosscompute-views-map-0.2.1/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2023-05-17 09:18:24.000000 crosscompute-views-map-0.2.1/setup.py
```

### Comparing `crosscompute-views-map-0.2.0/LICENSE.md` & `crosscompute-views-map-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.2.0/PKG-INFO` & `crosscompute-views-map-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-views-map
-Version: 0.2.0
+Version: 0.2.1
 Summary: Render maps in your automations.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-views-map/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-views-map
```

### Comparing `crosscompute-views-map-0.2.0/README.md` & `crosscompute-views-map-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.2.0/crosscompute_views_map/assets/deck-screengrid-output.js` & `crosscompute-views-map-0.2.1/crosscompute_views_map/assets/deck-screengrid-output.js`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-header.js` & `crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-location-input-header.js` & `crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-location-input-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-output.js` & `crosscompute-views-map-0.2.1/crosscompute_views_map/assets/mapbox-output.js`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.2.0/crosscompute_views_map/routines/asset.py` & `crosscompute-views-map-0.2.1/crosscompute_views_map/routines/asset.py`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.2.0/crosscompute_views_map/routines/variable.py` & `crosscompute-views-map-0.2.1/crosscompute_views_map/routines/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         save_map_configuration(array, path)
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
+        c = b.get_data_configuration(variable_definition)
         main_text = get_map_html(
             element_id, variable_id, c, x.mode_name, self.view_name,
             x.design_name)
         js_texts = [
             "mapboxgl.accessToken = '%s';" % environ['MAPBOX_TOKEN'],
             MAP_MAPBOX_HEADER_JS,
             MAP_MAPBOX_OUTPUT_HEADER_JS,
@@ -76,15 +76,15 @@
     css_texts = [MAP_CSS]
     js_uris = [MAPBOX_JS_URI]
 
     def render_input(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         element_id = x.id
         view_name = self.view_name
-        c = b.get_variable_configuration(variable_definition)
+        c = b.get_data_configuration(variable_definition)
         data = b.load_data(variable_definition)
         if 'value' in data:
             v = data['value']
             try:
                 longitude, latitude = v['center']
                 zoom = v['zoom']
             except (KeyError, TypeError):
@@ -123,15 +123,15 @@
         save_map_configuration(array, path)
 
     def render_output(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         variable_id = self.variable_id
         element_id = x.id
         data_uri = b.get_data_uri(variable_definition, x)
-        c = b.get_variable_configuration(variable_definition)
+        c = b.get_data_configuration(variable_definition)
         mapbox_token = environ['MAPBOX_TOKEN']
         main_text = get_map_html(
             element_id, variable_id, c, x.mode_name, self.view_name,
             x.design_name)
         js_texts = [
             f"mapboxgl.accessToken = '{mapbox_token}';",
             MAP_DECK_SCREENGRID_OUTPUT_HEADER_JS,
```

### Comparing `crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/PKG-INFO` & `crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-views-map
-Version: 0.2.0
+Version: 0.2.1
 Summary: Render maps in your automations.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-views-map/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-views-map
```

### Comparing `crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/SOURCES.txt` & `crosscompute-views-map-0.2.1/crosscompute_views_map.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.2.0/setup.cfg` & `crosscompute-views-map-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute-views-map
-version = 0.2.0
+version = 0.2.1
 description = Render maps in your automations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
```

