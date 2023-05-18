# Comparing `tmp/ni_measurementlink_generator-1.1.0.dev0.tar.gz` & `tmp/ni_measurementlink_generator-1.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_generator-1.1.0.dev0.tar", max compression
+gzip compressed data, was "ni_measurementlink_generator-1.1.0.dev1.tar", max compression
```

## Comparing `ni_measurementlink_generator-1.1.0.dev0.tar` & `ni_measurementlink_generator-1.1.0.dev1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      593 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/README.md
--rw-r--r--   0        0        0      148 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/__main__.py
--rw-r--r--   0        0        0        0 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/py.typed
--rw-r--r--   0        0        0     5599 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/template.py
--rw-r--r--   0        0        0     1690 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.measproj.mako
--rw-r--r--   0        0        0     5143 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.measui.mako
--rw-r--r--   0        0        0     1472 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.py.mako
--rw-r--r--   0        0        0      341 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
--rw-r--r--   0        0        0      241 2023-05-08 22:25:40.068291 ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/start.bat.mako
--rw-r--r--   0        0        0     1602 2023-05-08 22:27:14.811198 ni_measurementlink_generator-1.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev0/setup.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      593 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/README.md
+-rw-r--r--   0        0        0      148 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/py.typed
+-rw-r--r--   0        0        0     5599 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/template.py
+-rw-r--r--   0        0        0     1690 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.measproj.mako
+-rw-r--r--   0        0        0     5143 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.measui.mako
+-rw-r--r--   0        0        0     1472 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.py.mako
+-rw-r--r--   0        0        0      341 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
+-rw-r--r--   0        0        0      241 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/start.bat.mako
+-rw-r--r--   0        0        0     1602 2023-05-18 21:57:24.107064 ni_measurementlink_generator-1.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev1/setup.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev1/PKG-INFO
```

### Comparing `ni_measurementlink_generator-1.1.0.dev0/README.md` & `ni_measurementlink_generator-1.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/template.py` & `ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/template.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.measproj.mako` & `ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.measproj.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.measui.mako` & `ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.measui.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev0/ni_measurementlink_generator/templates/measurement.py.mako` & `ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.py.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev0/pyproject.toml` & `ni_measurementlink_generator-1.1.0.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ni_measurementlink_generator"
-version = "1.1.0-dev0"
+version = "1.1.0-dev1"
 description = "MeasurementLink Code Generator for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md"
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `ni_measurementlink_generator-1.1.0.dev0/setup.py` & `ni_measurementlink_generator-1.1.0.dev1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 entry_points = \
 {'console_scripts': ['ni-measurementlink-generator = '
                      'ni_measurementlink_generator.template:create_measurement']}
 
 setup_kwargs = {
     'name': 'ni-measurementlink-generator',
-    'version': '1.1.0.dev0',
+    'version': '1.1.0.dev1',
     'description': 'MeasurementLink Code Generator for Python',
     'long_description': '# MeasurementLink™ Code Generator for Python\n\n---\n\n## Introduction\n\nMeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a tool for generating measurement plugins.\n\nFor installation and usage, see [MeasurementLink Support for Python (`ni-measurementlink-service`)](https://pypi.org/project/ni-measurementlink-service/).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [mako >= 1.2.1, < 2.x](https://pypi.org/project/Mako/1.2.1/)\n- [click >= 8.1.3, < 9.x](https://pypi.org/project/click/8.1.3/)\n\n---',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/measurementlink-python/',
```

### Comparing `ni_measurementlink_generator-1.1.0.dev0/PKG-INFO` & `ni_measurementlink_generator-1.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ni-measurementlink-generator
-Version: 1.1.0.dev0
+Version: 1.1.0.dev1
 Summary: MeasurementLink Code Generator for Python
 Home-page: https://github.com/ni/measurementlink-python/
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

