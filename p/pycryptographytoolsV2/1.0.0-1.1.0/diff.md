# Comparing `tmp/pycryptographytoolsV2-1.0.0.tar.gz` & `tmp/pycryptographytoolsV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptographytoolsV2-1.0.0.tar", last modified: Fri May 19 14:33:49 2023, max compression
+gzip compressed data, was "pycryptographytoolsV2-1.1.0.tar", last modified: Fri May 19 14:35:54 2023, max compression
```

## Comparing `pycryptographytoolsV2-1.0.0.tar` & `pycryptographytoolsV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:33:49.630667 pycryptographytoolsV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-19 14:33:49.630667 pycryptographytoolsV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:33:49.630667 pycryptographytoolsV2-1.0.0/pycryptographytoolsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 14:33:49.000000 pycryptographytoolsV2-1.0.0/pycryptographytoolsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:33:49.630667 pycryptographytoolsV2-1.0.0/pycryptographytoolsV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-19 14:33:49.000000 pycryptographytoolsV2-1.0.0/pycryptographytoolsV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-19 14:33:49.000000 pycryptographytoolsV2-1.0.0/pycryptographytoolsV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 14:33:49.000000 pycryptographytoolsV2-1.0.0/pycryptographytoolsV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 14:33:49.000000 pycryptographytoolsV2-1.0.0/pycryptographytoolsV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 14:33:49.630667 pycryptographytoolsV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-19 14:33:49.000000 pycryptographytoolsV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:35:54.949286 pycryptographytoolsV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-19 14:35:54.949286 pycryptographytoolsV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:35:54.949286 pycryptographytoolsV2-1.1.0/pycryptographytoolsV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-19 14:35:54.000000 pycryptographytoolsV2-1.1.0/pycryptographytoolsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:35:54.949286 pycryptographytoolsV2-1.1.0/pycryptographytoolsV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-19 14:35:54.000000 pycryptographytoolsV2-1.1.0/pycryptographytoolsV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-19 14:35:54.000000 pycryptographytoolsV2-1.1.0/pycryptographytoolsV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 14:35:54.000000 pycryptographytoolsV2-1.1.0/pycryptographytoolsV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 14:35:54.000000 pycryptographytoolsV2-1.1.0/pycryptographytoolsV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 14:35:54.949286 pycryptographytoolsV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-19 14:35:54.000000 pycryptographytoolsV2-1.1.0/setup.py
```

### Comparing `pycryptographytoolsV2-1.0.0/setup.py` & `pycryptographytoolsV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pycryptographytoolsV2",
     version=VERSION,
```

