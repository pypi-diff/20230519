# Comparing `tmp/FFHT-non-official-1.2.tar.gz` & `tmp/FFHT-non-official-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFHT-non-official-1.2.tar", last modified: Fri May 19 11:17:25 2023, max compression
+gzip compressed data, was "FFHT-non-official-1.2.1.tar", last modified: Fri May 19 11:21:44 2023, max compression
```

## Comparing `FFHT-non-official-1.2.tar` & `FFHT-non-official-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:17:25.933639 FFHT-non-official-1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:17:25.933639 FFHT-non-official-1.2/FFHT_non_official.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-19 11:17:25.000000 FFHT-non-official-1.2/FFHT_non_official.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-19 11:17:25.000000 FFHT-non-official-1.2/FFHT_non_official.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:17:25.000000 FFHT-non-official-1.2/FFHT_non_official.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:17:25.000000 FFHT-non-official-1.2/FFHT_non_official.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-19 11:17:18.000000 FFHT-non-official-1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-19 11:17:25.933639 FFHT-non-official-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-19 11:17:18.000000 FFHT-non-official-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 11:17:18.000000 FFHT-non-official-1.2/fast_copy.c
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-19 11:17:18.000000 FFHT-non-official-1.2/fht-pybind11.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 11:17:18.000000 FFHT-non-official-1.2/fht.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:17:25.933639 FFHT-non-official-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-19 11:17:18.000000 FFHT-non-official-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:44.048530 FFHT-non-official-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:21:44.048530 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:21:44.000000 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-19 11:21:44.000000 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:21:44.000000 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:21:44.000000 FFHT-non-official-1.2.1/FFHT_non_official.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 11:21:44.048530 FFHT-non-official-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/fast_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/fht-pybind11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/fht.c
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:21:44.048530 FFHT-non-official-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-19 11:21:35.000000 FFHT-non-official-1.2.1/setup.py
```

### Comparing `FFHT-non-official-1.2/FFHT_non_official.egg-info/PKG-INFO` & `FFHT-non-official-1.2.1/FFHT_non_official.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFHT-non-official
-Version: 1.2
+Version: 1.2.1
 Summary: Fast implementation of the Fast Hadamard Transform (FHT)
 Home-page: https://github.com/FALCONN-LIB/FFHT
 Author: Ilya Razenshteyn, Ludwig Schmidt
 Author-email: falconn.lib@gmail.com
 License: MIT
 Keywords: fast Fourier Hadamard transform butterfly
 License-File: LICENSE.md
```

### Comparing `FFHT-non-official-1.2/LICENSE.md` & `FFHT-non-official-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2/PKG-INFO` & `FFHT-non-official-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFHT-non-official
-Version: 1.2
+Version: 1.2.1
 Summary: Fast implementation of the Fast Hadamard Transform (FHT)
 Home-page: https://github.com/FALCONN-LIB/FFHT
 Author: Ilya Razenshteyn, Ludwig Schmidt
 Author-email: falconn.lib@gmail.com
 License: MIT
 Keywords: fast Fourier Hadamard transform butterfly
 License-File: LICENSE.md
```

### Comparing `FFHT-non-official-1.2/README.md` & `FFHT-non-official-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2/fast_copy.c` & `FFHT-non-official-1.2.1/fast_copy.c`

 * *Files identical despite different names*

### Comparing `FFHT-non-official-1.2/fht-pybind11.cpp` & `FFHT-non-official-1.2.1/fht-pybind11.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include "pybind11/pybind11.h"
 #include "pybind11/numpy.h"
 #include "fht.h"
+#include "fast_copy.h"
 
 namespace py = pybind11;
 
 static constexpr inline unsigned ilog2(size_t x) noexcept {
     return __builtin_ctz(x);
 }
```

### Comparing `FFHT-non-official-1.2/setup.py` & `FFHT-non-official-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                                        '-Wstrict-prototypes', '-Wmissing-prototypes',
                                        '-std=c++11', '-fopenmp'],
                    extra_link_args=['-fopenmp'],
                    depends=['fast_copy.h'],
                    include_dirs=[np.get_include()] + ["pybind11/include"])
 
 setup(name='FFHT-non-official',
-      version='1.2',
+      version='1.2.1',
       author='Ilya Razenshteyn, Ludwig Schmidt',
       author_email='falconn.lib@gmail.com',
       url='https://github.com/FALCONN-LIB/FFHT',
       description='Fast implementation of the Fast Hadamard Transform (FHT)',
       long_description=long_description,
       license='MIT',
       keywords='fast Fourier Hadamard transform butterfly',
```

