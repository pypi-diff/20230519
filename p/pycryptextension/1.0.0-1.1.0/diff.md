# Comparing `tmp/pycryptextension-1.0.0.tar.gz` & `tmp/pycryptextension-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptextension-1.0.0.tar", last modified: Fri May 19 19:07:16 2023, max compression
+gzip compressed data, was "pycryptextension-1.1.0.tar", last modified: Fri May 19 19:09:22 2023, max compression
```

## Comparing `pycryptextension-1.0.0.tar` & `pycryptextension-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 19:07:16.786905 pycryptextension-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-19 19:07:16.786905 pycryptextension-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 19:07:16.786905 pycryptextension-1.0.0/pycryptextension/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 19:07:16.000000 pycryptextension-1.0.0/pycryptextension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 19:07:16.786905 pycryptextension-1.0.0/pycryptextension.egg-info/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-19 19:07:16.000000 pycryptextension-1.0.0/pycryptextension.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-19 19:07:16.000000 pycryptextension-1.0.0/pycryptextension.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 19:07:16.000000 pycryptextension-1.0.0/pycryptextension.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-19 19:07:16.000000 pycryptextension-1.0.0/pycryptextension.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 19:07:16.786905 pycryptextension-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      562 2023-05-19 19:07:16.000000 pycryptextension-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 19:09:22.065542 pycryptextension-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-19 19:09:22.065542 pycryptextension-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 19:09:22.065542 pycryptextension-1.1.0/pycryptextension/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-19 19:09:21.000000 pycryptextension-1.1.0/pycryptextension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 19:09:22.065542 pycryptextension-1.1.0/pycryptextension.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-19 19:09:21.000000 pycryptextension-1.1.0/pycryptextension.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-19 19:09:22.000000 pycryptextension-1.1.0/pycryptextension.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 19:09:21.000000 pycryptextension-1.1.0/pycryptextension.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-19 19:09:21.000000 pycryptextension-1.1.0/pycryptextension.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 19:09:22.065542 pycryptextension-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      562 2023-05-19 19:09:21.000000 pycryptextension-1.1.0/setup.py
```

### Comparing `pycryptextension-1.0.0/setup.py` & `pycryptextension-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pycryptextension",
     version=VERSION,
```

