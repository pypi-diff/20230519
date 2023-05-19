# Comparing `tmp/serializator-scocs-1.3.tar.gz` & `tmp/serializator-scocs-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializator-scocs-1.3.tar", last modified: Fri May 19 12:09:38 2023, max compression
+gzip compressed data, was "serializator-scocs-1.4.tar", last modified: Fri May 19 12:11:34 2023, max compression
```

## Comparing `serializator-scocs-1.3.tar` & `serializator-scocs-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:09:38.476068 serializator-scocs-1.3/
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      483 2023-05-19 12:09:38.475711 serializator-scocs-1.3/PKG-INFO
-drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:09:38.473109 serializator-scocs-1.3/serializator/
--rw-r--r--   0 fedortarasenko   (501) staff       (20)       35 2023-05-19 12:06:47.000000 serializator-scocs-1.3/serializator/__init__.py
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      289 2023-05-19 12:06:47.000000 serializator-scocs-1.3/serializator/main.py
-drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:09:38.475270 serializator-scocs-1.3/serializator_scocs.egg-info/
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      483 2023-05-19 12:09:38.000000 serializator-scocs-1.3/serializator_scocs.egg-info/PKG-INFO
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      222 2023-05-19 12:09:38.000000 serializator-scocs-1.3/serializator_scocs.egg-info/SOURCES.txt
--rw-r--r--   0 fedortarasenko   (501) staff       (20)        1 2023-05-19 12:09:38.000000 serializator-scocs-1.3/serializator_scocs.egg-info/dependency_links.txt
--rw-r--r--   0 fedortarasenko   (501) staff       (20)       13 2023-05-19 12:09:38.000000 serializator-scocs-1.3/serializator_scocs.egg-info/top_level.txt
--rw-r--r--   0 fedortarasenko   (501) staff       (20)       38 2023-05-19 12:09:38.476220 serializator-scocs-1.3/setup.cfg
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      653 2023-05-19 12:09:30.000000 serializator-scocs-1.3/setup.py
+drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:11:34.155508 serializator-scocs-1.4/
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      483 2023-05-19 12:11:34.155089 serializator-scocs-1.4/PKG-INFO
+drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:11:34.151668 serializator-scocs-1.4/serializator/
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)       35 2023-05-19 12:06:47.000000 serializator-scocs-1.4/serializator/__init__.py
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      250 2023-05-19 12:11:20.000000 serializator-scocs-1.4/serializator/main.py
+drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:11:34.154520 serializator-scocs-1.4/serializator_scocs.egg-info/
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      483 2023-05-19 12:11:34.000000 serializator-scocs-1.4/serializator_scocs.egg-info/PKG-INFO
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      222 2023-05-19 12:11:34.000000 serializator-scocs-1.4/serializator_scocs.egg-info/SOURCES.txt
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)        1 2023-05-19 12:11:34.000000 serializator-scocs-1.4/serializator_scocs.egg-info/dependency_links.txt
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)       13 2023-05-19 12:11:34.000000 serializator-scocs-1.4/serializator_scocs.egg-info/top_level.txt
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)       38 2023-05-19 12:11:34.155625 serializator-scocs-1.4/setup.cfg
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      653 2023-05-19 12:11:26.000000 serializator-scocs-1.4/setup.py
```

### Comparing `serializator-scocs-1.3/setup.py` & `serializator-scocs-1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from codecs import open
 from os import path
 
 setup(
     name="serializator-scocs",
-    version="1.3",
+    version="1.4",
     description="library for python serialization",
     long_description="SCoSC serialization/deserialization",
     long_description_content_type="text/markdown",
     author="Tarasenko Fyodor",
     author_email="tarasenkafiodar@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
```

