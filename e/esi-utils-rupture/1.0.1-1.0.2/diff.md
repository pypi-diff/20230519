# Comparing `tmp/esi_utils_rupture-1.0.1.tar.gz` & `tmp/esi-utils-rupture-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/ghsc/esi/esi-utils-rupture/dist/tmplo0yu9sw/esi_utils_rupture-1.0.1.tar", last modified: Thu Aug 11 02:03:14 2022, max compression
+gzip compressed data, was "/builds/ghsc/esi/esi-utils-rupture/dist/tmpxg1poxeh/esi-utils-rupture-1.0.2.tar", last modified: Fri Aug 12 17:33:30 2022, max compression
```

## Comparing `esi_utils_rupture-1.0.1.tar` & `esi-utils-rupture-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1627 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      281 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      537 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7083 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/base.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/constants.py
--rwxrwxrwx   0 root         (0) root         (0)     9440 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/distance.py
--rwxrwxrwx   0 root         (0) root         (0)    25980 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/edge_rupture.py
--rw-rw-rw-   0 root         (0) root         (0)    15157 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/factory.py
--rw-rw-rw-   0 root         (0) root         (0)    12082 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/gc2.py
--rwxrwxrwx   0 root         (0) root         (0)    19243 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/origin.py
--rwxrwxrwx   0 root         (0) root         (0)    10295 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/point_rupture.py
--rwxrwxrwx   0 root         (0) root         (0)    41279 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/quad_rupture.py
--rw-rw-rw-   0 root         (0) root         (0)     6387 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/tensor.py
--rwxrwxrwx   0 root         (0) root         (0)    18180 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/esi_utils_rupture/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/esi_utils_rupture.egg-info/
--rw-r--r--   0 root         (0) root         (0)      281 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/esi_utils_rupture.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/esi_utils_rupture.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/esi_utils_rupture.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/esi_utils_rupture.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      372 2022-08-11 02:03:04.000000 esi_utils_rupture-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-11 02:03:14.000000 esi_utils_rupture-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      318 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      537 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7083 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/constants.py
+-rwxrwxrwx   0 root         (0) root         (0)     9440 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/distance.py
+-rwxrwxrwx   0 root         (0) root         (0)    25980 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/edge_rupture.py
+-rw-rw-rw-   0 root         (0) root         (0)    15157 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    12082 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/gc2.py
+-rwxrwxrwx   0 root         (0) root         (0)    19243 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/origin.py
+-rwxrwxrwx   0 root         (0) root         (0)    10295 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/point_rupture.py
+-rwxrwxrwx   0 root         (0) root         (0)    41279 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/quad_rupture.py
+-rw-rw-rw-   0 root         (0) root         (0)     6387 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/tensor.py
+-rwxrwxrwx   0 root         (0) root         (0)    18180 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/esi_utils_rupture/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/esi_utils_rupture.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      318 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/esi_utils_rupture.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      606 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/esi_utils_rupture.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/esi_utils_rupture.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      307 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/esi_utils_rupture.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/esi_utils_rupture.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       87 2022-08-12 17:30:53.000000 esi-utils-rupture-1.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      722 2022-08-12 17:33:30.000000 esi-utils-rupture-1.0.2/setup.cfg
```

### Comparing `esi_utils_rupture-1.0.1/LICENSE.md` & `esi-utils-rupture-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/README.md` & `esi-utils-rupture-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/base.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/base.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/constants.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/constants.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/distance.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/distance.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/edge_rupture.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/edge_rupture.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/factory.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/factory.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/gc2.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/gc2.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/origin.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/origin.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/point_rupture.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/point_rupture.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/quad_rupture.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/quad_rupture.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/tensor.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/tensor.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture/utils.py` & `esi-utils-rupture-1.0.2/esi_utils_rupture/utils.py`

 * *Files identical despite different names*

### Comparing `esi_utils_rupture-1.0.1/esi_utils_rupture.egg-info/SOURCES.txt` & `esi-utils-rupture-1.0.2/esi_utils_rupture.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.md
 README.md
 pyproject.toml
+setup.cfg
 esi_utils_rupture/__init__.py
 esi_utils_rupture/base.py
 esi_utils_rupture/constants.py
 esi_utils_rupture/distance.py
 esi_utils_rupture/edge_rupture.py
 esi_utils_rupture/factory.py
 esi_utils_rupture/gc2.py
@@ -12,8 +13,9 @@
 esi_utils_rupture/point_rupture.py
 esi_utils_rupture/quad_rupture.py
 esi_utils_rupture/tensor.py
 esi_utils_rupture/utils.py
 esi_utils_rupture.egg-info/PKG-INFO
 esi_utils_rupture.egg-info/SOURCES.txt
 esi_utils_rupture.egg-info/dependency_links.txt
+esi_utils_rupture.egg-info/requires.txt
 esi_utils_rupture.egg-info/top_level.txt
```

