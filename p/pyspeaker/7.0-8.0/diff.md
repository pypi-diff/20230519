# Comparing `tmp/pyspeaker-7.0.tar.gz` & `tmp/pyspeaker-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspeaker-7.0.tar", last modified: Fri May 19 06:31:30 2023, max compression
+gzip compressed data, was "pyspeaker-8.0.tar", last modified: Fri May 19 06:38:20 2023, max compression
```

## Comparing `pyspeaker-7.0.tar` & `pyspeaker-8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 06:31:30.993124 pyspeaker-7.0/
--rw-rw-rw-   0        0        0     1091 2023-02-23 09:47:52.000000 pyspeaker-7.0/LICENSE.txt
--rw-rw-rw-   0        0        0      212 2023-05-19 06:31:30.992124 pyspeaker-7.0/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 06:31:30.975123 pyspeaker-7.0/app/
--rw-rw-rw-   0        0        0      924 2023-05-19 06:30:32.000000 pyspeaker-7.0/app/Audio.py
--rw-rw-rw-   0        0        0       26 2023-05-19 06:30:51.000000 pyspeaker-7.0/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:31:30.990123 pyspeaker-7.0/pyspeaker.egg-info/
--rw-rw-rw-   0        0        0      212 2023-05-19 06:31:30.000000 pyspeaker-7.0/pyspeaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-19 06:31:30.000000 pyspeaker-7.0/pyspeaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 06:31:30.000000 pyspeaker-7.0/pyspeaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-19 06:31:30.000000 pyspeaker-7.0/pyspeaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-19 06:31:30.000000 pyspeaker-7.0/pyspeaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 06:31:30.993124 pyspeaker-7.0/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-05-19 06:30:56.000000 pyspeaker-7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:38:20.685344 pyspeaker-8.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-19 06:36:47.000000 pyspeaker-8.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      490 2023-05-19 06:38:20.680344 pyspeaker-8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-18 11:26:55.000000 pyspeaker-8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 06:38:20.629749 pyspeaker-8.0/app/
+-rw-rw-rw-   0        0        0      926 2023-05-19 06:37:07.000000 pyspeaker-8.0/app/Audio.py
+-rw-rw-rw-   0        0        0       26 2023-05-19 06:30:51.000000 pyspeaker-8.0/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 06:38:20.678281 pyspeaker-8.0/pyspeaker.egg-info/
+-rw-rw-rw-   0        0        0      490 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-19 06:38:20.000000 pyspeaker-8.0/pyspeaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 06:38:20.685344 pyspeaker-8.0/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-05-19 06:37:50.000000 pyspeaker-8.0/setup.py
```

### Comparing `pyspeaker-7.0/LICENSE.txt` & `pyspeaker-8.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 The Python Packaging Authority
+Copyright (c) 2023 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyspeaker-7.0/app/Audio.py` & `pyspeaker-8.0/app/Audio.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         self._interface = self._devices.Activate(
             IAudioEndpointVolume._iid_, CLSCTX_ALL, None
         )
         self._volume = cast(self._interface, POINTER(IAudioEndpointVolume))
 
     def get_volume(self):
         """Returns the volume of the device's speakers"""
-        vol = self._volume.GetMasterVolumeLevel()
-        return vol
+        _vol = self._volume.GetMasterVolumeLevel()
+        return _vol
 
     def set_volume(self, VolumeLevel):
         """Sets volume of the device's speakers to the user specified value"""
         self._volume.SetMasterVolumeLevel(VolumeLevel, None)
 
     def rangify(self, x, from_tuple: tuple, to_tuple: tuple):
         _vol = np.interp(x, from_tuple, to_tuple)
```

### Comparing `pyspeaker-7.0/setup.py` & `pyspeaker-8.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import find_packages, setup
 
 if __name__ == "__main__":
     setup(
     name = "pyspeaker",
     author = "Akshat Sabharwal",
-    version = "7.0",
+    version = "8.0",
     package=['app'],
     author_email = "akshatsabharwal35@gmail.com",
-    description = """A module for controlling the Speakers of the device
+    description="A module for controlling the Speakers of the device",
+    long_description = """
     \bMethods\b
 
     get_volume: Returns the current volume of the device's speakers
     set_volume: Sets the volume of the device's speakers to the given volume level.
     rangify: Interpolates or maps the given volume range of the speakers to the user-specified range.""",
     install_requires = [
         'pycaw',
```

