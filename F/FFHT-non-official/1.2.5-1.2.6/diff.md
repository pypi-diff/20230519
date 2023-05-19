# Comparing `tmp/FFHT-non-official-1.2.5.tar.gz` & `tmp/FFHT-non-official-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFHT-non-official-1.2.5.tar", last modified: Fri May 19 11:46:46 2023, max compression
+gzip compressed data, was "FFHT-non-official-1.2.6.tar", last modified: Fri May 19 11:49:07 2023, max compression
```

## Comparing `FFHT-non-official-1.2.5.tar` & `FFHT-non-official-1.2.6.tar`

### file list

```diff
@@ -1,46 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:46:46.926514 FFHT-non-official-1.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:46:46.926514 FFHT-non-official-1.2.5/FFHT_non_official.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:46:46.000000 FFHT-non-official-1.2.5/FFHT_non_official.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-19 11:46:46.000000 FFHT-non-official-1.2.5/FFHT_non_official.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:46:46.000000 FFHT-non-official-1.2.5/FFHT_non_official.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:46:46.000000 FFHT-non-official-1.2.5/FFHT_non_official.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:46:46.926514 FFHT-non-official-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:46:46.910514 FFHT-non-official-1.2.5/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:46:46.910514 FFHT-non-official-1.2.5/external/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:46:46.910514 FFHT-non-official-1.2.5/external/benchmark/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:46:46.918514 FFHT-non-official-1.2.5/external/benchmark/include/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)    42137 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/include/benchmark/benchmark.h
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/include/benchmark/benchmark_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/include/benchmark/reporter.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:46:46.926514 FFHT-non-official-1.2.5/external/benchmark/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/arraysize.h
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/benchmark_api_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/check.h
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/colorprint.h
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/commandlineflags.h
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/complexity.h
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/counter.h
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/cycleclock.h
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/internal_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/log.h
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/re.h
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/sleep.h
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/stat.h
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/string_util.h
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/sysinfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/src/timers.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:46:46.926514 FFHT-non-official-1.2.5/external/benchmark/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/external/benchmark/test/output_test.h
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/fast_copy.c
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/fast_copy.h
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/fht-pybind11.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/fht.c
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/fht.h
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/fht_header_only.h
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/fht_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:46:46.926514 FFHT-non-official-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-19 11:46:38.000000 FFHT-non-official-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:49:07.214255 FFHT-non-official-1.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:49:07.214255 FFHT-non-official-1.2.6/FFHT_non_official.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:49:07.000000 FFHT-non-official-1.2.6/FFHT_non_official.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-19 11:49:07.000000 FFHT-non-official-1.2.6/FFHT_non_official.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:49:07.000000 FFHT-non-official-1.2.6/FFHT_non_official.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:49:07.000000 FFHT-non-official-1.2.6/FFHT_non_official.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:49:07.214255 FFHT-non-official-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/_ffht_2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/_ffht_3.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:49:07.202255 FFHT-non-official-1.2.6/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:49:07.206255 FFHT-non-official-1.2.6/external/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:49:07.202255 FFHT-non-official-1.2.6/external/benchmark/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:49:07.210255 FFHT-non-official-1.2.6/external/benchmark/include/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)    42137 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/include/benchmark/benchmark.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/include/benchmark/benchmark_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/include/benchmark/reporter.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:49:07.210255 FFHT-non-official-1.2.6/external/benchmark/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/arraysize.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/benchmark_api_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/check.h
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/colorprint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/commandlineflags.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/complexity.h
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/counter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/cycleclock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/internal_macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/re.h
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/sleep.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/stat.h
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/string_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/sysinfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/src/timers.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:49:07.210255 FFHT-non-official-1.2.6/external/benchmark/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/external/benchmark/test/output_test.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fast_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fast_copy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fht-pybind11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fht.c
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fht.h
+-rw-r--r--   0 runner    (1001) docker     (123)   875212 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fht_avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fht_header_only.h
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fht_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)  1006554 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/fht_sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:49:07.214255 FFHT-non-official-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/test_double.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/test_double_header_only.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/test_float.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-19 11:48:59.000000 FFHT-non-official-1.2.6/test_float_header_only.c
```

### Comparing `FFHT-non-official-1.2.5/FFHT_non_official.egg-info/PKG-INFO` & `FFHT-non-official-1.2.6/FFHT_non_official.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFHT-non-official
-Version: 1.2.5
+Version: 1.2.6
 Summary: Fast implementation of the Fast Hadamard Transform (FHT)
 Home-page: https://github.com/FALCONN-LIB/FFHT
 Author: Ilya Razenshteyn, Ludwig Schmidt
 Author-email: falconn.lib@gmail.com
 License: MIT
 Keywords: fast Fourier Hadamard transform butterfly
 License-File: LICENSE.md
