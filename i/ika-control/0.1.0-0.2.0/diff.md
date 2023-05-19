# Comparing `tmp/ika-control-0.1.0.tar.gz` & `tmp/ika-control-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ika-control-0.1.0.tar", last modified: Thu Mar 16 18:05:44 2023, max compression
+gzip compressed data, was "ika-control-0.2.0.tar", last modified: Fri May 19 19:32:25 2023, max compression
```

## Comparing `ika-control-0.1.0.tar` & `ika-control-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-16 18:05:44.477782 ika-control-0.1.0/
--rw-r--r--   0 a.ruddick   (502) staff       (20)    35149 2023-01-23 17:35:20.000000 ika-control-0.1.0/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2266 2023-03-16 18:05:44.477853 ika-control-0.1.0/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1388 2023-03-16 16:45:46.000000 ika-control-0.1.0/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-16 18:05:44.476281 ika-control-0.1.0/ika/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2056 2023-03-16 17:53:43.000000 ika-control-0.1.0/ika/__init__.py
--rwxr-xr-x   0 a.ruddick   (502) staff       (20)    14529 2023-03-16 17:41:01.000000 ika-control-0.1.0/ika/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     6106 2023-03-16 18:04:07.000000 ika-control-0.1.0/ika/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     6204 2023-03-16 16:45:46.000000 ika-control-0.1.0/ika/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-03-16 18:05:44.477636 ika-control-0.1.0/ika_control.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2266 2023-03-16 18:05:44.000000 ika-control-0.1.0/ika_control.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      302 2023-03-16 18:05:44.000000 ika-control-0.1.0/ika_control.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-03-16 18:05:44.000000 ika-control-0.1.0/ika_control.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       41 2023-03-16 18:05:44.000000 ika-control-0.1.0/ika_control.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      123 2023-03-16 18:05:44.000000 ika-control-0.1.0/ika_control.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        4 2023-03-16 18:05:44.000000 ika-control-0.1.0/ika_control.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      279 2023-03-16 18:05:44.478111 ika-control-0.1.0/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1620 2023-03-16 17:50:26.000000 ika-control-0.1.0/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-19 19:32:25.003232 ika-control-0.2.0/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    35149 2023-01-23 17:35:20.000000 ika-control-0.2.0/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2263 2023-05-19 19:32:25.003300 ika-control-0.2.0/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1389 2023-03-16 19:17:53.000000 ika-control-0.2.0/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-19 19:32:25.002083 ika-control-0.2.0/ika/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2232 2023-04-10 23:30:07.000000 ika-control-0.2.0/ika/__init__.py
+-rwxr-xr-x   0 a.ruddick   (502) staff       (20)    22553 2023-04-10 23:28:51.000000 ika-control-0.2.0/ika/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     9814 2023-04-28 19:55:58.000000 ika-control-0.2.0/ika/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     8627 2023-03-24 21:57:08.000000 ika-control-0.2.0/ika/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-19 19:32:25.003094 ika-control-0.2.0/ika_control.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2263 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      302 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       41 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      135 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        4 2023-05-19 19:32:24.000000 ika-control-0.2.0/ika_control.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      216 2023-05-19 19:32:25.003535 ika-control-0.2.0/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1506 2023-05-19 19:32:20.000000 ika-control-0.2.0/setup.py
```

### Comparing `ika-control-0.1.0/LICENSE` & `ika-control-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ika-control-0.1.0/PKG-INFO` & `ika-control-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ika-control
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python driver for IKA instruments.
-Home-page: https://github.com/alexrudd2/ika/
+Home-page: https://github.com/numat/ika/
 Author: Alex Ruddick
 Author-email: a.ruddick@numat-tech.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -73,9 +73,10 @@
 in the system settings.  Otherwise, the device will turn the heater off when the serial
 cable is unplugged.
 
 Acknowledgements
 ================
 
 ©2023 Alexander Ruddick
