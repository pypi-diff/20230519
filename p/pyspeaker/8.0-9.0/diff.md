# Comparing `tmp/pyspeaker-8.0.tar.gz` & `tmp/pyspeaker-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspeaker-8.0.tar", last modified: Fri May 19 06:38:20 2023, max compression
+gzip compressed data, was "pyspeaker-9.0.tar", last modified: Fri May 19 06:47:08 2023, max compression
```

## Comparing `pyspeaker-8.0.tar` & `pyspeaker-9.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 06:38:20.685344 pyspeaker-8.0/
--rw-rw-rw-   0        0        0     1091 2023-05-19 06:36:47.000000 pyspeaker-8.0/LICENSE.txt
--rw-rw-rw-   0        0        0      490 2023-05-19 06:38:20.680344 pyspeaker-8.0/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 06:38:20.629749 pyspeaker-8.0/app/
--rw-rw-rw-   0        0        0      926 2023-05-19 06:37:07.000000 pyspeaker-8.0/app/Audio.py
--rw-rw-rw-   0        0        0       26 2023-05-19 06:30:51.000000 pyspeaker-8.0/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:38:20.678281 pyspeaker-8.0/pyspeaker.egg-info/
--rw-rw-rw-   0        0        0      490 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 06:38:20.685344 pyspeaker-8.0/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-05-19 06:37:50.000000 pyspeaker-8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:47:08.639024 pyspeaker-9.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-19 06:36:47.000000 pyspeaker-9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      490 2023-05-19 06:47:08.637980 pyspeaker-9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-9.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 06:47:08.639024 pyspeaker-9.0/setup.cfg
+-rw-rw-rw-   0        0        0      780 2023-05-19 06:46:38.000000 pyspeaker-9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:47:08.600378 pyspeaker-9.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 06:47:08.610581 pyspeaker-9.0/src/pyspeaker/
+-rw-rw-rw-   0        0        0      926 2023-05-19 06:37:07.000000 pyspeaker-9.0/src/pyspeaker/Audio.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 06:44:22.000000 pyspeaker-9.0/src/pyspeaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:47:08.634717 pyspeaker-9.0/src/pyspeaker.egg-info/
+-rw-rw-rw-   0        0        0      490 2023-05-19 06:47:08.000000 pyspeaker-9.0/src/pyspeaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-19 06:47:08.000000 pyspeaker-9.0/src/pyspeaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 06:47:08.000000 pyspeaker-9.0/src/pyspeaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-19 06:47:08.000000 pyspeaker-9.0/src/pyspeaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 06:47:08.000000 pyspeaker-9.0/src/pyspeaker.egg-info/top_level.txt
```

### Comparing `pyspeaker-8.0/LICENSE.txt` & `pyspeaker-9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyspeaker-8.0/app/Audio.py` & `pyspeaker-9.0/src/pyspeaker/Audio.py`

 * *Files identical despite different names*

### Comparing `pyspeaker-8.0/setup.py` & `pyspeaker-9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import find_packages, setup
 
 if __name__ == "__main__":
     setup(
     name = "pyspeaker",
     author = "Akshat Sabharwal",
-    version = "8.0",
-    package=['app'],
+    version = "9.0",
+    package_dir={"":"src"},
+    package=['pyspeaker'],
     author_email = "akshatsabharwal35@gmail.com",
     description="A module for controlling the Speakers of the device",
     long_description = """
     \bMethods\b
 
     get_volume: Returns the current volume of the device's speakers
     set_volume: Sets the volume of the device's speakers to the given volume level.
```

