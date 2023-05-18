# Comparing `tmp/FMLEngine-0.0.1.tar.gz` & `tmp/FMLEngine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FMLEngine-0.0.1.tar", last modified: Thu May 18 00:40:51 2023, max compression
+gzip compressed data, was "FMLEngine-0.0.2.tar", last modified: Thu May 18 00:59:16 2023, max compression
```

## Comparing `FMLEngine-0.0.1.tar` & `FMLEngine-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 00:40:51.899595 FMLEngine-0.0.1/
--rw-rw-rw-   0        0        0       94 2023-05-17 23:44:41.000000 FMLEngine-0.0.1/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 00:40:51.861683 FMLEngine-0.0.1/FML/
--rw-rw-rw-   0        0        0       60 2023-05-17 22:49:34.000000 FMLEngine-0.0.1/FML/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 00:40:51.894598 FMLEngine-0.0.1/FMLEngine.egg-info/
--rw-rw-rw-   0        0        0      731 2023-05-18 00:40:51.000000 FMLEngine-0.0.1/FMLEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-18 00:40:51.000000 FMLEngine-0.0.1/FMLEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 00:40:51.000000 FMLEngine-0.0.1/FMLEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-18 00:40:51.000000 FMLEngine-0.0.1/FMLEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-05-17 23:00:24.000000 FMLEngine-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-17 22:55:59.000000 FMLEngine-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      731 2023-05-18 00:40:51.897596 FMLEngine-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-05-17 22:52:54.000000 FMLEngine-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 00:40:51.900595 FMLEngine-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      705 2023-05-18 00:40:46.000000 FMLEngine-0.0.1/setup.py
--rw-rw-rw-   0        0        0        0 2023-05-18 00:36:51.000000 FMLEngine-0.0.1/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:59:15.990377 FMLEngine-0.0.2/
+-rw-rw-rw-   0        0        0       94 2023-05-18 00:43:11.000000 FMLEngine-0.0.2/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 00:59:15.821477 FMLEngine-0.0.2/FML/
+-rw-rw-rw-   0        0        0       62 2023-05-18 00:49:21.000000 FMLEngine-0.0.2/FML/Start.py
+-rw-rw-rw-   0        0        0       46 2023-05-18 00:48:10.000000 FMLEngine-0.0.2/FML/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:59:15.953401 FMLEngine-0.0.2/FMLEngine.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-05-18 00:59:15.000000 FMLEngine-0.0.2/FMLEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-18 00:59:15.000000 FMLEngine-0.0.2/FMLEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 00:59:15.000000 FMLEngine-0.0.2/FMLEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-18 00:59:15.000000 FMLEngine-0.0.2/FMLEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-05-17 23:00:24.000000 FMLEngine-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-17 22:55:59.000000 FMLEngine-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      731 2023-05-18 00:59:15.985381 FMLEngine-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2023-05-18 00:41:33.000000 FMLEngine-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 00:59:15.991377 FMLEngine-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-05-18 00:59:11.000000 FMLEngine-0.0.2/setup.py
+-rw-rw-rw-   0        0        0      135 2023-05-18 00:42:58.000000 FMLEngine-0.0.2/setup.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 00:59:15.980384 FMLEngine-0.0.2/test/
+-rw-rw-rw-   0        0        0       12 2023-05-18 00:58:37.000000 FMLEngine-0.0.2/test/test.py
```

### Comparing `FMLEngine-0.0.1/LICENSE.txt` & `FMLEngine-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FMLEngine-0.0.1/setup.py` & `FMLEngine-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ] 
  
 setup(
   name='FMLEngine',
-  version='0.0.1',
+  version='0.0.2',
   description='Pre-Apha Graphics Engine',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Josh',
   author_email='kingcode102@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

