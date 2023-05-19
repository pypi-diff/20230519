# Comparing `tmp/udls-1.1.1.tar.gz` & `tmp/udls-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udls-1.1.1.tar", last modified: Tue Apr 11 15:37:11 2023, max compression
+gzip compressed data, was "udls-1.1.2.tar", last modified: Fri May 19 11:41:20 2023, max compression
```

## Comparing `udls-1.1.1.tar` & `udls-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:37:11.305177 udls-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 15:37:00.000000 udls-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 15:37:00.000000 udls-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-11 15:37:11.305177 udls-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:37:00.000000 udls-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 15:37:00.000000 udls-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:37:11.305177 udls-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-11 15:37:00.000000 udls-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:37:11.301176 udls-1.1.1/udls/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-11 15:37:00.000000 udls-1.1.1/udls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-11 15:37:00.000000 udls-1.1.1/udls/audio_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 15:37:00.000000 udls-1.1.1/udls/audio_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-11 15:37:00.000000 udls-1.1.1/udls/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-11 15:37:00.000000 udls-1.1.1/udls/duration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:37:11.305177 udls-1.1.1/udls/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 15:37:00.000000 udls-1.1.1/udls/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-11 15:37:00.000000 udls-1.1.1/udls/generated/audio_example_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-11 15:37:00.000000 udls-1.1.1/udls/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-11 15:37:00.000000 udls-1.1.1/udls/simple_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 15:37:00.000000 udls-1.1.1/udls/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:37:11.305177 udls-1.1.1/udls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-11 15:37:11.000000 udls-1.1.1/udls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-11 15:37:11.000000 udls-1.1.1/udls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:37:11.000000 udls-1.1.1/udls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 15:37:11.000000 udls-1.1.1/udls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-11 15:37:11.000000 udls-1.1.1/udls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 15:37:11.000000 udls-1.1.1/udls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:20.966738 udls-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 11:41:10.000000 udls-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 11:41:10.000000 udls-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 11:41:20.966738 udls-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:10.000000 udls-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 11:41:10.000000 udls-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:41:20.966738 udls-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-19 11:41:10.000000 udls-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:20.962738 udls-1.1.2/udls/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-19 11:41:10.000000 udls-1.1.2/udls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-19 11:41:10.000000 udls-1.1.2/udls/audio_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-19 11:41:10.000000 udls-1.1.2/udls/audio_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-19 11:41:10.000000 udls-1.1.2/udls/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 11:41:10.000000 udls-1.1.2/udls/duration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:20.966738 udls-1.1.2/udls/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-19 11:41:10.000000 udls-1.1.2/udls/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-19 11:41:10.000000 udls-1.1.2/udls/generated/audio_example_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-19 11:41:10.000000 udls-1.1.2/udls/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-19 11:41:10.000000 udls-1.1.2/udls/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-19 11:41:10.000000 udls-1.1.2/udls/simple_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-19 11:41:10.000000 udls-1.1.2/udls/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:20.962738 udls-1.1.2/udls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 11:41:20.000000 udls-1.1.2/udls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 11:41:20.000000 udls-1.1.2/udls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:41:20.000000 udls-1.1.2/udls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-19 11:41:20.000000 udls-1.1.2/udls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 11:41:20.000000 udls-1.1.2/udls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:41:20.000000 udls-1.1.2/udls.egg-info/top_level.txt
```

### Comparing `udls-1.1.1/LICENSE` & `udls-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `udls-1.1.1/setup.py` & `udls-1.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,13 +21,15 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
-        "console_scripts":
-        ["resample = udls.resample:main", "duration = udls.duration:main"]
+        "console_scripts": [
+            "resample = udls.resample:main", "duration = udls.duration:main",
+            "serve_dataset = udls.serve:main"
+        ]
     },
     install_requires=requirements.split("\n"),
     python_requires='>=3.7',
 )
```

### Comparing `udls-1.1.1/udls/audio_example.py` & `udls-1.1.2/udls/audio_example.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.1/udls/audio_example_dataset.py` & `udls-1.1.2/udls/audio_example_dataset.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.1/udls/base_dataset.py` & `udls-1.1.2/udls/base_dataset.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.1/udls/generated/audio_example_pb2.py` & `udls-1.1.2/udls/generated/audio_example_pb2.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.1/udls/resample.py` & `udls-1.1.2/udls/resample.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.1/udls/simple_dataset.py` & `udls-1.1.2/udls/simple_dataset.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.1/udls/transforms.py` & `udls-1.1.2/udls/transforms.py`

 * *Files identical despite different names*

