# Comparing `tmp/videoslides-0.0.4.tar.gz` & `tmp/videoslides-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\videoslides-0.0.4.tar", last modified: Fri May 19 04:01:34 2023, max compression
+gzip compressed data, was "dist\videoslides-0.0.5.tar", last modified: Fri May 19 16:30:38 2023, max compression
```

## Comparing `videoslides-0.0.4.tar` & `videoslides-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 04:01:34.000000 videoslides-0.0.4/
--rw-rw-rw-   0        0        0     6063 2022-07-20 03:36:12.000000 videoslides-0.0.4/esquema.drawio
--rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1398 2023-05-19 04:01:34.000000 videoslides-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 04:01:34.000000 videoslides-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2021 2023-05-19 03:20:48.000000 videoslides-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 04:01:34.000000 videoslides-0.0.4/src/
--rw-rw-rw-   0        0        0    45516 2023-05-11 02:57:14.000000 videoslides-0.0.4/src/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-19 04:01:34.000000 videoslides-0.0.4/src/videoslides.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-19 04:01:33.000000 videoslides-0.0.4/src/videoslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1398 2023-05-19 04:01:33.000000 videoslides-0.0.4/src/videoslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-05-19 04:01:33.000000 videoslides-0.0.4/src/videoslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2023-05-19 04:01:33.000000 videoslides-0.0.4/src/videoslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2023-05-19 04:01:33.000000 videoslides-0.0.4/src/videoslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13048 2023-05-11 03:10:08.000000 videoslides-0.0.4/src/videoslides.py
--rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:30:38.000000 videoslides-0.0.5/
+-rw-rw-rw-   0        0        0     6063 2022-07-20 03:36:12.000000 videoslides-0.0.5/esquema.drawio
+-rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1398 2023-05-19 16:30:38.000000 videoslides-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 16:30:38.000000 videoslides-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2049 2023-05-19 16:26:07.000000 videoslides-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/
+-rw-rw-rw-   0        0        0    45516 2023-05-11 02:57:14.000000 videoslides-0.0.5/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1398 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13048 2023-05-11 03:10:08.000000 videoslides-0.0.5/src/videoslides.py
+-rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.5/src/__init__.py
```

### Comparing `videoslides-0.0.4/esquema.drawio` & `videoslides-0.0.5/esquema.drawio`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.4/LICENSE.txt` & `videoslides-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.4/PKG-INFO` & `videoslides-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.4/README.md` & `videoslides-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.4/setup.py` & `videoslides-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="videoslides",
-    version='0.0.4',
+    version='0.0.5',
     description='Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file ',
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["videoslides", "functions"],
     package_dir={'':'src'},
     install_requires=[
         "easyocr >= 1.4.1",
         "stanza >= 1.4.0",
         "numpy >= 1.19.5",
         "matplotlib >= 3.3.4",
         "pytube >= 12.0.0",
         "scikit-image >= 0.17.2",
         "validators >= 0.20.0",
         "nltk >= 3.6.7",
-        "opencv-python-headless >= 4.1.2.30"
+        "opencv-python-headless >= 4.1.2.30",
+        "sewar >= 0.4.5" 
     ],
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent", 
         "Intended Audience :: Developers"
     ],
```

### Comparing `videoslides-0.0.4/src/functions.py` & `videoslides-0.0.5/src/functions.py`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.4/src/videoslides.egg-info/PKG-INFO` & `videoslides-0.0.5/src/videoslides.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.4/src/videoslides.py` & `videoslides-0.0.5/src/videoslides.py`

 * *Files identical despite different names*

