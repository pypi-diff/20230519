# Comparing `tmp/libheader-1.0.1.tar.gz` & `tmp/libheader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libheader-1.0.1.tar", last modified: Thu May 18 23:24:14 2023, max compression
+gzip compressed data, was "libheader-1.0.2.tar", last modified: Thu May 18 23:38:05 2023, max compression
```

## Comparing `libheader-1.0.1.tar` & `libheader-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:24:14.718547 libheader-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 23:24:14.718547 libheader-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-18 23:24:02.000000 libheader-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:24:14.714547 libheader-1.0.1/libheader/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/gcclh.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/lh.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-18 23:24:02.000000 libheader-1.0.1/libheader/makelh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:24:14.714547 libheader-1.0.1/libheader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 23:24:14.000000 libheader-1.0.1/libheader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-18 23:24:14.000000 libheader-1.0.1/libheader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:24:14.000000 libheader-1.0.1/libheader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 23:24:14.000000 libheader-1.0.1/libheader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:24:14.718547 libheader-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-18 23:24:02.000000 libheader-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:38:05.327624 libheader-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 23:38:05.327624 libheader-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-18 23:37:49.000000 libheader-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:38:05.323624 libheader-1.0.2/libheader/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/gcclh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/lh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-18 23:37:49.000000 libheader-1.0.2/libheader/makelh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:38:05.327624 libheader-1.0.2/libheader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 23:38:05.000000 libheader-1.0.2/libheader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-18 23:38:05.000000 libheader-1.0.2/libheader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:38:05.000000 libheader-1.0.2/libheader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 23:38:05.000000 libheader-1.0.2/libheader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:38:05.327624 libheader-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-18 23:37:49.000000 libheader-1.0.2/setup.py
```

### Comparing `libheader-1.0.1/libheader/gcclh.py` & `libheader-1.0.2/libheader/gcclh.py`

 * *Files identical despite different names*

### Comparing `libheader-1.0.1/libheader/lh.py` & `libheader-1.0.2/libheader/lh.py`

 * *Files identical despite different names*

### Comparing `libheader-1.0.1/libheader/makelh.py` & `libheader-1.0.2/libheader/makelh.py`

 * *Files identical despite different names*

### Comparing `libheader-1.0.1/setup.py` & `libheader-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='libheader',
-    version='1.0.1',    
+    version='1.0.2',    
     description='A new file format that makes C easier.',
     url='https://github.com/wk1093/libheader',
     author='Wyatt Kloos',
     author_email='wyattk1093@gmail.com',
     license='BSD 2-clause',
     packages=['libheader'],
     install_requires=[],
```

