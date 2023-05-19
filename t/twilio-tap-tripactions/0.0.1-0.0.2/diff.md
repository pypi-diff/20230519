# Comparing `tmp/twilio-tap-tripactions-0.0.1.tar.gz` & `tmp/twilio-tap-tripactions-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aigupta/custom_singer_taps/twilio-tap-tripactions/dist/tmp1qc0l3y2/twilio-tap-tripactions-0.0.1.tar", last modified: Wed Jul 28 13:20:13 2021, max compression
+gzip compressed data, was "twilio-tap-tripactions-0.0.2.tar", last modified: Fri May 19 09:18:49 2023, max compression
```

## Comparing `twilio-tap-tripactions-0.0.1.tar` & `twilio-tap-tripactions-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/
--rw-r--r--   0 aigupta    (501) staff       (20)    34523 2021-07-28 13:13:30.000000 twilio-tap-tripactions-0.0.1/LICENSE
--rw-r--r--   0 aigupta    (501) staff       (20)       38 2021-07-28 13:12:30.000000 twilio-tap-tripactions-0.0.1/MANIFEST.in
--rw-r--r--   0 aigupta    (501) staff       (20)      303 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/PKG-INFO
--rw-r--r--   0 aigupta    (501) staff       (20)      661 2021-07-28 13:12:30.000000 twilio-tap-tripactions-0.0.1/README.md
--rw-r--r--   0 aigupta    (501) staff       (20)       79 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/setup.cfg
--rwxr-xr-x   0 aigupta    (501) staff       (20)      582 2021-07-28 13:12:30.000000 twilio-tap-tripactions-0.0.1/setup.py
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/tap_tripactions/
--rw-r--r--   0 aigupta    (501) staff       (20)     1803 2021-07-28 13:12:30.000000 twilio-tap-tripactions-0.0.1/tap_tripactions/__init__.py
--rw-r--r--   0 aigupta    (501) staff       (20)     1001 2021-07-28 13:12:30.000000 twilio-tap-tripactions-0.0.1/tap_tripactions/client.py
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/tap_tripactions/schemas/
--rw-r--r--   0 aigupta    (501) staff       (20)    11453 2021-07-28 13:12:30.000000 twilio-tap-tripactions-0.0.1/tap_tripactions/schemas/bookings.json
--rw-r--r--   0 aigupta    (501) staff       (20)     5007 2021-07-28 13:12:30.000000 twilio-tap-tripactions-0.0.1/tap_tripactions/streams.py
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/test/
--rw-r--r--   0 aigupta    (501) staff       (20)     1487 2021-07-28 13:14:30.000000 twilio-tap-tripactions-0.0.1/test/test_client.py
--rw-r--r--   0 aigupta    (501) staff       (20)     1127 2021-07-28 13:12:31.000000 twilio-tap-tripactions-0.0.1/test/test_sync.py
-drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/twilio_tap_tripactions.egg-info/
--rw-r--r--   0 aigupta    (501) staff       (20)      303 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/twilio_tap_tripactions.egg-info/PKG-INFO
--rw-r--r--   0 aigupta    (501) staff       (20)      483 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/twilio_tap_tripactions.egg-info/SOURCES.txt
--rw-r--r--   0 aigupta    (501) staff       (20)        1 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/twilio_tap_tripactions.egg-info/dependency_links.txt
--rw-r--r--   0 aigupta    (501) staff       (20)       68 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/twilio_tap_tripactions.egg-info/entry_points.txt
--rw-r--r--   0 aigupta    (501) staff       (20)       23 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/twilio_tap_tripactions.egg-info/requires.txt
--rw-r--r--   0 aigupta    (501) staff       (20)       16 2021-07-28 13:20:13.000000 twilio-tap-tripactions-0.0.1/twilio_tap_tripactions.egg-info/top_level.txt
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2023-05-19 09:18:49.473739 twilio-tap-tripactions-0.0.2/
+-rw-r--r--   0 aigupta    (501) staff       (20)    34523 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/LICENSE
+-rw-r--r--   0 aigupta    (501) staff       (20)       38 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/MANIFEST.in
+-rw-r--r--   0 aigupta    (501) staff       (20)      258 2023-05-19 09:18:49.473846 twilio-tap-tripactions-0.0.2/PKG-INFO
+-rw-r--r--   0 aigupta    (501) staff       (20)      661 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/README.md
+-rw-r--r--   0 aigupta    (501) staff       (20)       79 2023-05-19 09:18:49.474361 twilio-tap-tripactions-0.0.2/setup.cfg
+-rwxr-xr-x   0 aigupta    (501) staff       (20)      590 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/setup.py
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2023-05-19 09:18:49.468716 twilio-tap-tripactions-0.0.2/tap_tripactions/
+-rw-r--r--   0 aigupta    (501) staff       (20)     1803 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/tap_tripactions/__init__.py
+-rw-r--r--   0 aigupta    (501) staff       (20)     1001 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/tap_tripactions/client.py
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2023-05-19 09:18:49.469263 twilio-tap-tripactions-0.0.2/tap_tripactions/schemas/
+-rw-r--r--   0 aigupta    (501) staff       (20)    11453 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/tap_tripactions/schemas/bookings.json
+-rw-r--r--   0 aigupta    (501) staff       (20)     5007 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/tap_tripactions/streams.py
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2023-05-19 09:18:49.470567 twilio-tap-tripactions-0.0.2/test/
+-rw-r--r--   0 aigupta    (501) staff       (20)     1487 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/test/test_client.py
+-rw-r--r--   0 aigupta    (501) staff       (20)     1127 2023-05-19 09:18:04.000000 twilio-tap-tripactions-0.0.2/test/test_sync.py
+drwxr-xr-x   0 aigupta    (501) staff       (20)        0 2023-05-19 09:18:49.473368 twilio-tap-tripactions-0.0.2/twilio_tap_tripactions.egg-info/
+-rw-r--r--   0 aigupta    (501) staff       (20)      258 2023-05-19 09:18:49.000000 twilio-tap-tripactions-0.0.2/twilio_tap_tripactions.egg-info/PKG-INFO
+-rw-r--r--   0 aigupta    (501) staff       (20)      483 2023-05-19 09:18:49.000000 twilio-tap-tripactions-0.0.2/twilio_tap_tripactions.egg-info/SOURCES.txt
+-rw-r--r--   0 aigupta    (501) staff       (20)        1 2023-05-19 09:18:49.000000 twilio-tap-tripactions-0.0.2/twilio_tap_tripactions.egg-info/dependency_links.txt
+-rw-r--r--   0 aigupta    (501) staff       (20)       57 2023-05-19 09:18:49.000000 twilio-tap-tripactions-0.0.2/twilio_tap_tripactions.egg-info/entry_points.txt
+-rw-r--r--   0 aigupta    (501) staff       (20)       31 2023-05-19 09:18:49.000000 twilio-tap-tripactions-0.0.2/twilio_tap_tripactions.egg-info/requires.txt
+-rw-r--r--   0 aigupta    (501) staff       (20)       16 2023-05-19 09:18:49.000000 twilio-tap-tripactions-0.0.2/twilio_tap_tripactions.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `twilio-tap-tripactions-0.0.1/LICENSE` & `twilio-tap-tripactions-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twilio-tap-tripactions-0.0.1/README.md` & `twilio-tap-tripactions-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `twilio-tap-tripactions-0.0.1/setup.py` & `twilio-tap-tripactions-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="twilio-tap-tripactions",
-    version="0.0.01",
+    version="0.0.02",
     description="Singer.io tap for extracting data from TripActions API",
     author="Twilio",
     url="https://www.twilio.com/",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_tripactions"],
     install_requires=[
         "singer-python",
-        "requests",
+        "requests==2.29.0",
     ],
     entry_points="""
     [console_scripts]
     tap-tripactions=tap_tripactions:main
     """,
     packages=["tap_tripactions"],
     include_package_data=True,
```

### Comparing `twilio-tap-tripactions-0.0.1/tap_tripactions/__init__.py` & `twilio-tap-tripactions-0.0.2/tap_tripactions/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-tripactions-0.0.1/tap_tripactions/client.py` & `twilio-tap-tripactions-0.0.2/tap_tripactions/client.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-tripactions-0.0.1/tap_tripactions/schemas/bookings.json` & `twilio-tap-tripactions-0.0.2/tap_tripactions/schemas/bookings.json`

 * *Files identical despite different names*

### Comparing `twilio-tap-tripactions-0.0.1/tap_tripactions/streams.py` & `twilio-tap-tripactions-0.0.2/tap_tripactions/streams.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-tripactions-0.0.1/test/test_client.py` & `twilio-tap-tripactions-0.0.2/test/test_client.py`

 * *Files identical despite different names*

### Comparing `twilio-tap-tripactions-0.0.1/test/test_sync.py` & `twilio-tap-tripactions-0.0.2/test/test_sync.py`

 * *Files identical despite different names*

