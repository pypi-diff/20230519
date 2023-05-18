# Comparing `tmp/FMLEngine-0.0.4.tar.gz` & `tmp/FMLEngine-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FMLEngine-0.0.4.tar", last modified: Thu May 18 18:44:33 2023, max compression
+gzip compressed data, was "FMLEngine-0.0.5.tar", last modified: Thu May 18 18:49:14 2023, max compression
```

## Comparing `FMLEngine-0.0.4.tar` & `FMLEngine-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 18:44:32.992465 FMLEngine-0.0.4/
--rw-rw-rw-   0        0        0      110 2023-05-18 18:44:13.000000 FMLEngine-0.0.4/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 18:44:32.942495 FMLEngine-0.0.4/FML/
--rw-rw-rw-   0        0        0       46 2023-05-18 17:13:51.000000 FMLEngine-0.0.4/FML/Graphics.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:44:32.984477 FMLEngine-0.0.4/FML/Workspace/
--rw-rw-rw-   0        0        0      772 2023-05-18 17:05:04.000000 FMLEngine-0.0.4/FML/Workspace/Window.py
--rw-rw-rw-   0        0        0      102 2023-05-18 18:44:23.000000 FMLEngine-0.0.4/FML/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:44:32.974476 FMLEngine-0.0.4/FMLEngine.egg-info/
--rw-rw-rw-   0        0        0     1195 2023-05-18 18:44:32.000000 FMLEngine-0.0.4/FMLEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-18 18:44:32.000000 FMLEngine-0.0.4/FMLEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 18:44:32.000000 FMLEngine-0.0.4/FMLEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 18:44:32.000000 FMLEngine-0.0.4/FMLEngine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-18 18:44:32.000000 FMLEngine-0.0.4/FMLEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      213 2023-05-18 18:27:23.000000 FMLEngine-0.0.4/INFO.txt
--rw-rw-rw-   0        0        0     1069 2023-05-17 23:00:24.000000 FMLEngine-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-17 22:55:59.000000 FMLEngine-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1195 2023-05-18 18:44:32.991466 FMLEngine-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-05-18 18:35:08.000000 FMLEngine-0.0.4/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 18:44:32.993466 FMLEngine-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-05-18 18:44:29.000000 FMLEngine-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:44:32.988469 FMLEngine-0.0.4/test/
--rw-rw-rw-   0        0        0      265 2023-05-18 18:42:44.000000 FMLEngine-0.0.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:49:14.806603 FMLEngine-0.0.5/
+-rw-rw-rw-   0        0        0      155 2023-05-18 18:48:16.000000 FMLEngine-0.0.5/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 18:49:14.765628 FMLEngine-0.0.5/FML/
+-rw-rw-rw-   0        0        0       40 2023-05-18 18:46:35.000000 FMLEngine-0.0.5/FML/Graphics.py
+-rw-rw-rw-   0        0        0      772 2023-05-18 17:05:04.000000 FMLEngine-0.0.5/FML/Window.py
+-rw-rw-rw-   0        0        0      102 2023-05-18 18:44:23.000000 FMLEngine-0.0.5/FML/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:49:14.795611 FMLEngine-0.0.5/FMLEngine.egg-info/
+-rw-rw-rw-   0        0        0     1242 2023-05-18 18:49:14.000000 FMLEngine-0.0.5/FMLEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-05-18 18:49:14.000000 FMLEngine-0.0.5/FMLEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:49:14.000000 FMLEngine-0.0.5/FMLEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 18:49:14.000000 FMLEngine-0.0.5/FMLEngine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-18 18:49:14.000000 FMLEngine-0.0.5/FMLEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      213 2023-05-18 18:27:23.000000 FMLEngine-0.0.5/INFO.txt
+-rw-rw-rw-   0        0        0     1069 2023-05-17 23:00:24.000000 FMLEngine-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-17 22:55:59.000000 FMLEngine-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1242 2023-05-18 18:49:14.802612 FMLEngine-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-05-18 18:47:05.000000 FMLEngine-0.0.5/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 18:49:14.808608 FMLEngine-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      711 2023-05-18 18:49:02.000000 FMLEngine-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:49:14.798610 FMLEngine-0.0.5/test/
+-rw-rw-rw-   0        0        0      265 2023-05-18 18:42:44.000000 FMLEngine-0.0.5/test/test.py
```

### Comparing `FMLEngine-0.0.4/FML/Workspace/Window.py` & `FMLEngine-0.0.5/FML/Window.py`

 * *Files identical despite different names*

### Comparing `FMLEngine-0.0.4/FMLEngine.egg-info/PKG-INFO` & `FMLEngine-0.0.5/FMLEngine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FMLEngine
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pre-Apha Graphics Engine
 Home-page: UNKNOWN
 Author: Josh
 Author-email: kingcode102@gmail.com
 License: MIT
 Keywords: Graphics Engine
 Platform: UNKNOWN
