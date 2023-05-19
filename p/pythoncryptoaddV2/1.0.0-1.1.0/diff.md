# Comparing `tmp/pythoncryptoaddV2-1.0.0.tar.gz` & `tmp/pythoncryptoaddV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncryptoaddV2-1.0.0.tar", last modified: Fri May 19 11:46:45 2023, max compression
+gzip compressed data, was "pythoncryptoaddV2-1.1.0.tar", last modified: Fri May 19 11:48:50 2023, max compression
```

## Comparing `pythoncryptoaddV2-1.0.0.tar` & `pythoncryptoaddV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:46:45.196396 pythoncryptoaddV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-19 11:46:45.196396 pythoncryptoaddV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:46:45.192396 pythoncryptoaddV2-1.0.0/pythoncryptoaddV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 11:46:44.000000 pythoncryptoaddV2-1.0.0/pythoncryptoaddV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:46:45.196396 pythoncryptoaddV2-1.0.0/pythoncryptoaddV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-19 11:46:45.000000 pythoncryptoaddV2-1.0.0/pythoncryptoaddV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-19 11:46:45.000000 pythoncryptoaddV2-1.0.0/pythoncryptoaddV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 11:46:45.000000 pythoncryptoaddV2-1.0.0/pythoncryptoaddV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-19 11:46:45.000000 pythoncryptoaddV2-1.0.0/pythoncryptoaddV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 11:46:45.196396 pythoncryptoaddV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-05-19 11:46:44.000000 pythoncryptoaddV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:48:50.118890 pythoncryptoaddV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-19 11:48:50.118890 pythoncryptoaddV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:48:50.118890 pythoncryptoaddV2-1.1.0/pythoncryptoaddV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-19 11:48:49.000000 pythoncryptoaddV2-1.1.0/pythoncryptoaddV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 11:48:50.118890 pythoncryptoaddV2-1.1.0/pythoncryptoaddV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-19 11:48:50.000000 pythoncryptoaddV2-1.1.0/pythoncryptoaddV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-19 11:48:50.000000 pythoncryptoaddV2-1.1.0/pythoncryptoaddV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 11:48:50.000000 pythoncryptoaddV2-1.1.0/pythoncryptoaddV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-19 11:48:50.000000 pythoncryptoaddV2-1.1.0/pythoncryptoaddV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 11:48:50.118890 pythoncryptoaddV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-05-19 11:48:49.000000 pythoncryptoaddV2-1.1.0/setup.py
```

### Comparing `pythoncryptoaddV2-1.0.0/setup.py` & `pythoncryptoaddV2-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncryptoaddV2",
     version=VERSION,
```

