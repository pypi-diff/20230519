# Comparing `tmp/getmonitorresolution-0.12.tar.gz` & `tmp/getmonitorresolution-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getmonitorresolution-0.12.tar", last modified: Wed May 10 04:09:44 2023, max compression
+gzip compressed data, was "getmonitorresolution-0.13.tar", last modified: Fri May 19 10:26:43 2023, max compression
```

## Comparing `getmonitorresolution-0.12.tar` & `getmonitorresolution-0.13.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 04:09:44.097670 getmonitorresolution-0.12/
--rw-rw-rw-   0        0        0     1148 2023-05-10 04:09:40.000000 getmonitorresolution-0.12/LICENSE.rst
--rw-rw-rw-   0        0        0      131 2023-05-10 04:09:40.000000 getmonitorresolution-0.12/MANIFEST.in
--rw-rw-rw-   0        0        0     3437 2023-05-10 04:09:44.097670 getmonitorresolution-0.12/PKG-INFO
--rw-rw-rw-   0        0        0     2764 2023-05-08 02:50:48.000000 getmonitorresolution-0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 04:09:44.093680 getmonitorresolution-0.12/getmonitorresolution/
--rw-rw-rw-   0        0        0     2764 2023-05-08 02:50:48.000000 getmonitorresolution-0.12/getmonitorresolution/README.md
--rw-rw-rw-   0        0        0     2775 2023-05-10 04:08:54.000000 getmonitorresolution-0.12/getmonitorresolution/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-10 04:09:43.000000 getmonitorresolution-0.12/getmonitorresolution/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-05-10 04:09:43.000000 getmonitorresolution-0.12/getmonitorresolution/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-10 04:09:44.096673 getmonitorresolution-0.12/getmonitorresolution.egg-info/
--rw-rw-rw-   0        0        0     3437 2023-05-10 04:09:43.000000 getmonitorresolution-0.12/getmonitorresolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-05-10 04:09:44.000000 getmonitorresolution-0.12/getmonitorresolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 04:09:43.000000 getmonitorresolution-0.12/getmonitorresolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-10 04:09:43.000000 getmonitorresolution-0.12/getmonitorresolution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-10 04:09:44.097670 getmonitorresolution-0.12/setup.cfg
--rw-rw-rw-   0        0        0     1330 2023-05-10 04:09:43.000000 getmonitorresolution-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 10:26:43.464814 getmonitorresolution-0.13/
+-rw-rw-rw-   0        0        0     1148 2023-05-19 10:26:36.000000 getmonitorresolution-0.13/LICENSE.rst
+-rw-rw-rw-   0        0        0      131 2023-05-19 10:26:34.000000 getmonitorresolution-0.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     4383 2023-05-19 10:26:43.464814 getmonitorresolution-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     3710 2023-05-19 10:25:36.000000 getmonitorresolution-0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 10:26:43.460825 getmonitorresolution-0.13/getmonitorresolution/
+-rw-rw-rw-   0        0        0     3710 2023-05-19 10:25:36.000000 getmonitorresolution-0.13/getmonitorresolution/README.md
+-rw-rw-rw-   0        0        0     5286 2023-05-19 10:23:38.000000 getmonitorresolution-0.13/getmonitorresolution/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-19 10:26:42.000000 getmonitorresolution-0.13/getmonitorresolution/requirements.txt
+-rw-rw-rw-   0        0        0     1277 2023-05-19 10:26:42.000000 getmonitorresolution-0.13/getmonitorresolution/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-19 10:26:43.463817 getmonitorresolution-0.13/getmonitorresolution.egg-info/
+-rw-rw-rw-   0        0        0     4383 2023-05-19 10:26:43.000000 getmonitorresolution-0.13/getmonitorresolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-05-19 10:26:43.000000 getmonitorresolution-0.13/getmonitorresolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 10:26:43.000000 getmonitorresolution-0.13/getmonitorresolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-19 10:26:43.000000 getmonitorresolution-0.13/getmonitorresolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-19 10:26:43.000000 getmonitorresolution-0.13/getmonitorresolution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-19 10:26:43.464814 getmonitorresolution-0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1412 2023-05-19 10:26:42.000000 getmonitorresolution-0.13/setup.py
```

### Comparing `getmonitorresolution-0.12/LICENSE.rst` & `getmonitorresolution-0.13/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `getmonitorresolution-0.12/PKG-INFO` & `getmonitorresolution-0.13/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1
-Name: getmonitorresolution
-Version: 0.12
-Summary: Uses ctypes to get the resolution information of all available monitors
-Home-page: https://github.com/hansalemaos/getmonitorresolution
-Author: Johannes Fischer
-Author-email: aulasparticularesdealemaosp@gmail.com
-License: MIT
-Keywords: ctypes,monitor,resolution
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-# Uses ctypes to get the resolution information of all available monitors
+# Uses ctypes to get the resolution and other useful information of all available monitors
 
 ## pip install getmonitorresolution
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 
 ```python
 The get_monitors_resolution() function retrieves the resolution information of all available monitors on a Windows machine. It takes an optional parameter dpi_awareness, which sets the DPI awareness level. The function returns a tuple containing two dictionaries, allmoni and moninfos.
@@ -58,11 +41,43 @@
 
 from getmonitorresolution import get_monitors_resolution
 eachmonitor,general = get_monitors_resolution()
 print(eachmonitor)
 print(general)
 
 # output 