@@ -17,22 +17,23 @@
 
 FML is a Graphics Library like Sdl2 or Sfml but for Python FML is currently in Pre-Apha their will be bugs 
 
 if your verison of FML isent the newist verison Run this command in your Terminal ``pip install FMLEngine --upgrade``
 
 to check if your on the newist verson import FML and it will output "FMLEngine Verison [what verison you have]"
 
-to learn more about FML goto the docs link[https://github.com/TheFakeKingIsTaken/FMLDocs/blob/main/Doc.md]
+to learn more about FML goto the docs [link](https://github.com/TheFakeKingIsTaken/FMLDocs/blob/main/Doc.md)
 
 INSTALLATION
 =============
 run ``pip install FMLEngine`` in your Terminal to Install FMLEngine
 
 
 Change Log
 ===========
 
 0.0.3 (5/18/2023)
 ------------------
 
--- Fixed error ``No file named graphics`` 
+-- Fixed error ``No file named Graphics`` 
+-- Fixed error ``No file named Workspace``
```

### Comparing `FMLEngine-0.0.4/LICENSE.txt` & `FMLEngine-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FMLEngine-0.0.4/PKG-INFO` & `FMLEngine-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FMLEngine
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pre-Apha Graphics Engine
 Home-page: UNKNOWN
 Author: Josh
 Author-email: kingcode102@gmail.com
 License: MIT
 Keywords: Graphics Engine
 Platform: UNKNOWN
@@ -17,22 +17,23 @@
 
 FML is a Graphics Library like Sdl2 or Sfml but for Python FML is currently in Pre-Apha their will be bugs 
 
 if your verison of FML isent the newist verison Run this command in your Terminal ``pip install FMLEngine --upgrade``
 
 to check if your on the newist verson import FML and it will output "FMLEngine Verison [what verison you have]"
 
-to learn more about FML goto the docs link[https://github.com/TheFakeKingIsTaken/FMLDocs/blob/main/Doc.md]
+to learn more about FML goto the docs [link](https://github.com/TheFakeKingIsTaken/FMLDocs/blob/main/Doc.md)
 
 INSTALLATION
 =============
 run ``pip install FMLEngine`` in your Terminal to Install FMLEngine
 
 
 Change Log
 ===========
 
 0.0.3 (5/18/2023)
 ------------------
 
--- Fixed error ``No file named graphics`` 
+-- Fixed error ``No file named Graphics`` 
+-- Fixed error ``No file named Workspace``
```

### Comparing `FMLEngine-0.0.4/README.txt` & `FMLEngine-0.0.5/README.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 FML is a Graphics Library like Sdl2 or Sfml but for Python FML is currently in Pre-Apha their will be bugs 
 
 if your verison of FML isent the newist verison Run this command in your Terminal ``pip install FMLEngine --upgrade``
 
 to check if your on the newist verson import FML and it will output "FMLEngine Verison [what verison you have]"
 
-to learn more about FML goto the docs link[https://github.com/TheFakeKingIsTaken/FMLDocs/blob/main/Doc.md]
+to learn more about FML goto the docs [link](https://github.com/TheFakeKingIsTaken/FMLDocs/blob/main/Doc.md)
 
 INSTALLATION
 =============
 run ``pip install FMLEngine`` in your Terminal to Install FMLEngine
```

### Comparing `FMLEngine-0.0.4/setup.py` & `FMLEngine-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ] 
  
 setup(
   name='FMLEngine',
-  version='0.0.4',
+  version='0.0.5',
   description='Pre-Apha Graphics Engine',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Josh',
   author_email='kingcode102@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

