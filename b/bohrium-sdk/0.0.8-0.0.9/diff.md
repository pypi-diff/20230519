# Comparing `tmp/bohrium-sdk-0.0.8.tar.gz` & `tmp/bohrium-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.0.8.tar", last modified: Fri May 19 01:59:41 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.0.9.tar", last modified: Fri May 19 02:01:02 2023, max compression
```

## Comparing `bohrium-sdk-0.0.8.tar` & `bohrium-sdk-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 01:59:41.824842 bohrium-sdk-0.0.8/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-19 01:59:41.824444 bohrium-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.0.8/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 01:59:41.820562 bohrium-sdk-0.0.8/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-19 01:59:41.000000 bohrium-sdk-0.0.8/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      319 2023-05-19 01:59:41.000000 bohrium-sdk-0.0.8/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-19 01:59:41.000000 bohrium-sdk-0.0.8/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-19 01:59:41.000000 bohrium-sdk-0.0.8/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-19 01:59:41.000000 bohrium-sdk-0.0.8/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 01:59:41.824122 bohrium-sdk-0.0.8/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.0.8/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3901 2023-05-19 01:59:25.000000 bohrium-sdk-0.0.8/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:16.000000 bohrium-sdk-0.0.8/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3465 2023-05-19 01:48:37.000000 bohrium-sdk-0.0.8/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1608 2023-05-19 01:47:21.000000 bohrium-sdk-0.0.8/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:51.000000 bohrium-sdk-0.0.8/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-19 01:59:41.824912 bohrium-sdk-0.0.8/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      499 2023-05-19 01:59:37.000000 bohrium-sdk-0.0.8/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 02:01:02.775052 bohrium-sdk-0.0.9/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-19 02:01:02.774707 bohrium-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.0.9/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 02:01:02.771121 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      319 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 02:01:02.774448 bohrium-sdk-0.0.9/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.0.9/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3901 2023-05-19 02:00:50.000000 bohrium-sdk-0.0.9/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:16.000000 bohrium-sdk-0.0.9/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3465 2023-05-19 01:48:37.000000 bohrium-sdk-0.0.9/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1608 2023-05-19 01:47:21.000000 bohrium-sdk-0.0.9/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:51.000000 bohrium-sdk-0.0.9/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-19 02:01:02.775254 bohrium-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      499 2023-05-19 02:00:47.000000 bohrium-sdk-0.0.9/setup.py
```

### Comparing `bohrium-sdk-0.0.8/bohriumsdk/client.py` & `bohrium-sdk-0.0.9/bohriumsdk/client.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.0.8/bohriumsdk/job.py` & `bohrium-sdk-0.0.9/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.0.8/bohriumsdk/node.py` & `bohrium-sdk-0.0.9/bohriumsdk/node.py`

 * *Files identical despite different names*