```

### Comparing `FFHT-non-official-1.2.5/LICENSE.md` & `FFHT-non-official-1.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/PKG-INFO` & `FFHT-non-official-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFHT-non-official
-Version: 1.2.5
+Version: 1.2.6
 Summary: Fast implementation of the Fast Hadamard Transform (FHT)
 Home-page: https://github.com/FALCONN-LIB/FFHT
 Author: Ilya Razenshteyn, Ludwig Schmidt
 Author-email: falconn.lib@gmail.com
 License: MIT
 Keywords: fast Fourier Hadamard transform butterfly
 License-File: LICENSE.md
```

### Comparing `FFHT-non-official-1.2.5/README.md` & `FFHT-non-official-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/include/benchmark/benchmark.h` & `FFHT-non-official-1.2.6/external/benchmark/include/benchmark/benchmark.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/include/benchmark/benchmark_api.h` & `FFHT-non-official-1.2.6/external/benchmark/include/benchmark/benchmark_api.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/include/benchmark/reporter.h` & `FFHT-non-official-1.2.6/external/benchmark/include/benchmark/reporter.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/arraysize.h` & `FFHT-non-official-1.2.6/external/benchmark/src/arraysize.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/benchmark_api_internal.h` & `FFHT-non-official-1.2.6/external/benchmark/src/benchmark_api_internal.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/check.h` & `FFHT-non-official-1.2.6/external/benchmark/src/check.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/colorprint.h` & `FFHT-non-official-1.2.6/external/benchmark/src/colorprint.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/commandlineflags.h` & `FFHT-non-official-1.2.6/external/benchmark/src/commandlineflags.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/complexity.h` & `FFHT-non-official-1.2.6/external/benchmark/src/complexity.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/counter.h` & `FFHT-non-official-1.2.6/external/benchmark/src/counter.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/cycleclock.h` & `FFHT-non-official-1.2.6/external/benchmark/src/cycleclock.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/internal_macros.h` & `FFHT-non-official-1.2.6/external/benchmark/src/internal_macros.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/log.h` & `FFHT-non-official-1.2.6/external/benchmark/src/log.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/mutex.h` & `FFHT-non-official-1.2.6/external/benchmark/src/mutex.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/re.h` & `FFHT-non-official-1.2.6/external/benchmark/src/re.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/stat.h` & `FFHT-non-official-1.2.6/external/benchmark/src/stat.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/string_util.h` & `FFHT-non-official-1.2.6/external/benchmark/src/string_util.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/src/timers.h` & `FFHT-non-official-1.2.6/external/benchmark/src/timers.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/external/benchmark/test/output_test.h` & `FFHT-non-official-1.2.6/external/benchmark/test/output_test.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/fast_copy.c` & `FFHT-non-official-1.2.6/fast_copy.c`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/fht-pybind11.cpp` & `FFHT-non-official-1.2.6/fht-pybind11.cpp`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/fht.h` & `FFHT-non-official-1.2.6/fht.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/fht_header_only.h` & `FFHT-non-official-1.2.6/fht_header_only.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/fht_impl.h` & `FFHT-non-official-1.2.6/fht_impl.h`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.5/setup.py` & `FFHT-non-official-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                                        '-Wstrict-prototypes', '-Wmissing-prototypes',
                                        '-std=c++11', '-fopenmp'],
                    extra_link_args=['-fopenmp'],
                    depends=['fast_copy.h', 'fht.h'],
                    include_dirs=[np.get_include()] + ["pybind11/include"])
 
 setup(name='FFHT-non-official',
-      version='1.2.5',
+      version='1.2.6',
       author='Ilya Razenshteyn, Ludwig Schmidt',
       author_email='falconn.lib@gmail.com',
       url='https://github.com/FALCONN-LIB/FFHT',
       description='Fast implementation of the Fast Hadamard Transform (FHT)',
       long_description=long_description,
       license='MIT',
       keywords='fast Fourier Hadamard transform butterfly',
```

