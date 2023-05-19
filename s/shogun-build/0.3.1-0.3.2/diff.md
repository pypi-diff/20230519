# Comparing `tmp/shogun-build-0.3.1.tar.gz` & `tmp/shogun-build-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shogun-build-0.3.1.tar", last modified: Mon Apr 17 00:00:28 2023, max compression
+gzip compressed data, was "shogun-build-0.3.2.tar", last modified: Fri May 19 18:38:01 2023, max compression
```

## Comparing `shogun-build-0.3.1.tar` & `shogun-build-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-17 00:00:28.308867 shogun-build-0.3.1/
--rw-r--r--   0 branalba  (1000) branalba  (1000)     1063 2023-04-17 00:00:15.000000 shogun-build-0.3.1/LICENSE
--rw-r--r--   0 branalba  (1000) branalba  (1000)     1478 2023-04-17 00:00:28.308867 shogun-build-0.3.1/PKG-INFO
--rw-r--r--   0 branalba  (1000) branalba  (1000)      582 2023-03-14 20:47:36.000000 shogun-build-0.3.1/README.md
--rw-r--r--   0 branalba  (1000) branalba  (1000)      510 2023-04-16 23:59:31.000000 shogun-build-0.3.1/pyproject.toml
--rw-r--r--   0 branalba  (1000) branalba  (1000)       38 2023-04-17 00:00:28.308867 shogun-build-0.3.1/setup.cfg
-drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-17 00:00:28.308867 shogun-build-0.3.1/shogun/
--rw-r--r--   0 branalba  (1000) branalba  (1000)        0 2022-08-03 19:14:34.000000 shogun-build-0.3.1/shogun/__init__.py
--rw-r--r--   0 branalba  (1000) branalba  (1000)     6130 2023-01-11 18:39:50.000000 shogun-build-0.3.1/shogun/buildutils.py
--rw-r--r--   0 branalba  (1000) branalba  (1000)     1907 2022-08-19 03:54:16.000000 shogun-build-0.3.1/shogun/pathutil.py
--rw-r--r--   0 branalba  (1000) branalba  (1000)     3657 2022-08-24 19:04:05.000000 shogun-build-0.3.1/shogun/platforms.py
-drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-17 00:00:28.308867 shogun-build-0.3.1/shogun/thirdparty/
--rw-r--r--   0 branalba  (1000) branalba  (1000)     6946 2022-08-06 18:24:39.000000 shogun-build-0.3.1/shogun/thirdparty/ninja_syntax.py
-drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-17 00:00:28.308867 shogun-build-0.3.1/shogun_build.egg-info/
--rw-r--r--   0 branalba  (1000) branalba  (1000)     1478 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/PKG-INFO
--rw-r--r--   0 branalba  (1000) branalba  (1000)      324 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/SOURCES.txt
--rw-r--r--   0 branalba  (1000) branalba  (1000)        1 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/dependency_links.txt
--rw-r--r--   0 branalba  (1000) branalba  (1000)        6 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/requires.txt
--rw-r--r--   0 branalba  (1000) branalba  (1000)        7 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/top_level.txt
+drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-05-19 18:38:01.760534 shogun-build-0.3.2/
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     1063 2023-04-17 00:00:15.000000 shogun-build-0.3.2/LICENSE
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     2101 2023-05-19 18:38:01.757201 shogun-build-0.3.2/PKG-INFO
+-rw-r--r--   0 branalba  (1000) branalba  (1000)      582 2023-03-14 20:47:36.000000 shogun-build-0.3.2/README.md
+-rw-r--r--   0 branalba  (1000) branalba  (1000)      531 2023-05-19 18:36:12.000000 shogun-build-0.3.2/pyproject.toml
+-rw-r--r--   0 branalba  (1000) branalba  (1000)       38 2023-05-19 18:38:01.760534 shogun-build-0.3.2/setup.cfg
+drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-05-19 18:38:01.757201 shogun-build-0.3.2/shogun/
+-rw-r--r--   0 branalba  (1000) branalba  (1000)        0 2022-08-03 19:14:34.000000 shogun-build-0.3.2/shogun/__init__.py
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     6130 2023-01-11 18:39:50.000000 shogun-build-0.3.2/shogun/buildutils.py
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     1907 2022-08-19 03:54:16.000000 shogun-build-0.3.2/shogun/pathutil.py
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     3587 2023-05-19 18:35:40.000000 shogun-build-0.3.2/shogun/platforms.py
+drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-05-19 18:38:01.757201 shogun-build-0.3.2/shogun/thirdparty/
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     6946 2022-08-06 18:24:39.000000 shogun-build-0.3.2/shogun/thirdparty/ninja_syntax.py
+drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-05-19 18:38:01.757201 shogun-build-0.3.2/shogun_build.egg-info/
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     2101 2023-05-19 18:38:01.000000 shogun-build-0.3.2/shogun_build.egg-info/PKG-INFO
+-rw-r--r--   0 branalba  (1000) branalba  (1000)      324 2023-05-19 18:38:01.000000 shogun-build-0.3.2/shogun_build.egg-info/SOURCES.txt
+-rw-r--r--   0 branalba  (1000) branalba  (1000)        1 2023-05-19 18:38:01.000000 shogun-build-0.3.2/shogun_build.egg-info/dependency_links.txt
+-rw-r--r--   0 branalba  (1000) branalba  (1000)        6 2023-05-19 18:38:01.000000 shogun-build-0.3.2/shogun_build.egg-info/requires.txt
+-rw-r--r--   0 branalba  (1000) branalba  (1000)        7 2023-05-19 18:38:01.000000 shogun-build-0.3.2/shogun_build.egg-info/top_level.txt
```

### Comparing `shogun-build-0.3.1/LICENSE` & `shogun-build-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.1/README.md` & `shogun-build-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.1/shogun/buildutils.py` & `shogun-build-0.3.2/shogun/buildutils.py`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.1/shogun/pathutil.py` & `shogun-build-0.3.2/shogun/pathutil.py`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.1/shogun/platforms.py` & `shogun-build-0.3.2/shogun/platforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,17 @@
         return self._common_flags
 
 class platform_x86 ( platform_gcc_base ):
 
     def __init__ ( self ):
         super().__init__()
 
-        self._cc_flags_base = ['-W', '-Wall', '-Wextra'] 
-        self._cpp_flags_base =  ['-std=c++17'] + self._cc_flags_base 
-        self._ld_flags_base = ['-lm', '-lc']
+        self._cc_flags_base = [] 
+        self._cpp_flags_base =  [] 
+        self._ld_flags_base = []
 
 class cortex_m ( platform_gcc_base ):
     '''
     Class definition for a Cortex-M platform target.
     '''
 
     _cmd_prefix = 'arm-none-eabi-'
```

### Comparing `shogun-build-0.3.1/shogun/thirdparty/ninja_syntax.py` & `shogun-build-0.3.2/shogun/thirdparty/ninja_syntax.py`

 * *Files identical despite different names*

