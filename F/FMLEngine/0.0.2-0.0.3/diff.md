# Comparing `tmp/FMLEngine-0.0.2.tar.gz` & `tmp/FMLEngine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FMLEngine-0.0.2.tar", last modified: Thu May 18 00:59:16 2023, max compression
+gzip compressed data, was "FMLEngine-0.0.3.tar", last modified: Thu May 18 18:33:59 2023, max compression
```

## Comparing `FMLEngine-0.0.2.tar` & `FMLEngine-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 00:59:15.990377 FMLEngine-0.0.2/
--rw-rw-rw-   0        0        0       94 2023-05-18 00:43:11.000000 FMLEngine-0.0.2/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 00:59:15.821477 FMLEngine-0.0.2/FML/
--rw-rw-rw-   0        0        0       62 2023-05-18 00:49:21.000000 FMLEngine-0.0.2/FML/Start.py
--rw-rw-rw-   0        0        0       46 2023-05-18 00:48:10.000000 FMLEngine-0.0.2/FML/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 00:59:15.953401 FMLEngine-0.0.2/FMLEngine.egg-info/
--rw-rw-rw-   0        0        0      731 2023-05-18 00:59:15.000000 FMLEngine-0.0.2/FMLEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-18 00:59:15.000000 FMLEngine-0.0.2/FMLEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 00:59:15.000000 FMLEngine-0.0.2/FMLEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-18 00:59:15.000000 FMLEngine-0.0.2/FMLEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-05-17 23:00:24.000000 FMLEngine-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-17 22:55:59.000000 FMLEngine-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      731 2023-05-18 00:59:15.985381 FMLEngine-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-05-18 00:41:33.000000 FMLEngine-0.0.2/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 00:59:15.991377 FMLEngine-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      705 2023-05-18 00:59:11.000000 FMLEngine-0.0.2/setup.py
--rw-rw-rw-   0        0        0      135 2023-05-18 00:42:58.000000 FMLEngine-0.0.2/setup.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 00:59:15.980384 FMLEngine-0.0.2/test/
--rw-rw-rw-   0        0        0       12 2023-05-18 00:58:37.000000 FMLEngine-0.0.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:33:59.039159 FMLEngine-0.0.3/
+-rw-rw-rw-   0        0        0      247 2023-05-18 18:33:30.000000 FMLEngine-0.0.3/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 18:33:58.908861 FMLEngine-0.0.3/FML/
+-rw-rw-rw-   0        0        0       46 2023-05-18 17:13:51.000000 FMLEngine-0.0.3/FML/Graphics.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:33:58.994290 FMLEngine-0.0.3/FML/Workspace/
+-rw-rw-rw-   0        0        0      772 2023-05-18 17:05:04.000000 FMLEngine-0.0.3/FML/Workspace/Window.py
+-rw-rw-rw-   0        0        0       98 2023-05-18 17:11:09.000000 FMLEngine-0.0.3/FML/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:33:58.961275 FMLEngine-0.0.3/FMLEngine.egg-info/
+-rw-rw-rw-   0        0        0     1330 2023-05-18 18:33:58.000000 FMLEngine-0.0.3/FMLEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-18 18:33:58.000000 FMLEngine-0.0.3/FMLEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:33:58.000000 FMLEngine-0.0.3/FMLEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 18:33:58.000000 FMLEngine-0.0.3/FMLEngine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-18 18:33:58.000000 FMLEngine-0.0.3/FMLEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      213 2023-05-18 18:27:23.000000 FMLEngine-0.0.3/INFO.txt
+-rw-rw-rw-   0        0        0     1069 2023-05-17 23:00:24.000000 FMLEngine-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-17 22:55:59.000000 FMLEngine-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1330 2023-05-18 18:33:59.037155 FMLEngine-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-05-18 18:33:18.000000 FMLEngine-0.0.3/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 18:33:59.039159 FMLEngine-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      711 2023-05-18 18:33:41.000000 FMLEngine-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:33:59.032426 FMLEngine-0.0.3/test/
+-rw-rw-rw-   0        0        0        0 2023-05-18 18:11:09.000000 FMLEngine-0.0.3/test/test.py
```

### Comparing `FMLEngine-0.0.2/FMLEngine.egg-info/PKG-INFO` & `FMLEngine-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-Metadata-Version: 2.1
-Name: FMLEngine
-Version: 0.0.2
-Summary: Pre-Apha Graphics Engine
-Home-page: UNKNOWN
-Author: Josh
-Author-email: kingcode102@gmail.com
-License: MIT
-Keywords: Graphics Engine
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-License-File: LICENSE.txt
-
-FML is a Graphics Library like Sdl2 or Sfml but for Python FML is currently in Pre-Apha their will be bugs 
-
-Change Log
-===========
-
-0.0.1 (5/17/2023)
-------------------
--- First Release aka Testing
-
+from setuptools import setup, find_packages
+ 
+classifiers = [
+    'Development Status :: 5 - Production/Stable',
+    'Intended Audience :: Developers',
+    'Operating System :: Microsoft :: Windows :: Windows 10',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3'
+] 
+ 
+setup(
+  name='FMLEngine',
+  version='0.0.3',
+  description='Pre-Apha Graphics Engine',
+  long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
+  url='',  
+  author='Josh',
+  author_email='kingcode102@gmail.com',
+  license='MIT', 
+  classifiers=classifiers,
+  keywords='Graphics Engine', 
+  packages=find_packages(),
+  install_requires=['PySDL2'],
+)
```

### Comparing `FMLEngine-0.0.2/LICENSE.txt` & `FMLEngine-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

