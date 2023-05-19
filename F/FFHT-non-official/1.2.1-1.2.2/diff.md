# Comparing `tmp/FFHT-non-official-1.2.1.tar.gz` & `tmp/FFHT-non-official-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFHT-non-official-1.2.1.tar", last modified: Fri May 19 11:21:44 2023, max compression
+gzip compressed data, was "FFHT-non-official-1.2.2.tar", last modified: Fri May 19 11:32:14 2023, max compression
```

## Comparing `FFHT-non-official-1.2.1.tar` & `FFHT-non-official-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:44.048530 FFHT-non-official-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:44.048530 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:21:44.000000 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-19 11:21:44.000000 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:21:44.000000 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:21:44.000000 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:21:44.048530 FFHT-non-official-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/fast_copy.c
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/fht-pybind11.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/fht.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:21:44.048530 FFHT-non-official-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:32:14.021846 FFHT-non-official-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:32:14.021846 FFHT-non-official-1.2.2/FFHT_non_official.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:32:14.000000 FFHT-non-official-1.2.2/FFHT_non_official.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-19 11:32:14.000000 FFHT-non-official-1.2.2/FFHT_non_official.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:32:14.000000 FFHT-non-official-1.2.2/FFHT_non_official.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:32:14.000000 FFHT-non-official-1.2.2/FFHT_non_official.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-19 11:32:04.000000 FFHT-non-official-1.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:32:14.021846 FFHT-non-official-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-19 11:32:04.000000 FFHT-non-official-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 11:32:04.000000 FFHT-non-official-1.2.2/fast_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-19 11:32:04.000000 FFHT-non-official-1.2.2/fht-pybind11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 11:32:04.000000 FFHT-non-official-1.2.2/fht.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:32:14.021846 FFHT-non-official-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-19 11:32:04.000000 FFHT-non-official-1.2.2/setup.py
```

### Comparing `FFHT-non-official-1.2.1/FFHT_non_official.egg-info/PKG-INFO` & `FFHT-non-official-1.2.2/FFHT_non_official.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFHT-non-official
-Version: 1.2.1
+Version: 1.2.2
 Summary: Fast implementation of the Fast Hadamard Transform (FHT)
 Home-page: https://github.com/FALCONN-LIB/FFHT
 Author: Ilya Razenshteyn, Ludwig Schmidt
 Author-email: falconn.lib@gmail.com
 License: MIT
 Keywords: fast Fourier Hadamard transform butterfly
 License-File: LICENSE.md
```

### Comparing `FFHT-non-official-1.2.1/LICENSE.md` & `FFHT-non-official-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.1/PKG-INFO` & `FFHT-non-official-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFHT-non-official
-Version: 1.2.1
+Version: 1.2.2
 Summary: Fast implementation of the Fast Hadamard Transform (FHT)
 Home-page: https://github.com/FALCONN-LIB/FFHT
 Author: Ilya Razenshteyn, Ludwig Schmidt
 Author-email: falconn.lib@gmail.com
 License: MIT
 Keywords: fast Fourier Hadamard transform butterfly
 License-File: LICENSE.md
```

### Comparing `FFHT-non-official-1.2.1/README.md` & `FFHT-non-official-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.1/fast_copy.c` & `FFHT-non-official-1.2.2/fast_copy.c`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.1/fht-pybind11.cpp` & `FFHT-non-official-1.2.2/fht-pybind11.cpp`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2.1/setup.py` & `FFHT-non-official-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,19 @@
 module = Pybind11Extension('ffht',
                    sources=["fht-pybind11.cpp", "fht.c", "fast_copy.c"],
                    extra_compile_args=['-march=native', '-O3', '-Wall', '-Wextra', '-pedantic',
                                        '-Wshadow', '-Wpointer-arith', '-Wcast-qual',
                                        '-Wstrict-prototypes', '-Wmissing-prototypes',
                                        '-std=c++11', '-fopenmp'],
                    extra_link_args=['-fopenmp'],
-                   depends=['fast_copy.h'],
+                   depends=['fast_copy.h', 'fht.h'],
                    include_dirs=[np.get_include()] + ["pybind11/include"])
 
 setup(name='FFHT-non-official',
-      version='1.2.1',
+      version='1.2.2',
       author='Ilya Razenshteyn, Ludwig Schmidt',
       author_email='falconn.lib@gmail.com',
       url='https://github.com/FALCONN-LIB/FFHT',
       description='Fast implementation of the Fast Hadamard Transform (FHT)',
       long_description=long_description,
       license='MIT',
       keywords='fast Fourier Hadamard transform butterfly',
```