+
 Uses code from [the Hein group](https://gitlab.com/heingroup/ika), but otherwise no affiliation.
 As of 2023, that project appears to have been abandoned.
```

### Comparing `ika-control-0.1.0/README.md` & `ika-control-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -50,9 +50,10 @@
 in the system settings.  Otherwise, the device will turn the heater off when the serial
 cable is unplugged.
 
 Acknowledgements
 ================
 
 ©2023 Alexander Ruddick
+
 Uses code from [the Hein group](https://gitlab.com/heingroup/ika), but otherwise no affiliation.
 As of 2023, that project appears to have been abandoned.
```

### Comparing `ika-control-0.1.0/ika/__init__.py` & `ika-control-0.2.0/ika/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Python driver for IKA equipment.
 
 Distributed under the GNU General Public License v3
 Copyright (C) 2022 NuMat Technologies
 """
-from ika.driver import Hotplate, OverheadStirrer, Vacuum
+from ika.driver import Hotplate, OverheadStirrer, Shaker, Vacuum
 
 
 def command_line(args=None):
     """Command line tool exposed through package install."""
     import argparse
     import asyncio
     import json
@@ -31,23 +31,28 @@
         async def get():
             async with Hotplate(args.address,
                                 include_surface_control=not args.no_info) as device:
                 d = await device.get()
                 if not args.no_info:
                     d['info'] = await device.get_info()
                 print(json.dumps(d, indent=4))
+    elif args.type == 'shaker':
+        async def get():
+            async with Shaker(args.address) as device:
+                d = await device.get()
+                if not args.no_info:
+                    d['info'] = await device.get_info()
+                print(json.dumps(d, indent=4))
     elif args.type == 'vacuum':
         async def get():
             async with Vacuum(args.address) as device:
                 d = await device.get()
                 if not args.no_info:
                     d['info'] = await device.get_info()
                 print(json.dumps(d, indent=4))
-    elif args.type in ['shaker']:
-        raise NotImplementedError((f"Not implemented yet for device type: {args.type}"))
     else:
         raise ValueError(f"Unsupported device type: {args.type}")
     asyncio.run(get())
 
 
 if __name__ == '__main__':
     command_line()
```

### Comparing `ika-control-0.1.0/ika_control.egg-info/PKG-INFO` & `ika-control-0.2.0/ika_control.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ika-control
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python driver for IKA instruments.
-Home-page: https://github.com/alexrudd2/ika/
+Home-page: https://github.com/numat/ika/
 Author: Alex Ruddick
 Author-email: a.ruddick@numat-tech.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -73,9 +73,10 @@
 in the system settings.  Otherwise, the device will turn the heater off when the serial
 cable is unplugged.
 
 Acknowledgements
 ================
 
 ©2023 Alexander Ruddick
+
 Uses code from [the Hein group](https://gitlab.com/heingroup/ika), but otherwise no affiliation.
 As of 2023, that project appears to have been abandoned.
```

### Comparing `ika-control-0.1.0/setup.py` & `ika-control-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 """Python driver and command line tool for IKA instruments."""
-from sys import version_info
-
 from setuptools import setup
 
-if version_info < (3, 7):
-    raise ImportError("This module requires Python >=3.7.")
-
-with open('README.md', 'r') as in_file:
+with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="ika-control",
-    version="0.1.0",
+    version="0.2.0",
     description="Python driver for IKA instruments.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="https://github.com/alexrudd2/ika/",
+    url="https://github.com/numat/ika/",
     author="Alex Ruddick",
     author_email="a.ruddick@numat-tech.com",
     packages=['ika'],
-    install_requires=[],
+    install_requires=['pyserial'],
     extras_require={
         'test': [
             'pytest>=6,<8',
             'pytest-cov>=4,<5',
             'pytest-asyncio==0.*',
             'pytest-xdist==3.*',
-            'flake8==6.*',
-            'flake8-docstrings==1.*',
-            'mypy==1.0.1',
+            'ruff==0.0.269',
+            'mypy==1.3.0',
+            'types-pyserial==3.5.0.8'
         ],
     },
     entry_points={
         'console_scripts': [('ika = ika:command_line')]
     },
     license='GPLv3',
     classifiers=[
```

