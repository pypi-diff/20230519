# Comparing `tmp/libheader-1.0.6.tar.gz` & `tmp/libheader-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libheader-1.0.6.tar", last modified: Fri May 19 00:15:24 2023, max compression
+gzip compressed data, was "libheader-1.0.7.tar", last modified: Fri May 19 00:18:20 2023, max compression
```

## Comparing `libheader-1.0.6.tar` & `libheader-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:15:24.217545 libheader-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 00:15:24.217545 libheader-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-19 00:15:13.000000 libheader-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:15:24.213545 libheader-1.0.6/libheader/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 00:15:13.000000 libheader-1.0.6/libheader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-19 00:15:13.000000 libheader-1.0.6/libheader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 00:15:13.000000 libheader-1.0.6/libheader/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 00:15:13.000000 libheader-1.0.6/libheader/gcclh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-19 00:15:13.000000 libheader-1.0.6/libheader/lh.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 00:15:13.000000 libheader-1.0.6/libheader/makelh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:15:24.213545 libheader-1.0.6/libheader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 00:15:24.000000 libheader-1.0.6/libheader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-19 00:15:24.000000 libheader-1.0.6/libheader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:15:24.000000 libheader-1.0.6/libheader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 00:15:24.000000 libheader-1.0.6/libheader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:15:24.217545 libheader-1.0.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 00:15:13.000000 libheader-1.0.6/scripts/gcclh.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 00:15:13.000000 libheader-1.0.6/scripts/makelh.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:15:24.217545 libheader-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-19 00:15:13.000000 libheader-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:18:20.153221 libheader-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 00:18:20.153221 libheader-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-19 00:18:04.000000 libheader-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:18:20.153221 libheader-1.0.7/libheader/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 00:18:04.000000 libheader-1.0.7/libheader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-19 00:18:04.000000 libheader-1.0.7/libheader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 00:18:04.000000 libheader-1.0.7/libheader/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 00:18:04.000000 libheader-1.0.7/libheader/gcclh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-19 00:18:04.000000 libheader-1.0.7/libheader/lh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 00:18:04.000000 libheader-1.0.7/libheader/makelh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:18:20.153221 libheader-1.0.7/libheader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 00:18:20.000000 libheader-1.0.7/libheader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-19 00:18:20.000000 libheader-1.0.7/libheader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:18:20.000000 libheader-1.0.7/libheader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 00:18:20.000000 libheader-1.0.7/libheader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:18:20.153221 libheader-1.0.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 00:18:04.000000 libheader-1.0.7/scripts/gcclh
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 00:18:04.000000 libheader-1.0.7/scripts/gcclh.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 00:18:04.000000 libheader-1.0.7/scripts/makelh
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 00:18:04.000000 libheader-1.0.7/scripts/makelh.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:18:20.153221 libheader-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-19 00:18:04.000000 libheader-1.0.7/setup.py
```

### Comparing `libheader-1.0.6/PKG-INFO` & `libheader-1.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libheader
-Version: 1.0.6
+Version: 1.0.7
 Summary: A new file format that makes C easier.
 Home-page: https://github.com/wk1093/libheader
 Author: Wyatt Kloos
 Author-email: wyattk1093@gmail.com
 License: BSD 2-clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `libheader-1.0.6/README.md` & `libheader-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `libheader-1.0.6/libheader/gcclh.py` & `libheader-1.0.7/libheader/gcclh.py`

 * *Files identical despite different names*

### Comparing `libheader-1.0.6/libheader/lh.py` & `libheader-1.0.7/libheader/lh.py`

 * *Files identical despite different names*

### Comparing `libheader-1.0.6/libheader.egg-info/PKG-INFO` & `libheader-1.0.7/libheader.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libheader
-Version: 1.0.6
+Version: 1.0.7
 Summary: A new file format that makes C easier.
 Home-page: https://github.com/wk1093/libheader
 Author: Wyatt Kloos
 Author-email: wyattk1093@gmail.com
 License: BSD 2-clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `libheader-1.0.6/setup.py` & `libheader-1.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,12 +21,14 @@
         'License :: OSI Approved :: BSD License',  
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
     ],
     scripts=[
         'scripts/gcclh.py',
-        'scripts/makelh.py'
+        'scripts/makelh.py',
+        'scripts/gcclh',
+        'scripts/makelh'
     ],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

