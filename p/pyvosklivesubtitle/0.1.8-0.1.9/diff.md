# Comparing `tmp/pyvosklivesubtitle-0.1.8.tar.gz` & `tmp/pyvosklivesubtitle-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyvosklivesubtitle-0.1.8.tar", last modified: Thu May 18 21:12:25 2023, max compression
+gzip compressed data, was "dist\pyvosklivesubtitle-0.1.9.tar", last modified: Thu May 18 22:26:02 2023, max compression
```

## Comparing `pyvosklivesubtitle-0.1.8.tar` & `pyvosklivesubtitle-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 21:12:25.667247 pyvosklivesubtitle-0.1.8/
--rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1490 2023-05-18 21:12:25.667996 pyvosklivesubtitle-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 21:12:25.600262 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle/
--rw-rw-rw-   0        0        0   146376 2023-05-18 21:10:21.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:12:25.665748 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/
--rw-rw-rw-   0        0        0     1490 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-18 21:12:25.000000 pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-05-18 21:12:25.676991 pyvosklivesubtitle-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1743 2023-05-18 21:12:20.000000 pyvosklivesubtitle-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:26:02.150182 pyvosklivesubtitle-0.1.9/
+-rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1490 2023-05-18 22:26:02.150932 pyvosklivesubtitle-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6636 2023-04-24 13:05:36.000000 pyvosklivesubtitle-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 22:26:02.117964 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle/
+-rw-rw-rw-   0        0        0   146397 2023-05-18 22:12:27.000000 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:26:02.147187 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle.egg-info/
+-rw-rw-rw-   0        0        0     1490 2023-05-18 22:26:01.000000 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-18 22:26:02.000000 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 22:26:01.000000 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-18 22:26:01.000000 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-05-18 22:26:01.000000 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-18 22:26:01.000000 pyvosklivesubtitle-0.1.9/pyvosklivesubtitle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-05-18 22:26:02.154681 pyvosklivesubtitle-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2132 2023-05-18 22:20:30.000000 pyvosklivesubtitle-0.1.9/setup.py
```

### Comparing `pyvosklivesubtitle-0.1.8/LICENSE` & `pyvosklivesubtitle-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.8/PKG-INFO` & `pyvosklivesubtitle-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pyvosklivesubtitle
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
 
 Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.8/README.md` & `pyvosklivesubtitle-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.8/pyvosklivesubtitle/__init__.py` & `pyvosklivesubtitle-0.1.9/pyvosklivesubtitle/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,14 +322,15 @@
     if sys.platform == 'win32':
         libvosk = "libvosk.dll"
     elif sys.platform == 'linux':
         libvosk = "libvosk.so"
     elif sys.platform == 'darwin':
         libvosk = "libvosk.dyld"
     dlldir = os.path.abspath(os.path.dirname(__file__))
+    print(__file__)
     os.environ["PATH"] = dlldir + os.pathsep + os.environ['PATH']
     for path in os.environ["PATH"].split(os.pathsep):
         path = path.strip('"')
         if os.path.isfile(os.path.join(path, libvosk)):
             return path
     raise TypeError('libvosk not found')
     
@@ -557,15 +558,15 @@
     def GetPendingChunks(self):
         return _c.vosk_batch_recognizer_get_pending_chunks(self._handle)
 
 #=======================================================================================================================================#
 
 #============================================================== APP PARTS ==============================================================#
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 arraylist_models = []
 arraylist_models.append("ca-es");
 arraylist_models.append("zh-cn")
 arraylist_models.append("cs-cz");
 arraylist_models.append("nl-nl");
 arraylist_models.append("en-us")
```

### Comparing `pyvosklivesubtitle-0.1.8/pyvosklivesubtitle.egg-info/PKG-INFO` & `pyvosklivesubtitle-0.1.9/pyvosklivesubtitle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pyvosklivesubtitle
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
 
 Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.8/setup.py` & `pyvosklivesubtitle-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #!/usr/bin/env python3.8
 from __future__ import unicode_literals
 import sys
 import platform
 import os
+import ctypes
 import stat
 from pyvosklivesubtitle import VERSION
 
-#from setuptools import setup
-#from setuptools.command.install import install
-#from distutils import log
-
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-
+current_platform = platform.system()
 
 if sys.version_info < (2, 6):
     print("THIS MODULE REQUIRES PYTHON 2.6, 2.7, OR 3.3+. YOU ARE CURRENTLY USING PYTHON {0}".format(sys.version))
     sys.exit(1)
 
 
 long_description = (
@@ -38,19 +35,31 @@
     "requests>=2.27.1",
     "tqdm>=4.64.0",
 ]
 
 if platform.system == "Windows":
     install_requires.append("pywin32>=306")
 
+if current_platform == 'Linux':
+    lib_files = ['libvosk.so']
+elif current_platform == 'Darwin':
+    lib_files = ['libvosk.dyld']
+elif current_platform == 'Windows':
+    lib_files = ['libgcc_s_seh-1.dll', 'libstdc++-6.dll', 'libvosk.dll', 'libwinpthread-1.dll']
+else:
+    raise NotImplementedError(f"Platform '{current_platform}' is not supported.")
+
+package_data = {'': lib_files} if lib_files else {}
+
 setup(
     name="pyvosklivesubtitle",
     description="A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES",
     version=VERSION,
     include_package_data=True,
+    package_data=package_data,
     author='Bot Bahlul',
     author_email='bot.bahlul@gmail.com',
     url='https://github.com/botbahlul/pyvosklivesubtitle',
     packages=[str('pyvosklivesubtitle')],
     entry_points={
         'console_scripts': [
             'pyvosklivesubtitle = pyvosklivesubtitle:main',
```