-{0: {'width': 1920, 'height': 1080}, 1: {'width': 1920, 'height': 1080}}
-{'width_all_monitors': 3840, 'height_all_monitors': 1920, 'max_monitor_width': 1920, 'min_monitor_width': 1920, 'max_monitor_height': 1080, 'min_monitor_height': 1080}
+eachmonitor,general = get_monitors_resolution()
+from pprint import pprint
+pprint(eachmonitor)
+{0: {'DeviceID': 'PCI\\VEN_10DE&DEV_1F06&Sxxxxxxxxxxxxxxxxx&REV_A1',
+     'DeviceKey': '\\Registry\\Machine\\System\\CurrentControlSet\\Control\\Video\\{xxxxxxxxxxxxxx}\\0000',
+     'DeviceName': '\\\\.\\DISPLAY1',
+     'DeviceString': 'NVIDIA GeForce RTX 2060 SUPER',
+     'StateFlags': 5,
+     'height': 1080,
+     'height_mm': 299,
+     'is_primary': True,
+     'width': 1920,
+     'width_mm': 531,
+     'x': 0,
+     'y': 0},
+ 1: {'DeviceID': 'PCI\\VEN_10DE&xxxxxxxx&xxxxxxxxxxxxx&REV_A1',
+     'DeviceKey': '\\Registry\\Machine\\System\\CurrentControlSet\\Control\\Video\\{xxxxxxxxxxxx}\\0001',
+     'DeviceName': '\\\\.\\DISPLAY2',
+     'DeviceString': 'NVIDIA GeForce RTX 2060 SUPER',
+     'StateFlags': 1,
+     'height': 1080,
+     'height_mm': 299,
+     'is_primary': False,
+     'width': 1920,
+     'width_mm': 531,
+     'x': 1920,
+     'y': 0}}
+pprint(general)
+{'height_all_monitors': 2160,
+ 'max_monitor_height': 1080,
+ 'max_monitor_width': 1920,
+ 'min_monitor_height': 1080,
+ 'min_monitor_width': 1920,
+ 'width_all_monitors': 3840}
 
-```
+```
```

### Comparing `getmonitorresolution-0.12/getmonitorresolution.egg-info/PKG-INFO` & `getmonitorresolution-0.13/getmonitorresolution/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1
-Name: getmonitorresolution
-Version: 0.12
-Summary: Uses ctypes to get the resolution information of all available monitors
-Home-page: https://github.com/hansalemaos/getmonitorresolution
-Author: Johannes Fischer
-Author-email: aulasparticularesdealemaosp@gmail.com
-License: MIT
-Keywords: ctypes,monitor,resolution
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-# Uses ctypes to get the resolution information of all available monitors
+# Uses ctypes to get the resolution and other useful information of all available monitors
 
 ## pip install getmonitorresolution
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 
 ```python
 The get_monitors_resolution() function retrieves the resolution information of all available monitors on a Windows machine. It takes an optional parameter dpi_awareness, which sets the DPI awareness level. The function returns a tuple containing two dictionaries, allmoni and moninfos.
@@ -58,11 +41,43 @@
 
 from getmonitorresolution import get_monitors_resolution
 eachmonitor,general = get_monitors_resolution()
 print(eachmonitor)
 print(general)
 
 # output 
-{0: {'width': 1920, 'height': 1080}, 1: {'width': 1920, 'height': 1080}}
-{'width_all_monitors': 3840, 'height_all_monitors': 1920, 'max_monitor_width': 1920, 'min_monitor_width': 1920, 'max_monitor_height': 1080, 'min_monitor_height': 1080}
+eachmonitor,general = get_monitors_resolution()
+from pprint import pprint
+pprint(eachmonitor)
+{0: {'DeviceID': 'PCI\\VEN_10DE&DEV_1F06&Sxxxxxxxxxxxxxxxxx&REV_A1',
+     'DeviceKey': '\\Registry\\Machine\\System\\CurrentControlSet\\Control\\Video\\{xxxxxxxxxxxxxx}\\0000',
+     'DeviceName': '\\\\.\\DISPLAY1',
+     'DeviceString': 'NVIDIA GeForce RTX 2060 SUPER',
+     'StateFlags': 5,
+     'height': 1080,
+     'height_mm': 299,
+     'is_primary': True,
+     'width': 1920,
+     'width_mm': 531,
+     'x': 0,
+     'y': 0},
+ 1: {'DeviceID': 'PCI\\VEN_10DE&xxxxxxxx&xxxxxxxxxxxxx&REV_A1',
+     'DeviceKey': '\\Registry\\Machine\\System\\CurrentControlSet\\Control\\Video\\{xxxxxxxxxxxx}\\0001',
+     'DeviceName': '\\\\.\\DISPLAY2',
+     'DeviceString': 'NVIDIA GeForce RTX 2060 SUPER',
+     'StateFlags': 1,
+     'height': 1080,
+     'height_mm': 299,
+     'is_primary': False,
+     'width': 1920,
+     'width_mm': 531,
+     'x': 1920,
+     'y': 0}}
+pprint(general)
+{'height_all_monitors': 2160,
+ 'max_monitor_height': 1080,
+ 'max_monitor_width': 1920,
+ 'min_monitor_height': 1080,
+ 'min_monitor_width': 1920,
+ 'width_all_monitors': 3840}
 
-```
+```
```

### Comparing `getmonitorresolution-0.12/setup.py` & `getmonitorresolution-0.13/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.12'''
+VERSION = '''0.13'''
 DESCRIPTION = '''Uses ctypes to get the resolution information of all available monitors'''
 
 # Setting up
 setup(
     name="getmonitorresolution",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/getmonitorresolution',
     author="Johannes Fischer",
     author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
 long_description = long_description,
 long_description_content_type="text/markdown",
-    #packages=[],
+    #packages=['flatten_any_dict_iterable_or_whatsoever'],
     keywords=['ctypes', 'monitor', 'resolution'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
-    install_requires=[],
+    install_requires=['flatten_any_dict_iterable_or_whatsoever'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

