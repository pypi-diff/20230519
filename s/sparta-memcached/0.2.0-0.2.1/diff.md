# Comparing `tmp/sparta-memcached-0.2.0.tar.gz` & `tmp/sparta-memcached-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparta-memcached-0.2.0.tar", last modified: Fri May 19 06:40:26 2023, max compression
+gzip compressed data, was "sparta-memcached-0.2.1.tar", last modified: Fri May 19 07:42:00 2023, max compression
```

## Comparing `sparta-memcached-0.2.0.tar` & `sparta-memcached-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:40:26.863771 sparta-memcached-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1283 2023-05-19 06:40:26.859770 sparta-memcached-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1550 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 06:40:26.863771 sparta-memcached-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1486 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:40:26.855770 sparta-memcached-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:40:26.855770 sparta-memcached-0.2.0/src/sparta/
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/src/sparta/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:40:26.859770 sparta-memcached-0.2.0/src/sparta/memcached/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/src/sparta/memcached/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5512 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/src/sparta/memcached/base.py
--rw-r--r--   0 root         (0) root         (0)     2580 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/src/sparta/memcached/client.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/src/sparta/memcached/decorator.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/src/sparta/memcached/dummy.py
--rw-r--r--   0 root         (0) root         (0)     1372 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/src/sparta/memcached/utils.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-05-19 06:39:05.000000 sparta-memcached-0.2.0/src/sparta/memcached/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:40:26.859770 sparta-memcached-0.2.0/src/sparta_memcached.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1283 2023-05-19 06:40:26.000000 sparta-memcached-0.2.0/src/sparta_memcached.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2023-05-19 06:40:26.000000 sparta-memcached-0.2.0/src/sparta_memcached.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 06:40:26.000000 sparta-memcached-0.2.0/src/sparta_memcached.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-19 06:40:26.000000 sparta-memcached-0.2.0/src/sparta_memcached.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-19 06:40:26.000000 sparta-memcached-0.2.0/src/sparta_memcached.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-19 06:40:26.000000 sparta-memcached-0.2.0/src/sparta_memcached.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:42:00.888698 sparta-memcached-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-05-19 07:42:00.888698 sparta-memcached-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 07:42:00.888698 sparta-memcached-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:42:00.884698 sparta-memcached-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:42:00.884698 sparta-memcached-0.2.1/src/sparta/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/src/sparta/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:42:00.888698 sparta-memcached-0.2.1/src/sparta/memcached/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/src/sparta/memcached/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5512 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/src/sparta/memcached/base.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/src/sparta/memcached/client.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/src/sparta/memcached/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/src/sparta/memcached/dummy.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/src/sparta/memcached/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-05-19 07:39:53.000000 sparta-memcached-0.2.1/src/sparta/memcached/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:42:00.888698 sparta-memcached-0.2.1/src/sparta_memcached.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-05-19 07:42:00.000000 sparta-memcached-0.2.1/src/sparta_memcached.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-19 07:42:00.000000 sparta-memcached-0.2.1/src/sparta_memcached.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 07:42:00.000000 sparta-memcached-0.2.1/src/sparta_memcached.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-19 07:42:00.000000 sparta-memcached-0.2.1/src/sparta_memcached.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-19 07:42:00.000000 sparta-memcached-0.2.1/src/sparta_memcached.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-19 07:42:00.000000 sparta-memcached-0.2.1/src/sparta_memcached.egg-info/top_level.txt
```

### Comparing `sparta-memcached-0.2.0/LICENSE` & `sparta-memcached-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparta-memcached-0.2.0/PKG-INFO` & `sparta-memcached-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparta-memcached
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sparta memcached library
 Home-page: https://github.com/Spartan-Approach/sparta-memcached
 Author: Spartan Approach
 Author-email: sparta@spartanapproach.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparta-memcached-0.2.0/README.md` & `sparta-memcached-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sparta-memcached-0.2.0/setup.py` & `sparta-memcached-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `sparta-memcached-0.2.0/src/sparta/memcached/base.py` & `sparta-memcached-0.2.1/src/sparta/memcached/base.py`

 * *Files identical despite different names*

### Comparing `sparta-memcached-0.2.0/src/sparta/memcached/client.py` & `sparta-memcached-0.2.1/src/sparta/memcached/client.py`

 * *Files identical despite different names*

### Comparing `sparta-memcached-0.2.0/src/sparta/memcached/decorator.py` & `sparta-memcached-0.2.1/src/sparta/memcached/decorator.py`

 * *Files identical despite different names*

### Comparing `sparta-memcached-0.2.0/src/sparta/memcached/utils.py` & `sparta-memcached-0.2.1/src/sparta/memcached/utils.py`

 * *Files identical despite different names*

### Comparing `sparta-memcached-0.2.0/src/sparta/memcached/wrapper.py` & `sparta-memcached-0.2.1/src/sparta/memcached/wrapper.py`

 * *Files identical despite different names*

### Comparing `sparta-memcached-0.2.0/src/sparta_memcached.egg-info/PKG-INFO` & `sparta-memcached-0.2.1/src/sparta_memcached.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparta-memcached
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sparta memcached library
 Home-page: https://github.com/Spartan-Approach/sparta-memcached
 Author: Spartan Approach
 Author-email: sparta@spartanapproach.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sparta-memcached-0.2.0/src/sparta_memcached.egg-info/SOURCES.txt` & `sparta-memcached-0.2.1/src/sparta_memcached.egg-info/SOURCES.txt`

 * *Files identical despite different names*

