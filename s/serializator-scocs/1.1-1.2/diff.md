# Comparing `tmp/serializator-scocs-1.1.tar.gz` & `tmp/serializator-scocs-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializator-scocs-1.1.tar", last modified: Fri May 19 11:57:03 2023, max compression
+gzip compressed data, was "serializator-scocs-1.2.tar", last modified: Fri May 19 12:01:30 2023, max compression
```

## Comparing `serializator-scocs-1.1.tar` & `serializator-scocs-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 11:57:03.386540 serializator-scocs-1.1/
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      483 2023-05-19 11:57:03.385156 serializator-scocs-1.1/PKG-INFO
-drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 11:57:03.382176 serializator-scocs-1.1/serializator/
--rw-r--r--   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 11:55:56.000000 serializator-scocs-1.1/serializator/__init__.py
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      230 2023-05-19 11:56:47.000000 serializator-scocs-1.1/serializator/main.py
-drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 11:57:03.384400 serializator-scocs-1.1/serializator_scocs.egg-info/
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      483 2023-05-19 11:57:03.000000 serializator-scocs-1.1/serializator_scocs.egg-info/PKG-INFO
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      222 2023-05-19 11:57:03.000000 serializator-scocs-1.1/serializator_scocs.egg-info/SOURCES.txt
--rw-r--r--   0 fedortarasenko   (501) staff       (20)        1 2023-05-19 11:57:03.000000 serializator-scocs-1.1/serializator_scocs.egg-info/dependency_links.txt
--rw-r--r--   0 fedortarasenko   (501) staff       (20)       13 2023-05-19 11:57:03.000000 serializator-scocs-1.1/serializator_scocs.egg-info/top_level.txt
--rw-r--r--   0 fedortarasenko   (501) staff       (20)       38 2023-05-19 11:57:03.387019 serializator-scocs-1.1/setup.cfg
--rw-r--r--   0 fedortarasenko   (501) staff       (20)      653 2023-05-19 11:56:44.000000 serializator-scocs-1.1/setup.py
+drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:01:30.840948 serializator-scocs-1.2/
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      483 2023-05-19 12:01:30.840546 serializator-scocs-1.2/PKG-INFO
+drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:01:30.837950 serializator-scocs-1.2/serializator/
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)       33 2023-05-19 12:01:14.000000 serializator-scocs-1.2/serializator/__init__.py
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      230 2023-05-19 11:56:47.000000 serializator-scocs-1.2/serializator/main.py
+drwxr-xr-x   0 fedortarasenko   (501) staff       (20)        0 2023-05-19 12:01:30.840025 serializator-scocs-1.2/serializator_scocs.egg-info/
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      483 2023-05-19 12:01:30.000000 serializator-scocs-1.2/serializator_scocs.egg-info/PKG-INFO
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      222 2023-05-19 12:01:30.000000 serializator-scocs-1.2/serializator_scocs.egg-info/SOURCES.txt
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)        1 2023-05-19 12:01:30.000000 serializator-scocs-1.2/serializator_scocs.egg-info/dependency_links.txt
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)       13 2023-05-19 12:01:30.000000 serializator-scocs-1.2/serializator_scocs.egg-info/top_level.txt
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)       38 2023-05-19 12:01:30.841054 serializator-scocs-1.2/setup.cfg
+-rw-r--r--   0 fedortarasenko   (501) staff       (20)      653 2023-05-19 12:01:21.000000 serializator-scocs-1.2/setup.py
```

### Comparing `serializator-scocs-1.1/setup.py` & `serializator-scocs-1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from codecs import open
 from os import path
 
 setup(
     name="serializator-scocs",
-    version="1.1",
+    version="1.2",
     description="library for python serialization",
     long_description="SCoSC serialization/deserialization",
     long_description_content_type="text/markdown",
     author="Tarasenko Fyodor",
     author_email="tarasenkafiodar@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
```

