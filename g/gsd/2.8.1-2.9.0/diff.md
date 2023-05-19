# Comparing `tmp/gsd-2.8.1.tar.gz` & `tmp/gsd-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsd-2.8.1.tar", last modified: Thu Apr 13 17:58:09 2023, max compression
+gzip compressed data, was "gsd-2.9.0.tar", last modified: Fri May 19 18:14:19 2023, max compression
```

## Comparing `gsd-2.8.1.tar` & `gsd-2.9.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:09.712750 gsd-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-13 17:58:00.000000 gsd-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 17:58:00.000000 gsd-2.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-13 17:58:09.712750 gsd-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-13 17:58:00.000000 gsd-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:09.712750 gsd-2.8.1/gsd/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   700278 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd/fl.c
--rw-r--r--   0 runner    (1001) docker     (123)    36552 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/fl.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    70351 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/gsd.c
--rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/gsd.h
--rw-r--r--   0 runner    (1001) docker     (123)    46531 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/libgsd.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/pygsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/pytest_plugin_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:09.712750 gsd-2.8.1/gsd/test/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)    34913 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/test_fl.py
--rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/test_gsd_v1.gsd
--rw-r--r--   0 runner    (1001) docker     (123)    34320 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/test_hoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/test/test_largefile.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-13 17:58:00.000000 gsd-2.8.1/gsd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:09.712750 gsd-2.8.1/gsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 17:58:09.000000 gsd-2.8.1/gsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 17:58:00.000000 gsd-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-13 17:58:09.716750 gsd-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-13 17:58:00.000000 gsd-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:14:19.489557 gsd-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-19 18:14:04.000000 gsd-2.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-19 18:14:04.000000 gsd-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-19 18:14:04.000000 gsd-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-19 18:14:19.489557 gsd-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-19 18:14:04.000000 gsd-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:14:19.485557 gsd-2.9.0/gsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   722119 2023-05-19 18:14:18.000000 gsd-2.9.0/gsd/fl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    38073 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/fl.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    70351 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/gsd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/gsd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47184 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/libgsd.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/pygsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/pytest_plugin_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:14:19.489557 gsd-2.9.0/gsd/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    34820 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/test_fl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72428 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/test_gsd_v1.gsd
+-rw-r--r--   0 runner    (1001) docker     (123)    34233 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/test_hoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/test/test_largefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-19 18:14:04.000000 gsd-2.9.0/gsd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:14:19.485557 gsd-2.9.0/gsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 18:14:19.000000 gsd-2.9.0/gsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-19 18:14:04.000000 gsd-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-19 18:14:19.489557 gsd-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-19 18:14:04.000000 gsd-2.9.0/setup.py
```

### Comparing `gsd-2.8.1/LICENSE` & `gsd-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gsd-2.8.1/PKG-INFO` & `gsd-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 2.8.1
+Version: 2.9.0
 Summary: General simulation data file format.
-Home-page: https://gsd.readthedocs.io
-Author: Joshua A. Anderson
-Author-email: joaander@umich.edu
-License: BSD - 2 clause
-Download-URL: https://github.com/glotzerlab/gsd/releases/download/v2.8.1/gsd-v2.8.1.tar.gz
+Author-email: "Joshua A. Anderson" <joaander@umich.edu>
+License: BSD-2-Clause
+Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Source Code, https://github.com/glotzerlab/gsd
-Project-URL: Issue Tracker, https://github.com/glotzerlab/gsd/issues
-Platform: UNKNOWN
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v2.9.0/gsd-v2.9.0.tar.gz
+Project-URL: Source, https://github.com/glotzerlab/gsd
+Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -48,15 +46,15 @@
 ```python
 >>> s = gsd.hoomd.Frame()
 >>> s.particles.N = 4
 >>> s.particles.types = ['A', 'B']
 >>> s.particles.typeid = [0,0,1,1]
 >>> s.particles.position = [[0,0,0],[1,1,1], [-1,-1,-1], [1,-1,-1]]
 >>> s.configuration.box = [3, 3, 3, 0, 0, 0]
->>> traj = gsd.hoomd.open(name='test.gsd', mode='wb')
+>>> traj = gsd.hoomd.open(name='test.gsd', mode='w')
 >>> traj.append(s)
 ```
 
 Append frames to a gsd file:
 ```python
 >>> def create_frame(i):
 ...     s = gsd.hoomd.Frame();
@@ -68,15 +66,15 @@
 ...     t.extend( (create_frame(i) for i in range(10)) )
 ...     print(len(t))
 11
 ```
 
 Randomly index frames:
 ```python
->>> with gsd.hoomd.open('test.gsd', 'rb') as t:
+>>> with gsd.hoomd.open('test.gsd', 'r') as t:
 ...     frame = t[5]
 ...     print(frame.configuration.step)
 4
 ...     print(frame.particles.N)
 8
 ...     print(frame.particles.position)
 [[ 0.56993282  0.42243481  0.5502916 ]
@@ -87,31 +85,29 @@
  [ 0.13724308  0.14253527  0.02505   ]
  [ 0.39287439  0.82519054  0.01613089]
  [ 0.23150323  0.95167434  0.7715748 ]]
 ```
 
 Slice frames:
 ```python
->>> with gsd.hoomd.open('test.gsd', 'rb') as t:
+>>> with gsd.hoomd.open('test.gsd', 'r') as t:
 ...     for s in t[5:-2]:
 ...         print(s.configuration.step, end=' ')
 4 5 6 7
 ```
 
 ## File layer examples
 
 ```python
-with gsd.fl.open(name='file.gsd', mode='wb') as f:
+with gsd.fl.open(name='file.gsd', mode='w') as f:
     f.write_chunk(name='position', data=numpy.array([[1,2,3],[4,5,6]], dtype=numpy.float32));
     f.write_chunk(name='angle', data=numpy.array([0, 1], dtype=numpy.float32));
     f.write_chunk(name='box', data=numpy.array([10, 10, 10], dtype=numpy.float32));
     f.end_frame()
 ```
 
 ```python
-with gsd.fl.open(name='file.gsd', mode='rb') as f:
+with gsd.fl.open(name='file.gsd', mode='r') as f:
     for i in range(1,f.nframes):
         position = f.read_chunk(frame=i, name='position');
         do_something(position);
 ```
-
-
```

### Comparing `gsd-2.8.1/README.md` & `gsd-2.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ```python
 >>> s = gsd.hoomd.Frame()
 >>> s.particles.N = 4
 >>> s.particles.types = ['A', 'B']
 >>> s.particles.typeid = [0,0,1,1]
 >>> s.particles.position = [[0,0,0],[1,1,1], [-1,-1,-1], [1,-1,-1]]
 >>> s.configuration.box = [3, 3, 3, 0, 0, 0]
->>> traj = gsd.hoomd.open(name='test.gsd', mode='wb')
+>>> traj = gsd.hoomd.open(name='test.gsd', mode='w')
 >>> traj.append(s)
 ```
 
 Append frames to a gsd file:
 ```python
 >>> def create_frame(i):
 ...     s = gsd.hoomd.Frame();
@@ -44,15 +44,15 @@
 ...     t.extend( (create_frame(i) for i in range(10)) )
 ...     print(len(t))
 11
 ```
 
 Randomly index frames:
 ```python
->>> with gsd.hoomd.open('test.gsd', 'rb') as t:
+>>> with gsd.hoomd.open('test.gsd', 'r') as t:
 ...     frame = t[5]
 ...     print(frame.configuration.step)
 4
 ...     print(frame.particles.N)
 8
 ...     print(frame.particles.position)
 [[ 0.56993282  0.42243481  0.5502916 ]
@@ -63,29 +63,29 @@
  [ 0.13724308  0.14253527  0.02505   ]
  [ 0.39287439  0.82519054  0.01613089]
  [ 0.23150323  0.95167434  0.7715748 ]]
 ```
 
 Slice frames:
 ```python
->>> with gsd.hoomd.open('test.gsd', 'rb') as t:
+>>> with gsd.hoomd.open('test.gsd', 'r') as t:
 ...     for s in t[5:-2]:
 ...         print(s.configuration.step, end=' ')
 4 5 6 7
 ```
 
 ## File layer examples
 
 ```python
-with gsd.fl.open(name='file.gsd', mode='wb') as f:
+with gsd.fl.open(name='file.gsd', mode='w') as f:
     f.write_chunk(name='position', data=numpy.array([[1,2,3],[4,5,6]], dtype=numpy.float32));
     f.write_chunk(name='angle', data=numpy.array([0, 1], dtype=numpy.float32));
     f.write_chunk(name='box', data=numpy.array([10, 10, 10], dtype=numpy.float32));
     f.end_frame()
 ```
 
 ```python
-with gsd.fl.open(name='file.gsd', mode='rb') as f:
+with gsd.fl.open(name='file.gsd', mode='r') as f:
     for i in range(1,f.nframes):
         position = f.read_chunk(frame=i, name='position');
         do_something(position);
 ```
```

### Comparing `gsd-2.8.1/gsd/__init__.py` & `gsd-2.9.0/gsd/__init__.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.1/gsd/__main__.py` & `gsd-2.9.0/gsd/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         handle = traj.file
         local_ns.update({
             'handle': handle,
             'traj': traj,
         })
         attributes.update({"Number of frames": len(traj)})
     else:
-        if args.mode not in ['rb', 'rb+', 'ab']:
+        if args.mode not in ['rb', 'rb+', 'ab', 'a', 'r', 'r+']:
             raise ValueError("Unsupported schema for creating a file.")
         handle = fl.open(args.file, args.mode)
         local_ns.update({
             'handle': handle,
         })
 
     extras = "\n".join(
@@ -112,21 +112,33 @@
                              help="GSD file to read.")
     parser_read.add_argument('-s',
                              '--schema',
                              type=str,
                              default='hoomd',
                              choices=['hoomd', 'none'],
                              help="The file schema.")
-    parser_read.add_argument(
-        '-m',
-        '--mode',
-        type=str,
-        default='rb',
-        choices=['rb', 'rb+', 'wb', 'wb+', 'xb', 'xb+', 'ab'],
-        help="The file mode.")
+    parser_read.add_argument('-m',
+                             '--mode',
+                             type=str,
+                             default='r',
+                             choices=[
+                                 'rb',
+                                 'rb+',
+                                 'wb',
+                                 'wb+',
+                                 'xb',
+                                 'xb+',
+                                 'ab',
+                                 'w',
+                                 'r',
+                                 'r+',
+                                 'x',
+                                 'a',
+                             ],
+                             help="The file mode.")
     parser_read.set_defaults(func=main_read)
 
     # This is a hack, as argparse itself does not
     # allow to parse only --version without any
     # of the other required arguments.
     if '--version' in sys.argv:
         print('gsd', __version__)
```

### Comparing `gsd-2.8.1/gsd/fl.c` & `gsd-2.9.0/gsd/fl.c`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "gsd/gsd.h"
         ],
         "include_dirs": [
             "./gsd",
-            "/opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/core/include"
+            "/tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "gsd.fl",
         "sources": [
             "gsd/fl.pyx",
             "gsd/gsd.c"
         ]
     },
@@ -1065,195 +1065,195 @@
 
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1281,51 +1281,51 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_3gsd_2fl_GSDFile;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "gsd/fl.pyx":239
+/* "gsd/fl.pyx":251
  * 
  * 
  * cdef class GSDFile:             # <<<<<<<<<<<<<<
  *     """GSDFile
  * 
  */
 struct __pyx_obj_3gsd_2fl_GSDFile {
@@ -2034,35 +2034,43 @@
 extern int __pyx_module_is_main_gsd__fl;
 int __pyx_module_is_main_gsd__fl = 0;
 
 /* Implementation of 'gsd.fl' */
 static PyObject *__pyx_builtin_IOError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_MemoryError;
+static PyObject *__pyx_builtin_FutureWarning;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_KeyError;
 static PyObject *__pyx_builtin_ImportError;
-static const char __pyx_k__6[] = " - ";
+static const char __pyx_k_a[] = "a";
+static const char __pyx_k_r[] = "r";
+static const char __pyx_k_w[] = "w";
+static const char __pyx_k_x[] = "x";
 static const char __pyx_k_ab[] = "ab";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_wb[] = "wb";
 static const char __pyx_k_xb[] = "xb";
+static const char __pyx_k__12[] = " - ";
+static const char __pyx_k_r_2[] = "r+";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_file[] = "file ";
 static const char __pyx_k_info[] = "info";
 static const char __pyx_k_int8[] = "int8";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_open[] = "open";
+static const char __pyx_k_path[] = "path";
 static const char __pyx_k_rb_2[] = "rb+";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_view[] = "view";
+static const char __pyx_k_warn[] = "warn";
 static const char __pyx_k_wb_2[] = "wb+";
 static const char __pyx_k_xb_2[] = "xb+";
 static const char __pyx_k_chunk[] = " / chunk ";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_debug[] = "debug";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
@@ -2071,14 +2079,15 @@
 static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_int64[] = "int64";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_uint8[] = "uint8";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_encode[] = "encode";
+static const char __pyx_k_exists[] = "exists";
 static const char __pyx_k_gsd_fl[] = "gsd.fl";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_logger[] = "logger";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_schema[] = "schema";
 static const char __pyx_k_uint16[] = "uint16";
@@ -2092,32 +2101,35 @@
 static const char __pyx_k_logging[] = "logging";
 static const char __pyx_k_reshape[] = "reshape";
 static const char __pyx_k_warning[] = "warning";
 static const char __pyx_k_KeyError[] = "KeyError";
 static const char __pyx_k_exc_type[] = "exc_type";
 static const char __pyx_k_schema_2[] = ", schema: ";
 static const char __pyx_k_strerror[] = "strerror";
+static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_end_frame[] = "end frame: ";
 static const char __pyx_k_exc_value[] = "exc_value";
 static const char __pyx_k_getLogger[] = "getLogger";
 static const char __pyx_k_traceback[] = "traceback";
 static const char __pyx_k_with_mode[] = " with mode: ";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_gsd_fl_pyx[] = "gsd/fl.pyx";
 static const char __pyx_k_read_chunk[] = "read chunk: ";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_application[] = "application";
 static const char __pyx_k_write_chunk[] = "write chunk: ";
+static const char __pyx_k_Invalid_mode[] = "Invalid mode: ";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_chunk_exists[] = "chunk exists: ";
 static const char __pyx_k_closing_file[] = "closing file: ";
 static const char __pyx_k_not_found_in[] = " not found in: ";
 static const char __pyx_k_opening_file[] = "opening file: ";
+static const char __pyx_k_FutureWarning[] = "FutureWarning";
 static const char __pyx_k_Unknown_error[] = "Unknown error: ";
 static const char __pyx_k_application_2[] = ", application: ";
 static const char __pyx_k_Not_a_GSD_file[] = "Not a GSD file: ";
 static const char __pyx_k_schema_version[] = "schema_version";
 static const char __pyx_k_upgrading_file[] = "upgrading file: ";
 static const char __pyx_k_truncating_file[] = "truncating file: ";
 static const char __pyx_k_Corrupt_GSD_file[] = "Corrupt GSD file: ";
@@ -2130,48 +2142,64 @@
 static const char __pyx_k_Invalid_gsd_argument[] = "Invalid gsd argument: ";
 static const char __pyx_k_has_incorrect_schema[] = " has incorrect schema: ";
 static const char __pyx_k_File_must_be_readable[] = "File must be readable: ";
 static const char __pyx_k_File_must_be_writable[] = "File must be writable: ";
 static const char __pyx_k_invalid_type_for_chunk[] = "invalid type for chunk: ";
 static const char __pyx_k_Memory_allocation_failed[] = "Memory allocation failed: ";
 static const char __pyx_k_Unsupported_GSD_file_version[] = "Unsupported GSD file version: ";
+static const char __pyx_k_The_ab_mode_is_deprecated_use_r[] = "The 'ab' mode is deprecated, use 'r+'";
+static const char __pyx_k_The_rb_mode_is_deprecated_use_r[] = "The 'rb' mode is deprecated, use 'r'";
+static const char __pyx_k_The_wb_mode_is_deprecated_use_w[] = "The 'wb' mode is deprecated, use 'w'";
+static const char __pyx_k_The_xb_mode_is_deprecated_use_x[] = "The 'xb' mode is deprecated, use 'x'";
 static const char __pyx_k_implicit_data_copy_when_writing[] = "implicit data copy when writing chunk: ";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_GSD_can_only_write_1_or_2_dimens[] = "GSD can only write 1 or 2 dimensional arrays: ";
 static const char __pyx_k_GSD_file_layer_API_Low_level_acc[] = "GSD file layer API.\n\nLow level access to gsd files. :py:mod:`gsd.fl` allows direct access to create,\nread, and write ``gsd`` files. The module is implemented in C and is optimized.\nSee :ref:`fl-examples` for detailed example code.\n\n* :py:class:`GSDFile` - Class interface to read and write gsd files.\n* :py:func:`open` - Open a gsd file.\n\n";
 static const char __pyx_k_Only_read_only_GSDFiles_can_be_p[] = "Only read only GSDFiles can be pickled.";
 static const char __pyx_k_Provide_application_when_creatin[] = "Provide application when creating a file";
 static const char __pyx_k_Provide_schema_version_when_crea[] = "Provide schema_version when creating a file";
 static const char __pyx_k_Provide_schema_when_creating_a_f[] = "Provide schema when creating a file";
-static const char __pyx_k_mode_must_be_wb_wb_rb_rb_xb_xb_o[] = "mode must be 'wb', 'wb+', 'rb', 'rb+', 'xb', 'xb+', or 'ab'";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
+static const char __pyx_k_The_rb_mode_is_deprecated_use_r_2[] = "The 'rb+' mode is deprecated, use 'r+'";
+static const char __pyx_k_The_wb_mode_is_deprecated_use_w_2[] = "The 'wb+' mode is deprecated, use 'w'";
+static const char __pyx_k_The_xb_mode_is_deprecated_use_x_2[] = "The 'xb+' mode is deprecated, use 'x'";
 static PyObject *__pyx_kp_u_Corrupt_GSD_file;
 static PyObject *__pyx_kp_u_File_is_not_open;
 static PyObject *__pyx_kp_u_File_must_be_readable;
 static PyObject *__pyx_kp_u_File_must_be_writable;
+static PyObject *__pyx_n_s_FutureWarning;
 static PyObject *__pyx_n_s_GSDFile;
 static PyObject *__pyx_kp_u_GSD_can_only_write_1_or_2_dimens;
 static PyObject *__pyx_kp_u_GSD_namelist_is_full;
 static PyObject *__pyx_n_s_IOError;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_u_Invalid_gsd_argument;
+static PyObject *__pyx_kp_u_Invalid_mode;
 static PyObject *__pyx_n_s_KeyError;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_u_Memory_allocation_failed;
 static PyObject *__pyx_kp_u_Not_a_GSD_file;
 static PyObject *__pyx_kp_u_Only_read_only_GSDFiles_can_be_p;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_kp_u_Provide_application_when_creatin;
 static PyObject *__pyx_kp_u_Provide_schema_version_when_crea;
 static PyObject *__pyx_kp_u_Provide_schema_when_creating_a_f;
 static PyObject *__pyx_n_s_RuntimeError;
+static PyObject *__pyx_kp_u_The_ab_mode_is_deprecated_use_r;
+static PyObject *__pyx_kp_u_The_rb_mode_is_deprecated_use_r;
+static PyObject *__pyx_kp_u_The_rb_mode_is_deprecated_use_r_2;
+static PyObject *__pyx_kp_u_The_wb_mode_is_deprecated_use_w;
+static PyObject *__pyx_kp_u_The_wb_mode_is_deprecated_use_w_2;
+static PyObject *__pyx_kp_u_The_xb_mode_is_deprecated_use_x;
+static PyObject *__pyx_kp_u_The_xb_mode_is_deprecated_use_x_2;
 static PyObject *__pyx_kp_u_Unknown_error;
 static PyObject *__pyx_kp_u_Unsupported_GSD_file_version;
 static PyObject *__pyx_n_s_ValueError;
-static PyObject *__pyx_kp_u__6;
+static PyObject *__pyx_kp_u__12;
+static PyObject *__pyx_n_u_a;
 static PyObject *__pyx_n_u_ab;
 static PyObject *__pyx_kp_u_and_schema_version;
 static PyObject *__pyx_n_s_application;
 static PyObject *__pyx_kp_u_application_2;
 static PyObject *__pyx_n_s_ascontiguousarray;
 static PyObject *__pyx_kp_u_chunk;
 static PyObject *__pyx_kp_u_chunk_exists;
@@ -2182,14 +2210,15 @@
 static PyObject *__pyx_n_s_debug;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_empty;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_kp_u_end_frame;
 static PyObject *__pyx_n_s_exc_type;
 static PyObject *__pyx_n_s_exc_value;
+static PyObject *__pyx_n_s_exists;
 static PyObject *__pyx_kp_u_file;
 static PyObject *__pyx_n_s_float32;
 static PyObject *__pyx_n_s_float64;
 static PyObject *__pyx_n_s_frame;
 static PyObject *__pyx_kp_u_frame_2;
 static PyObject *__pyx_n_s_getLogger;
 static PyObject *__pyx_n_s_gsd_fl;
@@ -2204,26 +2233,28 @@
 static PyObject *__pyx_n_s_int64;
 static PyObject *__pyx_n_s_int8;
 static PyObject *__pyx_kp_u_invalid_type_for_chunk;
 static PyObject *__pyx_n_s_logger;
 static PyObject *__pyx_n_s_logging;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_mode;
-static PyObject *__pyx_kp_u_mode_must_be_wb_wb_rb_rb_xb_xb_o;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_kp_u_not_found_in;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_open;
 static PyObject *__pyx_kp_u_opening_file;
 static PyObject *__pyx_n_s_os;
 static PyObject *__pyx_kp_u_overwriting_file;
+static PyObject *__pyx_n_s_path;
 static PyObject *__pyx_n_s_pickle;
+static PyObject *__pyx_n_u_r;
+static PyObject *__pyx_kp_u_r_2;
 static PyObject *__pyx_n_u_rb;
 static PyObject *__pyx_kp_u_rb_2;
 static PyObject *__pyx_kp_u_read_chunk;
 static PyObject *__pyx_n_s_reshape;
 static PyObject *__pyx_n_s_schema;
 static PyObject *__pyx_kp_u_schema_2;
 static PyObject *__pyx_n_s_schema_version;
@@ -2236,19 +2267,23 @@
 static PyObject *__pyx_n_s_uint16;
 static PyObject *__pyx_n_s_uint32;
 static PyObject *__pyx_n_s_uint64;
 static PyObject *__pyx_n_s_uint8;
 static PyObject *__pyx_kp_u_upgrading_file;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_view;
+static PyObject *__pyx_n_u_w;
+static PyObject *__pyx_n_s_warn;
 static PyObject *__pyx_n_s_warning;
+static PyObject *__pyx_n_s_warnings;
 static PyObject *__pyx_n_u_wb;
 static PyObject *__pyx_kp_u_wb_2;
 static PyObject *__pyx_kp_u_with_mode;
 static PyObject *__pyx_kp_u_write_chunk;
+static PyObject *__pyx_n_u_x;
 static PyObject *__pyx_n_u_xb;
 static PyObject *__pyx_kp_u_xb_2;
 static PyObject *__pyx_pf_3gsd_2fl_open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name, PyObject *__pyx_v_mode, PyObject *__pyx_v_application, PyObject *__pyx_v_schema, PyObject *__pyx_v_schema_version); /* proto */
 static int __pyx_pf_3gsd_2fl_7GSDFile___init__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_mode, PyObject *__pyx_v_application, PyObject *__pyx_v_schema, PyObject *__pyx_v_schema_version); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_2close(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4truncate(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_6end_frame(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self); /* proto */
@@ -2272,22 +2307,28 @@
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_codeobj__11;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__14;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__16;
+static PyObject *__pyx_codeobj__17;
 /* Late includes */
 
-/* "gsd/fl.pyx":30
+/* "gsd/fl.pyx":31
  * # Helper functions #
  * 
  * cdef __format_errno(fname):             # <<<<<<<<<<<<<<
  *     """Return a tuple for constructing an IOError."""
  *     return (errno, os.strerror(errno), fname)
  */
 
@@ -2300,63 +2341,63 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__format_errno", 0);
 
-  /* "gsd/fl.pyx":32
+  /* "gsd/fl.pyx":33
  * cdef __format_errno(fname):
  *     """Return a tuple for constructing an IOError."""
  *     return (errno, os.strerror(errno), fname)             # <<<<<<<<<<<<<<
  * 
  * cdef __raise_on_error(retval, extra):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(errno); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(errno); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strerror); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strerror); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(errno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(errno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_v_fname);
   __Pyx_GIVEREF(__pyx_v_fname);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_fname);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":30
+  /* "gsd/fl.pyx":31
  * # Helper functions #
  * 
  * cdef __format_errno(fname):             # <<<<<<<<<<<<<<
  *     """Return a tuple for constructing an IOError."""
  *     return (errno, os.strerror(errno), fname)
  */
 
@@ -2371,15 +2412,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":34
+/* "gsd/fl.pyx":35
  *     return (errno, os.strerror(errno), fname)
  * 
  * cdef __raise_on_error(retval, extra):             # <<<<<<<<<<<<<<
  *     """Raise the appropriate error type.
  * 
  */
 
@@ -2390,416 +2431,416 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__raise_on_error", 0);
 
-  /* "gsd/fl.pyx":41
+  /* "gsd/fl.pyx":42
  *         extra: Extra string to pass along with the exception
  *     """
  *     if retval == libgsd.GSD_ERROR_IO:             # <<<<<<<<<<<<<<
  *         raise IOError(*__format_errno(extra))
  *     elif retval == libgsd.GSD_ERROR_NOT_A_GSD_FILE:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_IO); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_IO); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":42
+    /* "gsd/fl.pyx":43
  *     """
  *     if retval == libgsd.GSD_ERROR_IO:
  *         raise IOError(*__format_errno(extra))             # <<<<<<<<<<<<<<
  *     elif retval == libgsd.GSD_ERROR_NOT_A_GSD_FILE:
  *         raise RuntimeError("Not a GSD file: " + extra)
  */
-    __pyx_t_2 = __pyx_f_3gsd_2fl___format_errno(__pyx_v_extra); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_3gsd_2fl___format_errno(__pyx_v_extra); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PySequence_Tuple(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PySequence_Tuple(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_IOError, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_IOError, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 42, __pyx_L1_error)
+    __PYX_ERR(0, 43, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":41
+    /* "gsd/fl.pyx":42
  *         extra: Extra string to pass along with the exception
  *     """
  *     if retval == libgsd.GSD_ERROR_IO:             # <<<<<<<<<<<<<<
  *         raise IOError(*__format_errno(extra))
  *     elif retval == libgsd.GSD_ERROR_NOT_A_GSD_FILE:
  */
   }
 
-  /* "gsd/fl.pyx":43
+  /* "gsd/fl.pyx":44
  *     if retval == libgsd.GSD_ERROR_IO:
  *         raise IOError(*__format_errno(extra))
  *     elif retval == libgsd.GSD_ERROR_NOT_A_GSD_FILE:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Not a GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_GSD_FILE_VERSION:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_NOT_A_GSD_FILE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_NOT_A_GSD_FILE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":44
+    /* "gsd/fl.pyx":45
  *         raise IOError(*__format_errno(extra))
  *     elif retval == libgsd.GSD_ERROR_NOT_A_GSD_FILE:
  *         raise RuntimeError("Not a GSD file: " + extra)             # <<<<<<<<<<<<<<
  *     elif retval == libgsd.GSD_ERROR_INVALID_GSD_FILE_VERSION:
  *         raise RuntimeError("Unsupported GSD file version: " + extra)
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Not_a_GSD_file, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Not_a_GSD_file, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 44, __pyx_L1_error)
+    __PYX_ERR(0, 45, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":43
+    /* "gsd/fl.pyx":44
  *     if retval == libgsd.GSD_ERROR_IO:
  *         raise IOError(*__format_errno(extra))
  *     elif retval == libgsd.GSD_ERROR_NOT_A_GSD_FILE:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Not a GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_GSD_FILE_VERSION:
  */
   }
 
-  /* "gsd/fl.pyx":45
+  /* "gsd/fl.pyx":46
  *     elif retval == libgsd.GSD_ERROR_NOT_A_GSD_FILE:
  *         raise RuntimeError("Not a GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_GSD_FILE_VERSION:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Unsupported GSD file version: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_CORRUPT:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_INVALID_GSD_FILE_VERSION); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_INVALID_GSD_FILE_VERSION); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":46
+    /* "gsd/fl.pyx":47
  *         raise RuntimeError("Not a GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_GSD_FILE_VERSION:
  *         raise RuntimeError("Unsupported GSD file version: " + extra)             # <<<<<<<<<<<<<<
  *     elif retval == libgsd.GSD_ERROR_FILE_CORRUPT:
  *         raise RuntimeError("Corrupt GSD file: " + extra)
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Unsupported_GSD_file_version, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Unsupported_GSD_file_version, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 46, __pyx_L1_error)
+    __PYX_ERR(0, 47, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":45
+    /* "gsd/fl.pyx":46
  *     elif retval == libgsd.GSD_ERROR_NOT_A_GSD_FILE:
  *         raise RuntimeError("Not a GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_GSD_FILE_VERSION:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Unsupported GSD file version: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_CORRUPT:
  */
   }
 
-  /* "gsd/fl.pyx":47
+  /* "gsd/fl.pyx":48
  *     elif retval == libgsd.GSD_ERROR_INVALID_GSD_FILE_VERSION:
  *         raise RuntimeError("Unsupported GSD file version: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_CORRUPT:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Corrupt GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_MEMORY_ALLOCATION_FAILED:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_FILE_CORRUPT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_FILE_CORRUPT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":48
+    /* "gsd/fl.pyx":49
  *         raise RuntimeError("Unsupported GSD file version: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_CORRUPT:
  *         raise RuntimeError("Corrupt GSD file: " + extra)             # <<<<<<<<<<<<<<
  *     elif retval == libgsd.GSD_ERROR_MEMORY_ALLOCATION_FAILED:
  *         raise MemoryError("Memory allocation failed: " + extra)
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Corrupt_GSD_file, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Corrupt_GSD_file, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 48, __pyx_L1_error)
+    __PYX_ERR(0, 49, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":47
+    /* "gsd/fl.pyx":48
  *     elif retval == libgsd.GSD_ERROR_INVALID_GSD_FILE_VERSION:
  *         raise RuntimeError("Unsupported GSD file version: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_CORRUPT:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Corrupt GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_MEMORY_ALLOCATION_FAILED:
  */
   }
 
-  /* "gsd/fl.pyx":49
+  /* "gsd/fl.pyx":50
  *     elif retval == libgsd.GSD_ERROR_FILE_CORRUPT:
  *         raise RuntimeError("Corrupt GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_MEMORY_ALLOCATION_FAILED:             # <<<<<<<<<<<<<<
  *         raise MemoryError("Memory allocation failed: " + extra)
  *     elif retval == libgsd.GSD_ERROR_NAMELIST_FULL:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_MEMORY_ALLOCATION_FAILED); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_MEMORY_ALLOCATION_FAILED); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":50
+    /* "gsd/fl.pyx":51
  *         raise RuntimeError("Corrupt GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_MEMORY_ALLOCATION_FAILED:
  *         raise MemoryError("Memory allocation failed: " + extra)             # <<<<<<<<<<<<<<
  *     elif retval == libgsd.GSD_ERROR_NAMELIST_FULL:
  *         raise RuntimeError("GSD namelist is full: " + extra)
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Memory_allocation_failed, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Memory_allocation_failed, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_MemoryError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 50, __pyx_L1_error)
+    __PYX_ERR(0, 51, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":49
+    /* "gsd/fl.pyx":50
  *     elif retval == libgsd.GSD_ERROR_FILE_CORRUPT:
  *         raise RuntimeError("Corrupt GSD file: " + extra)
  *     elif retval == libgsd.GSD_ERROR_MEMORY_ALLOCATION_FAILED:             # <<<<<<<<<<<<<<
  *         raise MemoryError("Memory allocation failed: " + extra)
  *     elif retval == libgsd.GSD_ERROR_NAMELIST_FULL:
  */
   }
 
-  /* "gsd/fl.pyx":51
+  /* "gsd/fl.pyx":52
  *     elif retval == libgsd.GSD_ERROR_MEMORY_ALLOCATION_FAILED:
  *         raise MemoryError("Memory allocation failed: " + extra)
  *     elif retval == libgsd.GSD_ERROR_NAMELIST_FULL:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("GSD namelist is full: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_WRITABLE:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_NAMELIST_FULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_NAMELIST_FULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":52
+    /* "gsd/fl.pyx":53
  *         raise MemoryError("Memory allocation failed: " + extra)
  *     elif retval == libgsd.GSD_ERROR_NAMELIST_FULL:
  *         raise RuntimeError("GSD namelist is full: " + extra)             # <<<<<<<<<<<<<<
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_WRITABLE:
  *         raise RuntimeError("File must be writable: " + extra)
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_GSD_namelist_is_full, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_GSD_namelist_is_full, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 52, __pyx_L1_error)
+    __PYX_ERR(0, 53, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":51
+    /* "gsd/fl.pyx":52
  *     elif retval == libgsd.GSD_ERROR_MEMORY_ALLOCATION_FAILED:
  *         raise MemoryError("Memory allocation failed: " + extra)
  *     elif retval == libgsd.GSD_ERROR_NAMELIST_FULL:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("GSD namelist is full: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_WRITABLE:
  */
   }
 
-  /* "gsd/fl.pyx":53
+  /* "gsd/fl.pyx":54
  *     elif retval == libgsd.GSD_ERROR_NAMELIST_FULL:
  *         raise RuntimeError("GSD namelist is full: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_WRITABLE:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("File must be writable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_READABLE:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_FILE_MUST_BE_WRITABLE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_FILE_MUST_BE_WRITABLE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":54
+    /* "gsd/fl.pyx":55
  *         raise RuntimeError("GSD namelist is full: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_WRITABLE:
  *         raise RuntimeError("File must be writable: " + extra)             # <<<<<<<<<<<<<<
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_READABLE:
  *         raise RuntimeError("File must be readable: " + extra)
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_File_must_be_writable, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_File_must_be_writable, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 54, __pyx_L1_error)
+    __PYX_ERR(0, 55, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":53
+    /* "gsd/fl.pyx":54
  *     elif retval == libgsd.GSD_ERROR_NAMELIST_FULL:
  *         raise RuntimeError("GSD namelist is full: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_WRITABLE:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("File must be writable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_READABLE:
  */
   }
 
-  /* "gsd/fl.pyx":55
+  /* "gsd/fl.pyx":56
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_WRITABLE:
  *         raise RuntimeError("File must be writable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_READABLE:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("File must be readable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_ARGUMENT:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_FILE_MUST_BE_READABLE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_FILE_MUST_BE_READABLE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":56
+    /* "gsd/fl.pyx":57
  *         raise RuntimeError("File must be writable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_READABLE:
  *         raise RuntimeError("File must be readable: " + extra)             # <<<<<<<<<<<<<<
  *     elif retval == libgsd.GSD_ERROR_INVALID_ARGUMENT:
  *         raise RuntimeError("Invalid gsd argument: " + extra)
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_File_must_be_readable, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_File_must_be_readable, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 56, __pyx_L1_error)
+    __PYX_ERR(0, 57, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":55
+    /* "gsd/fl.pyx":56
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_WRITABLE:
  *         raise RuntimeError("File must be writable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_READABLE:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("File must be readable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_ARGUMENT:
  */
   }
 
-  /* "gsd/fl.pyx":57
+  /* "gsd/fl.pyx":58
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_READABLE:
  *         raise RuntimeError("File must be readable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_ARGUMENT:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Invalid gsd argument: " + extra)
  *     elif retval != 0:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_INVALID_ARGUMENT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__gsd_error(GSD_ERROR_INVALID_ARGUMENT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_retval, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":58
+    /* "gsd/fl.pyx":59
  *         raise RuntimeError("File must be readable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_ARGUMENT:
  *         raise RuntimeError("Invalid gsd argument: " + extra)             # <<<<<<<<<<<<<<
  *     elif retval != 0:
  *         raise RuntimeError("Unknown error: " + extra)
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Invalid_gsd_argument, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Invalid_gsd_argument, __pyx_v_extra); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 58, __pyx_L1_error)
+    __PYX_ERR(0, 59, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":57
+    /* "gsd/fl.pyx":58
  *     elif retval == libgsd.GSD_ERROR_FILE_MUST_BE_READABLE:
  *         raise RuntimeError("File must be readable: " + extra)
  *     elif retval == libgsd.GSD_ERROR_INVALID_ARGUMENT:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Invalid gsd argument: " + extra)
  *     elif retval != 0:
  */
   }
 
-  /* "gsd/fl.pyx":59
+  /* "gsd/fl.pyx":60
  *     elif retval == libgsd.GSD_ERROR_INVALID_ARGUMENT:
  *         raise RuntimeError("Invalid gsd argument: " + extra)
  *     elif retval != 0:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Unknown error: " + extra)
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_v_retval, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_v_retval, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":60
+    /* "gsd/fl.pyx":61
  *         raise RuntimeError("Invalid gsd argument: " + extra)
  *     elif retval != 0:
  *         raise RuntimeError("Unknown error: " + extra)             # <<<<<<<<<<<<<<
  * 
  * # Getter methods for 2D numpy arrays of all supported types
  */
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_Unknown_error, __pyx_v_extra); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_Unknown_error, __pyx_v_extra); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 60, __pyx_L1_error)
+    __PYX_ERR(0, 61, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":59
+    /* "gsd/fl.pyx":60
  *     elif retval == libgsd.GSD_ERROR_INVALID_ARGUMENT:
  *         raise RuntimeError("Invalid gsd argument: " + extra)
  *     elif retval != 0:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Unknown error: " + extra)
  * 
  */
   }
 
-  /* "gsd/fl.pyx":34
+  /* "gsd/fl.pyx":35
  *     return (errno, os.strerror(errno), fname)
  * 
  * cdef __raise_on_error(retval, extra):             # <<<<<<<<<<<<<<
  *     """Raise the appropriate error type.
  * 
  */
 
@@ -2813,15 +2854,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":67
+/* "gsd/fl.pyx":68
  * # from the read and write routines
  * 
  * cdef void * __get_ptr_uint8(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[uint8_t, ndim=2, mode="c"] data_array_uint8
  *     data_array_uint8 = data
  */
 
@@ -2845,22 +2886,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_uint8", 0);
   __pyx_pybuffer_data_array_uint8.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_uint8.refcount = 0;
   __pyx_pybuffernd_data_array_uint8.data = NULL;
   __pyx_pybuffernd_data_array_uint8.rcbuffer = &__pyx_pybuffer_data_array_uint8;
 
-  /* "gsd/fl.pyx":69
+  /* "gsd/fl.pyx":70
  * cdef void * __get_ptr_uint8(data):
  *     cdef numpy.ndarray[uint8_t, ndim=2, mode="c"] data_array_uint8
  *     data_array_uint8 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 70, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_uint8.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_uint8.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint8_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -2870,55 +2911,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_uint8.diminfo[0].strides = __pyx_pybuffernd_data_array_uint8.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_uint8.diminfo[0].shape = __pyx_pybuffernd_data_array_uint8.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_uint8.diminfo[1].strides = __pyx_pybuffernd_data_array_uint8.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_uint8.diminfo[1].shape = __pyx_pybuffernd_data_array_uint8.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 69, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
   }
   __pyx_v_data_array_uint8 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":70
+  /* "gsd/fl.pyx":71
  *     cdef numpy.ndarray[uint8_t, ndim=2, mode="c"] data_array_uint8
  *     data_array_uint8 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":71
+    /* "gsd/fl.pyx":72
  *     data_array_uint8 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_uint8[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":70
+    /* "gsd/fl.pyx":71
  *     cdef numpy.ndarray[uint8_t, ndim=2, mode="c"] data_array_uint8
  *     data_array_uint8 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":73
+  /* "gsd/fl.pyx":74
  *         return NULL
  *     else:
  *         return <void*>&data_array_uint8[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_uint16(data):
  */
   /*else*/ {
@@ -2931,21 +2972,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_uint8.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_uint8.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_uint8.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 73, __pyx_L1_error)
+      __PYX_ERR(0, 74, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(uint8_t *, __pyx_pybuffernd_data_array_uint8.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_uint8.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_uint8.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":67
+  /* "gsd/fl.pyx":68
  * # from the read and write routines
  * 
  * cdef void * __get_ptr_uint8(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[uint8_t, ndim=2, mode="c"] data_array_uint8
  *     data_array_uint8 = data
  */
 
@@ -2966,15 +3007,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_uint8.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_uint8);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":75
+/* "gsd/fl.pyx":76
  *         return <void*>&data_array_uint8[0, 0]
  * 
  * cdef void * __get_ptr_uint16(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[uint16_t, ndim=2, mode="c"] data_array_uint16
  *     data_array_uint16 = data
  */
 
@@ -2998,22 +3039,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_uint16", 0);
   __pyx_pybuffer_data_array_uint16.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_uint16.refcount = 0;
   __pyx_pybuffernd_data_array_uint16.data = NULL;
   __pyx_pybuffernd_data_array_uint16.rcbuffer = &__pyx_pybuffer_data_array_uint16;
 
-  /* "gsd/fl.pyx":77
+  /* "gsd/fl.pyx":78
  * cdef void * __get_ptr_uint16(data):
  *     cdef numpy.ndarray[uint16_t, ndim=2, mode="c"] data_array_uint16
  *     data_array_uint16 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 78, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_uint16.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_uint16.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint16_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -3023,55 +3064,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_uint16.diminfo[0].strides = __pyx_pybuffernd_data_array_uint16.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_uint16.diminfo[0].shape = __pyx_pybuffernd_data_array_uint16.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_uint16.diminfo[1].strides = __pyx_pybuffernd_data_array_uint16.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_uint16.diminfo[1].shape = __pyx_pybuffernd_data_array_uint16.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 77, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 78, __pyx_L1_error)
   }
   __pyx_v_data_array_uint16 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":78
+  /* "gsd/fl.pyx":79
  *     cdef numpy.ndarray[uint16_t, ndim=2, mode="c"] data_array_uint16
  *     data_array_uint16 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":79
+    /* "gsd/fl.pyx":80
  *     data_array_uint16 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_uint16[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":78
+    /* "gsd/fl.pyx":79
  *     cdef numpy.ndarray[uint16_t, ndim=2, mode="c"] data_array_uint16
  *     data_array_uint16 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":81
+  /* "gsd/fl.pyx":82
  *         return NULL
  *     else:
  *         return <void*>&data_array_uint16[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_uint32(data):
  */
   /*else*/ {
@@ -3084,21 +3125,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_uint16.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_uint16.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_uint16.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 81, __pyx_L1_error)
+      __PYX_ERR(0, 82, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(uint16_t *, __pyx_pybuffernd_data_array_uint16.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_uint16.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_uint16.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":75
+  /* "gsd/fl.pyx":76
  *         return <void*>&data_array_uint8[0, 0]
  * 
  * cdef void * __get_ptr_uint16(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[uint16_t, ndim=2, mode="c"] data_array_uint16
  *     data_array_uint16 = data
  */
 
@@ -3119,15 +3160,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_uint16.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_uint16);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":83
+/* "gsd/fl.pyx":84
  *         return <void*>&data_array_uint16[0, 0]
  * 
  * cdef void * __get_ptr_uint32(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[uint32_t, ndim=2, mode="c"] data_array_uint32
  *     data_array_uint32 = data
  */
 
@@ -3151,22 +3192,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_uint32", 0);
   __pyx_pybuffer_data_array_uint32.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_uint32.refcount = 0;
   __pyx_pybuffernd_data_array_uint32.data = NULL;
   __pyx_pybuffernd_data_array_uint32.rcbuffer = &__pyx_pybuffer_data_array_uint32;
 
-  /* "gsd/fl.pyx":85
+  /* "gsd/fl.pyx":86
  * cdef void * __get_ptr_uint32(data):
  *     cdef numpy.ndarray[uint32_t, ndim=2, mode="c"] data_array_uint32
  *     data_array_uint32 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 86, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_uint32.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_uint32.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint32_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -3176,55 +3217,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_uint32.diminfo[0].strides = __pyx_pybuffernd_data_array_uint32.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_uint32.diminfo[0].shape = __pyx_pybuffernd_data_array_uint32.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_uint32.diminfo[1].strides = __pyx_pybuffernd_data_array_uint32.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_uint32.diminfo[1].shape = __pyx_pybuffernd_data_array_uint32.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
   }
   __pyx_v_data_array_uint32 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":86
+  /* "gsd/fl.pyx":87
  *     cdef numpy.ndarray[uint32_t, ndim=2, mode="c"] data_array_uint32
  *     data_array_uint32 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":87
+    /* "gsd/fl.pyx":88
  *     data_array_uint32 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_uint32[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":86
+    /* "gsd/fl.pyx":87
  *     cdef numpy.ndarray[uint32_t, ndim=2, mode="c"] data_array_uint32
  *     data_array_uint32 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":89
+  /* "gsd/fl.pyx":90
  *         return NULL
  *     else:
  *         return <void*>&data_array_uint32[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_uint64(data):
  */
   /*else*/ {
@@ -3237,21 +3278,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_uint32.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_uint32.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_uint32.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 89, __pyx_L1_error)
+      __PYX_ERR(0, 90, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(uint32_t *, __pyx_pybuffernd_data_array_uint32.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_uint32.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_uint32.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":83
+  /* "gsd/fl.pyx":84
  *         return <void*>&data_array_uint16[0, 0]
  * 
  * cdef void * __get_ptr_uint32(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[uint32_t, ndim=2, mode="c"] data_array_uint32
  *     data_array_uint32 = data
  */
 
@@ -3272,15 +3313,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_uint32.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_uint32);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":91
+/* "gsd/fl.pyx":92
  *         return <void*>&data_array_uint32[0, 0]
  * 
  * cdef void * __get_ptr_uint64(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[uint64_t, ndim=2, mode="c"] data_array_uint64
  *     data_array_uint64 = data
  */
 
@@ -3304,22 +3345,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_uint64", 0);
   __pyx_pybuffer_data_array_uint64.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_uint64.refcount = 0;
   __pyx_pybuffernd_data_array_uint64.data = NULL;
   __pyx_pybuffernd_data_array_uint64.rcbuffer = &__pyx_pybuffer_data_array_uint64;
 
-  /* "gsd/fl.pyx":93
+  /* "gsd/fl.pyx":94
  * cdef void * __get_ptr_uint64(data):
  *     cdef numpy.ndarray[uint64_t, ndim=2, mode="c"] data_array_uint64
  *     data_array_uint64 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 94, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_uint64.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_uint64.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint64_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -3329,55 +3370,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_uint64.diminfo[0].strides = __pyx_pybuffernd_data_array_uint64.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_uint64.diminfo[0].shape = __pyx_pybuffernd_data_array_uint64.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_uint64.diminfo[1].strides = __pyx_pybuffernd_data_array_uint64.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_uint64.diminfo[1].shape = __pyx_pybuffernd_data_array_uint64.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 93, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
   }
   __pyx_v_data_array_uint64 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":94
+  /* "gsd/fl.pyx":95
  *     cdef numpy.ndarray[uint64_t, ndim=2, mode="c"] data_array_uint64
  *     data_array_uint64 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":95
+    /* "gsd/fl.pyx":96
  *     data_array_uint64 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_uint64[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":94
+    /* "gsd/fl.pyx":95
  *     cdef numpy.ndarray[uint64_t, ndim=2, mode="c"] data_array_uint64
  *     data_array_uint64 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":97
+  /* "gsd/fl.pyx":98
  *         return NULL
  *     else:
  *         return <void*>&data_array_uint64[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_int8(data):
  */
   /*else*/ {
@@ -3390,21 +3431,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_uint64.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_uint64.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_uint64.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 97, __pyx_L1_error)
+      __PYX_ERR(0, 98, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(uint64_t *, __pyx_pybuffernd_data_array_uint64.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_uint64.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_uint64.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":91
+  /* "gsd/fl.pyx":92
  *         return <void*>&data_array_uint32[0, 0]
  * 
  * cdef void * __get_ptr_uint64(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[uint64_t, ndim=2, mode="c"] data_array_uint64
  *     data_array_uint64 = data
  */
 
@@ -3425,15 +3466,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_uint64.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_uint64);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":99
+/* "gsd/fl.pyx":100
  *         return <void*>&data_array_uint64[0, 0]
  * 
  * cdef void * __get_ptr_int8(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[int8_t, ndim=2, mode="c"] data_array_int8
  *     data_array_int8 = data
  */
 
@@ -3457,22 +3498,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_int8", 0);
   __pyx_pybuffer_data_array_int8.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_int8.refcount = 0;
   __pyx_pybuffernd_data_array_int8.data = NULL;
   __pyx_pybuffernd_data_array_int8.rcbuffer = &__pyx_pybuffer_data_array_int8;
 
-  /* "gsd/fl.pyx":101
+  /* "gsd/fl.pyx":102
  * cdef void * __get_ptr_int8(data):
  *     cdef numpy.ndarray[int8_t, ndim=2, mode="c"] data_array_int8
  *     data_array_int8 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 102, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_int8.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_int8.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn_int8_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -3482,55 +3523,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_int8.diminfo[0].strides = __pyx_pybuffernd_data_array_int8.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_int8.diminfo[0].shape = __pyx_pybuffernd_data_array_int8.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_int8.diminfo[1].strides = __pyx_pybuffernd_data_array_int8.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_int8.diminfo[1].shape = __pyx_pybuffernd_data_array_int8.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
   }
   __pyx_v_data_array_int8 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":102
+  /* "gsd/fl.pyx":103
  *     cdef numpy.ndarray[int8_t, ndim=2, mode="c"] data_array_int8
  *     data_array_int8 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":103
+    /* "gsd/fl.pyx":104
  *     data_array_int8 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_int8[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":102
+    /* "gsd/fl.pyx":103
  *     cdef numpy.ndarray[int8_t, ndim=2, mode="c"] data_array_int8
  *     data_array_int8 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":105
+  /* "gsd/fl.pyx":106
  *         return NULL
  *     else:
  *         return <void*>&data_array_int8[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_int16(data):
  */
   /*else*/ {
@@ -3543,21 +3584,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_int8.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_int8.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_int8.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 105, __pyx_L1_error)
+      __PYX_ERR(0, 106, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(int8_t *, __pyx_pybuffernd_data_array_int8.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_int8.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_int8.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":99
+  /* "gsd/fl.pyx":100
  *         return <void*>&data_array_uint64[0, 0]
  * 
  * cdef void * __get_ptr_int8(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[int8_t, ndim=2, mode="c"] data_array_int8
  *     data_array_int8 = data
  */
 
@@ -3578,15 +3619,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_int8.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_int8);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":107
+/* "gsd/fl.pyx":108
  *         return <void*>&data_array_int8[0, 0]
  * 
  * cdef void * __get_ptr_int16(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[int16_t, ndim=2, mode="c"] data_array_int16
  *     data_array_int16 = data
  */
 
@@ -3610,22 +3651,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_int16", 0);
   __pyx_pybuffer_data_array_int16.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_int16.refcount = 0;
   __pyx_pybuffernd_data_array_int16.data = NULL;
   __pyx_pybuffernd_data_array_int16.rcbuffer = &__pyx_pybuffer_data_array_int16;
 
-  /* "gsd/fl.pyx":109
+  /* "gsd/fl.pyx":110
  * cdef void * __get_ptr_int16(data):
  *     cdef numpy.ndarray[int16_t, ndim=2, mode="c"] data_array_int16
  *     data_array_int16 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 110, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_int16.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_int16.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn_int16_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -3635,55 +3676,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_int16.diminfo[0].strides = __pyx_pybuffernd_data_array_int16.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_int16.diminfo[0].shape = __pyx_pybuffernd_data_array_int16.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_int16.diminfo[1].strides = __pyx_pybuffernd_data_array_int16.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_int16.diminfo[1].shape = __pyx_pybuffernd_data_array_int16.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
   }
   __pyx_v_data_array_int16 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":110
+  /* "gsd/fl.pyx":111
  *     cdef numpy.ndarray[int16_t, ndim=2, mode="c"] data_array_int16
  *     data_array_int16 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":111
+    /* "gsd/fl.pyx":112
  *     data_array_int16 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_int16[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":110
+    /* "gsd/fl.pyx":111
  *     cdef numpy.ndarray[int16_t, ndim=2, mode="c"] data_array_int16
  *     data_array_int16 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":113
+  /* "gsd/fl.pyx":114
  *         return NULL
  *     else:
  *         return <void*>&data_array_int16[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_int32(data):
  */
   /*else*/ {
@@ -3696,21 +3737,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_int16.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_int16.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_int16.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 113, __pyx_L1_error)
+      __PYX_ERR(0, 114, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(int16_t *, __pyx_pybuffernd_data_array_int16.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_int16.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_int16.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":107
+  /* "gsd/fl.pyx":108
  *         return <void*>&data_array_int8[0, 0]
  * 
  * cdef void * __get_ptr_int16(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[int16_t, ndim=2, mode="c"] data_array_int16
  *     data_array_int16 = data
  */
 
@@ -3731,15 +3772,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_int16.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_int16);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":115
+/* "gsd/fl.pyx":116
  *         return <void*>&data_array_int16[0, 0]
  * 
  * cdef void * __get_ptr_int32(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[int32_t, ndim=2, mode="c"] data_array_int32
  *     data_array_int32 = data
  */
 
@@ -3763,22 +3804,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_int32", 0);
   __pyx_pybuffer_data_array_int32.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_int32.refcount = 0;
   __pyx_pybuffernd_data_array_int32.data = NULL;
   __pyx_pybuffernd_data_array_int32.rcbuffer = &__pyx_pybuffer_data_array_int32;
 
-  /* "gsd/fl.pyx":117
+  /* "gsd/fl.pyx":118
  * cdef void * __get_ptr_int32(data):
  *     cdef numpy.ndarray[int32_t, ndim=2, mode="c"] data_array_int32
  *     data_array_int32 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 118, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_int32.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_int32.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn_int32_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -3788,55 +3829,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_int32.diminfo[0].strides = __pyx_pybuffernd_data_array_int32.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_int32.diminfo[0].shape = __pyx_pybuffernd_data_array_int32.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_int32.diminfo[1].strides = __pyx_pybuffernd_data_array_int32.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_int32.diminfo[1].shape = __pyx_pybuffernd_data_array_int32.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 117, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
   }
   __pyx_v_data_array_int32 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":118
+  /* "gsd/fl.pyx":119
  *     cdef numpy.ndarray[int32_t, ndim=2, mode="c"] data_array_int32
  *     data_array_int32 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":119
+    /* "gsd/fl.pyx":120
  *     data_array_int32 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_int32[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":118
+    /* "gsd/fl.pyx":119
  *     cdef numpy.ndarray[int32_t, ndim=2, mode="c"] data_array_int32
  *     data_array_int32 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":121
+  /* "gsd/fl.pyx":122
  *         return NULL
  *     else:
  *         return <void*>&data_array_int32[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_int64(data):
  */
   /*else*/ {
@@ -3849,21 +3890,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_int32.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_int32.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_int32.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 121, __pyx_L1_error)
+      __PYX_ERR(0, 122, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(int32_t *, __pyx_pybuffernd_data_array_int32.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_int32.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_int32.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":115
+  /* "gsd/fl.pyx":116
  *         return <void*>&data_array_int16[0, 0]
  * 
  * cdef void * __get_ptr_int32(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[int32_t, ndim=2, mode="c"] data_array_int32
  *     data_array_int32 = data
  */
 
@@ -3884,15 +3925,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_int32.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_int32);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":123
+/* "gsd/fl.pyx":124
  *         return <void*>&data_array_int32[0, 0]
  * 
  * cdef void * __get_ptr_int64(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[int64_t, ndim=2, mode="c"] data_array_int64
  *     data_array_int64 = data
  */
 
@@ -3916,22 +3957,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_int64", 0);
   __pyx_pybuffer_data_array_int64.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_int64.refcount = 0;
   __pyx_pybuffernd_data_array_int64.data = NULL;
   __pyx_pybuffernd_data_array_int64.rcbuffer = &__pyx_pybuffer_data_array_int64;
 
-  /* "gsd/fl.pyx":125
+  /* "gsd/fl.pyx":126
  * cdef void * __get_ptr_int64(data):
  *     cdef numpy.ndarray[int64_t, ndim=2, mode="c"] data_array_int64
  *     data_array_int64 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 125, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 126, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_int64.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_int64.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn_int64_t, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -3941,55 +3982,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_int64.diminfo[0].strides = __pyx_pybuffernd_data_array_int64.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_int64.diminfo[0].shape = __pyx_pybuffernd_data_array_int64.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_int64.diminfo[1].strides = __pyx_pybuffernd_data_array_int64.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_int64.diminfo[1].shape = __pyx_pybuffernd_data_array_int64.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 125, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 126, __pyx_L1_error)
   }
   __pyx_v_data_array_int64 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":126
+  /* "gsd/fl.pyx":127
  *     cdef numpy.ndarray[int64_t, ndim=2, mode="c"] data_array_int64
  *     data_array_int64 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 127, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":127
+    /* "gsd/fl.pyx":128
  *     data_array_int64 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_int64[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":126
+    /* "gsd/fl.pyx":127
  *     cdef numpy.ndarray[int64_t, ndim=2, mode="c"] data_array_int64
  *     data_array_int64 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":129
+  /* "gsd/fl.pyx":130
  *         return NULL
  *     else:
  *         return <void*>&data_array_int64[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_float32(data):
  */
   /*else*/ {
@@ -4002,21 +4043,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_int64.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_int64.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_int64.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 129, __pyx_L1_error)
+      __PYX_ERR(0, 130, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(int64_t *, __pyx_pybuffernd_data_array_int64.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_int64.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_int64.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":123
+  /* "gsd/fl.pyx":124
  *         return <void*>&data_array_int32[0, 0]
  * 
  * cdef void * __get_ptr_int64(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[int64_t, ndim=2, mode="c"] data_array_int64
  *     data_array_int64 = data
  */
 
@@ -4037,15 +4078,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_int64.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_int64);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":131
+/* "gsd/fl.pyx":132
  *         return <void*>&data_array_int64[0, 0]
  * 
  * cdef void * __get_ptr_float32(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[float, ndim=2, mode="c"] data_array_float32
  *     data_array_float32 = data
  */
 
@@ -4069,22 +4110,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_float32", 0);
   __pyx_pybuffer_data_array_float32.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_float32.refcount = 0;
   __pyx_pybuffernd_data_array_float32.data = NULL;
   __pyx_pybuffernd_data_array_float32.rcbuffer = &__pyx_pybuffer_data_array_float32;
 
-  /* "gsd/fl.pyx":133
+  /* "gsd/fl.pyx":134
  * cdef void * __get_ptr_float32(data):
  *     cdef numpy.ndarray[float, ndim=2, mode="c"] data_array_float32
  *     data_array_float32 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 134, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_float32.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_float32.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -4094,55 +4135,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_float32.diminfo[0].strides = __pyx_pybuffernd_data_array_float32.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_float32.diminfo[0].shape = __pyx_pybuffernd_data_array_float32.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_float32.diminfo[1].strides = __pyx_pybuffernd_data_array_float32.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_float32.diminfo[1].shape = __pyx_pybuffernd_data_array_float32.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 134, __pyx_L1_error)
   }
   __pyx_v_data_array_float32 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":134
+  /* "gsd/fl.pyx":135
  *     cdef numpy.ndarray[float, ndim=2, mode="c"] data_array_float32
  *     data_array_float32 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":135
+    /* "gsd/fl.pyx":136
  *     data_array_float32 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_float32[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":134
+    /* "gsd/fl.pyx":135
  *     cdef numpy.ndarray[float, ndim=2, mode="c"] data_array_float32
  *     data_array_float32 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":137
+  /* "gsd/fl.pyx":138
  *         return NULL
  *     else:
  *         return <void*>&data_array_float32[0, 0]             # <<<<<<<<<<<<<<
  * 
  * cdef void * __get_ptr_float64(data):
  */
   /*else*/ {
@@ -4155,21 +4196,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_float32.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_float32.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_float32.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 137, __pyx_L1_error)
+      __PYX_ERR(0, 138, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(float *, __pyx_pybuffernd_data_array_float32.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_float32.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_float32.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":131
+  /* "gsd/fl.pyx":132
  *         return <void*>&data_array_int64[0, 0]
  * 
  * cdef void * __get_ptr_float32(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[float, ndim=2, mode="c"] data_array_float32
  *     data_array_float32 = data
  */
 
@@ -4190,15 +4231,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_float32.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_float32);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":139
+/* "gsd/fl.pyx":140
  *         return <void*>&data_array_float32[0, 0]
  * 
  * cdef void * __get_ptr_float64(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[double, ndim=2, mode="c"] data_array_float64
  *     data_array_float64 = data
  */
 
@@ -4222,22 +4263,22 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_ptr_float64", 0);
   __pyx_pybuffer_data_array_float64.pybuffer.buf = NULL;
   __pyx_pybuffer_data_array_float64.refcount = 0;
   __pyx_pybuffernd_data_array_float64.data = NULL;
   __pyx_pybuffernd_data_array_float64.rcbuffer = &__pyx_pybuffer_data_array_float64;
 
-  /* "gsd/fl.pyx":141
+  /* "gsd/fl.pyx":142
  * cdef void * __get_ptr_float64(data):
  *     cdef numpy.ndarray[double, ndim=2, mode="c"] data_array_float64
  *     data_array_float64 = data             # <<<<<<<<<<<<<<
  *     if (data.size == 0):
  *         return NULL
  */
-  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (!(likely(((__pyx_v_data) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_data, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 142, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_data;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_float64.rcbuffer->pybuffer);
     __pyx_t_2 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_data_array_float64.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_C_CONTIGUOUS, 2, 0, __pyx_stack);
     if (unlikely(__pyx_t_2 < 0)) {
@@ -4247,55 +4288,55 @@
         __Pyx_RaiseBufferFallbackError();
       } else {
         PyErr_Restore(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       }
       __pyx_t_3 = __pyx_t_4 = __pyx_t_5 = 0;
     }
     __pyx_pybuffernd_data_array_float64.diminfo[0].strides = __pyx_pybuffernd_data_array_float64.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_data_array_float64.diminfo[0].shape = __pyx_pybuffernd_data_array_float64.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_data_array_float64.diminfo[1].strides = __pyx_pybuffernd_data_array_float64.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_data_array_float64.diminfo[1].shape = __pyx_pybuffernd_data_array_float64.rcbuffer->pybuffer.shape[1];
-    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 141, __pyx_L1_error)
+    if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
   }
   __pyx_v_data_array_float64 = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":142
+  /* "gsd/fl.pyx":143
  *     cdef numpy.ndarray[double, ndim=2, mode="c"] data_array_float64
  *     data_array_float64 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_EqObjC(__pyx_t_1, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_7) {
 
-    /* "gsd/fl.pyx":143
+    /* "gsd/fl.pyx":144
  *     data_array_float64 = data
  *     if (data.size == 0):
  *         return NULL             # <<<<<<<<<<<<<<
  *     else:
  *         return <void*>&data_array_float64[0, 0]
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":142
+    /* "gsd/fl.pyx":143
  *     cdef numpy.ndarray[double, ndim=2, mode="c"] data_array_float64
  *     data_array_float64 = data
  *     if (data.size == 0):             # <<<<<<<<<<<<<<
  *         return NULL
  *     else:
  */
   }
 
-  /* "gsd/fl.pyx":145
+  /* "gsd/fl.pyx":146
  *         return NULL
  *     else:
  *         return <void*>&data_array_float64[0, 0]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
@@ -4308,21 +4349,21 @@
     } else if (unlikely(__pyx_t_8 >= __pyx_pybuffernd_data_array_float64.diminfo[0].shape)) __pyx_t_2 = 0;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_pybuffernd_data_array_float64.diminfo[1].shape;
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_2 = 1;
     } else if (unlikely(__pyx_t_9 >= __pyx_pybuffernd_data_array_float64.diminfo[1].shape)) __pyx_t_2 = 1;
     if (unlikely(__pyx_t_2 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_2);
-      __PYX_ERR(0, 145, __pyx_L1_error)
+      __PYX_ERR(0, 146, __pyx_L1_error)
     }
     __pyx_r = ((void *)(&(*__Pyx_BufPtrCContig2d(double *, __pyx_pybuffernd_data_array_float64.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_data_array_float64.diminfo[0].strides, __pyx_t_9, __pyx_pybuffernd_data_array_float64.diminfo[1].strides))));
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":139
+  /* "gsd/fl.pyx":140
  *         return <void*>&data_array_float32[0, 0]
  * 
  * cdef void * __get_ptr_float64(data):             # <<<<<<<<<<<<<<
  *     cdef numpy.ndarray[double, ndim=2, mode="c"] data_array_float64
  *     data_array_float64 = data
  */
 
@@ -4343,25 +4384,25 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_array_float64.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data_array_float64);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":148
+/* "gsd/fl.pyx":149
  * 
  * 
  * def open(name, mode, application=None, schema=None, schema_version=None):             # <<<<<<<<<<<<<<
  *     """open(name, mode, application=None, schema=None, schema_version=None)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_1open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_3gsd_2fl_open[] = "open(name, mode, application=None, schema=None, schema_version=None)\n\n    :py:func:`open` opens a GSD file and returns a :py:class:`GSDFile` instance.\n    The return value of :py:func:`open` can be used as a context manager.\n\n    Args:\n        name (str): File name to open.\n\n        mode (str): File access mode.\n\n        application (str): Name of the application creating the file.\n\n        schema (str): Name of the data schema.\n\n        schema_version (tuple[int, int]): Schema version number\n            (major, minor).\n\n    Valid values for mode:\n\n    +------------------+---------------------------------------------+\n    | mode             | description                                 |\n    +==================+=============================================+\n    | ``'rb'``         | Open an existing file for reading.          |\n    +------------------+---------------------------------------------+\n    | ``'rb+'``        | Open an existing file for reading and       |\n    |                  | writing.                                    |\n    +------------------+---------------------------------------------+\n    | ``'wb'``         | Open a file for reading and writing.        |\n    |                  | Creates the file if needed, or overwrites   |\n    |                  | an existing file.                           |\n    +------------------+---------------------------------------------+\n    | ``'wb+'``        | Open a file for reading and writing.        |\n    |                  | Creates the file if needed, or overwrites   |\n    |                  | an existing file.                           |\n    +------------------+---------------------------------------------+\n    | ``'xb'``         | Create a gsd file exclusively and opens it  |\n    |                  | for reading and writing.                    |\n    |                  | Raise :py:exc:`FileExistsError`             |\n    |                  | if it already exists.            ""           |\n    +------------------+---------------------------------------------+\n    | ``'xb+'``        | Create a gsd file exclusively and opens it  |\n    |                  | for reading and writing.                    |\n    |                  | Raise :py:exc:`FileExistsError`             |\n    |                  | if it already exists.                       |\n    +------------------+---------------------------------------------+\n    | ``'ab'``         | Open an existing file for reading and       |\n    |                  | writing. Does *not* create or overwrite     |\n    |                  | existing files.                             |\n    +------------------+---------------------------------------------+\n\n    When opening a file for reading (``'r'`` and ``'a'`` modes): ``application``\n    and ``schema_version`` are ignored and may be ``None``. When ``schema`` is\n    not ``None``, :py:func:`open` throws an exception if the file's schema does\n    not match ``schema``.\n\n    When opening a file for writing (``'w'`` or ``'x'`` modes): The given\n    ``application``, ``schema``, and ``schema_version`` are saved in the file\n    and must not be None.\n\n    Example:\n\n        .. ipython:: python\n\n            with gsd.fl.open(name='file.gsd', mode='wb',\n                             application=\"My application\", schema=\"My Schema\",\n                             schema_version=[1,0]) as f:\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([1,2,3,4], dtype=numpy.float32))\n                f.write_chunk(name='chunk2',\n                              data=numpy.array([[5,6],[7,8]],\n                                               dtype=numpy.float32))\n                f.end_frame()\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([9,10,11,12],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='chunk2',""\n                              data=numpy.array([[13,14],[15,16]],\n                                               dtype=numpy.float32))\n                f.end_frame()\n\n            f = gsd.fl.open(name='file.gsd', mode='rb')\n            if f.chunk_exists(frame=0, name='chunk1'):\n                data = f.read_chunk(frame=0, name='chunk1')\n            data\n            f.close()\n    ";
+static char __pyx_doc_3gsd_2fl_open[] = "open(name, mode, application=None, schema=None, schema_version=None)\n\n    :py:func:`open` opens a GSD file and returns a :py:class:`GSDFile` instance.\n    The return value of :py:func:`open` can be used as a context manager.\n\n    Args:\n        name (str): File name to open.\n\n        mode (str): File access mode.\n\n        application (str): Name of the application creating the file.\n\n        schema (str): Name of the data schema.\n\n        schema_version (tuple[int, int]): Schema version number\n            (major, minor).\n\n    Valid values for ``mode``:\n\n    +------------------+---------------------------------------------+\n    | mode             | description                                 |\n    +==================+=============================================+\n    | ``'r'``          | Open an existing file for reading.          |\n    +------------------+---------------------------------------------+\n    | ``'r+'``         | Open an existing file for reading and       |\n    |                  | writing.                                    |\n    +------------------+---------------------------------------------+\n    | ``'w'``          | Open a file for reading and writing.        |\n    |                  | Creates the file if needed, or overwrites   |\n    |                  | an existing file.                           |\n    +------------------+---------------------------------------------+\n    | ``'x'``          | Create a gsd file exclusively and opens it  |\n    |                  | for reading and writing.                    |\n    |                  | Raise :py:exc:`FileExistsError`             |\n    |                  | if it already exists.                       |\n    +------------------+---------------------------------------------+\n    | ``'a'``          | Open a file for reading and writing.        |\n    |                  | Creates the file if it doesn't exist.       |\n    +------------------+------------------------------""---------------+\n\n    When opening a file for reading (``'r'`` and ``'r+'`` modes):\n    ``application`` and ``schema_version`` are ignored and may be ``None``.\n    When ``schema`` is not ``None``, :py:func:`open` throws an exception if the\n    file's schema does not match ``schema``.\n\n    When opening a file for writing (``'w'``, ``'x'``, or ``'a'`` modes): The\n    given ``application``, ``schema``, and ``schema_version`` must not be None.\n\n    .. deprecated:: 2.9.0\n\n        The following values to ``mode`` are deprecated:\n\n        +------------------+---------------------------------------------+\n        | mode             | description                                 |\n        +==================+=============================================+\n        | ``'rb'``         | Equivalent to ``'r'``                       |\n        +------------------+---------------------------------------------+\n        | ``'rb+'``        | Equivalent to ``'r+'``                      |\n        +------------------+---------------------------------------------+\n        | ``'wb'``         | Equivalent to ``'w'``                       |\n        +------------------+---------------------------------------------+\n        | ``'wb+'``        | Equivalent to ``'w'``                       |\n        +------------------+---------------------------------------------+\n        | ``'xb'``         | Equivalent to ``'x'``                       |\n        +------------------+---------------------------------------------+\n        | ``'xb+'``        | Equivalent to ``'x'``                       |\n        +------------------+---------------------------------------------+\n        | ``'ab'``         | Equivalent to ``'r+'``                      |\n        +------------------+---------------------------------------------+\n\n    Example:\n\n        .. ipython:: python\n\n            with gsd.fl.open(name='file.gsd', mode='w',\n                             application=\"My application""\", schema=\"My Schema\",\n                             schema_version=[1,0]) as f:\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([1,2,3,4], dtype=numpy.float32))\n                f.write_chunk(name='chunk2',\n                              data=numpy.array([[5,6],[7,8]],\n                                               dtype=numpy.float32))\n                f.end_frame()\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([9,10,11,12],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='chunk2',\n                              data=numpy.array([[13,14],[15,16]],\n                                               dtype=numpy.float32))\n                f.end_frame()\n\n            f = gsd.fl.open(name='file.gsd', mode='r')\n            if f.chunk_exists(frame=0, name='chunk1'):\n                data = f.read_chunk(frame=0, name='chunk1')\n            data\n            f.close()\n    ";
 static PyMethodDef __pyx_mdef_3gsd_2fl_1open = {"open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3gsd_2fl_1open, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3gsd_2fl_open};
 static PyObject *__pyx_pw_3gsd_2fl_1open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
   PyObject *__pyx_v_mode = 0;
   PyObject *__pyx_v_application = 0;
   PyObject *__pyx_v_schema = 0;
   PyObject *__pyx_v_schema_version = 0;
@@ -4399,15 +4440,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("open", 0, 2, 5, 1); __PYX_ERR(0, 148, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("open", 0, 2, 5, 1); __PYX_ERR(0, 149, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_application);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -4421,15 +4462,15 @@
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_schema_version);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 148, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 149, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -4445,15 +4486,15 @@
     __pyx_v_mode = values[1];
     __pyx_v_application = values[2];
     __pyx_v_schema = values[3];
     __pyx_v_schema_version = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 148, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 149, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3gsd_2fl_open(__pyx_self, __pyx_v_name, __pyx_v_mode, __pyx_v_application, __pyx_v_schema, __pyx_v_schema_version);
 
@@ -4468,25 +4509,25 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
 
-  /* "gsd/fl.pyx":236
+  /* "gsd/fl.pyx":248
  *     """
  * 
  *     return GSDFile(str(name), mode, application, schema, schema_version)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_v_mode);
   __Pyx_GIVEREF(__pyx_v_mode);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_mode);
   __Pyx_INCREF(__pyx_v_application);
@@ -4495,22 +4536,22 @@
   __Pyx_INCREF(__pyx_v_schema);
   __Pyx_GIVEREF(__pyx_v_schema);
   PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_v_schema);
   __Pyx_INCREF(__pyx_v_schema_version);
   __Pyx_GIVEREF(__pyx_v_schema_version);
   PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_v_schema_version);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":148
+  /* "gsd/fl.pyx":149
  * 
  * 
  * def open(name, mode, application=None, schema=None, schema_version=None):             # <<<<<<<<<<<<<<
  *     """open(name, mode, application=None, schema=None, schema_version=None)
  * 
  */
 
@@ -4522,15 +4563,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":291
+/* "gsd/fl.pyx":303
  *     cdef str name
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  name,
  *                  mode,
  */
 
@@ -4573,37 +4614,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 1); __PYX_ERR(0, 291, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 1); __PYX_ERR(0, 303, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_application)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 2); __PYX_ERR(0, 291, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 2); __PYX_ERR(0, 303, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_schema)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 3); __PYX_ERR(0, 291, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 3); __PYX_ERR(0, 303, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_schema_version)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 4); __PYX_ERR(0, 291, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, 4); __PYX_ERR(0, 303, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 291, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 303, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 5) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -4614,15 +4655,15 @@
     __pyx_v_mode = values[1];
     __pyx_v_application = values[2];
     __pyx_v_schema = values[3];
     __pyx_v_schema_version = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 291, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 303, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile___init__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_name, __pyx_v_mode, __pyx_v_application, __pyx_v_schema, __pyx_v_schema_version);
 
@@ -4642,1063 +4683,1421 @@
   PyObject *__pyx_v_schema_truncated = 0;
   PyObject *__pyx_v_name_e = NULL;
   PyObject *__pyx_v_application_e = NULL;
   PyObject *__pyx_v_schema_e = NULL;
   int __pyx_v_retval;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  int __pyx_t_3;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   char *__pyx_t_8;
   unsigned int __pyx_t_9;
   unsigned int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_INCREF(__pyx_v_mode);
 
-  /* "gsd/fl.pyx":298
+  /* "gsd/fl.pyx":310
  *                  schema_version):
  *         cdef libgsd.gsd_open_flag c_flags
  *         cdef int exclusive_create = 0             # <<<<<<<<<<<<<<
  *         cdef int overwrite = 0
  * 
  */
   __pyx_v_exclusive_create = 0;
 
-  /* "gsd/fl.pyx":299
+  /* "gsd/fl.pyx":311
  *         cdef libgsd.gsd_open_flag c_flags
  *         cdef int exclusive_create = 0
  *         cdef int overwrite = 0             # <<<<<<<<<<<<<<
  * 
- *         if mode == 'wb':
+ *         self.mode = mode
  */
   __pyx_v_overwrite = 0;
 
-  /* "gsd/fl.pyx":301
+  /* "gsd/fl.pyx":313
  *         cdef int overwrite = 0
  * 
+ *         self.mode = mode             # <<<<<<<<<<<<<<
+ * 
+ *         if mode == 'wb':
+ */
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_mode))||((__pyx_v_mode) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_mode)->tp_name), 0))) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_1 = __pyx_v_mode;
+  __Pyx_INCREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->mode);
+  __Pyx_DECREF(__pyx_v_self->mode);
+  __pyx_v_self->mode = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "gsd/fl.pyx":315
+ *         self.mode = mode
+ * 
  *         if mode == 'wb':             # <<<<<<<<<<<<<<
- *             c_flags = libgsd.GSD_OPEN_APPEND
- *             overwrite = 1
+ *             mode = 'w'
+ *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_wb, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 301, __pyx_L1_error)
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_wb, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 315, __pyx_L1_error)
+  if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":302
+    /* "gsd/fl.pyx":316
  * 
  *         if mode == 'wb':
- *             c_flags = libgsd.GSD_OPEN_APPEND             # <<<<<<<<<<<<<<
- *             overwrite = 1
- *         elif mode == 'wb+':
+ *             mode = 'w'             # <<<<<<<<<<<<<<
+ *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
+ *                            FutureWarning)
  */
-    __pyx_v_c_flags = GSD_OPEN_APPEND;
+    __Pyx_INCREF(__pyx_n_u_w);
+    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_w);
 
-    /* "gsd/fl.pyx":303
+    /* "gsd/fl.pyx":317
  *         if mode == 'wb':
- *             c_flags = libgsd.GSD_OPEN_APPEND
- *             overwrite = 1             # <<<<<<<<<<<<<<
+ *             mode = 'w'
+ *             warnings.warn("The 'wb' mode is deprecated, use 'w'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
  *         elif mode == 'wb+':
- *             c_flags = libgsd.GSD_OPEN_READWRITE
  */
-    __pyx_v_overwrite = 1;
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "gsd/fl.pyx":301
- *         cdef int overwrite = 0
+    /* "gsd/fl.pyx":318
+ *             mode = 'w'
+ *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
+ *                            FutureWarning)             # <<<<<<<<<<<<<<
+ *         elif mode == 'wb+':
+ *             mode = 'w'
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":315
+ *         self.mode = mode
  * 
  *         if mode == 'wb':             # <<<<<<<<<<<<<<
- *             c_flags = libgsd.GSD_OPEN_APPEND
- *             overwrite = 1
+ *             mode = 'w'
+ *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
  */
     goto __pyx_L3;
   }
 
-  /* "gsd/fl.pyx":304
- *             c_flags = libgsd.GSD_OPEN_APPEND
- *             overwrite = 1
+  /* "gsd/fl.pyx":319
+ *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
+ *                            FutureWarning)
+ *         elif mode == 'wb+':             # <<<<<<<<<<<<<<
+ *             mode = 'w'
+ *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
+ */
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_wb_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "gsd/fl.pyx":320
+ *                            FutureWarning)
+ *         elif mode == 'wb+':
+ *             mode = 'w'             # <<<<<<<<<<<<<<
+ *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
+ *                            FutureWarning)
+ */
+    __Pyx_INCREF(__pyx_n_u_w);
+    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_w);
+
+    /* "gsd/fl.pyx":321
+ *         elif mode == 'wb+':
+ *             mode = 'w'
+ *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'rb':
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 321, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":322
+ *             mode = 'w'
+ *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
+ *                            FutureWarning)             # <<<<<<<<<<<<<<
+ *         elif mode == 'rb':
+ *             mode = 'r'
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":319
+ *             warnings.warn("The 'wb' mode is deprecated, use 'w'",
+ *                            FutureWarning)
  *         elif mode == 'wb+':             # <<<<<<<<<<<<<<
+ *             mode = 'w'
+ *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
+ */
+    goto __pyx_L3;
+  }
+
+  /* "gsd/fl.pyx":323
+ *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
+ *                            FutureWarning)
+ *         elif mode == 'rb':             # <<<<<<<<<<<<<<
+ *             mode = 'r'
+ *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
+ */
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_rb, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 323, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "gsd/fl.pyx":324
+ *                            FutureWarning)
+ *         elif mode == 'rb':
+ *             mode = 'r'             # <<<<<<<<<<<<<<
+ *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
+ *                            FutureWarning)
+ */
+    __Pyx_INCREF(__pyx_n_u_r);
+    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_r);
+
+    /* "gsd/fl.pyx":325
+ *         elif mode == 'rb':
+ *             mode = 'r'
+ *             warnings.warn("The 'rb' mode is deprecated, use 'r'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'rb+':
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 325, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":326
+ *             mode = 'r'
+ *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
+ *                            FutureWarning)             # <<<<<<<<<<<<<<
+ *         elif mode == 'rb+':
+ *             mode = 'r+'
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":323
+ *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",
+ *                            FutureWarning)
+ *         elif mode == 'rb':             # <<<<<<<<<<<<<<
+ *             mode = 'r'
+ *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
+ */
+    goto __pyx_L3;
+  }
+
+  /* "gsd/fl.pyx":327
+ *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
+ *                            FutureWarning)
+ *         elif mode == 'rb+':             # <<<<<<<<<<<<<<
+ *             mode = 'r+'
+ *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
+ */
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_rb_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 327, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "gsd/fl.pyx":328
+ *                            FutureWarning)
+ *         elif mode == 'rb+':
+ *             mode = 'r+'             # <<<<<<<<<<<<<<
+ *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
+ *                            FutureWarning)
+ */
+    __Pyx_INCREF(__pyx_kp_u_r_2);
+    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_kp_u_r_2);
+
+    /* "gsd/fl.pyx":329
+ *         elif mode == 'rb+':
+ *             mode = 'r+'
+ *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'xb':
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":330
+ *             mode = 'r+'
+ *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
+ *                            FutureWarning)             # <<<<<<<<<<<<<<
+ *         elif mode == 'xb':
+ *             mode = 'x'
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":327
+ *             warnings.warn("The 'rb' mode is deprecated, use 'r'",
+ *                            FutureWarning)
+ *         elif mode == 'rb+':             # <<<<<<<<<<<<<<
+ *             mode = 'r+'
+ *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
+ */
+    goto __pyx_L3;
+  }
+
+  /* "gsd/fl.pyx":331
+ *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
+ *                            FutureWarning)
+ *         elif mode == 'xb':             # <<<<<<<<<<<<<<
+ *             mode = 'x'
+ *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
+ */
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_xb, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "gsd/fl.pyx":332
+ *                            FutureWarning)
+ *         elif mode == 'xb':
+ *             mode = 'x'             # <<<<<<<<<<<<<<
+ *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
+ *                            FutureWarning)
+ */
+    __Pyx_INCREF(__pyx_n_u_x);
+    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_x);
+
+    /* "gsd/fl.pyx":333
+ *         elif mode == 'xb':
+ *             mode = 'x'
+ *             warnings.warn("The 'xb' mode is deprecated, use 'x'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'xb+':
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 333, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":334
+ *             mode = 'x'
+ *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
+ *                            FutureWarning)             # <<<<<<<<<<<<<<
+ *         elif mode == 'xb+':
+ *             mode = 'x'
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":331
+ *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
+ *                            FutureWarning)
+ *         elif mode == 'xb':             # <<<<<<<<<<<<<<
+ *             mode = 'x'
+ *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
+ */
+    goto __pyx_L3;
+  }
+
+  /* "gsd/fl.pyx":335
+ *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
+ *                            FutureWarning)
+ *         elif mode == 'xb+':             # <<<<<<<<<<<<<<
+ *             mode = 'x'
+ *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
+ */
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_xb_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 335, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "gsd/fl.pyx":336
+ *                            FutureWarning)
+ *         elif mode == 'xb+':
+ *             mode = 'x'             # <<<<<<<<<<<<<<
+ *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
+ *                            FutureWarning)
+ */
+    __Pyx_INCREF(__pyx_n_u_x);
+    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_u_x);
+
+    /* "gsd/fl.pyx":337
+ *         elif mode == 'xb+':
+ *             mode = 'x'
+ *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'ab':
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":338
+ *             mode = 'x'
+ *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
+ *                            FutureWarning)             # <<<<<<<<<<<<<<
+ *         elif mode == 'ab':
+ *             mode = 'r+'
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":335
+ *             warnings.warn("The 'xb' mode is deprecated, use 'x'",
+ *                            FutureWarning)
+ *         elif mode == 'xb+':             # <<<<<<<<<<<<<<
+ *             mode = 'x'
+ *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
+ */
+    goto __pyx_L3;
+  }
+
+  /* "gsd/fl.pyx":339
+ *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
+ *                            FutureWarning)
+ *         elif mode == 'ab':             # <<<<<<<<<<<<<<
+ *             mode = 'r+'
+ *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",
+ */
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_ab, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 339, __pyx_L1_error)
+  if (__pyx_t_2) {
+
+    /* "gsd/fl.pyx":340
+ *                            FutureWarning)
+ *         elif mode == 'ab':
+ *             mode = 'r+'             # <<<<<<<<<<<<<<
+ *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",
+ *                            FutureWarning)
+ */
+    __Pyx_INCREF(__pyx_kp_u_r_2);
+    __Pyx_DECREF_SET(__pyx_v_mode, __pyx_kp_u_r_2);
+
+    /* "gsd/fl.pyx":341
+ *         elif mode == 'ab':
+ *             mode = 'r+'
+ *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ * 
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":342
+ *             mode = 'r+'
+ *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",
+ *                            FutureWarning)             # <<<<<<<<<<<<<<
+ * 
+ *         if mode == 'w':
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "gsd/fl.pyx":339
+ *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",
+ *                            FutureWarning)
+ *         elif mode == 'ab':             # <<<<<<<<<<<<<<
+ *             mode = 'r+'
+ *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",
+ */
+  }
+  __pyx_L3:;
+
+  /* "gsd/fl.pyx":344
+ *                            FutureWarning)
+ * 
+ *         if mode == 'w':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_wb_2, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 304, __pyx_L1_error)
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_w, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 344, __pyx_L1_error)
+  if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":305
- *             overwrite = 1
- *         elif mode == 'wb+':
+    /* "gsd/fl.pyx":345
+ * 
+ *         if mode == 'w':
  *             c_flags = libgsd.GSD_OPEN_READWRITE             # <<<<<<<<<<<<<<
  *             overwrite = 1
- *         elif mode == 'rb':
+ *         elif mode == 'r':
  */
     __pyx_v_c_flags = GSD_OPEN_READWRITE;
 
-    /* "gsd/fl.pyx":306
- *         elif mode == 'wb+':
+    /* "gsd/fl.pyx":346
+ *         if mode == 'w':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1             # <<<<<<<<<<<<<<
- *         elif mode == 'rb':
+ *         elif mode == 'r':
  *             c_flags = libgsd.GSD_OPEN_READONLY
  */
     __pyx_v_overwrite = 1;
 
-    /* "gsd/fl.pyx":304
- *             c_flags = libgsd.GSD_OPEN_APPEND
- *             overwrite = 1
- *         elif mode == 'wb+':             # <<<<<<<<<<<<<<
+    /* "gsd/fl.pyx":344
+ *                            FutureWarning)
+ * 
+ *         if mode == 'w':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "gsd/fl.pyx":307
+  /* "gsd/fl.pyx":347
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
- *         elif mode == 'rb':             # <<<<<<<<<<<<<<
+ *         elif mode == 'r':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READONLY
- *         elif mode == 'rb+':
+ *         elif mode == 'r+':
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_rb, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 307, __pyx_L1_error)
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_r, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 347, __pyx_L1_error)
+  if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":308
+    /* "gsd/fl.pyx":348
  *             overwrite = 1
- *         elif mode == 'rb':
+ *         elif mode == 'r':
  *             c_flags = libgsd.GSD_OPEN_READONLY             # <<<<<<<<<<<<<<
- *         elif mode == 'rb+':
+ *         elif mode == 'r+':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  */
     __pyx_v_c_flags = GSD_OPEN_READONLY;
 
-    /* "gsd/fl.pyx":307
+    /* "gsd/fl.pyx":347
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
- *         elif mode == 'rb':             # <<<<<<<<<<<<<<
+ *         elif mode == 'r':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READONLY
- *         elif mode == 'rb+':
+ *         elif mode == 'r+':
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "gsd/fl.pyx":309
- *         elif mode == 'rb':
+  /* "gsd/fl.pyx":349
+ *         elif mode == 'r':
  *             c_flags = libgsd.GSD_OPEN_READONLY
- *         elif mode == 'rb+':             # <<<<<<<<<<<<<<
+ *         elif mode == 'r+':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
- *         elif mode == 'xb':
+ *         elif mode == 'x':
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_rb_2, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 309, __pyx_L1_error)
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_r_2, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
+  if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":310
+    /* "gsd/fl.pyx":350
  *             c_flags = libgsd.GSD_OPEN_READONLY
- *         elif mode == 'rb+':
+ *         elif mode == 'r+':
  *             c_flags = libgsd.GSD_OPEN_READWRITE             # <<<<<<<<<<<<<<
- *         elif mode == 'xb':
- *             c_flags = libgsd.GSD_OPEN_APPEND
+ *         elif mode == 'x':
+ *             c_flags = libgsd.GSD_OPEN_READWRITE
  */
     __pyx_v_c_flags = GSD_OPEN_READWRITE;
 
-    /* "gsd/fl.pyx":309
- *         elif mode == 'rb':
+    /* "gsd/fl.pyx":349
+ *         elif mode == 'r':
  *             c_flags = libgsd.GSD_OPEN_READONLY
- *         elif mode == 'rb+':             # <<<<<<<<<<<<<<
+ *         elif mode == 'r+':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
- *         elif mode == 'xb':
+ *         elif mode == 'x':
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "gsd/fl.pyx":311
- *         elif mode == 'rb+':
+  /* "gsd/fl.pyx":351
+ *         elif mode == 'r+':
+ *             c_flags = libgsd.GSD_OPEN_READWRITE
+ *         elif mode == 'x':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
- *         elif mode == 'xb':             # <<<<<<<<<<<<<<
- *             c_flags = libgsd.GSD_OPEN_APPEND
  *             overwrite = 1
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_xb, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 311, __pyx_L1_error)
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_x, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 351, __pyx_L1_error)
+  if (__pyx_t_2) {
 
-    /* "gsd/fl.pyx":312
+    /* "gsd/fl.pyx":352
  *             c_flags = libgsd.GSD_OPEN_READWRITE
- *         elif mode == 'xb':
- *             c_flags = libgsd.GSD_OPEN_APPEND             # <<<<<<<<<<<<<<
+ *         elif mode == 'x':
+ *             c_flags = libgsd.GSD_OPEN_READWRITE             # <<<<<<<<<<<<<<
  *             overwrite = 1
  *             exclusive_create = 1
  */
-    __pyx_v_c_flags = GSD_OPEN_APPEND;
+    __pyx_v_c_flags = GSD_OPEN_READWRITE;
 
-    /* "gsd/fl.pyx":313
- *         elif mode == 'xb':
- *             c_flags = libgsd.GSD_OPEN_APPEND
+    /* "gsd/fl.pyx":353
+ *         elif mode == 'x':
+ *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1             # <<<<<<<<<<<<<<
  *             exclusive_create = 1
- *         elif mode == 'xb+':
+ *         elif mode == 'a':
  */
     __pyx_v_overwrite = 1;
 
-    /* "gsd/fl.pyx":314
- *             c_flags = libgsd.GSD_OPEN_APPEND
+    /* "gsd/fl.pyx":354
+ *             c_flags = libgsd.GSD_OPEN_READWRITE
  *             overwrite = 1
  *             exclusive_create = 1             # <<<<<<<<<<<<<<
- *         elif mode == 'xb+':
+ *         elif mode == 'a':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
  */
     __pyx_v_exclusive_create = 1;
 
-    /* "gsd/fl.pyx":311
- *         elif mode == 'rb+':
+    /* "gsd/fl.pyx":351
+ *         elif mode == 'r+':
+ *             c_flags = libgsd.GSD_OPEN_READWRITE
+ *         elif mode == 'x':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
- *         elif mode == 'xb':             # <<<<<<<<<<<<<<
- *             c_flags = libgsd.GSD_OPEN_APPEND
  *             overwrite = 1
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "gsd/fl.pyx":315
+  /* "gsd/fl.pyx":355
  *             overwrite = 1
  *             exclusive_create = 1
- *         elif mode == 'xb+':             # <<<<<<<<<<<<<<
+ *         elif mode == 'a':             # <<<<<<<<<<<<<<
  *             c_flags = libgsd.GSD_OPEN_READWRITE
- *             overwrite = 1
+ *             if not os.path.exists(name):
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_kp_u_xb_2, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 315, __pyx_L1_error)
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_a, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 355, __pyx_L1_error)
+  if (likely(__pyx_t_2)) {
 
-    /* "gsd/fl.pyx":316
+    /* "gsd/fl.pyx":356
  *             exclusive_create = 1
- *         elif mode == 'xb+':
+ *         elif mode == 'a':
  *             c_flags = libgsd.GSD_OPEN_READWRITE             # <<<<<<<<<<<<<<
- *             overwrite = 1
- *             exclusive_create = 1
+ *             if not os.path.exists(name):
+ *                 overwrite = 1
  */
     __pyx_v_c_flags = GSD_OPEN_READWRITE;
 
-    /* "gsd/fl.pyx":317
- *         elif mode == 'xb+':
+    /* "gsd/fl.pyx":357
+ *         elif mode == 'a':
  *             c_flags = libgsd.GSD_OPEN_READWRITE
- *             overwrite = 1             # <<<<<<<<<<<<<<
- *             exclusive_create = 1
- *         elif mode == 'ab':
+ *             if not os.path.exists(name):             # <<<<<<<<<<<<<<
+ *                 overwrite = 1
+ *         else:
  */
-    __pyx_v_overwrite = 1;
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_path); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_exists); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_4);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_name);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_5 = ((!__pyx_t_2) != 0);
+    if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":318
+      /* "gsd/fl.pyx":358
  *             c_flags = libgsd.GSD_OPEN_READWRITE
- *             overwrite = 1
- *             exclusive_create = 1             # <<<<<<<<<<<<<<
- *         elif mode == 'ab':
- *             c_flags = libgsd.GSD_OPEN_APPEND
- */
-    __pyx_v_exclusive_create = 1;
-
-    /* "gsd/fl.pyx":315
- *             overwrite = 1
- *             exclusive_create = 1
- *         elif mode == 'xb+':             # <<<<<<<<<<<<<<
- *             c_flags = libgsd.GSD_OPEN_READWRITE
- *             overwrite = 1
- */
-    goto __pyx_L3;
-  }
-
-  /* "gsd/fl.pyx":319
- *             overwrite = 1
- *             exclusive_create = 1
- *         elif mode == 'ab':             # <<<<<<<<<<<<<<
- *             c_flags = libgsd.GSD_OPEN_APPEND
+ *             if not os.path.exists(name):
+ *                 overwrite = 1             # <<<<<<<<<<<<<<
  *         else:
+ *             raise ValueError("Invalid mode: " + mode)
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_ab, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 319, __pyx_L1_error)
-  if (likely(__pyx_t_1)) {
+      __pyx_v_overwrite = 1;
 
-    /* "gsd/fl.pyx":320
- *             exclusive_create = 1
- *         elif mode == 'ab':
- *             c_flags = libgsd.GSD_OPEN_APPEND             # <<<<<<<<<<<<<<
+      /* "gsd/fl.pyx":357
+ *         elif mode == 'a':
+ *             c_flags = libgsd.GSD_OPEN_READWRITE
+ *             if not os.path.exists(name):             # <<<<<<<<<<<<<<
+ *                 overwrite = 1
  *         else:
- *             raise ValueError("mode must be 'wb', 'wb+', 'rb', 'rb+', "
  */
-    __pyx_v_c_flags = GSD_OPEN_APPEND;
+    }
 
-    /* "gsd/fl.pyx":319
+    /* "gsd/fl.pyx":355
  *             overwrite = 1
  *             exclusive_create = 1
- *         elif mode == 'ab':             # <<<<<<<<<<<<<<
- *             c_flags = libgsd.GSD_OPEN_APPEND
- *         else:
+ *         elif mode == 'a':             # <<<<<<<<<<<<<<
+ *             c_flags = libgsd.GSD_OPEN_READWRITE
+ *             if not os.path.exists(name):
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "gsd/fl.pyx":322
- *             c_flags = libgsd.GSD_OPEN_APPEND
+  /* "gsd/fl.pyx":360
+ *                 overwrite = 1
  *         else:
- *             raise ValueError("mode must be 'wb', 'wb+', 'rb', 'rb+', "             # <<<<<<<<<<<<<<
- *                              "'xb', 'xb+', or 'ab'")
+ *             raise ValueError("Invalid mode: " + mode)             # <<<<<<<<<<<<<<
  * 
+ *         self.name = name
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 322, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_Invalid_mode, __pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 360, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 360, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __PYX_ERR(0, 360, __pyx_L1_error)
   }
-  __pyx_L3:;
+  __pyx_L4:;
 
-  /* "gsd/fl.pyx":325
- *                              "'xb', 'xb+', or 'ab'")
+  /* "gsd/fl.pyx":362
+ *             raise ValueError("Invalid mode: " + mode)
  * 
  *         self.name = name             # <<<<<<<<<<<<<<
- *         self.mode = mode
  * 
+ *         cdef char * c_name
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_name))||((__pyx_v_name) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_name)->tp_name), 0))) __PYX_ERR(0, 325, __pyx_L1_error)
-  __pyx_t_2 = __pyx_v_name;
-  __Pyx_INCREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_2);
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_name))||((__pyx_v_name) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_name)->tp_name), 0))) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_3 = __pyx_v_name;
+  __Pyx_INCREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
-  __pyx_v_self->name = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
-
-  /* "gsd/fl.pyx":326
- * 
- *         self.name = name
- *         self.mode = mode             # <<<<<<<<<<<<<<
- * 
- *         cdef char * c_name
- */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_mode))||((__pyx_v_mode) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_mode)->tp_name), 0))) __PYX_ERR(0, 326, __pyx_L1_error)
-  __pyx_t_2 = __pyx_v_mode;
-  __Pyx_INCREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_2);
-  __Pyx_GOTREF(__pyx_v_self->mode);
-  __Pyx_DECREF(__pyx_v_self->mode);
-  __pyx_v_self->mode = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __pyx_v_self->name = ((PyObject*)__pyx_t_3);
+  __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":334
+  /* "gsd/fl.pyx":370
  *         cdef str schema_truncated
  * 
  *         if overwrite:             # <<<<<<<<<<<<<<
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")
  */
-  __pyx_t_1 = (__pyx_v_overwrite != 0);
-  if (__pyx_t_1) {
+  __pyx_t_5 = (__pyx_v_overwrite != 0);
+  if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":335
+    /* "gsd/fl.pyx":371
  * 
  *         if overwrite:
  *             if application is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:
  */
-    __pyx_t_1 = (__pyx_v_application == Py_None);
-    __pyx_t_3 = (__pyx_t_1 != 0);
-    if (unlikely(__pyx_t_3)) {
+    __pyx_t_5 = (__pyx_v_application == Py_None);
+    __pyx_t_2 = (__pyx_t_5 != 0);
+    if (unlikely(__pyx_t_2)) {
 
-      /* "gsd/fl.pyx":336
+      /* "gsd/fl.pyx":372
  *         if overwrite:
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")             # <<<<<<<<<<<<<<
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 336, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __PYX_ERR(0, 372, __pyx_L1_error)
 
-      /* "gsd/fl.pyx":335
+      /* "gsd/fl.pyx":371
  * 
  *         if overwrite:
  *             if application is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:
  */
     }
 
-    /* "gsd/fl.pyx":337
+    /* "gsd/fl.pyx":373
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:
  */
-    __pyx_t_3 = (__pyx_v_schema == Py_None);
-    __pyx_t_1 = (__pyx_t_3 != 0);
-    if (unlikely(__pyx_t_1)) {
+    __pyx_t_2 = (__pyx_v_schema == Py_None);
+    __pyx_t_5 = (__pyx_t_2 != 0);
+    if (unlikely(__pyx_t_5)) {
 
-      /* "gsd/fl.pyx":338
+      /* "gsd/fl.pyx":374
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")             # <<<<<<<<<<<<<<
  *             if schema_version is None:
  *                 raise ValueError("Provide schema_version when creating a file")
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 338, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __PYX_ERR(0, 374, __pyx_L1_error)
 
-      /* "gsd/fl.pyx":337
+      /* "gsd/fl.pyx":373
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:
  */
     }
 
-    /* "gsd/fl.pyx":339
+    /* "gsd/fl.pyx":375
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide schema_version when creating a file")
  * 
  */
-    __pyx_t_1 = (__pyx_v_schema_version == Py_None);
-    __pyx_t_3 = (__pyx_t_1 != 0);
-    if (unlikely(__pyx_t_3)) {
+    __pyx_t_5 = (__pyx_v_schema_version == Py_None);
+    __pyx_t_2 = (__pyx_t_5 != 0);
+    if (unlikely(__pyx_t_2)) {
 
-      /* "gsd/fl.pyx":340
+      /* "gsd/fl.pyx":376
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:
  *                 raise ValueError("Provide schema_version when creating a file")             # <<<<<<<<<<<<<<
  * 
  *             # create a new file or overwrite an existing one
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 340, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 376, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __PYX_ERR(0, 376, __pyx_L1_error)
 
-      /* "gsd/fl.pyx":339
+      /* "gsd/fl.pyx":375
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Provide schema_version when creating a file")
  * 
  */
     }
 
-    /* "gsd/fl.pyx":343
+    /* "gsd/fl.pyx":379
  * 
  *             # create a new file or overwrite an existing one
  *             logger.info('overwriting file: ' + name + ' with mode: ' + mode             # <<<<<<<<<<<<<<
  *                         + ', application: ' + application
  *                         + ', schema: ' + schema
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 343, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_info); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 343, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_overwriting_file, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_with_mode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = PyNumber_Add(__pyx_kp_u_overwriting_file, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_with_mode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Add(__pyx_t_6, __pyx_v_mode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 343, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "gsd/fl.pyx":344
+    /* "gsd/fl.pyx":380
  *             # create a new file or overwrite an existing one
  *             logger.info('overwriting file: ' + name + ' with mode: ' + mode
  *                         + ', application: ' + application             # <<<<<<<<<<<<<<
  *                         + ', schema: ' + schema
  *                         + ', and schema_version: ' + str(schema_version))
  */
-    __pyx_t_6 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_application_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_application_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 380, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Add(__pyx_t_6, __pyx_v_application); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 344, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_application); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 380, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "gsd/fl.pyx":345
+    /* "gsd/fl.pyx":381
  *             logger.info('overwriting file: ' + name + ' with mode: ' + mode
  *                         + ', application: ' + application
  *                         + ', schema: ' + schema             # <<<<<<<<<<<<<<
  *                         + ', and schema_version: ' + str(schema_version))
  *             name_e = name.encode('utf-8')
  */
-    __pyx_t_6 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_schema_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_schema_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 381, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Add(__pyx_t_6, __pyx_v_schema); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 345, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_v_schema); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 381, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "gsd/fl.pyx":346
+    /* "gsd/fl.pyx":382
  *                         + ', application: ' + application
  *                         + ', schema: ' + schema
  *                         + ', and schema_version: ' + str(schema_version))             # <<<<<<<<<<<<<<
  *             name_e = name.encode('utf-8')
  *             c_name = name_e
  */
-    __pyx_t_6 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_and_schema_version); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_and_schema_version); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 382, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_schema_version); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = PyNumber_Add(__pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_schema_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_7 = PyNumber_Add(__pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 382, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":347
+    /* "gsd/fl.pyx":383
  *                         + ', schema: ' + schema
  *                         + ', and schema_version: ' + str(schema_version))
  *             name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *             c_name = name_e
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u_utf_8);
+    __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_v_name_e = __pyx_t_2;
-    __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_v_name_e = __pyx_t_3;
+    __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":348
+    /* "gsd/fl.pyx":384
  *                         + ', and schema_version: ' + str(schema_version))
  *             name_e = name.encode('utf-8')
  *             c_name = name_e             # <<<<<<<<<<<<<<
  * 
  *             application_e = application.encode('utf-8')
  */
-    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 384, __pyx_L1_error)
     __pyx_v_c_name = __pyx_t_8;
 
-    /* "gsd/fl.pyx":350
+    /* "gsd/fl.pyx":386
  *             c_name = name_e
  * 
  *             application_e = application.encode('utf-8')             # <<<<<<<<<<<<<<
  *             c_application = application_e
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_application, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 350, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_application, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u_utf_8);
+    __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_v_application_e = __pyx_t_2;
-    __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_v_application_e = __pyx_t_3;
+    __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":351
+    /* "gsd/fl.pyx":387
  * 
  *             application_e = application.encode('utf-8')
  *             c_application = application_e             # <<<<<<<<<<<<<<
  * 
  *             schema_e = schema.encode('utf-8')
  */
-    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_application_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_application_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
     __pyx_v_c_application = __pyx_t_8;
 
-    /* "gsd/fl.pyx":353
+    /* "gsd/fl.pyx":389
  *             c_application = application_e
  * 
  *             schema_e = schema.encode('utf-8')             # <<<<<<<<<<<<<<
  *             c_schema = schema_e
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_schema, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 353, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_schema, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 389, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u_utf_8);
+    __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 353, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_v_schema_e = __pyx_t_2;
-    __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_v_schema_e = __pyx_t_3;
+    __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":354
+    /* "gsd/fl.pyx":390
  * 
  *             schema_e = schema.encode('utf-8')
  *             c_schema = schema_e             # <<<<<<<<<<<<<<
  * 
  *             _c_schema_version = libgsd.gsd_make_version(schema_version[0],
  */
-    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_schema_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_schema_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L1_error)
     __pyx_v_c_schema = __pyx_t_8;
 
-    /* "gsd/fl.pyx":356
+    /* "gsd/fl.pyx":392
  *             c_schema = schema_e
  * 
  *             _c_schema_version = libgsd.gsd_make_version(schema_version[0],             # <<<<<<<<<<<<<<
  *                                                         schema_version[1])
  * 
  */
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_schema_version, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_9 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_schema_version, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 392, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_9 = __Pyx_PyInt_As_unsigned_int(__pyx_t_3); if (unlikely((__pyx_t_9 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 392, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":357
+    /* "gsd/fl.pyx":393
  * 
  *             _c_schema_version = libgsd.gsd_make_version(schema_version[0],
  *                                                         schema_version[1])             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_schema_version, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_10 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_10 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_schema_version, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_10 = __Pyx_PyInt_As_unsigned_int(__pyx_t_3); if (unlikely((__pyx_t_10 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":356
+    /* "gsd/fl.pyx":392
  *             c_schema = schema_e
  * 
  *             _c_schema_version = libgsd.gsd_make_version(schema_version[0],             # <<<<<<<<<<<<<<
  *                                                         schema_version[1])
  * 
  */
     __pyx_v__c_schema_version = gsd_make_version(__pyx_t_9, __pyx_t_10);
 
-    /* "gsd/fl.pyx":359
+    /* "gsd/fl.pyx":395
  *                                                         schema_version[1])
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_create_and_open(&self.__handle,
  *                                                     c_name,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":360
+          /* "gsd/fl.pyx":396
  * 
  *             with nogil:
  *                 retval = libgsd.gsd_create_and_open(&self.__handle,             # <<<<<<<<<<<<<<
  *                                                     c_name,
  *                                                     c_application,
  */
           __pyx_v_retval = gsd_create_and_open((&__pyx_v_self->__pyx___handle), __pyx_v_c_name, __pyx_v_c_application, __pyx_v_c_schema, __pyx_v__c_schema_version, __pyx_v_c_flags, __pyx_v_exclusive_create);
         }
 
-        /* "gsd/fl.pyx":359
+        /* "gsd/fl.pyx":395
  *                                                         schema_version[1])
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_create_and_open(&self.__handle,
  *                                                     c_name,
  */
         /*finally:*/ {
           /*normal exit:*/{
             #ifdef WITH_THREAD
             __Pyx_FastGIL_Forget();
             Py_BLOCK_THREADS
             #endif
-            goto __pyx_L10;
+            goto __pyx_L12;
           }
-          __pyx_L10:;
+          __pyx_L12:;
         }
     }
 
-    /* "gsd/fl.pyx":334
+    /* "gsd/fl.pyx":370
  *         cdef str schema_truncated
  * 
  *         if overwrite:             # <<<<<<<<<<<<<<
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")
  */
-    goto __pyx_L4;
+    goto __pyx_L6;
   }
 
-  /* "gsd/fl.pyx":369
+  /* "gsd/fl.pyx":405
  *         else:
  *             # open an existing file
  *             logger.info('opening file: ' + name + ' with mode: ' + mode)             # <<<<<<<<<<<<<<
  *             name_e = name.encode('utf-8')
  *             c_name = name_e
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 369, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_info); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_info); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyNumber_Add(__pyx_kp_u_opening_file, __pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 369, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PyNumber_Add(__pyx_t_5, __pyx_kp_u_with_mode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_opening_file, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_v_mode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 369, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_with_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = NULL;
+    __pyx_t_4 = PyNumber_Add(__pyx_t_1, __pyx_v_mode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_4)) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":370
+    /* "gsd/fl.pyx":406
  *             # open an existing file
  *             logger.info('opening file: ' + name + ' with mode: ' + mode)
  *             name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *             c_name = name_e
  * 
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 370, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = NULL;
+    __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_5)) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_5, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_utf_8);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 370, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_4, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_utf_8);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_v_name_e = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __pyx_v_name_e = __pyx_t_3;
+    __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":371
+    /* "gsd/fl.pyx":407
  *             logger.info('opening file: ' + name + ' with mode: ' + mode)
  *             name_e = name.encode('utf-8')
  *             c_name = name_e             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
     __pyx_v_c_name = __pyx_t_8;
 
-    /* "gsd/fl.pyx":373
+    /* "gsd/fl.pyx":409
  *             c_name = name_e
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_open(&self.__handle, c_name, c_flags)
  * 
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":374
+          /* "gsd/fl.pyx":410
  * 
  *             with nogil:
  *                 retval = libgsd.gsd_open(&self.__handle, c_name, c_flags)             # <<<<<<<<<<<<<<
  * 
  *         __raise_on_error(retval, name)
  */
           __pyx_v_retval = gsd_open((&__pyx_v_self->__pyx___handle), __pyx_v_c_name, __pyx_v_c_flags);
         }
 
-        /* "gsd/fl.pyx":373
+        /* "gsd/fl.pyx":409
  *             c_name = name_e
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_open(&self.__handle, c_name, c_flags)
  * 
  */
         /*finally:*/ {
           /*normal exit:*/{
             #ifdef WITH_THREAD
             __Pyx_FastGIL_Forget();
             Py_BLOCK_THREADS
             #endif
-            goto __pyx_L13;
+            goto __pyx_L15;
           }
-          __pyx_L13:;
+          __pyx_L15:;
         }
     }
   }
-  __pyx_L4:;
+  __pyx_L6:;
 
-  /* "gsd/fl.pyx":376
+  /* "gsd/fl.pyx":412
  *                 retval = libgsd.gsd_open(&self.__handle, c_name, c_flags)
  * 
  *         __raise_on_error(retval, name)             # <<<<<<<<<<<<<<
  * 
  *         # validate schema
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_7 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_3, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "gsd/fl.pyx":379
+  /* "gsd/fl.pyx":415
  * 
  *         # validate schema
  *         if schema is not None:             # <<<<<<<<<<<<<<
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:
  */
-  __pyx_t_3 = (__pyx_v_schema != Py_None);
-  __pyx_t_1 = (__pyx_t_3 != 0);
-  if (__pyx_t_1) {
+  __pyx_t_2 = (__pyx_v_schema != Py_None);
+  __pyx_t_5 = (__pyx_t_2 != 0);
+  if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":380
+    /* "gsd/fl.pyx":416
  *         # validate schema
  *         if schema is not None:
  *             schema_truncated = schema             # <<<<<<<<<<<<<<
  *             if len(schema_truncated) > 64:
  *                 schema_truncated = schema_truncated[0:63]
  */
-    if (!(likely(PyUnicode_CheckExact(__pyx_v_schema))||((__pyx_v_schema) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_schema)->tp_name), 0))) __PYX_ERR(0, 380, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_v_schema))||((__pyx_v_schema) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_schema)->tp_name), 0))) __PYX_ERR(0, 416, __pyx_L1_error)
     __pyx_t_7 = __pyx_v_schema;
     __Pyx_INCREF(__pyx_t_7);
     __pyx_v_schema_truncated = ((PyObject*)__pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":381
+    /* "gsd/fl.pyx":417
  *         if schema is not None:
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:             # <<<<<<<<<<<<<<
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:
  */
     if (unlikely(__pyx_v_schema_truncated == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 381, __pyx_L1_error)
+      __PYX_ERR(0, 417, __pyx_L1_error)
     }
-    __pyx_t_11 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_schema_truncated); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 381, __pyx_L1_error)
-    __pyx_t_1 = ((__pyx_t_11 > 64) != 0);
-    if (__pyx_t_1) {
+    __pyx_t_11 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_schema_truncated); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_5 = ((__pyx_t_11 > 64) != 0);
+    if (__pyx_t_5) {
 
-      /* "gsd/fl.pyx":382
+      /* "gsd/fl.pyx":418
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:
  *                 schema_truncated = schema_truncated[0:63]             # <<<<<<<<<<<<<<
  *             if self.schema != schema_truncated:
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '
  */
       if (unlikely(__pyx_v_schema_truncated == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 382, __pyx_L1_error)
+        __PYX_ERR(0, 418, __pyx_L1_error)
       }
-      __pyx_t_7 = __Pyx_PyUnicode_Substring(__pyx_v_schema_truncated, 0, 63); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 382, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyUnicode_Substring(__pyx_v_schema_truncated, 0, 63); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF_SET(__pyx_v_schema_truncated, ((PyObject*)__pyx_t_7));
       __pyx_t_7 = 0;
 
-      /* "gsd/fl.pyx":381
+      /* "gsd/fl.pyx":417
  *         if schema is not None:
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:             # <<<<<<<<<<<<<<
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:
  */
     }
 
-    /* "gsd/fl.pyx":383
+    /* "gsd/fl.pyx":419
  *             if len(schema_truncated) > 64:
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '
  *                                    + self.schema)
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_7, __pyx_v_schema_truncated, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_7, __pyx_v_schema_truncated, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(__pyx_t_1)) {
+    if (unlikely(__pyx_t_5)) {
 
-      /* "gsd/fl.pyx":384
+      /* "gsd/fl.pyx":420
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '             # <<<<<<<<<<<<<<
  *                                    + self.schema)
  * 
  */
-      __pyx_t_7 = PyNumber_Add(__pyx_kp_u_file, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 384, __pyx_L1_error)
+      __pyx_t_7 = PyNumber_Add(__pyx_kp_u_file, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_2 = PyNumber_Add(__pyx_t_7, __pyx_kp_u_has_incorrect_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 384, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_3 = PyNumber_Add(__pyx_t_7, __pyx_kp_u_has_incorrect_schema); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "gsd/fl.pyx":385
+      /* "gsd/fl.pyx":421
  *             if self.schema != schema_truncated:
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '
  *                                    + self.schema)             # <<<<<<<<<<<<<<
  * 
  *         self.__is_open = True
  */
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 385, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_5 = PyNumber_Add(__pyx_t_2, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 385, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "gsd/fl.pyx":384
+      /* "gsd/fl.pyx":420
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '             # <<<<<<<<<<<<<<
  *                                    + self.schema)
  * 
  */
-      __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 384, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_7, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __PYX_ERR(0, 384, __pyx_L1_error)
+      __PYX_ERR(0, 420, __pyx_L1_error)
 
-      /* "gsd/fl.pyx":383
+      /* "gsd/fl.pyx":419
  *             if len(schema_truncated) > 64:
  *                 schema_truncated = schema_truncated[0:63]
  *             if self.schema != schema_truncated:             # <<<<<<<<<<<<<<
  *                 raise RuntimeError('file ' + name + ' has incorrect schema: '
  *                                    + self.schema)
  */
     }
 
-    /* "gsd/fl.pyx":379
+    /* "gsd/fl.pyx":415
  * 
  *         # validate schema
  *         if schema is not None:             # <<<<<<<<<<<<<<
  *             schema_truncated = schema
  *             if len(schema_truncated) > 64:
  */
   }
 
-  /* "gsd/fl.pyx":387
+  /* "gsd/fl.pyx":423
  *                                    + self.schema)
  * 
  *         self.__is_open = True             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
   __pyx_v_self->__pyx___is_open = 1;
 
-  /* "gsd/fl.pyx":291
+  /* "gsd/fl.pyx":303
  *     cdef str name
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  name,
  *                  mode,
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("gsd.fl.GSDFile.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_schema_truncated);
   __Pyx_XDECREF(__pyx_v_name_e);
   __Pyx_XDECREF(__pyx_v_application_e);
   __Pyx_XDECREF(__pyx_v_schema_e);
+  __Pyx_XDECREF(__pyx_v_mode);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":389
+/* "gsd/fl.pyx":425
  *         self.__is_open = True
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """close()
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_3close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_2close[] = "close()\n\n        Close the file.\n\n        Once closed, any other operation on the file object will result in a\n        `ValueError`. :py:meth:`close()` may be called more than once.\n        The file is automatically closed when garbage collected or when\n        the context manager exits.\n\n        Example:\n            .. ipython:: python\n                :okexcept:\n\n                f = gsd.fl.open(name='file.gsd', mode='wb+',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([1,2,3,4], dtype=numpy.float32))\n                f.end_frame()\n                data = f.read_chunk(frame=0, name='chunk1')\n\n                f.close()\n                # Read fails because the file is closed\n                data = f.read_chunk(frame=0, name='chunk1')\n\n        ";
+static char __pyx_doc_3gsd_2fl_7GSDFile_2close[] = "close()\n\n        Close the file.\n\n        Once closed, any other operation on the file object will result in a\n        `ValueError`. :py:meth:`close()` may be called more than once.\n        The file is automatically closed when garbage collected or when\n        the context manager exits.\n\n        Example:\n            .. ipython:: python\n                :okexcept:\n\n                f = gsd.fl.open(name='file.gsd', mode='w',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([1,2,3,4], dtype=numpy.float32))\n                f.end_frame()\n                data = f.read_chunk(frame=0, name='chunk1')\n\n                f.close()\n                # Read fails because the file is closed\n                data = f.read_chunk(frame=0, name='chunk1')\n\n        ";
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_3close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close (wrapper)", 0);
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_2close(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
 
   /* function exit code */
@@ -5716,82 +6115,82 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "gsd/fl.pyx":416
+  /* "gsd/fl.pyx":452
  * 
  *         """
  *         if self.__is_open:             # <<<<<<<<<<<<<<
  *             logger.info('closing file: ' + self.name)
  *             with nogil:
  */
   __pyx_t_1 = (__pyx_v_self->__pyx___is_open != 0);
   if (__pyx_t_1) {
 
-    /* "gsd/fl.pyx":417
+    /* "gsd/fl.pyx":453
  *         """
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)             # <<<<<<<<<<<<<<
  *             with nogil:
  *                 retval = libgsd.gsd_close(&self.__handle)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_closing_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_closing_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":418
+    /* "gsd/fl.pyx":454
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":419
+          /* "gsd/fl.pyx":455
  *             logger.info('closing file: ' + self.name)
  *             with nogil:
  *                 retval = libgsd.gsd_close(&self.__handle)             # <<<<<<<<<<<<<<
  *             self.__is_open = False
  * 
  */
           __pyx_v_retval = gsd_close((&__pyx_v_self->__pyx___handle));
         }
 
-        /* "gsd/fl.pyx":418
+        /* "gsd/fl.pyx":454
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False
  */
         /*finally:*/ {
@@ -5802,50 +6201,50 @@
             #endif
             goto __pyx_L6;
           }
           __pyx_L6:;
         }
     }
 
-    /* "gsd/fl.pyx":420
+    /* "gsd/fl.pyx":456
  *             with nogil:
  *                 retval = libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False             # <<<<<<<<<<<<<<
  * 
  *             __raise_on_error(retval, self.name)
  */
     __pyx_v_self->__pyx___is_open = 0;
 
-    /* "gsd/fl.pyx":422
+    /* "gsd/fl.pyx":458
  *             self.__is_open = False
  * 
  *             __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def truncate(self):
  */
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __pyx_v_self->name;
     __Pyx_INCREF(__pyx_t_4);
-    __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":416
+    /* "gsd/fl.pyx":452
  * 
  *         """
  *         if self.__is_open:             # <<<<<<<<<<<<<<
  *             logger.info('closing file: ' + self.name)
  *             with nogil:
  */
   }
 
-  /* "gsd/fl.pyx":389
+  /* "gsd/fl.pyx":425
  *         self.__is_open = True
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """close()
  * 
  */
 
@@ -5861,25 +6260,25 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":424
+/* "gsd/fl.pyx":460
  *             __raise_on_error(retval, self.name)
  * 
  *     def truncate(self):             # <<<<<<<<<<<<<<
  *         """truncate()
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_5truncate(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_4truncate[] = "truncate()\n\n        Truncate all data from the file. After truncation, the file has no\n        frames and no data chunks. The application, schema, and schema version\n        remain the same.\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='wb',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    for i in range(10):\n                        f.write_chunk(name='chunk1',\n                                      data=numpy.array([1,2,3,4],\n                                                       dtype=numpy.float32))\n                        f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='ab',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n                f.nframes\n                f.schema, f.schema_version, f.application\n                f.truncate()\n                f.nframes\n                f.schema, f.schema_version, f.application\n                f.close()\n        ";
+static char __pyx_doc_3gsd_2fl_7GSDFile_4truncate[] = "truncate()\n\n        Truncate all data from the file. After truncation, the file has no\n        frames and no data chunks. The application, schema, and schema version\n        remain the same.\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    for i in range(10):\n                        f.write_chunk(name='chunk1',\n                                      data=numpy.array([1,2,3,4],\n                                                       dtype=numpy.float32))\n                        f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r+',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n                f.nframes\n                f.schema, f.schema_version, f.application\n                f.truncate()\n                f.nframes\n                f.schema, f.schema_version, f.application\n                f.close()\n        ";
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_5truncate(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("truncate (wrapper)", 0);
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_4truncate(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
 
   /* function exit code */
@@ -5897,104 +6296,104 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("truncate", 0);
 
-  /* "gsd/fl.pyx":454
+  /* "gsd/fl.pyx":490
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":455
+    /* "gsd/fl.pyx":491
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         logger.info('truncating file: ' + self.name)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 455, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 455, __pyx_L1_error)
+    __PYX_ERR(0, 491, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":454
+    /* "gsd/fl.pyx":490
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":457
+  /* "gsd/fl.pyx":493
  *             raise ValueError("File is not open")
  * 
  *         logger.info('truncating file: ' + self.name)             # <<<<<<<<<<<<<<
  *         with nogil:
  *             retval = libgsd.gsd_truncate(&self.__handle)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_truncating_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_truncating_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":458
+  /* "gsd/fl.pyx":494
  * 
  *         logger.info('truncating file: ' + self.name)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_truncate(&self.__handle)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":459
+        /* "gsd/fl.pyx":495
  *         logger.info('truncating file: ' + self.name)
  *         with nogil:
  *             retval = libgsd.gsd_truncate(&self.__handle)             # <<<<<<<<<<<<<<
  * 
  *         __raise_on_error(retval, self.name)
  */
         __pyx_v_retval = gsd_truncate((&__pyx_v_self->__pyx___handle));
       }
 
-      /* "gsd/fl.pyx":458
+      /* "gsd/fl.pyx":494
  * 
  *         logger.info('truncating file: ' + self.name)
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_truncate(&self.__handle)
  * 
  */
       /*finally:*/ {
@@ -6005,32 +6404,32 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":461
+  /* "gsd/fl.pyx":497
  *             retval = libgsd.gsd_truncate(&self.__handle)
  * 
  *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def end_frame(self):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_4);
-  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":424
+  /* "gsd/fl.pyx":460
  *             __raise_on_error(retval, self.name)
  * 
  *     def truncate(self):             # <<<<<<<<<<<<<<
  *         """truncate()
  * 
  */
 
@@ -6046,25 +6445,25 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":463
+/* "gsd/fl.pyx":499
  *         __raise_on_error(retval, self.name)
  * 
  *     def end_frame(self):             # <<<<<<<<<<<<<<
  *         """end_frame()
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_7end_frame(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_6end_frame[] = "end_frame()\n\n        Complete writing the current frame. After calling :py:meth:`end_frame()`\n        future calls to :py:meth:`write_chunk()` will write to the **next**\n        frame in the file.\n\n        .. danger::\n            Call :py:meth:`end_frame()` to complete the current frame\n            **before** closing the file. If you fail to call\n            :py:meth:`end_frame()`, the last frame will not be written\n            to disk.\n\n        Example:\n            .. ipython:: python\n\n                f = gsd.fl.open(name='file.gsd', mode='wb',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([1,2,3,4], dtype=numpy.float32))\n                f.end_frame()\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([9,10,11,12],\n                                               dtype=numpy.float32))\n                f.end_frame()\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([13,14],\n                                               dtype=numpy.float32))\n                f.end_frame()\n                f.nframes\n                f.close()\n\n        ";
+static char __pyx_doc_3gsd_2fl_7GSDFile_6end_frame[] = "end_frame()\n\n        Complete writing the current frame. After calling :py:meth:`end_frame()`\n        future calls to :py:meth:`write_chunk()` will write to the **next**\n        frame in the file.\n\n        .. danger::\n            Call :py:meth:`end_frame()` to complete the current frame\n            **before** closing the file. If you fail to call\n            :py:meth:`end_frame()`, the last frame will not be written\n            to disk.\n\n        Example:\n            .. ipython:: python\n\n                f = gsd.fl.open(name='file.gsd', mode='w',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([1,2,3,4], dtype=numpy.float32))\n                f.end_frame()\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([9,10,11,12],\n                                               dtype=numpy.float32))\n                f.end_frame()\n                f.write_chunk(name='chunk1',\n                              data=numpy.array([13,14],\n                                               dtype=numpy.float32))\n                f.end_frame()\n                f.nframes\n                f.close()\n\n        ";
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_7end_frame(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("end_frame (wrapper)", 0);
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_6end_frame(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self));
 
   /* function exit code */
@@ -6082,104 +6481,104 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("end_frame", 0);
 
-  /* "gsd/fl.pyx":499
+  /* "gsd/fl.pyx":535
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":500
+    /* "gsd/fl.pyx":536
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         logger.debug('end frame: ' + self.name)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 500, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 536, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 500, __pyx_L1_error)
+    __PYX_ERR(0, 536, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":499
+    /* "gsd/fl.pyx":535
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":502
+  /* "gsd/fl.pyx":538
  *             raise ValueError("File is not open")
  * 
  *         logger.debug('end frame: ' + self.name)             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_end_frame, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_end_frame, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":504
+  /* "gsd/fl.pyx":540
  *         logger.debug('end frame: ' + self.name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_end_frame(&self.__handle)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":505
+        /* "gsd/fl.pyx":541
  * 
  *         with nogil:
  *             retval = libgsd.gsd_end_frame(&self.__handle)             # <<<<<<<<<<<<<<
  * 
  *         __raise_on_error(retval, self.name)
  */
         __pyx_v_retval = gsd_end_frame((&__pyx_v_self->__pyx___handle));
       }
 
-      /* "gsd/fl.pyx":504
+      /* "gsd/fl.pyx":540
  *         logger.debug('end frame: ' + self.name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_end_frame(&self.__handle)
  * 
  */
       /*finally:*/ {
@@ -6190,32 +6589,32 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":507
+  /* "gsd/fl.pyx":543
  *             retval = libgsd.gsd_end_frame(&self.__handle)
  * 
  *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def write_chunk(self, name, data):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_4);
-  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":463
+  /* "gsd/fl.pyx":499
  *         __raise_on_error(retval, self.name)
  * 
  *     def end_frame(self):             # <<<<<<<<<<<<<<
  *         """end_frame()
  * 
  */
 
@@ -6231,25 +6630,25 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":509
+/* "gsd/fl.pyx":545
  *         __raise_on_error(retval, self.name)
  * 
  *     def write_chunk(self, name, data):             # <<<<<<<<<<<<<<
  *         """write_chunk(name, data)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_9write_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_8write_chunk[] = "write_chunk(name, data)\n\n        Write a data chunk to the file. After writing all chunks in the\n        current frame, call :py:meth:`end_frame()`.\n\n        Args:\n            name (str): Name of the chunk\n            data: Data to write into the chunk. Must be a numpy\n                  array, or array-like, with 2 or fewer\n                  dimensions.\n\n        Warning:\n            :py:meth:`write_chunk()` will implicitly converts array-like and\n            non-contiguous numpy arrays to contiguous numpy arrays with\n            ``numpy.ascontiguousarray(data)``. This may or may not produce\n            desired data types in the output file and incurs overhead.\n\n        Example:\n            .. ipython:: python\n\n                f = gsd.fl.open(name='file.gsd', mode='wb',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.write_chunk(name='float1d',\n                              data=numpy.array([1,2,3,4],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='float2d',\n                              data=numpy.array([[13,14],[15,16],[17,19]],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='double2d',\n                              data=numpy.array([[1,4],[5,6],[7,9]],\n                                               dtype=numpy.float64))\n                f.write_chunk(name='int1d',\n                              data=numpy.array([70,80,90],\n                                               dtype=numpy.int64))\n                f.end_frame()\n                f.nframes\n                f.close()\n        ";
+static char __pyx_doc_3gsd_2fl_7GSDFile_8write_chunk[] = "write_chunk(name, data)\n\n        Write a data chunk to the file. After writing all chunks in the\n        current frame, call :py:meth:`end_frame()`.\n\n        Args:\n            name (str): Name of the chunk\n            data: Data to write into the chunk. Must be a numpy\n                  array, or array-like, with 2 or fewer\n                  dimensions.\n\n        Warning:\n            :py:meth:`write_chunk()` will implicitly converts array-like and\n            non-contiguous numpy arrays to contiguous numpy arrays with\n            ``numpy.ascontiguousarray(data)``. This may or may not produce\n            desired data types in the output file and incurs overhead.\n\n        Example:\n            .. ipython:: python\n\n                f = gsd.fl.open(name='file.gsd', mode='w',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.write_chunk(name='float1d',\n                              data=numpy.array([1,2,3,4],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='float2d',\n                              data=numpy.array([[13,14],[15,16],[17,19]],\n                                               dtype=numpy.float32))\n                f.write_chunk(name='double2d',\n                              data=numpy.array([[1,4],[5,6],[7,9]],\n                                               dtype=numpy.float64))\n                f.write_chunk(name='int1d',\n                              data=numpy.array([70,80,90],\n                                               dtype=numpy.int64))\n                f.end_frame()\n                f.nframes\n                f.close()\n        ";
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_9write_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
   PyObject *__pyx_v_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -6274,32 +6673,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("write_chunk", 1, 2, 2, 1); __PYX_ERR(0, 509, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("write_chunk", 1, 2, 2, 1); __PYX_ERR(0, 545, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write_chunk") < 0)) __PYX_ERR(0, 509, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "write_chunk") < 0)) __PYX_ERR(0, 545, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("write_chunk", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 509, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("write_chunk", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 545, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.write_chunk", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_8write_chunk(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_name, __pyx_v_data);
 
@@ -6330,231 +6729,231 @@
   uint32_t __pyx_t_9;
   char *__pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("write_chunk", 0);
 
-  /* "gsd/fl.pyx":551
+  /* "gsd/fl.pyx":587
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":552
+    /* "gsd/fl.pyx":588
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         data_array = numpy.ascontiguousarray(data)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 552, __pyx_L1_error)
+    __PYX_ERR(0, 588, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":551
+    /* "gsd/fl.pyx":587
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":554
+  /* "gsd/fl.pyx":590
  *             raise ValueError("File is not open")
  * 
  *         data_array = numpy.ascontiguousarray(data)             # <<<<<<<<<<<<<<
  *         if data_array is not data:
  *             logger.warning('implicit data copy when writing chunk: ' + name)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 554, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 554, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 554, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_data_array = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":555
+  /* "gsd/fl.pyx":591
  * 
  *         data_array = numpy.ascontiguousarray(data)
  *         if data_array is not data:             # <<<<<<<<<<<<<<
  *             logger.warning('implicit data copy when writing chunk: ' + name)
  *         data_array = data_array.view()
  */
   __pyx_t_1 = (__pyx_v_data_array != __pyx_v_data);
   __pyx_t_5 = (__pyx_t_1 != 0);
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":556
+    /* "gsd/fl.pyx":592
  *         data_array = numpy.ascontiguousarray(data)
  *         if data_array is not data:
  *             logger.warning('implicit data copy when writing chunk: ' + name)             # <<<<<<<<<<<<<<
  *         data_array = data_array.view()
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 556, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 556, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_implicit_data_copy_when_writing, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 556, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_implicit_data_copy_when_writing, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 556, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":555
+    /* "gsd/fl.pyx":591
  * 
  *         data_array = numpy.ascontiguousarray(data)
  *         if data_array is not data:             # <<<<<<<<<<<<<<
  *             logger.warning('implicit data copy when writing chunk: ' + name)
  *         data_array = data_array.view()
  */
   }
 
-  /* "gsd/fl.pyx":557
+  /* "gsd/fl.pyx":593
  *         if data_array is not data:
  *             logger.warning('implicit data copy when writing chunk: ' + name)
  *         data_array = data_array.view()             # <<<<<<<<<<<<<<
  * 
  *         cdef uint64_t N
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_view); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_view); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 557, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_data_array, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":562
+  /* "gsd/fl.pyx":598
  *         cdef uint32_t M
  * 
  *         if len(data_array.shape) > 2:             # <<<<<<<<<<<<<<
  *             raise ValueError("GSD can only write 1 or 2 dimensional arrays: "
  *                              + name)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_5 = ((__pyx_t_7 > 2) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "gsd/fl.pyx":564
+    /* "gsd/fl.pyx":600
  *         if len(data_array.shape) > 2:
  *             raise ValueError("GSD can only write 1 or 2 dimensional arrays: "
  *                              + name)             # <<<<<<<<<<<<<<
  * 
  *         if len(data_array.shape) == 1:
  */
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_GSD_can_only_write_1_or_2_dimens, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_GSD_can_only_write_1_or_2_dimens, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "gsd/fl.pyx":563
+    /* "gsd/fl.pyx":599
  * 
  *         if len(data_array.shape) > 2:
  *             raise ValueError("GSD can only write 1 or 2 dimensional arrays: "             # <<<<<<<<<<<<<<
  *                              + name)
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 563, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 563, __pyx_L1_error)
+    __PYX_ERR(0, 599, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":562
+    /* "gsd/fl.pyx":598
  *         cdef uint32_t M
  * 
  *         if len(data_array.shape) > 2:             # <<<<<<<<<<<<<<
  *             raise ValueError("GSD can only write 1 or 2 dimensional arrays: "
  *                              + name)
  */
   }
 
-  /* "gsd/fl.pyx":566
+  /* "gsd/fl.pyx":602
  *                              + name)
  * 
  *         if len(data_array.shape) == 1:             # <<<<<<<<<<<<<<
  *             data_array = data_array.reshape([data_array.shape[0], 1])
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 566, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 566, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = ((__pyx_t_7 == 1) != 0);
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":567
+    /* "gsd/fl.pyx":603
  * 
  *         if len(data_array.shape) == 1:
  *             data_array = data_array.reshape([data_array.shape[0], 1])             # <<<<<<<<<<<<<<
  * 
  *         N = data_array.shape[0]
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_reshape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_reshape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_6);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyList_SET_ITEM(__pyx_t_4, 1, __pyx_int_1);
     __pyx_t_6 = 0;
@@ -6567,588 +6966,588 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_data_array, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":566
+    /* "gsd/fl.pyx":602
  *                              + name)
  * 
  *         if len(data_array.shape) == 1:             # <<<<<<<<<<<<<<
  *             data_array = data_array.reshape([data_array.shape[0], 1])
  * 
  */
   }
 
-  /* "gsd/fl.pyx":569
+  /* "gsd/fl.pyx":605
  *             data_array = data_array.reshape([data_array.shape[0], 1])
  * 
  *         N = data_array.shape[0]             # <<<<<<<<<<<<<<
  *         M = data_array.shape[1]
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_t_2); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 569, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_uint64_t(__pyx_t_2); if (unlikely((__pyx_t_8 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_N = __pyx_t_8;
 
-  /* "gsd/fl.pyx":570
+  /* "gsd/fl.pyx":606
  * 
  *         N = data_array.shape[0]
  *         M = data_array.shape[1]             # <<<<<<<<<<<<<<
  * 
  *         cdef libgsd.gsd_type gsd_type
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 570, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 570, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 570, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_M = __pyx_t_9;
 
-  /* "gsd/fl.pyx":574
+  /* "gsd/fl.pyx":610
  *         cdef libgsd.gsd_type gsd_type
  *         cdef void *data_ptr
  *         if data_array.dtype == numpy.uint8:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":575
+    /* "gsd/fl.pyx":611
  *         cdef void *data_ptr
  *         if data_array.dtype == numpy.uint8:
  *             gsd_type = libgsd.GSD_TYPE_UINT8             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_uint8(data_array)
  *         elif data_array.dtype == numpy.uint16:
  */
     __pyx_v_gsd_type = GSD_TYPE_UINT8;
 
-    /* "gsd/fl.pyx":576
+    /* "gsd/fl.pyx":612
  *         if data_array.dtype == numpy.uint8:
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.uint16:
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint8(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":574
+    /* "gsd/fl.pyx":610
  *         cdef libgsd.gsd_type gsd_type
  *         cdef void *data_ptr
  *         if data_array.dtype == numpy.uint8:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":577
+  /* "gsd/fl.pyx":613
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)
  *         elif data_array.dtype == numpy.uint16:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":578
+    /* "gsd/fl.pyx":614
  *             data_ptr = __get_ptr_uint8(data_array)
  *         elif data_array.dtype == numpy.uint16:
  *             gsd_type = libgsd.GSD_TYPE_UINT16             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_uint16(data_array)
  *         elif data_array.dtype == numpy.uint32:
  */
     __pyx_v_gsd_type = GSD_TYPE_UINT16;
 
-    /* "gsd/fl.pyx":579
+    /* "gsd/fl.pyx":615
  *         elif data_array.dtype == numpy.uint16:
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.uint32:
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint16(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":577
+    /* "gsd/fl.pyx":613
  *             gsd_type = libgsd.GSD_TYPE_UINT8
  *             data_ptr = __get_ptr_uint8(data_array)
  *         elif data_array.dtype == numpy.uint16:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":580
+  /* "gsd/fl.pyx":616
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)
  *         elif data_array.dtype == numpy.uint32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":581
+    /* "gsd/fl.pyx":617
  *             data_ptr = __get_ptr_uint16(data_array)
  *         elif data_array.dtype == numpy.uint32:
  *             gsd_type = libgsd.GSD_TYPE_UINT32             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_uint32(data_array)
  *         elif data_array.dtype == numpy.uint64:
  */
     __pyx_v_gsd_type = GSD_TYPE_UINT32;
 
-    /* "gsd/fl.pyx":582
+    /* "gsd/fl.pyx":618
  *         elif data_array.dtype == numpy.uint32:
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.uint64:
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint32(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":580
+    /* "gsd/fl.pyx":616
  *             gsd_type = libgsd.GSD_TYPE_UINT16
  *             data_ptr = __get_ptr_uint16(data_array)
  *         elif data_array.dtype == numpy.uint32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":583
+  /* "gsd/fl.pyx":619
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)
  *         elif data_array.dtype == numpy.uint64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":584
+    /* "gsd/fl.pyx":620
  *             data_ptr = __get_ptr_uint32(data_array)
  *         elif data_array.dtype == numpy.uint64:
  *             gsd_type = libgsd.GSD_TYPE_UINT64             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_uint64(data_array)
  *         elif data_array.dtype == numpy.int8:
  */
     __pyx_v_gsd_type = GSD_TYPE_UINT64;
 
-    /* "gsd/fl.pyx":585
+    /* "gsd/fl.pyx":621
  *         elif data_array.dtype == numpy.uint64:
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.int8:
  *             gsd_type = libgsd.GSD_TYPE_INT8
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint64(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":583
+    /* "gsd/fl.pyx":619
  *             gsd_type = libgsd.GSD_TYPE_UINT32
  *             data_ptr = __get_ptr_uint32(data_array)
  *         elif data_array.dtype == numpy.uint64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":586
+  /* "gsd/fl.pyx":622
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)
  *         elif data_array.dtype == numpy.int8:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 622, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 622, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 622, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 622, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 622, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":587
+    /* "gsd/fl.pyx":623
  *             data_ptr = __get_ptr_uint64(data_array)
  *         elif data_array.dtype == numpy.int8:
  *             gsd_type = libgsd.GSD_TYPE_INT8             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_int8(data_array)
  *         elif data_array.dtype == numpy.int16:
  */
     __pyx_v_gsd_type = GSD_TYPE_INT8;
 
-    /* "gsd/fl.pyx":588
+    /* "gsd/fl.pyx":624
  *         elif data_array.dtype == numpy.int8:
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.int16:
  *             gsd_type = libgsd.GSD_TYPE_INT16
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int8(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":586
+    /* "gsd/fl.pyx":622
  *             gsd_type = libgsd.GSD_TYPE_UINT64
  *             data_ptr = __get_ptr_uint64(data_array)
  *         elif data_array.dtype == numpy.int8:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":589
+  /* "gsd/fl.pyx":625
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)
  *         elif data_array.dtype == numpy.int16:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":590
+    /* "gsd/fl.pyx":626
  *             data_ptr = __get_ptr_int8(data_array)
  *         elif data_array.dtype == numpy.int16:
  *             gsd_type = libgsd.GSD_TYPE_INT16             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_int16(data_array)
  *         elif data_array.dtype == numpy.int32:
  */
     __pyx_v_gsd_type = GSD_TYPE_INT16;
 
-    /* "gsd/fl.pyx":591
+    /* "gsd/fl.pyx":627
  *         elif data_array.dtype == numpy.int16:
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.int32:
  *             gsd_type = libgsd.GSD_TYPE_INT32
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int16(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":589
+    /* "gsd/fl.pyx":625
  *             gsd_type = libgsd.GSD_TYPE_INT8
  *             data_ptr = __get_ptr_int8(data_array)
  *         elif data_array.dtype == numpy.int16:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":592
+  /* "gsd/fl.pyx":628
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)
  *         elif data_array.dtype == numpy.int32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":593
+    /* "gsd/fl.pyx":629
  *             data_ptr = __get_ptr_int16(data_array)
  *         elif data_array.dtype == numpy.int32:
  *             gsd_type = libgsd.GSD_TYPE_INT32             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_int32(data_array)
  *         elif data_array.dtype == numpy.int64:
  */
     __pyx_v_gsd_type = GSD_TYPE_INT32;
 
-    /* "gsd/fl.pyx":594
+    /* "gsd/fl.pyx":630
  *         elif data_array.dtype == numpy.int32:
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.int64:
  *             gsd_type = libgsd.GSD_TYPE_INT64
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int32(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":592
+    /* "gsd/fl.pyx":628
  *             gsd_type = libgsd.GSD_TYPE_INT16
  *             data_ptr = __get_ptr_int16(data_array)
  *         elif data_array.dtype == numpy.int32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":595
+  /* "gsd/fl.pyx":631
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)
  *         elif data_array.dtype == numpy.int64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":596
+    /* "gsd/fl.pyx":632
  *             data_ptr = __get_ptr_int32(data_array)
  *         elif data_array.dtype == numpy.int64:
  *             gsd_type = libgsd.GSD_TYPE_INT64             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_int64(data_array)
  *         elif data_array.dtype == numpy.float32:
  */
     __pyx_v_gsd_type = GSD_TYPE_INT64;
 
-    /* "gsd/fl.pyx":597
+    /* "gsd/fl.pyx":633
  *         elif data_array.dtype == numpy.int64:
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.float32:
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int64(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":595
+    /* "gsd/fl.pyx":631
  *             gsd_type = libgsd.GSD_TYPE_INT32
  *             data_ptr = __get_ptr_int32(data_array)
  *         elif data_array.dtype == numpy.int64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":598
+  /* "gsd/fl.pyx":634
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)
  *         elif data_array.dtype == numpy.float32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_4, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "gsd/fl.pyx":599
+    /* "gsd/fl.pyx":635
  *             data_ptr = __get_ptr_int64(data_array)
  *         elif data_array.dtype == numpy.float32:
  *             gsd_type = libgsd.GSD_TYPE_FLOAT             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_float32(data_array)
  *         elif data_array.dtype == numpy.float64:
  */
     __pyx_v_gsd_type = GSD_TYPE_FLOAT;
 
-    /* "gsd/fl.pyx":600
+    /* "gsd/fl.pyx":636
  *         elif data_array.dtype == numpy.float32:
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)             # <<<<<<<<<<<<<<
  *         elif data_array.dtype == numpy.float64:
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_float32(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":598
+    /* "gsd/fl.pyx":634
  *             gsd_type = libgsd.GSD_TYPE_INT64
  *             data_ptr = __get_ptr_int64(data_array)
  *         elif data_array.dtype == numpy.float32:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":601
+  /* "gsd/fl.pyx":637
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)
  *         elif data_array.dtype == numpy.float64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE
  *             data_ptr = __get_ptr_float64(data_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(__pyx_t_5)) {
 
-    /* "gsd/fl.pyx":602
+    /* "gsd/fl.pyx":638
  *             data_ptr = __get_ptr_float32(data_array)
  *         elif data_array.dtype == numpy.float64:
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE             # <<<<<<<<<<<<<<
  *             data_ptr = __get_ptr_float64(data_array)
  *         else:
  */
     __pyx_v_gsd_type = GSD_TYPE_DOUBLE;
 
-    /* "gsd/fl.pyx":603
+    /* "gsd/fl.pyx":639
  *         elif data_array.dtype == numpy.float64:
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE
  *             data_ptr = __get_ptr_float64(data_array)             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("invalid type for chunk: " + name)
  */
     __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_float64(__pyx_v_data_array);
 
-    /* "gsd/fl.pyx":601
+    /* "gsd/fl.pyx":637
  *             gsd_type = libgsd.GSD_TYPE_FLOAT
  *             data_ptr = __get_ptr_float32(data_array)
  *         elif data_array.dtype == numpy.float64:             # <<<<<<<<<<<<<<
  *             gsd_type = libgsd.GSD_TYPE_DOUBLE
  *             data_ptr = __get_ptr_float64(data_array)
  */
     goto __pyx_L7;
   }
 
-  /* "gsd/fl.pyx":605
+  /* "gsd/fl.pyx":641
  *             data_ptr = __get_ptr_float64(data_array)
  *         else:
  *             raise ValueError("invalid type for chunk: " + name)             # <<<<<<<<<<<<<<
  * 
  *         logger.debug('write chunk: ' + self.name + ' - ' + name)
  */
   /*else*/ {
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 641, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 605, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 641, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 605, __pyx_L1_error)
+    __PYX_ERR(0, 641, __pyx_L1_error)
   }
   __pyx_L7:;
 
-  /* "gsd/fl.pyx":607
+  /* "gsd/fl.pyx":643
  *             raise ValueError("invalid type for chunk: " + name)
  * 
  *         logger.debug('write chunk: ' + self.name + ' - ' + name)             # <<<<<<<<<<<<<<
  * 
  *         cdef char * c_name
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_write_chunk, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_write_chunk, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7156,82 +7555,82 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 607, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "gsd/fl.pyx":610
+  /* "gsd/fl.pyx":646
  * 
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *         c_name = name_e
  *         with nogil:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 610, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_name_e = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "gsd/fl.pyx":611
+  /* "gsd/fl.pyx":647
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')
  *         c_name = name_e             # <<<<<<<<<<<<<<
  *         with nogil:
  *             retval = libgsd.gsd_write_chunk(&self.__handle,
  */
-  __pyx_t_10 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 611, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 647, __pyx_L1_error)
   __pyx_v_c_name = __pyx_t_10;
 
-  /* "gsd/fl.pyx":612
+  /* "gsd/fl.pyx":648
  *         name_e = name.encode('utf-8')
  *         c_name = name_e
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_write_chunk(&self.__handle,
  *                                             c_name,
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":613
+        /* "gsd/fl.pyx":649
  *         c_name = name_e
  *         with nogil:
  *             retval = libgsd.gsd_write_chunk(&self.__handle,             # <<<<<<<<<<<<<<
  *                                             c_name,
  *                                             gsd_type,
  */
         __pyx_v_retval = gsd_write_chunk((&__pyx_v_self->__pyx___handle), __pyx_v_c_name, __pyx_v_gsd_type, __pyx_v_N, __pyx_v_M, 0, __pyx_v_data_ptr);
       }
 
-      /* "gsd/fl.pyx":612
+      /* "gsd/fl.pyx":648
  *         name_e = name.encode('utf-8')
  *         c_name = name_e
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_write_chunk(&self.__handle,
  *                                             c_name,
  */
       /*finally:*/ {
@@ -7242,32 +7641,32 @@
           #endif
           goto __pyx_L10;
         }
         __pyx_L10:;
       }
   }
 
-  /* "gsd/fl.pyx":621
+  /* "gsd/fl.pyx":657
  *                                             data_ptr)
  * 
  *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def chunk_exists(self, frame, name):
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 657, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_3);
-  __pyx_t_2 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 657, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":509
+  /* "gsd/fl.pyx":545
  *         __raise_on_error(retval, self.name)
  * 
  *     def write_chunk(self, name, data):             # <<<<<<<<<<<<<<
  *         """write_chunk(name, data)
  * 
  */
 
@@ -7285,25 +7684,25 @@
   __Pyx_XDECREF(__pyx_v_data_array);
   __Pyx_XDECREF(__pyx_v_name_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":623
+/* "gsd/fl.pyx":659
  *         __raise_on_error(retval, self.name)
  * 
  *     def chunk_exists(self, frame, name):             # <<<<<<<<<<<<<<
  *         """chunk_exists(frame, name)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_11chunk_exists(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_10chunk_exists[] = "chunk_exists(frame, name)\n\n        Test if a chunk exists.\n\n        Args:\n            frame (int): Index of the frame to check\n            name (str): Name of the chunk\n\n        Returns:\n            bool: ``True`` if the chunk exists in the file at the given frame.              ``False`` if it does not.\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='wb',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([9,10,11,12],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[13,14],[15,16]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='rb',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.chunk_exists(frame=0, name='chunk1')\n                f.chunk_exists(frame=0, name='chunk2')\n                f.chunk_exists(frame=0, name='chunk3')\n                f.chunk_exists(frame=10, name='chunk1')\n                f.close()\n        ";
+static char __pyx_doc_3gsd_2fl_7GSDFile_10chunk_exists[] = "chunk_exists(frame, name)\n\n        Test if a chunk exists.\n\n        Args:\n            frame (int): Index of the frame to check\n            name (str): Name of the chunk\n\n        Returns:\n            bool: ``True`` if the chunk exists in the file at the given frame.              ``False`` if it does not.\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([9,10,11,12],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[13,14],[15,16]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.chunk_exists(frame=0, name='chunk1')\n                f.chunk_exists(frame=0, name='chunk2')\n                f.chunk_exists(frame=0, name='chunk3')\n                f.chunk_exists(frame=10, name='chunk1')\n                f.close()\n        ";
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_11chunk_exists(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_frame = 0;
   PyObject *__pyx_v_name = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -7328,32 +7727,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("chunk_exists", 1, 2, 2, 1); __PYX_ERR(0, 623, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("chunk_exists", 1, 2, 2, 1); __PYX_ERR(0, 659, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "chunk_exists") < 0)) __PYX_ERR(0, 623, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "chunk_exists") < 0)) __PYX_ERR(0, 659, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_frame = values[0];
     __pyx_v_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("chunk_exists", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 623, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("chunk_exists", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 659, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.chunk_exists", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_10chunk_exists(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_frame, __pyx_v_name);
 
@@ -7376,79 +7775,79 @@
   int64_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chunk_exists", 0);
 
-  /* "gsd/fl.pyx":670
+  /* "gsd/fl.pyx":706
  *         cdef const libgsd.gsd_index_entry* index_entry
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *         c_name = name_e
  *         cdef int64_t c_frame
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 706, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 670, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 706, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_name_e = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":671
+  /* "gsd/fl.pyx":707
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')
  *         c_name = name_e             # <<<<<<<<<<<<<<
  *         cdef int64_t c_frame
  *         c_frame = frame
  */
-  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 671, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 707, __pyx_L1_error)
   __pyx_v_c_name = __pyx_t_4;
 
-  /* "gsd/fl.pyx":673
+  /* "gsd/fl.pyx":709
  *         c_name = name_e
  *         cdef int64_t c_frame
  *         c_frame = frame             # <<<<<<<<<<<<<<
  * 
  *         logger.debug('chunk exists: ' + self.name + ' - ' + name)
  */
-  __pyx_t_5 = __Pyx_PyInt_As_int64_t(__pyx_v_frame); if (unlikely((__pyx_t_5 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 673, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int64_t(__pyx_v_frame); if (unlikely((__pyx_t_5 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 709, __pyx_L1_error)
   __pyx_v_c_frame = __pyx_t_5;
 
-  /* "gsd/fl.pyx":675
+  /* "gsd/fl.pyx":711
  *         c_frame = frame
  * 
  *         logger.debug('chunk exists: ' + self.name + ' - ' + name)             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 711, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_chunk_exists, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_chunk_exists, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 711, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7456,45 +7855,45 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 675, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":677
+  /* "gsd/fl.pyx":713
  *         logger.debug('chunk exists: ' + self.name + ' - ' + name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":678
+        /* "gsd/fl.pyx":714
  * 
  *         with nogil:
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)             # <<<<<<<<<<<<<<
  * 
  *         return index_entry != NULL
  */
         __pyx_v_index_entry = gsd_find_chunk((&__pyx_v_self->__pyx___handle), __pyx_v_c_frame, __pyx_v_c_name);
       }
 
-      /* "gsd/fl.pyx":677
+      /* "gsd/fl.pyx":713
  *         logger.debug('chunk exists: ' + self.name + ' - ' + name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  */
       /*finally:*/ {
@@ -7505,29 +7904,29 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "gsd/fl.pyx":680
+  /* "gsd/fl.pyx":716
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  *         return index_entry != NULL             # <<<<<<<<<<<<<<
  * 
  *     def read_chunk(self, frame, name):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_index_entry != NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_index_entry != NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":623
+  /* "gsd/fl.pyx":659
  *         __raise_on_error(retval, self.name)
  * 
  *     def chunk_exists(self, frame, name):             # <<<<<<<<<<<<<<
  *         """chunk_exists(frame, name)
  * 
  */
 
@@ -7542,25 +7941,25 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_name_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":682
+/* "gsd/fl.pyx":718
  *         return index_entry != NULL
  * 
  *     def read_chunk(self, frame, name):             # <<<<<<<<<<<<<<
  *         """read_chunk(frame, name)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_13read_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_12read_chunk[] = "read_chunk(frame, name)\n\n        Read a data chunk from the file and return it as a numpy array.\n\n        Args:\n            frame (int): Index of the frame to read\n            name (str): Name of the chunk\n\n        Returns:\n            ``(N,M)`` or ``(N,)`` `numpy.ndarray` of ``type``: Data read from\n            file. ``N``, ``M``, and ``type`` are determined by the chunk\n            metadata. If the data is NxM in the file and M > 1, return a 2D\n            array. If the data is Nx1, return a 1D array.\n\n        .. tip::\n            Each call invokes a disk read and allocation of a\n            new numpy array for storage. To avoid overhead, call\n            :py:meth:`read_chunk()` on the same chunk only once.\n\n        Example:\n            .. ipython:: python\n                :okexcept:\n\n                with gsd.fl.open(name='file.gsd', mode='wb',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([9,10,11,12],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[13,14],[15,16]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='rb',\n                                application=\"My application\",\n       ""                         schema=\"My Schema\", schema_version=[1,0])\n                f.read_chunk(frame=0, name='chunk1')\n                f.read_chunk(frame=1, name='chunk1')\n                f.read_chunk(frame=2, name='chunk1')\n                f.close()\n        ";
+static char __pyx_doc_3gsd_2fl_7GSDFile_12read_chunk[] = "read_chunk(frame, name)\n\n        Read a data chunk from the file and return it as a numpy array.\n\n        Args:\n            frame (int): Index of the frame to read\n            name (str): Name of the chunk\n\n        Returns:\n            ``(N,M)`` or ``(N,)`` `numpy.ndarray` of ``type``: Data read from\n            file. ``N``, ``M``, and ``type`` are determined by the chunk\n            metadata. If the data is NxM in the file and M > 1, return a 2D\n            array. If the data is Nx1, return a 1D array.\n\n        .. tip::\n            Each call invokes a disk read and allocation of a\n            new numpy array for storage. To avoid overhead, call\n            :py:meth:`read_chunk()` on the same chunk only once.\n\n        Example:\n            .. ipython:: python\n                :okexcept:\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='chunk1',\n                                  data=numpy.array([9,10,11,12],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='chunk2',\n                                  data=numpy.array([[13,14],[15,16]],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n         ""                       schema=\"My Schema\", schema_version=[1,0])\n                f.read_chunk(frame=0, name='chunk1')\n                f.read_chunk(frame=1, name='chunk1')\n                f.read_chunk(frame=2, name='chunk1')\n                f.close()\n        ";
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_13read_chunk(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_frame = 0;
   PyObject *__pyx_v_name = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -7585,32 +7984,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_chunk", 1, 2, 2, 1); __PYX_ERR(0, 682, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_chunk", 1, 2, 2, 1); __PYX_ERR(0, 718, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_chunk") < 0)) __PYX_ERR(0, 682, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_chunk") < 0)) __PYX_ERR(0, 718, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_frame = values[0];
     __pyx_v_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_chunk", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 682, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_chunk", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 718, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.read_chunk", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_12read_chunk(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_frame, __pyx_v_name);
 
@@ -7640,119 +8039,119 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_chunk", 0);
 
-  /* "gsd/fl.pyx":733
+  /* "gsd/fl.pyx":769
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":734
+    /* "gsd/fl.pyx":770
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         cdef const libgsd.gsd_index_entry* index_entry
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 734, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 734, __pyx_L1_error)
+    __PYX_ERR(0, 770, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":733
+    /* "gsd/fl.pyx":769
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":738
+  /* "gsd/fl.pyx":774
  *         cdef const libgsd.gsd_index_entry* index_entry
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')             # <<<<<<<<<<<<<<
  *         c_name = name_e
  *         cdef int64_t c_frame
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 738, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_name_e = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":739
+  /* "gsd/fl.pyx":775
  *         cdef char * c_name
  *         name_e = name.encode('utf-8')
  *         c_name = name_e             # <<<<<<<<<<<<<<
  *         cdef int64_t c_frame
  *         c_frame = frame
  */
-  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 739, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_name_e); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 775, __pyx_L1_error)
   __pyx_v_c_name = __pyx_t_5;
 
-  /* "gsd/fl.pyx":741
+  /* "gsd/fl.pyx":777
  *         c_name = name_e
  *         cdef int64_t c_frame
  *         c_frame = frame             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_v_frame); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 741, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int64_t(__pyx_v_frame); if (unlikely((__pyx_t_6 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 777, __pyx_L1_error)
   __pyx_v_c_frame = __pyx_t_6;
 
-  /* "gsd/fl.pyx":743
+  /* "gsd/fl.pyx":779
  *         c_frame = frame
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":744
+        /* "gsd/fl.pyx":780
  * 
  *         with nogil:
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)             # <<<<<<<<<<<<<<
  * 
  *         if index_entry == NULL:
  */
         __pyx_v_index_entry = gsd_find_chunk((&__pyx_v_self->__pyx___handle), __pyx_v_c_frame, __pyx_v_c_name);
       }
 
-      /* "gsd/fl.pyx":743
+      /* "gsd/fl.pyx":779
  *         c_frame = frame
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  */
       /*finally:*/ {
@@ -7763,832 +8162,832 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":746
+  /* "gsd/fl.pyx":782
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  *         if index_entry == NULL:             # <<<<<<<<<<<<<<
  *             raise KeyError("frame " + str(frame) + " / chunk " + name
  *                            + " not found in: " + self.name)
  */
   __pyx_t_1 = ((__pyx_v_index_entry == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":747
+    /* "gsd/fl.pyx":783
  * 
  *         if index_entry == NULL:
  *             raise KeyError("frame " + str(frame) + " / chunk " + name             # <<<<<<<<<<<<<<
  *                            + " not found in: " + self.name)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 747, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_frame_2, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 747, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_frame_2, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_3, __pyx_kp_u_chunk); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 747, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_3, __pyx_kp_u_chunk); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 747, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":748
+    /* "gsd/fl.pyx":784
  *         if index_entry == NULL:
  *             raise KeyError("frame " + str(frame) + " / chunk " + name
  *                            + " not found in: " + self.name)             # <<<<<<<<<<<<<<
  * 
  *         cdef libgsd.gsd_type gsd_type
  */
-    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_kp_u_not_found_in); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 748, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_kp_u_not_found_in); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 784, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 748, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 784, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":747
+    /* "gsd/fl.pyx":783
  * 
  *         if index_entry == NULL:
  *             raise KeyError("frame " + str(frame) + " / chunk " + name             # <<<<<<<<<<<<<<
  *                            + " not found in: " + self.name)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 747, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 747, __pyx_L1_error)
+    __PYX_ERR(0, 783, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":746
+    /* "gsd/fl.pyx":782
  *             index_entry = libgsd.gsd_find_chunk(&self.__handle, c_frame, c_name)
  * 
  *         if index_entry == NULL:             # <<<<<<<<<<<<<<
  *             raise KeyError("frame " + str(frame) + " / chunk " + name
  *                            + " not found in: " + self.name)
  */
   }
 
-  /* "gsd/fl.pyx":751
+  /* "gsd/fl.pyx":787
  * 
  *         cdef libgsd.gsd_type gsd_type
  *         gsd_type = <libgsd.gsd_type>index_entry.type             # <<<<<<<<<<<<<<
  * 
  *         cdef void *data_ptr
  */
   __pyx_v_gsd_type = ((enum gsd_type)__pyx_v_index_entry->type);
 
-  /* "gsd/fl.pyx":754
+  /* "gsd/fl.pyx":790
  * 
  *         cdef void *data_ptr
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint8,
  *                                      shape=[index_entry.N, index_entry.M])
  */
   switch (__pyx_v_gsd_type) {
     case GSD_TYPE_UINT8:
 
-    /* "gsd/fl.pyx":755
+    /* "gsd/fl.pyx":791
  *         cdef void *data_ptr
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:
  *             data_array = numpy.empty(dtype=numpy.uint8,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 755, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 755, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 755, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 755, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 755, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_uint8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 755, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":756
+    /* "gsd/fl.pyx":792
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:
  *             data_array = numpy.empty(dtype=numpy.uint8,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *             data_array = numpy.empty(dtype=numpy.uint16,
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 756, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 756, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 756, __pyx_L1_error)
+    __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
     __pyx_t_7 = 0;
     __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_t_8) < 0) __PYX_ERR(0, 755, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_t_8) < 0) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":755
+    /* "gsd/fl.pyx":791
  *         cdef void *data_ptr
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:
  *             data_array = numpy.empty(dtype=numpy.uint8,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  */
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 755, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_data_array = __pyx_t_8;
     __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":754
+    /* "gsd/fl.pyx":790
  * 
  *         cdef void *data_ptr
  *         if gsd_type == libgsd.GSD_TYPE_UINT8:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint8,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_UINT16:
 
-    /* "gsd/fl.pyx":758
+    /* "gsd/fl.pyx":794
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *             data_array = numpy.empty(dtype=numpy.uint16,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 758, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 758, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 758, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 758, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 758, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_uint16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 758, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":759
+    /* "gsd/fl.pyx":795
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *             data_array = numpy.empty(dtype=numpy.uint16,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *             data_array = numpy.empty(dtype=numpy.uint32,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 759, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 795, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 759, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 795, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 759, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 795, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 758, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":758
+    /* "gsd/fl.pyx":794
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *             data_array = numpy.empty(dtype=numpy.uint16,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  */
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 758, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_v_data_array = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":757
+    /* "gsd/fl.pyx":793
  *             data_array = numpy.empty(dtype=numpy.uint8,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT16:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint16,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_UINT32:
 
-    /* "gsd/fl.pyx":761
+    /* "gsd/fl.pyx":797
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *             data_array = numpy.empty(dtype=numpy.uint32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 761, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 761, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 761, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 761, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 761, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":762
+    /* "gsd/fl.pyx":798
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *             data_array = numpy.empty(dtype=numpy.uint32,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *             data_array = numpy.empty(dtype=numpy.uint64,
  */
-    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 762, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 798, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 762, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 798, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 762, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 798, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_4) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_4) < 0) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":761
+    /* "gsd/fl.pyx":797
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *             data_array = numpy.empty(dtype=numpy.uint32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 761, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 797, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_data_array = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":760
+    /* "gsd/fl.pyx":796
  *             data_array = numpy.empty(dtype=numpy.uint16,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT32:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint32,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_UINT64:
 
-    /* "gsd/fl.pyx":764
+    /* "gsd/fl.pyx":800
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *             data_array = numpy.empty(dtype=numpy.uint64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 764, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 764, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 764, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 764, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 764, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 764, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":765
+    /* "gsd/fl.pyx":801
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *             data_array = numpy.empty(dtype=numpy.uint64,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  *             data_array = numpy.empty(dtype=numpy.int8,
  */
-    __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 765, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 801, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 765, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 801, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 765, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 801, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_8);
     PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_8);
     __pyx_t_2 = 0;
     __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_3) < 0) __PYX_ERR(0, 764, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_3) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":764
+    /* "gsd/fl.pyx":800
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *             data_array = numpy.empty(dtype=numpy.uint64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 764, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_data_array = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":763
+    /* "gsd/fl.pyx":799
  *             data_array = numpy.empty(dtype=numpy.uint32,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_UINT64:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.uint64,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_INT8:
 
-    /* "gsd/fl.pyx":767
+    /* "gsd/fl.pyx":803
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  *             data_array = numpy.empty(dtype=numpy.int8,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 767, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 803, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 767, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 803, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 767, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 803, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 767, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 803, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 767, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 803, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 767, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 803, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":768
+    /* "gsd/fl.pyx":804
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  *             data_array = numpy.empty(dtype=numpy.int8,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  *             data_array = numpy.empty(dtype=numpy.int16,
  */
-    __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 768, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 804, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 768, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 804, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 768, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 804, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_8);
     PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_2, 1, __pyx_t_7);
     __pyx_t_8 = 0;
     __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_t_2) < 0) __PYX_ERR(0, 767, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_t_2) < 0) __PYX_ERR(0, 803, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":767
+    /* "gsd/fl.pyx":803
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:
  *             data_array = numpy.empty(dtype=numpy.int8,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 767, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 803, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_data_array = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":766
+    /* "gsd/fl.pyx":802
  *             data_array = numpy.empty(dtype=numpy.uint64,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT8:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.int8,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_INT16:
 
-    /* "gsd/fl.pyx":770
+    /* "gsd/fl.pyx":806
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  *             data_array = numpy.empty(dtype=numpy.int16,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 806, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 806, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 806, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 806, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int16); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 806, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 770, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 806, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":771
+    /* "gsd/fl.pyx":807
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  *             data_array = numpy.empty(dtype=numpy.int16,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  *             data_array = numpy.empty(dtype=numpy.int32,
  */
-    __pyx_t_7 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 771, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 807, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 771, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 807, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 771, __pyx_L1_error)
+    __pyx_t_8 = PyList_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 807, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
     __pyx_t_7 = 0;
     __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_t_8) < 0) __PYX_ERR(0, 770, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_t_8) < 0) __PYX_ERR(0, 806, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":770
+    /* "gsd/fl.pyx":806
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:
  *             data_array = numpy.empty(dtype=numpy.int16,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  */
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 770, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 806, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_data_array = __pyx_t_8;
     __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":769
+    /* "gsd/fl.pyx":805
  *             data_array = numpy.empty(dtype=numpy.int8,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT16:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.int16,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_INT32:
 
-    /* "gsd/fl.pyx":773
+    /* "gsd/fl.pyx":809
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  *             data_array = numpy.empty(dtype=numpy.int32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 773, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 773, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 773, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 773, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 773, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 773, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":774
+    /* "gsd/fl.pyx":810
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  *             data_array = numpy.empty(dtype=numpy.int32,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  *             data_array = numpy.empty(dtype=numpy.int64,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 774, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 810, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 774, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 810, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 774, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 810, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyList_SET_ITEM(__pyx_t_7, 1, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 773, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_shape, __pyx_t_7) < 0) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":773
+    /* "gsd/fl.pyx":809
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:
  *             data_array = numpy.empty(dtype=numpy.int32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  */
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 773, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 809, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_v_data_array = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "gsd/fl.pyx":772
+    /* "gsd/fl.pyx":808
  *             data_array = numpy.empty(dtype=numpy.int16,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT32:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.int32,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_INT64:
 
-    /* "gsd/fl.pyx":776
+    /* "gsd/fl.pyx":812
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  *             data_array = numpy.empty(dtype=numpy.int64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 776, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":777
+    /* "gsd/fl.pyx":813
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  *             data_array = numpy.empty(dtype=numpy.int64,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *             data_array = numpy.empty(dtype=numpy.float32,
  */
-    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 777, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 777, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 777, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_4) < 0) __PYX_ERR(0, 776, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_4) < 0) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":776
+    /* "gsd/fl.pyx":812
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:
  *             data_array = numpy.empty(dtype=numpy.int64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 812, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_data_array = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "gsd/fl.pyx":775
+    /* "gsd/fl.pyx":811
  *             data_array = numpy.empty(dtype=numpy.int32,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_INT64:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.int64,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_FLOAT:
 
-    /* "gsd/fl.pyx":779
+    /* "gsd/fl.pyx":815
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *             data_array = numpy.empty(dtype=numpy.float32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 815, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 815, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 815, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 815, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 815, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 779, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 815, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":780
+    /* "gsd/fl.pyx":816
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *             data_array = numpy.empty(dtype=numpy.float32,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *             data_array = numpy.empty(dtype=numpy.float64,
  */
-    __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 780, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 816, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 780, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 816, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 780, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 816, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_8);
     PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_8);
     __pyx_t_2 = 0;
     __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_3) < 0) __PYX_ERR(0, 779, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_t_3) < 0) __PYX_ERR(0, 815, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":779
+    /* "gsd/fl.pyx":815
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *             data_array = numpy.empty(dtype=numpy.float32,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 815, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_data_array = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gsd/fl.pyx":778
+    /* "gsd/fl.pyx":814
  *             data_array = numpy.empty(dtype=numpy.int64,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_FLOAT:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.float32,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     case GSD_TYPE_DOUBLE:
 
-    /* "gsd/fl.pyx":782
+    /* "gsd/fl.pyx":818
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *             data_array = numpy.empty(dtype=numpy.float64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 782, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 818, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 782, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 818, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 782, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 818, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 782, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_numpy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 818, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float64); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 782, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_float64); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 818, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 782, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 818, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":783
+    /* "gsd/fl.pyx":819
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *             data_array = numpy.empty(dtype=numpy.float64,
  *                                      shape=[index_entry.N, index_entry.M])             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("invalid type for chunk: " + name)
  */
-    __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 819, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_index_entry->M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 819, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 819, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_8);
     PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyList_SET_ITEM(__pyx_t_2, 1, __pyx_t_7);
     __pyx_t_8 = 0;
     __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_t_2) < 0) __PYX_ERR(0, 782, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_t_2) < 0) __PYX_ERR(0, 818, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":782
+    /* "gsd/fl.pyx":818
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *             data_array = numpy.empty(dtype=numpy.float64,             # <<<<<<<<<<<<<<
  *                                      shape=[index_entry.N, index_entry.M])
  *         else:
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 782, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 818, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_data_array = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":781
+    /* "gsd/fl.pyx":817
  *             data_array = numpy.empty(dtype=numpy.float32,
  *                                      shape=[index_entry.N, index_entry.M])
  *         elif gsd_type == libgsd.GSD_TYPE_DOUBLE:             # <<<<<<<<<<<<<<
  *             data_array = numpy.empty(dtype=numpy.float64,
  *                                      shape=[index_entry.N, index_entry.M])
  */
     break;
     default:
 
-    /* "gsd/fl.pyx":785
+    /* "gsd/fl.pyx":821
  *                                      shape=[index_entry.N, index_entry.M])
  *         else:
  *             raise ValueError("invalid type for chunk: " + name)             # <<<<<<<<<<<<<<
  * 
  *         logger.debug('read chunk: ' + self.name + ' - '
  */
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 785, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 821, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 785, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 821, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 785, __pyx_L1_error)
+    __PYX_ERR(0, 821, __pyx_L1_error)
     break;
   }
 
-  /* "gsd/fl.pyx":787
+  /* "gsd/fl.pyx":823
  *             raise ValueError("invalid type for chunk: " + name)
  * 
  *         logger.debug('read chunk: ' + self.name + ' - '             # <<<<<<<<<<<<<<
  *                      + str(frame) + ' - ' + name)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 787, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 787, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_read_chunk, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 787, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_read_chunk, __pyx_v_self->name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 787, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_t_2, __pyx_kp_u__12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":788
+  /* "gsd/fl.pyx":824
  * 
  *         logger.debug('read chunk: ' + self.name + ' - '
  *                      + str(frame) + ' - ' + name)             # <<<<<<<<<<<<<<
  * 
  *         # only read chunk if we have data
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_frame); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 824, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = __Pyx_PyUnicode_Concat(__pyx_t_7, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyUnicode_Concat(__pyx_t_7, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 824, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_8, __pyx_kp_u__6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_8, __pyx_kp_u__12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 824, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyNumber_Add(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_8 = PyNumber_Add(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 824, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -8596,20 +8995,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 787, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":791
+  /* "gsd/fl.pyx":827
  * 
  *         # only read chunk if we have data
  *         if index_entry.N != 0 and index_entry.M != 0:             # <<<<<<<<<<<<<<
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:
  *                 data_ptr = __get_ptr_uint8(data_array)
  */
   __pyx_t_9 = ((__pyx_v_index_entry->N != 0) != 0);
@@ -8619,258 +9018,258 @@
     goto __pyx_L9_bool_binop_done;
   }
   __pyx_t_9 = ((__pyx_v_index_entry->M != 0) != 0);
   __pyx_t_1 = __pyx_t_9;
   __pyx_L9_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "gsd/fl.pyx":792
+    /* "gsd/fl.pyx":828
  *         # only read chunk if we have data
  *         if index_entry.N != 0 and index_entry.M != 0:
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  */
     switch (__pyx_v_gsd_type) {
       case GSD_TYPE_UINT8:
 
-      /* "gsd/fl.pyx":793
+      /* "gsd/fl.pyx":829
  *         if index_entry.N != 0 and index_entry.M != 0:
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:
  *                 data_ptr = __get_ptr_uint8(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *                 data_ptr = __get_ptr_uint16(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint8(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":792
+      /* "gsd/fl.pyx":828
  *         # only read chunk if we have data
  *         if index_entry.N != 0 and index_entry.M != 0:
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  */
       break;
       case GSD_TYPE_UINT16:
 
-      /* "gsd/fl.pyx":795
+      /* "gsd/fl.pyx":831
  *                 data_ptr = __get_ptr_uint8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *                 data_ptr = __get_ptr_uint16(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *                 data_ptr = __get_ptr_uint32(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint16(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":794
+      /* "gsd/fl.pyx":830
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:
  *                 data_ptr = __get_ptr_uint8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:
  */
       break;
       case GSD_TYPE_UINT32:
 
-      /* "gsd/fl.pyx":797
+      /* "gsd/fl.pyx":833
  *                 data_ptr = __get_ptr_uint16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *                 data_ptr = __get_ptr_uint32(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *                 data_ptr = __get_ptr_uint64(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint32(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":796
+      /* "gsd/fl.pyx":832
  *             elif gsd_type == libgsd.GSD_TYPE_UINT16:
  *                 data_ptr = __get_ptr_uint16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:
  */
       break;
       case GSD_TYPE_UINT64:
 
-      /* "gsd/fl.pyx":799
+      /* "gsd/fl.pyx":835
  *                 data_ptr = __get_ptr_uint32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *                 data_ptr = __get_ptr_uint64(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:
  *                 data_ptr = __get_ptr_int8(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_uint64(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":798
+      /* "gsd/fl.pyx":834
  *             elif gsd_type == libgsd.GSD_TYPE_UINT32:
  *                 data_ptr = __get_ptr_uint32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_uint64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:
  */
       break;
       case GSD_TYPE_INT8:
 
-      /* "gsd/fl.pyx":801
+      /* "gsd/fl.pyx":837
  *                 data_ptr = __get_ptr_uint64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:
  *                 data_ptr = __get_ptr_int8(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:
  *                 data_ptr = __get_ptr_int16(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int8(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":800
+      /* "gsd/fl.pyx":836
  *             elif gsd_type == libgsd.GSD_TYPE_UINT64:
  *                 data_ptr = __get_ptr_uint64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_int8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:
  */
       break;
       case GSD_TYPE_INT16:
 
-      /* "gsd/fl.pyx":803
+      /* "gsd/fl.pyx":839
  *                 data_ptr = __get_ptr_int8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:
  *                 data_ptr = __get_ptr_int16(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:
  *                 data_ptr = __get_ptr_int32(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int16(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":802
+      /* "gsd/fl.pyx":838
  *             elif gsd_type == libgsd.GSD_TYPE_INT8:
  *                 data_ptr = __get_ptr_int8(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_int16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:
  */
       break;
       case GSD_TYPE_INT32:
 
-      /* "gsd/fl.pyx":805
+      /* "gsd/fl.pyx":841
  *                 data_ptr = __get_ptr_int16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:
  *                 data_ptr = __get_ptr_int32(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:
  *                 data_ptr = __get_ptr_int64(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int32(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":804
+      /* "gsd/fl.pyx":840
  *             elif gsd_type == libgsd.GSD_TYPE_INT16:
  *                 data_ptr = __get_ptr_int16(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_int32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:
  */
       break;
       case GSD_TYPE_INT64:
 
-      /* "gsd/fl.pyx":807
+      /* "gsd/fl.pyx":843
  *                 data_ptr = __get_ptr_int32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:
  *                 data_ptr = __get_ptr_int64(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *                 data_ptr = __get_ptr_float32(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_int64(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":806
+      /* "gsd/fl.pyx":842
  *             elif gsd_type == libgsd.GSD_TYPE_INT32:
  *                 data_ptr = __get_ptr_int32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_int64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  */
       break;
       case GSD_TYPE_FLOAT:
 
-      /* "gsd/fl.pyx":809
+      /* "gsd/fl.pyx":845
  *                 data_ptr = __get_ptr_int64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *                 data_ptr = __get_ptr_float32(data_array)             # <<<<<<<<<<<<<<
  *             elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *                 data_ptr = __get_ptr_float64(data_array)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_float32(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":808
+      /* "gsd/fl.pyx":844
  *             elif gsd_type == libgsd.GSD_TYPE_INT64:
  *                 data_ptr = __get_ptr_int64(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_float32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  */
       break;
       case GSD_TYPE_DOUBLE:
 
-      /* "gsd/fl.pyx":811
+      /* "gsd/fl.pyx":847
  *                 data_ptr = __get_ptr_float32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_DOUBLE:
  *                 data_ptr = __get_ptr_float64(data_array)             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError("invalid type for chunk: " + name)
  */
       __pyx_v_data_ptr = __pyx_f_3gsd_2fl___get_ptr_float64(__pyx_v_data_array);
 
-      /* "gsd/fl.pyx":810
+      /* "gsd/fl.pyx":846
  *             elif gsd_type == libgsd.GSD_TYPE_FLOAT:
  *                 data_ptr = __get_ptr_float32(data_array)
  *             elif gsd_type == libgsd.GSD_TYPE_DOUBLE:             # <<<<<<<<<<<<<<
  *                 data_ptr = __get_ptr_float64(data_array)
  *             else:
  */
       break;
       default:
 
-      /* "gsd/fl.pyx":813
+      /* "gsd/fl.pyx":849
  *                 data_ptr = __get_ptr_float64(data_array)
  *             else:
  *                 raise ValueError("invalid type for chunk: " + name)             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-      __pyx_t_3 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 813, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_kp_u_invalid_type_for_chunk, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 849, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 813, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 849, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 813, __pyx_L1_error)
+      __PYX_ERR(0, 849, __pyx_L1_error)
       break;
     }
 
-    /* "gsd/fl.pyx":815
+    /* "gsd/fl.pyx":851
  *                 raise ValueError("invalid type for chunk: " + name)
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_read_chunk(&self.__handle,
  *                                                data_ptr,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":816
+          /* "gsd/fl.pyx":852
  * 
  *             with nogil:
  *                 retval = libgsd.gsd_read_chunk(&self.__handle,             # <<<<<<<<<<<<<<
  *                                                data_ptr,
  *                                                index_entry)
  */
           __pyx_v_retval = gsd_read_chunk((&__pyx_v_self->__pyx___handle), __pyx_v_data_ptr, __pyx_v_index_entry);
         }
 
-        /* "gsd/fl.pyx":815
+        /* "gsd/fl.pyx":851
  *                 raise ValueError("invalid type for chunk: " + name)
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 retval = libgsd.gsd_read_chunk(&self.__handle,
  *                                                data_ptr,
  */
         /*finally:*/ {
@@ -8881,63 +9280,63 @@
             #endif
             goto __pyx_L13;
           }
           __pyx_L13:;
         }
     }
 
-    /* "gsd/fl.pyx":820
+    /* "gsd/fl.pyx":856
  *                                                index_entry)
  * 
  *             __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *         if index_entry.M == 1:
  */
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 820, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 856, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_v_self->name;
     __Pyx_INCREF(__pyx_t_3);
-    __pyx_t_8 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 820, __pyx_L1_error)
+    __pyx_t_8 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 856, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "gsd/fl.pyx":791
+    /* "gsd/fl.pyx":827
  * 
  *         # only read chunk if we have data
  *         if index_entry.N != 0 and index_entry.M != 0:             # <<<<<<<<<<<<<<
  *             if gsd_type == libgsd.GSD_TYPE_UINT8:
  *                 data_ptr = __get_ptr_uint8(data_array)
  */
   }
 
-  /* "gsd/fl.pyx":822
+  /* "gsd/fl.pyx":858
  *             __raise_on_error(retval, self.name)
  * 
  *         if index_entry.M == 1:             # <<<<<<<<<<<<<<
  *             return data_array.reshape([index_entry.N])
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_index_entry->M == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "gsd/fl.pyx":823
+    /* "gsd/fl.pyx":859
  * 
  *         if index_entry.M == 1:
  *             return data_array.reshape([index_entry.N])             # <<<<<<<<<<<<<<
  *         else:
  *             return data_array
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_reshape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 823, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_reshape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 859, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 823, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint64_t(__pyx_v_index_entry->N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 859, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 823, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 859, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_4);
     PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
     __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8947,45 +9346,45 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 823, __pyx_L1_error)
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 859, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "gsd/fl.pyx":822
+    /* "gsd/fl.pyx":858
  *             __raise_on_error(retval, self.name)
  * 
  *         if index_entry.M == 1:             # <<<<<<<<<<<<<<
  *             return data_array.reshape([index_entry.N])
  *         else:
  */
   }
 
-  /* "gsd/fl.pyx":825
+  /* "gsd/fl.pyx":861
  *             return data_array.reshape([index_entry.N])
  *         else:
  *             return data_array             # <<<<<<<<<<<<<<
  * 
  *     def find_matching_chunk_names(self, match):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_data_array);
     __pyx_r = __pyx_v_data_array;
     goto __pyx_L0;
   }
 
-  /* "gsd/fl.pyx":682
+  /* "gsd/fl.pyx":718
  *         return index_entry != NULL
  * 
  *     def read_chunk(self, frame, name):             # <<<<<<<<<<<<<<
  *         """read_chunk(frame, name)
  * 
  */
 
@@ -9002,25 +9401,25 @@
   __Pyx_XDECREF(__pyx_v_name_e);
   __Pyx_XDECREF(__pyx_v_data_array);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":827
+/* "gsd/fl.pyx":863
  *             return data_array
  * 
  *     def find_matching_chunk_names(self, match):             # <<<<<<<<<<<<<<
  *         """find_matching_chunk_names(match)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_15find_matching_chunk_names(PyObject *__pyx_v_self, PyObject *__pyx_v_match); /*proto*/
-static char __pyx_doc_3gsd_2fl_7GSDFile_14find_matching_chunk_names[] = "find_matching_chunk_names(match)\n\n        Find all the chunk names in the file that start with the string *match*.\n\n        Args:\n            match (str): Start of the chunk name to match\n\n        Returns:\n            list[str]: Matching chunk names\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='wb',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='data/chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='data/chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='input/chunk3',\n                                  data=numpy.array([9, 10],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='input/chunk4',\n                                  data=numpy.array([11, 12, 13, 14],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='rb',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.find_matching_chunk_names('')\n                f.find_matching_chunk_names('data')\n                f.find_matching_chunk_names('input')\n                f.find_matching_chunk_names('other')\n                f.close()\n        ";
+static char __pyx_doc_3gsd_2fl_7GSDFile_14find_matching_chunk_names[] = "find_matching_chunk_names(match)\n\n        Find all the chunk names in the file that start with the string *match*.\n\n        Args:\n            match (str): Start of the chunk name to match\n\n        Returns:\n            list[str]: Matching chunk names\n\n        Example:\n            .. ipython:: python\n\n                with gsd.fl.open(name='file.gsd', mode='w',\n                                 application=\"My application\",\n                                 schema=\"My Schema\", schema_version=[1,0]) as f:\n                    f.write_chunk(name='data/chunk1',\n                                  data=numpy.array([1,2,3,4],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='data/chunk2',\n                                  data=numpy.array([[5,6],[7,8]],\n                                                   dtype=numpy.float32))\n                    f.write_chunk(name='input/chunk3',\n                                  data=numpy.array([9, 10],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n                    f.write_chunk(name='input/chunk4',\n                                  data=numpy.array([11, 12, 13, 14],\n                                                   dtype=numpy.float32))\n                    f.end_frame()\n\n                f = gsd.fl.open(name='file.gsd', mode='r',\n                                application=\"My application\",\n                                schema=\"My Schema\", schema_version=[1,0])\n\n                f.find_matching_chunk_names('')\n                f.find_matching_chunk_names('data')\n                f.find_matching_chunk_names('input')\n                f.find_matching_chunk_names('other')\n                f.close()\n        ";
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_15find_matching_chunk_names(PyObject *__pyx_v_self, PyObject *__pyx_v_match) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find_matching_chunk_names (wrapper)", 0);
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_14find_matching_chunk_names(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), ((PyObject *)__pyx_v_match));
 
   /* function exit code */
@@ -9042,121 +9441,121 @@
   char *__pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_matching_chunk_names", 0);
 
-  /* "gsd/fl.pyx":870
+  /* "gsd/fl.pyx":906
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":871
+    /* "gsd/fl.pyx":907
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         cdef const char * c_found
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 871, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 907, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 871, __pyx_L1_error)
+    __PYX_ERR(0, 907, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":870
+    /* "gsd/fl.pyx":906
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":875
+  /* "gsd/fl.pyx":911
  *         cdef const char * c_found
  *         cdef char * c_match
  *         match_e = match.encode('utf-8')             # <<<<<<<<<<<<<<
  *         c_match = match_e
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 875, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_match, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 911, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 875, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 911, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_match_e = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":876
+  /* "gsd/fl.pyx":912
  *         cdef char * c_match
  *         match_e = match.encode('utf-8')
  *         c_match = match_e             # <<<<<<<<<<<<<<
  * 
  *         retval = []
  */
-  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_match_e); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 876, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_v_match_e); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 912, __pyx_L1_error)
   __pyx_v_c_match = __pyx_t_5;
 
-  /* "gsd/fl.pyx":878
+  /* "gsd/fl.pyx":914
  *         c_match = match_e
  * 
  *         retval = []             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 878, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 914, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_retval = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":880
+  /* "gsd/fl.pyx":916
  *         retval = []
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,
  *                                                           c_match,
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":881
+        /* "gsd/fl.pyx":917
  * 
  *         with nogil:
  *             c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,             # <<<<<<<<<<<<<<
  *                                                           c_match,
  *                                                           NULL)
  */
         __pyx_v_c_found = gsd_find_matching_chunk_name((&__pyx_v_self->__pyx___handle), __pyx_v_c_match, NULL);
       }
 
-      /* "gsd/fl.pyx":880
+      /* "gsd/fl.pyx":916
  *         retval = []
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,
  *                                                           c_match,
  */
       /*finally:*/ {
@@ -9167,63 +9566,63 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":885
+  /* "gsd/fl.pyx":921
  *                                                           NULL)
  * 
  *         while c_found != NULL:             # <<<<<<<<<<<<<<
  *             retval.append(c_found.decode('utf-8'))
  * 
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_c_found != NULL) != 0);
     if (!__pyx_t_1) break;
 
-    /* "gsd/fl.pyx":886
+    /* "gsd/fl.pyx":922
  * 
  *         while c_found != NULL:
  *             retval.append(c_found.decode('utf-8'))             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_c_found, 0, strlen(__pyx_v_c_found), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 886, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_c_found, 0, strlen(__pyx_v_c_found), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 922, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_retval, __pyx_t_2); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 886, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_retval, __pyx_t_2); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 922, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":888
+    /* "gsd/fl.pyx":924
  *             retval.append(c_found.decode('utf-8'))
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,
  *                                                               c_match,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "gsd/fl.pyx":889
+          /* "gsd/fl.pyx":925
  * 
  *             with nogil:
  *                 c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,             # <<<<<<<<<<<<<<
  *                                                               c_match,
  *                                                               c_found)
  */
           __pyx_v_c_found = gsd_find_matching_chunk_name((&__pyx_v_self->__pyx___handle), __pyx_v_c_match, __pyx_v_c_found);
         }
 
-        /* "gsd/fl.pyx":888
+        /* "gsd/fl.pyx":924
  *             retval.append(c_found.decode('utf-8'))
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 c_found = libgsd.gsd_find_matching_chunk_name(&self.__handle,
  *                                                               c_match,
  */
         /*finally:*/ {
@@ -9235,27 +9634,27 @@
             goto __pyx_L13;
           }
           __pyx_L13:;
         }
     }
   }
 
-  /* "gsd/fl.pyx":893
+  /* "gsd/fl.pyx":929
  *                                                               c_found)
  * 
  *         return retval             # <<<<<<<<<<<<<<
  * 
  *     def upgrade(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_retval);
   __pyx_r = __pyx_v_retval;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":827
+  /* "gsd/fl.pyx":863
  *             return data_array
  * 
  *     def find_matching_chunk_names(self, match):             # <<<<<<<<<<<<<<
  *         """find_matching_chunk_names(match)
  * 
  */
 
@@ -9270,15 +9669,15 @@
   __Pyx_XDECREF(__pyx_v_match_e);
   __Pyx_XDECREF(__pyx_v_retval);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":895
+/* "gsd/fl.pyx":931
  *         return retval
  * 
  *     def upgrade(self):             # <<<<<<<<<<<<<<
  *         """upgrade()
  * 
  */
 
@@ -9306,104 +9705,104 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("upgrade", 0);
 
-  /* "gsd/fl.pyx":903
+  /* "gsd/fl.pyx":939
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":904
+    /* "gsd/fl.pyx":940
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         logger.info('upgrading file: ' + self.name)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 904, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 940, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 904, __pyx_L1_error)
+    __PYX_ERR(0, 940, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":903
+    /* "gsd/fl.pyx":939
  *         """
  * 
  *         if not self.__is_open:             # <<<<<<<<<<<<<<
  *             raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":906
+  /* "gsd/fl.pyx":942
  *             raise ValueError("File is not open")
  * 
  *         logger.info('upgrading file: ' + self.name)             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 906, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 906, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_upgrading_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 906, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_upgrading_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 906, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":908
+  /* "gsd/fl.pyx":944
  *         logger.info('upgrading file: ' + self.name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_upgrade(&self.__handle)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "gsd/fl.pyx":909
+        /* "gsd/fl.pyx":945
  * 
  *         with nogil:
  *             retval = libgsd.gsd_upgrade(&self.__handle)             # <<<<<<<<<<<<<<
  * 
  *         __raise_on_error(retval, self.name)
  */
         __pyx_v_retval = gsd_upgrade((&__pyx_v_self->__pyx___handle));
       }
 
-      /* "gsd/fl.pyx":908
+      /* "gsd/fl.pyx":944
  *         logger.info('upgrading file: ' + self.name)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             retval = libgsd.gsd_upgrade(&self.__handle)
  * 
  */
       /*finally:*/ {
@@ -9414,32 +9813,32 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "gsd/fl.pyx":911
+  /* "gsd/fl.pyx":947
  *             retval = libgsd.gsd_upgrade(&self.__handle)
  * 
  *         __raise_on_error(retval, self.name)             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_retval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_4);
-  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_3gsd_2fl___raise_on_error(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "gsd/fl.pyx":895
+  /* "gsd/fl.pyx":931
  *         return retval
  * 
  *     def upgrade(self):             # <<<<<<<<<<<<<<
  *         """upgrade()
  * 
  */
 
@@ -9455,15 +9854,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":913
+/* "gsd/fl.pyx":949
  *         __raise_on_error(retval, self.name)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -9481,42 +9880,42 @@
 }
 
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_18__enter__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "gsd/fl.pyx":914
+  /* "gsd/fl.pyx":950
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, exc_type, exc_value, traceback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":913
+  /* "gsd/fl.pyx":949
  *         __raise_on_error(retval, self.name)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":916
+/* "gsd/fl.pyx":952
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -9553,40 +9952,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 916, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 952, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_traceback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 916, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 952, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 916, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 952, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_exc_type = values[0];
     __pyx_v_exc_value = values[1];
     __pyx_v_traceback = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 916, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 952, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gsd.fl.GSDFile.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3gsd_2fl_7GSDFile_20__exit__(((struct __pyx_obj_3gsd_2fl_GSDFile *)__pyx_v_self), __pyx_v_exc_type, __pyx_v_exc_value, __pyx_v_traceback);
 
@@ -9602,41 +10001,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "gsd/fl.pyx":917
+  /* "gsd/fl.pyx":953
  * 
  *     def __exit__(self, exc_type, exc_value, traceback):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def __reduce__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 917, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 953, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 917, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 953, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "gsd/fl.pyx":916
+  /* "gsd/fl.pyx":952
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -9651,20 +10050,20 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":919
+/* "gsd/fl.pyx":955
  *         self.close()
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         """Allows filehandles to be pickled when in read only mode."""
- *         if self.mode not in ['rb', 'rb+']:
+ *         if self.mode not in ['rb', 'r']:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_23__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static char __pyx_doc_3gsd_2fl_7GSDFile_22__reduce__[] = "Allows filehandles to be pickled when in read only mode.";
 static PyObject *__pyx_pw_3gsd_2fl_7GSDFile_23__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
@@ -9689,114 +10088,114 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce__", 0);
 
-  /* "gsd/fl.pyx":921
+  /* "gsd/fl.pyx":957
  *     def __reduce__(self):
  *         """Allows filehandles to be pickled when in read only mode."""
- *         if self.mode not in ['rb', 'rb+']:             # <<<<<<<<<<<<<<
+ *         if self.mode not in ['rb', 'r']:             # <<<<<<<<<<<<<<
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,
  */
   __Pyx_INCREF(__pyx_v_self->mode);
   __pyx_t_1 = __pyx_v_self->mode;
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_rb, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 921, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_rb, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 957, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u_rb_2, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 921, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_r, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 957, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "gsd/fl.pyx":922
+    /* "gsd/fl.pyx":958
  *         """Allows filehandles to be pickled when in read only mode."""
- *         if self.mode not in ['rb', 'rb+']:
+ *         if self.mode not in ['rb', 'r']:
  *             raise PickleError("Only read only GSDFiles can be pickled.")             # <<<<<<<<<<<<<<
  *         return (GSDFile,
  *                 (self.name, self.mode, self.application,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 922, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 958, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_kp_u_Only_read_only_GSDFiles_can_be_p) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_kp_u_Only_read_only_GSDFiles_can_be_p);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 922, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 958, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 922, __pyx_L1_error)
+    __PYX_ERR(0, 958, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":921
+    /* "gsd/fl.pyx":957
  *     def __reduce__(self):
  *         """Allows filehandles to be pickled when in read only mode."""
- *         if self.mode not in ['rb', 'rb+']:             # <<<<<<<<<<<<<<
+ *         if self.mode not in ['rb', 'r']:             # <<<<<<<<<<<<<<
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,
  */
   }
 
-  /* "gsd/fl.pyx":923
- *         if self.mode not in ['rb', 'rb+']:
+  /* "gsd/fl.pyx":959
+ *         if self.mode not in ['rb', 'r']:
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,             # <<<<<<<<<<<<<<
  *                 (self.name, self.mode, self.application,
  *                     self.schema, self.schema_version),
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "gsd/fl.pyx":924
+  /* "gsd/fl.pyx":960
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,
  *                 (self.name, self.mode, self.application,             # <<<<<<<<<<<<<<
  *                     self.schema, self.schema_version),
  *                 )
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_application); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 924, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_application); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 960, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "gsd/fl.pyx":925
+  /* "gsd/fl.pyx":961
  *         return (GSDFile,
  *                 (self.name, self.mode, self.application,
  *                     self.schema, self.schema_version),             # <<<<<<<<<<<<<<
  *                 )
  * 
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 925, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 961, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema_version); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 925, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_schema_version); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 961, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "gsd/fl.pyx":924
+  /* "gsd/fl.pyx":960
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,
  *                 (self.name, self.mode, self.application,             # <<<<<<<<<<<<<<
  *                     self.schema, self.schema_version),
  *                 )
  */
-  __pyx_t_8 = PyTuple_New(5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 924, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 960, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_v_self->name);
   __Pyx_GIVEREF(__pyx_v_self->name);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_self->name);
   __Pyx_INCREF(__pyx_v_self->mode);
   __Pyx_GIVEREF(__pyx_v_self->mode);
   PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_self->mode);
@@ -9806,39 +10205,39 @@
   PyTuple_SET_ITEM(__pyx_t_8, 3, __pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_8, 4, __pyx_t_7);
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
 
-  /* "gsd/fl.pyx":923
- *         if self.mode not in ['rb', 'rb+']:
+  /* "gsd/fl.pyx":959
+ *         if self.mode not in ['rb', 'r']:
  *             raise PickleError("Only read only GSDFiles can be pickled.")
  *         return (GSDFile,             # <<<<<<<<<<<<<<
  *                 (self.name, self.mode, self.application,
  *                     self.schema, self.schema_version),
  */
-  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 923, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 959, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile));
   PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)__pyx_ptype_3gsd_2fl_GSDFile));
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_8);
   __pyx_t_8 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":919
+  /* "gsd/fl.pyx":955
  *         self.close()
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         """Allows filehandles to be pickled when in read only mode."""
- *         if self.mode not in ['rb', 'rb+']:
+ *         if self.mode not in ['rb', 'r']:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
@@ -9848,15 +10247,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":929
+/* "gsd/fl.pyx":965
  * 
  *     property name:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.name
  * 
  */
 
@@ -9874,42 +10273,42 @@
 }
 
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4name___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":930
+  /* "gsd/fl.pyx":966
  *     property name:
  *         def __get__(self):
  *             return self.name             # <<<<<<<<<<<<<<
  * 
  *     property mode:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_r = __pyx_v_self->name;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":929
+  /* "gsd/fl.pyx":965
  * 
  *     property name:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.name
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":933
+/* "gsd/fl.pyx":969
  * 
  *     property mode:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.mode
  * 
  */
 
@@ -9927,42 +10326,42 @@
 }
 
 static PyObject *__pyx_pf_3gsd_2fl_7GSDFile_4mode___get__(struct __pyx_obj_3gsd_2fl_GSDFile *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":934
+  /* "gsd/fl.pyx":970
  *     property mode:
  *         def __get__(self):
  *             return self.mode             # <<<<<<<<<<<<<<
  * 
  *     property gsd_version:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->mode);
   __pyx_r = __pyx_v_self->mode;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":933
+  /* "gsd/fl.pyx":969
  * 
  *     property mode:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.mode
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":937
+/* "gsd/fl.pyx":973
  * 
  *     property gsd_version:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             cdef uint32_t v = self.__handle.header.gsd_version
  *             return (v >> 16, v & 0xffff)
  */
 
@@ -9988,49 +10387,49 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":938
+  /* "gsd/fl.pyx":974
  *     property gsd_version:
  *         def __get__(self):
  *             cdef uint32_t v = self.__handle.header.gsd_version             # <<<<<<<<<<<<<<
  *             return (v >> 16, v & 0xffff)
  * 
  */
   __pyx_t_1 = __pyx_v_self->__pyx___handle.header.gsd_version;
   __pyx_v_v = __pyx_t_1;
 
-  /* "gsd/fl.pyx":939
+  /* "gsd/fl.pyx":975
  *         def __get__(self):
  *             cdef uint32_t v = self.__handle.header.gsd_version
  *             return (v >> 16, v & 0xffff)             # <<<<<<<<<<<<<<
  * 
  *     property schema_version:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_v >> 16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 939, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_v >> 16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 975, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_long((__pyx_v_v & 0xffff)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 939, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long((__pyx_v_v & 0xffff)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 975, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 939, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 975, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":937
+  /* "gsd/fl.pyx":973
  * 
  *     property gsd_version:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             cdef uint32_t v = self.__handle.header.gsd_version
  *             return (v >> 16, v & 0xffff)
  */
 
@@ -10043,15 +10442,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":942
+/* "gsd/fl.pyx":978
  * 
  *     property schema_version:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             cdef uint32_t v = self.__handle.header.schema_version
  *             return (v >> 16, v & 0xffff)
  */
 
@@ -10077,49 +10476,49 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":943
+  /* "gsd/fl.pyx":979
  *     property schema_version:
  *         def __get__(self):
  *             cdef uint32_t v = self.__handle.header.schema_version             # <<<<<<<<<<<<<<
  *             return (v >> 16, v & 0xffff)
  * 
  */
   __pyx_t_1 = __pyx_v_self->__pyx___handle.header.schema_version;
   __pyx_v_v = __pyx_t_1;
 
-  /* "gsd/fl.pyx":944
+  /* "gsd/fl.pyx":980
  *         def __get__(self):
  *             cdef uint32_t v = self.__handle.header.schema_version
  *             return (v >> 16, v & 0xffff)             # <<<<<<<<<<<<<<
  * 
  *     property schema:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_v >> 16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_v >> 16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 980, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_long((__pyx_v_v & 0xffff)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long((__pyx_v_v & 0xffff)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 980, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 980, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":942
+  /* "gsd/fl.pyx":978
  * 
  *     property schema_version:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             cdef uint32_t v = self.__handle.header.schema_version
  *             return (v >> 16, v & 0xffff)
  */
 
@@ -10132,15 +10531,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":947
+/* "gsd/fl.pyx":983
  * 
  *     property schema:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.__handle.header.schema.decode('utf-8')
  * 
  */
 
@@ -10163,31 +10562,31 @@
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":948
+  /* "gsd/fl.pyx":984
  *     property schema:
  *         def __get__(self):
  *             return self.__handle.header.schema.decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  *     property application:
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->__pyx___handle.header.schema;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 948, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":947
+  /* "gsd/fl.pyx":983
  * 
  *     property schema:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.__handle.header.schema.decode('utf-8')
  * 
  */
 
@@ -10198,15 +10597,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":951
+/* "gsd/fl.pyx":987
  * 
  *     property application:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.__handle.header.application.decode('utf-8')
  * 
  */
 
@@ -10229,31 +10628,31 @@
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":952
+  /* "gsd/fl.pyx":988
  *     property application:
  *         def __get__(self):
  *             return self.__handle.header.application.decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  *     property nframes:
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->__pyx___handle.header.application;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 952, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 988, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":951
+  /* "gsd/fl.pyx":987
  * 
  *     property application:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             return self.__handle.header.application.decode('utf-8')
  * 
  */
 
@@ -10264,15 +10663,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":955
+/* "gsd/fl.pyx":991
  * 
  *     property nframes:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if not self.__is_open:
  *                 raise ValueError("File is not open")
  */
 
@@ -10295,61 +10694,61 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gsd/fl.pyx":956
+  /* "gsd/fl.pyx":992
  *     property nframes:
  *         def __get__(self):
  *             if not self.__is_open:             # <<<<<<<<<<<<<<
  *                 raise ValueError("File is not open")
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->__pyx___is_open != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "gsd/fl.pyx":957
+    /* "gsd/fl.pyx":993
  *         def __get__(self):
  *             if not self.__is_open:
  *                 raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *             return libgsd.gsd_get_nframes(&self.__handle)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 957, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 993, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 957, __pyx_L1_error)
+    __PYX_ERR(0, 993, __pyx_L1_error)
 
-    /* "gsd/fl.pyx":956
+    /* "gsd/fl.pyx":992
  *     property nframes:
  *         def __get__(self):
  *             if not self.__is_open:             # <<<<<<<<<<<<<<
  *                 raise ValueError("File is not open")
  * 
  */
   }
 
-  /* "gsd/fl.pyx":959
+  /* "gsd/fl.pyx":995
  *                 raise ValueError("File is not open")
  * 
  *             return libgsd.gsd_get_nframes(&self.__handle)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(gsd_get_nframes((&__pyx_v_self->__pyx___handle))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 959, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(gsd_get_nframes((&__pyx_v_self->__pyx___handle))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 995, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gsd/fl.pyx":955
+  /* "gsd/fl.pyx":991
  * 
  *     property nframes:
  *         def __get__(self):             # <<<<<<<<<<<<<<
  *             if not self.__is_open:
  *                 raise ValueError("File is not open")
  */
 
@@ -10360,15 +10759,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gsd/fl.pyx":961
+/* "gsd/fl.pyx":997
  *             return libgsd.gsd_get_nframes(&self.__handle)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  */
 
@@ -10391,81 +10790,81 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "gsd/fl.pyx":962
+  /* "gsd/fl.pyx":998
  * 
  *     def __dealloc__(self):
  *         if self.__is_open:             # <<<<<<<<<<<<<<
  *             logger.info('closing file: ' + self.name)
  *             libgsd.gsd_close(&self.__handle)
  */
   __pyx_t_1 = (__pyx_v_self->__pyx___is_open != 0);
   if (__pyx_t_1) {
 
-    /* "gsd/fl.pyx":963
+    /* "gsd/fl.pyx":999
  *     def __dealloc__(self):
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)             # <<<<<<<<<<<<<<
  *             libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 963, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 999, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 963, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 999, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_closing_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 963, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u_closing_file, __pyx_v_self->name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 999, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 963, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 999, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "gsd/fl.pyx":964
+    /* "gsd/fl.pyx":1000
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  *             libgsd.gsd_close(&self.__handle)             # <<<<<<<<<<<<<<
  *             self.__is_open = False
  */
     (void)(gsd_close((&__pyx_v_self->__pyx___handle)));
 
-    /* "gsd/fl.pyx":965
+    /* "gsd/fl.pyx":1001
  *             logger.info('closing file: ' + self.name)
  *             libgsd.gsd_close(&self.__handle)
  *             self.__is_open = False             # <<<<<<<<<<<<<<
  */
     __pyx_v_self->__pyx___is_open = 0;
 
-    /* "gsd/fl.pyx":962
+    /* "gsd/fl.pyx":998
  * 
  *     def __dealloc__(self):
  *         if self.__is_open:             # <<<<<<<<<<<<<<
  *             logger.info('closing file: ' + self.name)
  *             libgsd.gsd_close(&self.__handle)
  */
   }
 
-  /* "gsd/fl.pyx":961
+  /* "gsd/fl.pyx":997
  *             return libgsd.gsd_get_nframes(&self.__handle)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         if self.__is_open:
  *             logger.info('closing file: ' + self.name)
  */
 
@@ -10477,15 +10876,15 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_WriteUnraisable("gsd.fl.GSDFile.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10494,29 +10893,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10527,15 +10926,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10544,29 +10943,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10577,15 +10976,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10594,29 +10993,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10627,15 +11026,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10644,29 +11043,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10677,15 +11076,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10694,29 +11093,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10727,212 +11126,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10948,15 +11347,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -10964,84 +11363,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11056,15 +11455,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11080,15 +11479,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11096,84 +11495,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11188,15 +11587,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11212,15 +11611,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11228,84 +11627,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11320,176 +11719,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -11705,34 +12104,44 @@
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_Corrupt_GSD_file, __pyx_k_Corrupt_GSD_file, sizeof(__pyx_k_Corrupt_GSD_file), 0, 1, 0, 0},
   {&__pyx_kp_u_File_is_not_open, __pyx_k_File_is_not_open, sizeof(__pyx_k_File_is_not_open), 0, 1, 0, 0},
   {&__pyx_kp_u_File_must_be_readable, __pyx_k_File_must_be_readable, sizeof(__pyx_k_File_must_be_readable), 0, 1, 0, 0},
   {&__pyx_kp_u_File_must_be_writable, __pyx_k_File_must_be_writable, sizeof(__pyx_k_File_must_be_writable), 0, 1, 0, 0},
+  {&__pyx_n_s_FutureWarning, __pyx_k_FutureWarning, sizeof(__pyx_k_FutureWarning), 0, 0, 1, 1},
   {&__pyx_n_s_GSDFile, __pyx_k_GSDFile, sizeof(__pyx_k_GSDFile), 0, 0, 1, 1},
   {&__pyx_kp_u_GSD_can_only_write_1_or_2_dimens, __pyx_k_GSD_can_only_write_1_or_2_dimens, sizeof(__pyx_k_GSD_can_only_write_1_or_2_dimens), 0, 1, 0, 0},
   {&__pyx_kp_u_GSD_namelist_is_full, __pyx_k_GSD_namelist_is_full, sizeof(__pyx_k_GSD_namelist_is_full), 0, 1, 0, 0},
   {&__pyx_n_s_IOError, __pyx_k_IOError, sizeof(__pyx_k_IOError), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_u_Invalid_gsd_argument, __pyx_k_Invalid_gsd_argument, sizeof(__pyx_k_Invalid_gsd_argument), 0, 1, 0, 0},
+  {&__pyx_kp_u_Invalid_mode, __pyx_k_Invalid_mode, sizeof(__pyx_k_Invalid_mode), 0, 1, 0, 0},
   {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_u_Memory_allocation_failed, __pyx_k_Memory_allocation_failed, sizeof(__pyx_k_Memory_allocation_failed), 0, 1, 0, 0},
   {&__pyx_kp_u_Not_a_GSD_file, __pyx_k_Not_a_GSD_file, sizeof(__pyx_k_Not_a_GSD_file), 0, 1, 0, 0},
   {&__pyx_kp_u_Only_read_only_GSDFiles_can_be_p, __pyx_k_Only_read_only_GSDFiles_can_be_p, sizeof(__pyx_k_Only_read_only_GSDFiles_can_be_p), 0, 1, 0, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_kp_u_Provide_application_when_creatin, __pyx_k_Provide_application_when_creatin, sizeof(__pyx_k_Provide_application_when_creatin), 0, 1, 0, 0},
   {&__pyx_kp_u_Provide_schema_version_when_crea, __pyx_k_Provide_schema_version_when_crea, sizeof(__pyx_k_Provide_schema_version_when_crea), 0, 1, 0, 0},
   {&__pyx_kp_u_Provide_schema_when_creating_a_f, __pyx_k_Provide_schema_when_creating_a_f, sizeof(__pyx_k_Provide_schema_when_creating_a_f), 0, 1, 0, 0},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
+  {&__pyx_kp_u_The_ab_mode_is_deprecated_use_r, __pyx_k_The_ab_mode_is_deprecated_use_r, sizeof(__pyx_k_The_ab_mode_is_deprecated_use_r), 0, 1, 0, 0},
+  {&__pyx_kp_u_The_rb_mode_is_deprecated_use_r, __pyx_k_The_rb_mode_is_deprecated_use_r, sizeof(__pyx_k_The_rb_mode_is_deprecated_use_r), 0, 1, 0, 0},
+  {&__pyx_kp_u_The_rb_mode_is_deprecated_use_r_2, __pyx_k_The_rb_mode_is_deprecated_use_r_2, sizeof(__pyx_k_The_rb_mode_is_deprecated_use_r_2), 0, 1, 0, 0},
+  {&__pyx_kp_u_The_wb_mode_is_deprecated_use_w, __pyx_k_The_wb_mode_is_deprecated_use_w, sizeof(__pyx_k_The_wb_mode_is_deprecated_use_w), 0, 1, 0, 0},
+  {&__pyx_kp_u_The_wb_mode_is_deprecated_use_w_2, __pyx_k_The_wb_mode_is_deprecated_use_w_2, sizeof(__pyx_k_The_wb_mode_is_deprecated_use_w_2), 0, 1, 0, 0},
+  {&__pyx_kp_u_The_xb_mode_is_deprecated_use_x, __pyx_k_The_xb_mode_is_deprecated_use_x, sizeof(__pyx_k_The_xb_mode_is_deprecated_use_x), 0, 1, 0, 0},
+  {&__pyx_kp_u_The_xb_mode_is_deprecated_use_x_2, __pyx_k_The_xb_mode_is_deprecated_use_x_2, sizeof(__pyx_k_The_xb_mode_is_deprecated_use_x_2), 0, 1, 0, 0},
   {&__pyx_kp_u_Unknown_error, __pyx_k_Unknown_error, sizeof(__pyx_k_Unknown_error), 0, 1, 0, 0},
   {&__pyx_kp_u_Unsupported_GSD_file_version, __pyx_k_Unsupported_GSD_file_version, sizeof(__pyx_k_Unsupported_GSD_file_version), 0, 1, 0, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-  {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
+  {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
+  {&__pyx_n_u_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 1, 0, 1},
   {&__pyx_n_u_ab, __pyx_k_ab, sizeof(__pyx_k_ab), 0, 1, 0, 1},
   {&__pyx_kp_u_and_schema_version, __pyx_k_and_schema_version, sizeof(__pyx_k_and_schema_version), 0, 1, 0, 0},
   {&__pyx_n_s_application, __pyx_k_application, sizeof(__pyx_k_application), 0, 0, 1, 1},
   {&__pyx_kp_u_application_2, __pyx_k_application_2, sizeof(__pyx_k_application_2), 0, 1, 0, 0},
   {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
   {&__pyx_kp_u_chunk, __pyx_k_chunk, sizeof(__pyx_k_chunk), 0, 1, 0, 0},
   {&__pyx_kp_u_chunk_exists, __pyx_k_chunk_exists, sizeof(__pyx_k_chunk_exists), 0, 1, 0, 0},
@@ -11743,14 +12152,15 @@
   {&__pyx_n_s_debug, __pyx_k_debug, sizeof(__pyx_k_debug), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_kp_u_end_frame, __pyx_k_end_frame, sizeof(__pyx_k_end_frame), 0, 1, 0, 0},
   {&__pyx_n_s_exc_type, __pyx_k_exc_type, sizeof(__pyx_k_exc_type), 0, 0, 1, 1},
   {&__pyx_n_s_exc_value, __pyx_k_exc_value, sizeof(__pyx_k_exc_value), 0, 0, 1, 1},
+  {&__pyx_n_s_exists, __pyx_k_exists, sizeof(__pyx_k_exists), 0, 0, 1, 1},
   {&__pyx_kp_u_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 1, 0, 0},
   {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
   {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
   {&__pyx_n_s_frame, __pyx_k_frame, sizeof(__pyx_k_frame), 0, 0, 1, 1},
   {&__pyx_kp_u_frame_2, __pyx_k_frame_2, sizeof(__pyx_k_frame_2), 0, 1, 0, 0},
   {&__pyx_n_s_getLogger, __pyx_k_getLogger, sizeof(__pyx_k_getLogger), 0, 0, 1, 1},
   {&__pyx_n_s_gsd_fl, __pyx_k_gsd_fl, sizeof(__pyx_k_gsd_fl), 0, 0, 1, 1},
@@ -11765,26 +12175,28 @@
   {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
   {&__pyx_n_s_int8, __pyx_k_int8, sizeof(__pyx_k_int8), 0, 0, 1, 1},
   {&__pyx_kp_u_invalid_type_for_chunk, __pyx_k_invalid_type_for_chunk, sizeof(__pyx_k_invalid_type_for_chunk), 0, 1, 0, 0},
   {&__pyx_n_s_logger, __pyx_k_logger, sizeof(__pyx_k_logger), 0, 0, 1, 1},
   {&__pyx_n_s_logging, __pyx_k_logging, sizeof(__pyx_k_logging), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
-  {&__pyx_kp_u_mode_must_be_wb_wb_rb_rb_xb_xb_o, __pyx_k_mode_must_be_wb_wb_rb_rb_xb_xb_o, sizeof(__pyx_k_mode_must_be_wb_wb_rb_rb_xb_xb_o), 0, 1, 0, 0},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_kp_u_not_found_in, __pyx_k_not_found_in, sizeof(__pyx_k_not_found_in), 0, 1, 0, 0},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
   {&__pyx_kp_u_opening_file, __pyx_k_opening_file, sizeof(__pyx_k_opening_file), 0, 1, 0, 0},
   {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
   {&__pyx_kp_u_overwriting_file, __pyx_k_overwriting_file, sizeof(__pyx_k_overwriting_file), 0, 1, 0, 0},
+  {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
+  {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
+  {&__pyx_kp_u_r_2, __pyx_k_r_2, sizeof(__pyx_k_r_2), 0, 1, 0, 0},
   {&__pyx_n_u_rb, __pyx_k_rb, sizeof(__pyx_k_rb), 0, 1, 0, 1},
   {&__pyx_kp_u_rb_2, __pyx_k_rb_2, sizeof(__pyx_k_rb_2), 0, 1, 0, 0},
   {&__pyx_kp_u_read_chunk, __pyx_k_read_chunk, sizeof(__pyx_k_read_chunk), 0, 1, 0, 0},
   {&__pyx_n_s_reshape, __pyx_k_reshape, sizeof(__pyx_k_reshape), 0, 0, 1, 1},
   {&__pyx_n_s_schema, __pyx_k_schema, sizeof(__pyx_k_schema), 0, 0, 1, 1},
   {&__pyx_kp_u_schema_2, __pyx_k_schema_2, sizeof(__pyx_k_schema_2), 0, 1, 0, 0},
   {&__pyx_n_s_schema_version, __pyx_k_schema_version, sizeof(__pyx_k_schema_version), 0, 0, 1, 1},
@@ -11797,138 +12209,209 @@
   {&__pyx_n_s_uint16, __pyx_k_uint16, sizeof(__pyx_k_uint16), 0, 0, 1, 1},
   {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
   {&__pyx_n_s_uint64, __pyx_k_uint64, sizeof(__pyx_k_uint64), 0, 0, 1, 1},
   {&__pyx_n_s_uint8, __pyx_k_uint8, sizeof(__pyx_k_uint8), 0, 0, 1, 1},
   {&__pyx_kp_u_upgrading_file, __pyx_k_upgrading_file, sizeof(__pyx_k_upgrading_file), 0, 1, 0, 0},
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
+  {&__pyx_n_u_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 1, 0, 1},
+  {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
   {&__pyx_n_s_warning, __pyx_k_warning, sizeof(__pyx_k_warning), 0, 0, 1, 1},
+  {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
   {&__pyx_n_u_wb, __pyx_k_wb, sizeof(__pyx_k_wb), 0, 1, 0, 1},
   {&__pyx_kp_u_wb_2, __pyx_k_wb_2, sizeof(__pyx_k_wb_2), 0, 1, 0, 0},
   {&__pyx_kp_u_with_mode, __pyx_k_with_mode, sizeof(__pyx_k_with_mode), 0, 1, 0, 0},
   {&__pyx_kp_u_write_chunk, __pyx_k_write_chunk, sizeof(__pyx_k_write_chunk), 0, 1, 0, 0},
+  {&__pyx_n_u_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 1, 0, 1},
   {&__pyx_n_u_xb, __pyx_k_xb, sizeof(__pyx_k_xb), 0, 1, 0, 1},
   {&__pyx_kp_u_xb_2, __pyx_k_xb_2, sizeof(__pyx_k_xb_2), 0, 1, 0, 0},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_IOError = __Pyx_GetBuiltinName(__pyx_n_s_IOError); if (!__pyx_builtin_IOError) __PYX_ERR(0, 42, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 44, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 50, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 322, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 747, __pyx_L1_error)
+  __pyx_builtin_IOError = __Pyx_GetBuiltinName(__pyx_n_s_IOError); if (!__pyx_builtin_IOError) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_builtin_FutureWarning = __Pyx_GetBuiltinName(__pyx_n_s_FutureWarning); if (!__pyx_builtin_FutureWarning) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 783, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "gsd/fl.pyx":322
- *             c_flags = libgsd.GSD_OPEN_APPEND
- *         else:
- *             raise ValueError("mode must be 'wb', 'wb+', 'rb', 'rb+', "             # <<<<<<<<<<<<<<
- *                              "'xb', 'xb+', or 'ab'")
- * 
+  /* "gsd/fl.pyx":317
+ *         if mode == 'wb':
+ *             mode = 'w'
+ *             warnings.warn("The 'wb' mode is deprecated, use 'w'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'wb+':
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_mode_must_be_wb_wb_rb_rb_xb_xb_o); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(2, __pyx_kp_u_The_wb_mode_is_deprecated_use_w, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "gsd/fl.pyx":336
+  /* "gsd/fl.pyx":321
+ *         elif mode == 'wb+':
+ *             mode = 'w'
+ *             warnings.warn("The 'wb+' mode is deprecated, use 'w'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'rb':
+ */
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_kp_u_The_wb_mode_is_deprecated_use_w_2, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  /* "gsd/fl.pyx":325
+ *         elif mode == 'rb':
+ *             mode = 'r'
+ *             warnings.warn("The 'rb' mode is deprecated, use 'r'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'rb+':
+ */
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_kp_u_The_rb_mode_is_deprecated_use_r, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+
+  /* "gsd/fl.pyx":329
+ *         elif mode == 'rb+':
+ *             mode = 'r+'
+ *             warnings.warn("The 'rb+' mode is deprecated, use 'r+'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'xb':
+ */
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_kp_u_The_rb_mode_is_deprecated_use_r_2, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+
+  /* "gsd/fl.pyx":333
+ *         elif mode == 'xb':
+ *             mode = 'x'
+ *             warnings.warn("The 'xb' mode is deprecated, use 'x'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'xb+':
+ */
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_kp_u_The_xb_mode_is_deprecated_use_x, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+
+  /* "gsd/fl.pyx":337
+ *         elif mode == 'xb+':
+ *             mode = 'x'
+ *             warnings.warn("The 'xb+' mode is deprecated, use 'x'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ *         elif mode == 'ab':
+ */
+  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_kp_u_The_xb_mode_is_deprecated_use_x_2, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+
+  /* "gsd/fl.pyx":341
+ *         elif mode == 'ab':
+ *             mode = 'r+'
+ *             warnings.warn("The 'ab' mode is deprecated, use 'r+'",             # <<<<<<<<<<<<<<
+ *                            FutureWarning)
+ * 
+ */
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_kp_u_The_ab_mode_is_deprecated_use_r, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+
+  /* "gsd/fl.pyx":372
  *         if overwrite:
  *             if application is None:
  *                 raise ValueError("Provide application when creating a file")             # <<<<<<<<<<<<<<
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Provide_application_when_creatin); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 336, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Provide_application_when_creatin); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "gsd/fl.pyx":338
+  /* "gsd/fl.pyx":374
  *                 raise ValueError("Provide application when creating a file")
  *             if schema is None:
  *                 raise ValueError("Provide schema when creating a file")             # <<<<<<<<<<<<<<
  *             if schema_version is None:
  *                 raise ValueError("Provide schema_version when creating a file")
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Provide_schema_when_creating_a_f); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 338, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Provide_schema_when_creating_a_f); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "gsd/fl.pyx":340
+  /* "gsd/fl.pyx":376
  *                 raise ValueError("Provide schema when creating a file")
  *             if schema_version is None:
  *                 raise ValueError("Provide schema_version when creating a file")             # <<<<<<<<<<<<<<
  * 
  *             # create a new file or overwrite an existing one
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Provide_schema_version_when_crea); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 340, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Provide_schema_version_when_crea); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "gsd/fl.pyx":455
+  /* "gsd/fl.pyx":491
  * 
  *         if not self.__is_open:
  *             raise ValueError("File is not open")             # <<<<<<<<<<<<<<
  * 
  *         logger.info('truncating file: ' + self.name)
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_File_is_not_open); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 455, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_File_is_not_open); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "gsd/fl.pyx":25
+  /* "gsd/fl.pyx":26
  * cimport numpy
  * 
  * logger = logging.getLogger('gsd.fl')             # <<<<<<<<<<<<<<
  * 
  * ####################
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_gsd_fl); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_gsd_fl); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "gsd/fl.pyx":148
+  /* "gsd/fl.pyx":149
  * 
  * 
  * def open(name, mode, application=None, schema=None, schema_version=None):             # <<<<<<<<<<<<<<
  *     """open(name, mode, application=None, schema=None, schema_version=None)
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(5, __pyx_n_s_name, __pyx_n_s_mode, __pyx_n_s_application, __pyx_n_s_schema, __pyx_n_s_schema_version); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gsd_fl_pyx, __pyx_n_s_open, 148, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_name, __pyx_n_s_mode, __pyx_n_s_application, __pyx_n_s_schema, __pyx_n_s_schema_version); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gsd_fl_pyx, __pyx_n_s_open, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -11976,22 +12459,22 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_3gsd_2fl_GSDFile) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_3gsd_2fl_GSDFile) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_3gsd_2fl_GSDFile.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_3gsd_2fl_GSDFile.tp_dictoffset && __pyx_type_3gsd_2fl_GSDFile.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_3gsd_2fl_GSDFile.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_GSDFile, (PyObject *)&__pyx_type_3gsd_2fl_GSDFile) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_GSDFile, (PyObject *)&__pyx_type_3gsd_2fl_GSDFile) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
   __pyx_ptype_3gsd_2fl_GSDFile = &__pyx_type_3gsd_2fl_GSDFile;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -12313,27 +12796,27 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "gsd/fl.pyx":17
  * import logging
  * import numpy
  * import os             # <<<<<<<<<<<<<<
  * from pickle import PickleError
- * from libc.stdint cimport uint8_t, int8_t, uint16_t, int16_t, uint32_t, int32_t,\
+ * import warnings
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_os, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_os, __pyx_t_1) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "gsd/fl.pyx":18
  * import numpy
  * import os
  * from pickle import PickleError             # <<<<<<<<<<<<<<
+ * import warnings
  * from libc.stdint cimport uint8_t, int8_t, uint16_t, int16_t, uint32_t, int32_t,\
- *     uint64_t, int64_t
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_PickleError);
   __Pyx_GIVEREF(__pyx_n_s_PickleError);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
@@ -12341,55 +12824,67 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_PickleError, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":25
+  /* "gsd/fl.pyx":19
+ * import os
+ * from pickle import PickleError
+ * import warnings             # <<<<<<<<<<<<<<
+ * from libc.stdint cimport uint8_t, int8_t, uint16_t, int16_t, uint32_t, int32_t,\
+ *     uint64_t, int64_t
+ */
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "gsd/fl.pyx":26
  * cimport numpy
  * 
  * logger = logging.getLogger('gsd.fl')             # <<<<<<<<<<<<<<
  * 
  * ####################
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logger, __pyx_t_2) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_logger, __pyx_t_2) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gsd/fl.pyx":148
+  /* "gsd/fl.pyx":149
  * 
  * 
  * def open(name, mode, application=None, schema=None, schema_version=None):             # <<<<<<<<<<<<<<
  *     """open(name, mode, application=None, schema=None, schema_version=None)
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_3gsd_2fl_1open, NULL, __pyx_n_s_gsd_fl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_3gsd_2fl_1open, NULL, __pyx_n_s_gsd_fl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_open, __pyx_t_2) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_open, __pyx_t_2) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "gsd/fl.pyx":1
  * # Copyright (c) 2016-2023 The Regents of the University of Michigan             # <<<<<<<<<<<<<<
  * # Part of GSD, released under the BSD 2-Clause License.
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../../../opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-mmk_n76d/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `gsd-2.8.1/gsd/fl.pyx` & `gsd-2.9.0/gsd/fl.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 """
 
 import logging
 import numpy
 import os
 from pickle import PickleError
+import warnings
 from libc.stdint cimport uint8_t, int8_t, uint16_t, int16_t, uint32_t, int32_t,\
     uint64_t, int64_t
 from libc.errno cimport errno
 cimport gsd.libgsd as libgsd
 cimport numpy
 
 logger = logging.getLogger('gsd.fl')
@@ -159,61 +160,72 @@
         application (str): Name of the application creating the file.
 
         schema (str): Name of the data schema.
 
         schema_version (tuple[int, int]): Schema version number
             (major, minor).
 
-    Valid values for mode:
+    Valid values for ``mode``:
 
     +------------------+---------------------------------------------+
     | mode             | description                                 |
     +==================+=============================================+
-    | ``'rb'``         | Open an existing file for reading.          |
+    | ``'r'``          | Open an existing file for reading.          |
     +------------------+---------------------------------------------+
-    | ``'rb+'``        | Open an existing file for reading and       |
+    | ``'r+'``         | Open an existing file for reading and       |
     |                  | writing.                                    |
     +------------------+---------------------------------------------+
-    | ``'wb'``         | Open a file for reading and writing.        |
+    | ``'w'``          | Open a file for reading and writing.        |
     |                  | Creates the file if needed, or overwrites   |
     |                  | an existing file.                           |
     +------------------+---------------------------------------------+
-    | ``'wb+'``        | Open a file for reading and writing.        |
-    |                  | Creates the file if needed, or overwrites   |
-    |                  | an existing file.                           |
-    +------------------+---------------------------------------------+
-    | ``'xb'``         | Create a gsd file exclusively and opens it  |
-    |                  | for reading and writing.                    |
-    |                  | Raise :py:exc:`FileExistsError`             |
-    |                  | if it already exists.                       |
-    +------------------+---------------------------------------------+
-    | ``'xb+'``        | Create a gsd file exclusively and opens it  |
+    | ``'x'``          | Create a gsd file exclusively and opens it  |
     |                  | for reading and writing.                    |
     |                  | Raise :py:exc:`FileExistsError`             |
     |                  | if it already exists.                       |
     +------------------+---------------------------------------------+
-    | ``'ab'``         | Open an existing file for reading and       |
-    |                  | writing. Does *not* create or overwrite     |
-    |                  | existing files.                             |
+    | ``'a'``          | Open a file for reading and writing.        |
+    |                  | Creates the file if it doesn't exist.       |
     +------------------+---------------------------------------------+
 
-    When opening a file for reading (``'r'`` and ``'a'`` modes): ``application``
-    and ``schema_version`` are ignored and may be ``None``. When ``schema`` is
-    not ``None``, :py:func:`open` throws an exception if the file's schema does
-    not match ``schema``.
-
-    When opening a file for writing (``'w'`` or ``'x'`` modes): The given
-    ``application``, ``schema``, and ``schema_version`` are saved in the file
-    and must not be None.
+    When opening a file for reading (``'r'`` and ``'r+'`` modes):
+    ``application`` and ``schema_version`` are ignored and may be ``None``.
+    When ``schema`` is not ``None``, :py:func:`open` throws an exception if the
+    file's schema does not match ``schema``.
+
+    When opening a file for writing (``'w'``, ``'x'``, or ``'a'`` modes): The
+    given ``application``, ``schema``, and ``schema_version`` must not be None.
+
+    .. deprecated:: 2.9.0
+
+        The following values to ``mode`` are deprecated:
+
+        +------------------+---------------------------------------------+
+        | mode             | description                                 |
+        +==================+=============================================+
+        | ``'rb'``         | Equivalent to ``'r'``                       |
+        +------------------+---------------------------------------------+
+        | ``'rb+'``        | Equivalent to ``'r+'``                      |
+        +------------------+---------------------------------------------+
+        | ``'wb'``         | Equivalent to ``'w'``                       |
+        +------------------+---------------------------------------------+
+        | ``'wb+'``        | Equivalent to ``'w'``                       |
+        +------------------+---------------------------------------------+
+        | ``'xb'``         | Equivalent to ``'x'``                       |
+        +------------------+---------------------------------------------+
+        | ``'xb+'``        | Equivalent to ``'x'``                       |
+        +------------------+---------------------------------------------+
+        | ``'ab'``         | Equivalent to ``'r+'``                      |
+        +------------------+---------------------------------------------+
 
     Example:
 
         .. ipython:: python
 
-            with gsd.fl.open(name='file.gsd', mode='wb',
+            with gsd.fl.open(name='file.gsd', mode='w',
                              application="My application", schema="My Schema",
                              schema_version=[1,0]) as f:
                 f.write_chunk(name='chunk1',
                               data=numpy.array([1,2,3,4], dtype=numpy.float32))
                 f.write_chunk(name='chunk2',
                               data=numpy.array([[5,6],[7,8]],
                                                dtype=numpy.float32))
@@ -222,15 +234,15 @@
                               data=numpy.array([9,10,11,12],
                                                dtype=numpy.float32))
                 f.write_chunk(name='chunk2',
                               data=numpy.array([[13,14],[15,16]],
                                                dtype=numpy.float32))
                 f.end_frame()
 
-            f = gsd.fl.open(name='file.gsd', mode='rb')
+            f = gsd.fl.open(name='file.gsd', mode='r')
             if f.chunk_exists(frame=0, name='chunk1'):
                 data = f.read_chunk(frame=0, name='chunk1')
             data
             f.close()
     """
 
     return GSDFile(str(name), mode, application, schema, schema_version)
@@ -294,40 +306,64 @@
                  application,
                  schema,
                  schema_version):
         cdef libgsd.gsd_open_flag c_flags
         cdef int exclusive_create = 0
         cdef int overwrite = 0
 
+        self.mode = mode
+
         if mode == 'wb':
-            c_flags = libgsd.GSD_OPEN_APPEND
-            overwrite = 1
+            mode = 'w'
+            warnings.warn("The 'wb' mode is deprecated, use 'w'",
+                           FutureWarning)
         elif mode == 'wb+':
-            c_flags = libgsd.GSD_OPEN_READWRITE
-            overwrite = 1
+            mode = 'w'
+            warnings.warn("The 'wb+' mode is deprecated, use 'w'",
+                           FutureWarning)
         elif mode == 'rb':
-            c_flags = libgsd.GSD_OPEN_READONLY
+            mode = 'r'
+            warnings.warn("The 'rb' mode is deprecated, use 'r'",
+                           FutureWarning)
         elif mode == 'rb+':
-            c_flags = libgsd.GSD_OPEN_READWRITE
+            mode = 'r+'
+            warnings.warn("The 'rb+' mode is deprecated, use 'r+'",
+                           FutureWarning)
         elif mode == 'xb':
-            c_flags = libgsd.GSD_OPEN_APPEND
-            overwrite = 1
-            exclusive_create = 1
+            mode = 'x'
+            warnings.warn("The 'xb' mode is deprecated, use 'x'",
+                           FutureWarning)
         elif mode == 'xb+':
+            mode = 'x'
+            warnings.warn("The 'xb+' mode is deprecated, use 'x'",
+                           FutureWarning)
+        elif mode == 'ab':
+            mode = 'r+'
+            warnings.warn("The 'ab' mode is deprecated, use 'r+'",
+                           FutureWarning)
+
+        if mode == 'w':
+            c_flags = libgsd.GSD_OPEN_READWRITE
+            overwrite = 1
+        elif mode == 'r':
+            c_flags = libgsd.GSD_OPEN_READONLY
+        elif mode == 'r+':
+            c_flags = libgsd.GSD_OPEN_READWRITE
+        elif mode == 'x':
             c_flags = libgsd.GSD_OPEN_READWRITE
             overwrite = 1
             exclusive_create = 1
-        elif mode == 'ab':
-            c_flags = libgsd.GSD_OPEN_APPEND
+        elif mode == 'a':
+            c_flags = libgsd.GSD_OPEN_READWRITE
+            if not os.path.exists(name):
+                overwrite = 1
         else:
-            raise ValueError("mode must be 'wb', 'wb+', 'rb', 'rb+', "
-                             "'xb', 'xb+', or 'ab'")
+            raise ValueError("Invalid mode: " + mode)
 
         self.name = name
-        self.mode = mode
 
         cdef char * c_name
         cdef char * c_application
         cdef char * c_schema
         cdef int _c_schema_version
         cdef str schema_truncated
 
@@ -396,15 +432,15 @@
         The file is automatically closed when garbage collected or when
         the context manager exits.
 
         Example:
             .. ipython:: python
                 :okexcept:
 
-                f = gsd.fl.open(name='file.gsd', mode='wb+',
+                f = gsd.fl.open(name='file.gsd', mode='w',
                                 application="My application",
                                 schema="My Schema", schema_version=[1,0])
                 f.write_chunk(name='chunk1',
                               data=numpy.array([1,2,3,4], dtype=numpy.float32))
                 f.end_frame()
                 data = f.read_chunk(frame=0, name='chunk1')
 
@@ -427,24 +463,24 @@
         Truncate all data from the file. After truncation, the file has no
         frames and no data chunks. The application, schema, and schema version
         remain the same.
 
         Example:
             .. ipython:: python
 
-                with gsd.fl.open(name='file.gsd', mode='wb',
+                with gsd.fl.open(name='file.gsd', mode='w',
                                  application="My application",
                                  schema="My Schema", schema_version=[1,0]) as f:
                     for i in range(10):
                         f.write_chunk(name='chunk1',
                                       data=numpy.array([1,2,3,4],
                                                        dtype=numpy.float32))
                         f.end_frame()
 
-                f = gsd.fl.open(name='file.gsd', mode='ab',
+                f = gsd.fl.open(name='file.gsd', mode='r+',
                                 application="My application",
                                 schema="My Schema", schema_version=[1,0])
                 f.nframes
                 f.schema, f.schema_version, f.application
                 f.truncate()
                 f.nframes
                 f.schema, f.schema_version, f.application
@@ -472,15 +508,15 @@
             **before** closing the file. If you fail to call
             :py:meth:`end_frame()`, the last frame will not be written
             to disk.
 
         Example:
             .. ipython:: python
 
-                f = gsd.fl.open(name='file.gsd', mode='wb',
+                f = gsd.fl.open(name='file.gsd', mode='w',
                                 application="My application",
                                 schema="My Schema", schema_version=[1,0])
 
                 f.write_chunk(name='chunk1',
                               data=numpy.array([1,2,3,4], dtype=numpy.float32))
                 f.end_frame()
                 f.write_chunk(name='chunk1',
@@ -523,15 +559,15 @@
             non-contiguous numpy arrays to contiguous numpy arrays with
             ``numpy.ascontiguousarray(data)``. This may or may not produce
             desired data types in the output file and incurs overhead.
 
         Example:
             .. ipython:: python
 
-                f = gsd.fl.open(name='file.gsd', mode='wb',
+                f = gsd.fl.open(name='file.gsd', mode='w',
                                 application="My application",
                                 schema="My Schema", schema_version=[1,0])
 
                 f.write_chunk(name='float1d',
                               data=numpy.array([1,2,3,4],
                                                dtype=numpy.float32))
                 f.write_chunk(name='float2d',
@@ -632,15 +668,15 @@
         Returns:
             bool: ``True`` if the chunk exists in the file at the given frame.\
               ``False`` if it does not.
 
         Example:
             .. ipython:: python
 
-                with gsd.fl.open(name='file.gsd', mode='wb',
+                with gsd.fl.open(name='file.gsd', mode='w',
                                  application="My application",
                                  schema="My Schema", schema_version=[1,0]) as f:
                     f.write_chunk(name='chunk1',
                                   data=numpy.array([1,2,3,4],
                                                    dtype=numpy.float32))
                     f.write_chunk(name='chunk2',
                                   data=numpy.array([[5,6],[7,8]],
@@ -650,15 +686,15 @@
                                   data=numpy.array([9,10,11,12],
                                                    dtype=numpy.float32))
                     f.write_chunk(name='chunk2',
                                   data=numpy.array([[13,14],[15,16]],
                                                    dtype=numpy.float32))
                     f.end_frame()
 
-                f = gsd.fl.open(name='file.gsd', mode='rb',
+                f = gsd.fl.open(name='file.gsd', mode='r',
                                 application="My application",
                                 schema="My Schema", schema_version=[1,0])
 
                 f.chunk_exists(frame=0, name='chunk1')
                 f.chunk_exists(frame=0, name='chunk2')
                 f.chunk_exists(frame=0, name='chunk3')
                 f.chunk_exists(frame=10, name='chunk1')
@@ -699,15 +735,15 @@
             new numpy array for storage. To avoid overhead, call
             :py:meth:`read_chunk()` on the same chunk only once.
 
         Example:
             .. ipython:: python
                 :okexcept:
 
-                with gsd.fl.open(name='file.gsd', mode='wb',
+                with gsd.fl.open(name='file.gsd', mode='w',
                                  application="My application",
                                  schema="My Schema", schema_version=[1,0]) as f:
                     f.write_chunk(name='chunk1',
                                   data=numpy.array([1,2,3,4],
                                                    dtype=numpy.float32))
                     f.write_chunk(name='chunk2',
                                   data=numpy.array([[5,6],[7,8]],
@@ -717,15 +753,15 @@
                                   data=numpy.array([9,10,11,12],
                                                    dtype=numpy.float32))
                     f.write_chunk(name='chunk2',
                                   data=numpy.array([[13,14],[15,16]],
                                                    dtype=numpy.float32))
                     f.end_frame()
 
-                f = gsd.fl.open(name='file.gsd', mode='rb',
+                f = gsd.fl.open(name='file.gsd', mode='r',
                                 application="My application",
                                 schema="My Schema", schema_version=[1,0])
                 f.read_chunk(frame=0, name='chunk1')
                 f.read_chunk(frame=1, name='chunk1')
                 f.read_chunk(frame=2, name='chunk1')
                 f.close()
         """
@@ -834,15 +870,15 @@
 
         Returns:
             list[str]: Matching chunk names
 
         Example:
             .. ipython:: python
 
-                with gsd.fl.open(name='file.gsd', mode='wb',
+                with gsd.fl.open(name='file.gsd', mode='w',
                                  application="My application",
                                  schema="My Schema", schema_version=[1,0]) as f:
                     f.write_chunk(name='data/chunk1',
                                   data=numpy.array([1,2,3,4],
                                                    dtype=numpy.float32))
                     f.write_chunk(name='data/chunk2',
                                   data=numpy.array([[5,6],[7,8]],
@@ -852,15 +888,15 @@
                                                    dtype=numpy.float32))
                     f.end_frame()
                     f.write_chunk(name='input/chunk4',
                                   data=numpy.array([11, 12, 13, 14],
                                                    dtype=numpy.float32))
                     f.end_frame()
 
-                f = gsd.fl.open(name='file.gsd', mode='rb',
+                f = gsd.fl.open(name='file.gsd', mode='r',
                                 application="My application",
                                 schema="My Schema", schema_version=[1,0])
 
                 f.find_matching_chunk_names('')
                 f.find_matching_chunk_names('data')
                 f.find_matching_chunk_names('input')
                 f.find_matching_chunk_names('other')
@@ -914,15 +950,15 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def __reduce__(self):
         """Allows filehandles to be pickled when in read only mode."""
-        if self.mode not in ['rb', 'rb+']:
+        if self.mode not in ['rb', 'r']:
             raise PickleError("Only read only GSDFiles can be pickled.")
         return (GSDFile,
                 (self.name, self.mode, self.application,
                     self.schema, self.schema_version),
                 )
 
     property name:
```

### Comparing `gsd-2.8.1/gsd/gsd.c` & `gsd-2.9.0/gsd/gsd.c`

 * *Files identical despite different names*

### Comparing `gsd-2.8.1/gsd/gsd.h` & `gsd-2.9.0/gsd/gsd.h`

 * *Files identical despite different names*

### Comparing `gsd-2.8.1/gsd/hoomd.py` & `gsd-2.9.0/gsd/hoomd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1055,59 +1055,71 @@
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Close the file when the context manager exits."""
         self.file.close()
 
 
-def open(name, mode='rb'):
+def open(name, mode='r'):
     """Open a hoomd schema GSD file.
 
     The return value of `open` can be used as a context manager.
 
     Args:
         name (str): File name to open.
         mode (str): File open mode.
 
     Returns:
         `HOOMDTrajectory` instance that accesses the file **name** with the
         given **mode**.
 
-    Valid values for mode:
+    Valid values for ``mode``:
 
     +------------------+---------------------------------------------+
     | mode             | description                                 |
     +==================+=============================================+
-    | ``'rb'``         | Open an existing file for reading.          |
+    | ``'r'``          | Open an existing file for reading.          |
     +------------------+---------------------------------------------+
-    | ``'rb+'``        | Open an existing file for reading and       |
+    | ``'r+'``         | Open an existing file for reading and       |
     |                  | writing.                                    |
     +------------------+---------------------------------------------+
-    | ``'wb'``         | Open a file for reading and writing.        |
+    | ``'w'``          | Open a file for reading and writing.        |
     |                  | Creates the file if needed, or overwrites   |
     |                  | an existing file.                           |
     +------------------+---------------------------------------------+
-    | ``'wb+'``        | Open a file for reading and writing.        |
-    |                  | Creates the file if needed, or overwrites   |
-    |                  | an existing file.                           |
-    +------------------+---------------------------------------------+
-    | ``'xb'``         | Create a gsd file exclusively and opens it  |
-    |                  | for reading and writing.                    |
-    |                  | Raise :py:exc:`FileExistsError`             |
-    |                  | if it already exists.                       |
-    +------------------+---------------------------------------------+
-    | ``'xb+'``        | Create a gsd file exclusively and opens it  |
+    | ``'x'``          | Create a gsd file exclusively and opens it  |
     |                  | for reading and writing.                    |
     |                  | Raise :py:exc:`FileExistsError`             |
     |                  | if it already exists.                       |
     +------------------+---------------------------------------------+
-    | ``'ab'``         | Open an existing file for reading and       |
-    |                  | writing. Does *not* create or overwrite     |
-    |                  | existing files.                             |
+    | ``'a'``          | Open a file for reading and writing.        |
+    |                  | Creates the file if it doesn't exist.       |
     +------------------+---------------------------------------------+
+
+    .. deprecated:: 2.9.0
+
+        The following values to ``mode`` are deprecated:
+
+        +------------------+---------------------------------------------+
+        | mode             | description                                 |
+        +==================+=============================================+
+        | ``'rb'``         | Equivalent to ``'r'``                       |
+        +------------------+---------------------------------------------+
+        | ``'rb+'``        | Equivalent to ``'r+'``                      |
+        +------------------+---------------------------------------------+
+        | ``'wb'``         | Equivalent to ``'w'``                       |
+        +------------------+---------------------------------------------+
+        | ``'wb+'``        | Equivalent to ``'w'``                       |
+        +------------------+---------------------------------------------+
+        | ``'xb'``         | Equivalent to ``'x'``                       |
+        +------------------+---------------------------------------------+
+        | ``'xb+'``        | Equivalent to ``'x'``                       |
+        +------------------+---------------------------------------------+
+        | ``'ab'``         | Equivalent to ``'r+'``                      |
+        +------------------+---------------------------------------------+
     """
     if fl is None:
         raise RuntimeError("file layer module is not available")
     if gsd is None:
         raise RuntimeError("gsd module is not available")
 
     gsdfileobj = fl.open(name=str(name),
@@ -1154,15 +1166,15 @@
     """
     if fl is None:
         raise RuntimeError("file layer module is not available")
     if gsd is None:
         raise RuntimeError("gsd module is not available")
 
     with fl.open(name=str(name),
-                 mode='rb',
+                 mode='r',
                  application='gsd.hoomd ' + gsd.__version__,
                  schema='hoomd',
                  schema_version=[1, 4]) as gsdfileobj:
 
         logged_data_names = gsdfileobj.find_matching_chunk_names('log/')
         # Always log timestep associated with each log entry
         logged_data_names.insert(0, 'configuration/step')
```

### Comparing `gsd-2.8.1/gsd/libgsd.pxd` & `gsd-2.9.0/gsd/libgsd.pxd`

 * *Files identical despite different names*

### Comparing `gsd-2.8.1/gsd/pygsd.py` & `gsd-2.9.0/gsd/pygsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 The reader reads from file-like Python objects, which may be useful for reading
 from in memory buffers, and in-database grid files, For regular files on the
 filesystem, and for writing gsd files, use :py:mod:`gsd.fl`.
 
 The :py:class:`GSDFile` in this module can be used with the
 :py:class:`gsd.hoomd.HOOMDTrajectory` hoomd reader:
 
->>> with gsd.pygsd.GSDFile('test.gsd', 'rb') as f:
+>>> with gsd.pygsd.GSDFile('test.gsd', 'r') as f:
 ...     t = gsd.hoomd.HOOMDTrajectory(f)
 ...     pos = t[0].particles.position
 
 """
 
 from __future__ import print_function
 from __future__ import division
 import logging
 import numpy
 import struct
 from collections import namedtuple
 import sys
 
-__version__ = "2.8.1"
+__version__ = "2.9.0"
 
 logger = logging.getLogger('gsd.pygsd')
 
 gsd_header = namedtuple(
     'gsd_header',
     'magic index_location index_allocated_entries '
     'namelist_location namelist_allocated_entries '
@@ -81,28 +81,28 @@
     read-write access to files, use the full featured C implementation in
     :py:mod:`gsd.fl`. Otherwise, the two implementations can be used
     interchangeably.
 
     Examples:
         Open a file in **read-only** mode::
 
-            f = GSDFile(open('file.gsd', mode='rb'))
+            f = GSDFile(open('file.gsd', mode='r'))
             if f.chunk_exists(frame=0, name='chunk'):
                 data = f.read_chunk(frame=0, name='chunk')
 
         Access file **metadata**::
 
-            f = GSDFile(open('file.gsd', mode='rb'))
+            f = GSDFile(open('file.gsd', mode='r'))
             print(f.name, f.mode, f.gsd_version)
             print(f.application, f.schema, f.schema_version)
             print(f.nframes)
 
         Use as a **context manager**::
 
-            with GSDFile(open('file.gsd', mode='rb')) as f:
+            with GSDFile(open('file.gsd', mode='r')) as f:
                 data = f.read_chunk(frame=0, name='chunk')
     """
 
     def __init__(self, file):
         self.__file = file
 
         logger.info('opening file: ' + str(file))
@@ -265,15 +265,15 @@
         Returns:
             bool: True if the chunk exists in the file. False if it does not.
 
         Example:
 
             Handle non-existent chunks::
 
-                with GSDFile(open('file.gsd', mode='rb')) as f:
+                with GSDFile(open('file.gsd', mode='r')) as f:
                     if f.chunk_exists(frame=0, name='chunk'):
                         return f.read_chunk(frame=0, name='chunk')
                     else:
                         return None
         """
         if not self.__is_open:
             raise ValueError("File is not open")
@@ -290,27 +290,27 @@
 
         Returns:
             `numpy.ndarray`: Data read from file.
 
         Examples:
             Read a 1D array::
 
-                with GSDFile(name=filename, mode='rb') as f:
+                with GSDFile(name=filename, mode='r') as f:
                     data = f.read_chunk(frame=0, name='chunk1d')
                     # data.shape == [N]
 
             Read a 2D array::
 
-                with GSDFile(name=filename, mode='rb') as f:
+                with GSDFile(name=filename, mode='r') as f:
                     data = f.read_chunk(frame=0, name='chunk2d')
                     # data.shape == [N,M]
 
             Read multiple frames::
 
-                with GSDFile(name=filename, mode='rb') as f:
+                with GSDFile(name=filename, mode='r') as f:
                     data0 = f.read_chunk(frame=0, name='chunk')
                     data1 = f.read_chunk(frame=1, name='chunk')
                     data2 = f.read_chunk(frame=2, name='chunk')
                     data3 = f.read_chunk(frame=3, name='chunk')
 
         .. tip::
             Each call invokes a disk read and allocation of a
@@ -393,15 +393,15 @@
     def file(self):
         """File-like object opened."""
         return self.__file
 
     @property
     def mode(self):
         """str: Mode of the open file."""
-        return 'rb'
+        return 'r'
 
     @property
     def gsd_version(self):
         """tuple[int, int]: GSD file layer version number.
 
         The tuple is in the order (major, minor).
         """
```

### Comparing `gsd-2.8.1/gsd/pytest_plugin_validate.py` & `gsd-2.9.0/gsd/pytest_plugin_validate.py`

 * *Files identical despite different names*

### Comparing `gsd-2.8.1/gsd/test/conftest.py` & `gsd-2.9.0/gsd/test/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Pytest fixtures common to all tests."""
 
 import pytest
 import collections
 
 Mode = collections.namedtuple('Mode', 'read write')
-mode_list = [Mode('rb', 'wb'), Mode('rb+', 'wb+')]
+mode_list = [Mode('r', 'w'), Mode('a', 'x'), Mode('r', 'a')]
 
 
 def open_mode_name(mode):
     """Provide a name for the open mode fixture."""
     return '(' + mode.read + ',' + mode.write + ')'
```

### Comparing `gsd-2.8.1/gsd/test/test_fl.py` & `gsd-2.9.0/gsd/test/test_fl.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import os
 import shutil
 import sys
 
 test_path = pathlib.Path(os.path.realpath(__file__)).parent
 
 
-def test_create(tmp_path):
+def test_create(tmp_path, open_mode):
     """Test creation of GSD files."""
-    gsd.fl.open(mode='xb',
+    gsd.fl.open(mode=open_mode.write,
                 name=tmp_path / "test_create.gsd",
                 application="test_create",
                 schema="none",
                 schema_version=[1, 2])
 
 
 @pytest.mark.parametrize('typ', [
@@ -40,32 +40,32 @@
 ])
 def test_dtype(tmp_path, typ):
     """Test all supported data types."""
     data1d = numpy.array([1, 2, 3, 4, 5, 127], dtype=typ)
     data2d = numpy.array([[10, 20], [30, 40], [50, 80]], dtype=typ)
     data_zero = numpy.array([], dtype=typ)
 
-    gsd.fl.open(mode='xb',
+    gsd.fl.open(mode='x',
                 name=tmp_path / "test_dtype.gsd",
                 application="test_dtype",
                 schema="none",
                 schema_version=[1, 2])
 
     with gsd.fl.open(name=tmp_path / "test_dtype.gsd",
-                     mode='wb',
+                     mode='w',
                      application="test_dtype",
                      schema="none",
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='data1d', data=data1d)
         f.write_chunk(name='data2d', data=data2d)
         f.write_chunk(name='data_zero', data=data_zero)
         f.end_frame()
 
     with gsd.fl.open(name=tmp_path / "test_dtype.gsd",
-                     mode='rb',
+                     mode='r',
                      application="test_dtype",
                      schema="none",
                      schema_version=[1, 2]) as f:
         read_data1d = f.read_chunk(frame=0, name='data1d')
         read_data2d = f.read_chunk(frame=0, name='data2d')
         read_data_zero = f.read_chunk(frame=0, name='data_zero')
 
@@ -115,15 +115,15 @@
         assert f.nframes == 150
         assert f.gsd_version == (2, 0)
 
     # test again with pygsd
     with gsd.pygsd.GSDFile(
             file=open(str(tmp_path / 'test_metadata.gsd'), mode='rb')) as f:
         assert f.name == str(tmp_path / 'test_metadata.gsd')
-        assert f.mode == 'rb'
+        assert f.mode == 'r'
         assert f.application == 'test_metadata'
         assert f.schema == 'none'
         assert f.schema_version == (1, 2)
         assert f.nframes == 150
         assert f.gsd_version == (2, 0)
 
 
@@ -136,19 +136,19 @@
                      schema_version=[1, 2]):
         pass
 
     data = numpy.array([10], dtype=numpy.int64)
     nframes = 1024
 
     with gsd.fl.open(name=tmp_path / 'test_append.gsd',
-                     mode='ab',
+                     mode='a',
                      application='test_append',
                      schema='none',
                      schema_version=[1, 2]) as f:
-        assert f.mode == 'ab'
+        assert f.mode == 'a'
         for i in range(nframes):
             data[0] = i
             f.write_chunk(name='data1', data=data)
             data[0] = i * 10
             f.write_chunk(name='data10', data=data)
             f.end_frame()
 
@@ -162,16 +162,15 @@
             data1 = f.read_chunk(frame=i, name='data1')
             data10 = f.read_chunk(frame=i, name='data10')
             assert data1[0] == i
             assert data10[0] == i * 10
 
     # test again with pygsd
     with gsd.pygsd.GSDFile(
-            file=open(str(tmp_path
-                          / 'test_append.gsd'), mode=open_mode.read)) as f:
+            file=open(str(tmp_path / 'test_append.gsd'), mode='rb')) as f:
         assert f.nframes == nframes
         for i in range(nframes):
             data1 = f.read_chunk(frame=i, name='data1')
             data10 = f.read_chunk(frame=i, name='data10')
             assert data1[0] == i
             assert data10[0] == i * 10
 
@@ -264,15 +263,15 @@
                      schema_version=[1, 2]) as f:
         for i in range(10):
             f.write_chunk(name='chunk1', data=data)
             f.end_frame()
 
     data = numpy.array([1, 2, 3, 4, 5, 10012], dtype=numpy.int64)
     with gsd.fl.open(name=tmp_path / 'test_readonly_errors.gsd',
-                     mode='rb',
+                     mode='r',
                      application='test_readonly_errors',
                      schema='none',
                      schema_version=[1, 2]) as f:
         with pytest.raises(Exception):
             f.end_frame()
 
         with pytest.raises(Exception):
@@ -295,16 +294,15 @@
     if platform.system() != "Windows":
         with pytest.raises(Exception):
             gsd.fl.open(name='/this/file/does/not/exist',
                         application='test_readonly_errors',
                         schema='none',
                         schema_version=[1, 2])
 
-        with open(str(tmp_path / 'test_fileio_errors.gsd'),
-                  open_mode.write) as f:
+        with open(str(tmp_path / 'test_fileio_errors.gsd'), 'wb') as f:
             f.write(b'test')
 
         with pytest.raises(RuntimeError):
             f = gsd.fl.open(name=tmp_path / 'test_fileio_errors.gsd',
                             mode=open_mode.read,
                             application='test_readonly_errors',
                             schema='none',
@@ -312,66 +310,66 @@
 
 
 def test_dtype_errors(tmp_path, open_mode):
     """Test that unsupported data types result in errors."""
     with pytest.raises(Exception):
         data = numpy.array([1, 2, 3, 4, 5, 10012], dtype=numpy.bool_)
 
-        with gsd.fl.open(name=tmp_path / 'test_dtype_errors.gsd',
+        with gsd.fl.open(name=tmp_path / 'test_dtype_errors1.gsd',
                          mode=open_mode.write,
                          application='test_dtype_errors',
                          schema='none',
                          schema_version=[1, 2]) as f:
             f.write_chunk(name='chunk1', data=data)
             f.end_frame()
 
     with pytest.raises(Exception):
         data = numpy.array([1, 2, 3, 4, 5, 10012], dtype=numpy.float16)
 
-        with gsd.fl.open(name=tmp_path / 'test_dtype_errors.gsd',
+        with gsd.fl.open(name=tmp_path / 'test_dtype_errors2.gsd',
                          mode=open_mode.write,
                          application='test_dtype_errors',
                          schema='none',
                          schema_version=[1, 2]) as f:
             f.write_chunk(name='chunk1', data=data)
             f.end_frame()
 
     with pytest.raises(Exception):
         data = numpy.array([1, 2, 3, 4, 5, 10012], dtype=numpy.complex64)
 
-        with gsd.fl.open(name=tmp_path / 'test_dtype_errors.gsd',
+        with gsd.fl.open(name=tmp_path / 'test_dtype_errors3.gsd',
                          mode=open_mode.write,
                          application='test_dtype_errors',
                          schema='none',
                          schema_version=[1, 2]) as f:
             f.write_chunk(name='chunk1', data=data)
             f.end_frame()
 
     with pytest.raises(Exception):
         data = numpy.array([1, 2, 3, 4, 5, 10012], dtype=numpy.complex128)
 
-        with gsd.fl.open(name=tmp_path / 'test_dtype_errors.gsd',
+        with gsd.fl.open(name=tmp_path / 'test_dtype_errors4.gsd',
                          mode=open_mode.write,
                          application='test_dtype_errors',
                          schema='none',
                          schema_version=[1, 2]) as f:
             f.write_chunk(name='chunk1', data=data)
             f.end_frame()
 
 
 def test_truncate(tmp_path):
     """Test that the truncate method functions."""
     data = numpy.ascontiguousarray(numpy.random.random(size=(1000, 3)),
                                    dtype=numpy.float32)
     with gsd.fl.open(name=tmp_path / 'test_truncate.gsd',
-                     mode='wb',
+                     mode='w',
                      application='test_truncate',
                      schema='none',
                      schema_version=[1, 2]) as f:
-        assert f.mode == 'wb'
+        assert f.mode == 'w'
         for i in range(10):
             f.write_chunk(name='data', data=data)
             f.end_frame()
 
         assert f.nframes == 10
 
         f.truncate()
@@ -380,20 +378,20 @@
         assert f.schema == 'none'
         assert f.schema_version == (1, 2)
 
         f.write_chunk(name='data', data=data)
         f.end_frame()
 
     with gsd.fl.open(name=tmp_path / 'test_truncate.gsd',
-                     mode='rb',
+                     mode='r',
                      application='test_truncate',
                      schema='none',
                      schema_version=[1, 2]) as f:
         assert f.name == str(tmp_path / 'test_truncate.gsd')
-        assert f.mode == 'rb'
+        assert f.mode == 'r'
         assert f.application == 'test_truncate'
         assert f.schema == 'none'
         assert f.schema_version == (1, 2)
         assert f.nframes == 1
 
 
 def test_namelen(tmp_path, open_mode):
@@ -430,65 +428,65 @@
 
 
 def test_open(tmp_path):
     """Test the open() API."""
     data = numpy.array([1, 2, 3, 4, 5, 10012], dtype=numpy.int64)
 
     with gsd.fl.open(name=tmp_path / 'test.gsd',
-                     mode='xb',
+                     mode='x',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='chunk1', data=data)
         f.end_frame()
 
     with gsd.fl.open(name=tmp_path / 'test_2.gsd',
-                     mode='xb+',
+                     mode='x',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='chunk1', data=data)
         f.end_frame()
         f.read_chunk(0, name='chunk1')
 
     with gsd.fl.open(name=tmp_path / 'test.gsd',
-                     mode='wb',
+                     mode='w',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='chunk1', data=data)
         f.end_frame()
 
     with gsd.fl.open(name=tmp_path / 'test.gsd',
-                     mode='wb+',
+                     mode='w',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='chunk1', data=data)
         f.end_frame()
         f.read_chunk(0, name='chunk1')
 
     with gsd.fl.open(name=tmp_path / 'test.gsd',
-                     mode='ab',
+                     mode='a',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='chunk1', data=data)
         f.end_frame()
 
     with gsd.fl.open(name=tmp_path / 'test.gsd',
-                     mode='rb',
+                     mode='r',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.read_chunk(0, name='chunk1')
         f.read_chunk(1, name='chunk1')
 
     with gsd.fl.open(name=tmp_path / 'test.gsd',
-                     mode='rb+',
+                     mode='r+',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='chunk1', data=data)
         f.end_frame()
         f.read_chunk(0, name='chunk1')
         f.read_chunk(1, name='chunk1')
@@ -631,15 +629,15 @@
 
         chunk_names = f.find_matching_chunk_names('')
         chunk_names.sort()
         assert chunk_names == values_str
 
     # test with the C implemantation
     with gsd.fl.open(name=test_path / 'test_gsd_v1.gsd',
-                     mode='rb',
+                     mode='r',
                      application='test_gsd_v1',
                      schema='none',
                      schema_version=[1, 2]) as f:
 
         check_v1_file_read(f)
 
     # and the pure Python implementation
@@ -671,15 +669,15 @@
         chunk_names = f.find_matching_chunk_names('')
         chunk_names.sort()
         assert chunk_names == values_str
 
     shutil.copy(test_path / 'test_gsd_v1.gsd', tmp_path / 'test_gsd_v1.gsd')
 
     with gsd.fl.open(name=tmp_path / 'test_gsd_v1.gsd',
-                     mode='rb+',
+                     mode='r+',
                      application='test_gsd_v1',
                      schema='none',
                      schema_version=[1, 2]) as f:
 
         assert f.gsd_version == (1, 0)
 
         f.upgrade()
@@ -746,15 +744,15 @@
                     value = value[0:63]
 
             data_read = f.read_chunk(frame=frame, name=str(value))
             numpy.testing.assert_array_equal(data, data_read)
 
     # test that we can write new entries to the file
     with gsd.fl.open(name=tmp_path / 'test_gsd_v1.gsd',
-                     mode='rb+',
+                     mode='r+',
                      application='test_gsd_v1',
                      schema='none',
                      schema_version=[1, 2]) as f:
 
         assert f.gsd_version == (1, 0)
 
         for value in values:
@@ -815,15 +813,15 @@
                 data = numpy.array([hash(value)], dtype=numpy.int64)
 
             data_read = f.read_chunk(frame=frame, name=str(value))
             numpy.testing.assert_array_equal(data, data_read)
 
     # test that we can write new entries to the file
     with gsd.fl.open(name=tmp_path / 'test_gsd_v1.gsd',
-                     mode='rb+',
+                     mode='r+',
                      application='test_gsd_v1',
                      schema='none',
                      schema_version=[1, 2]) as f:
 
         assert f.gsd_version == (1, 0)
 
         f.upgrade()
@@ -880,17 +878,16 @@
                      schema_version=[1, 2]) as f:
         assert f.nframes == 1
         data_read = f.read_chunk(frame=0, name='data')
         assert data_read.shape == (0,)
         assert data_read.dtype == numpy.float32
 
     # test again with pygsd
-    with gsd.pygsd.GSDFile(
-            file=open(str(tmp_path
-                          / 'test_zero.gsd'), mode=open_mode.read)) as f:
+    with gsd.pygsd.GSDFile(file=open(str(tmp_path
+                                         / 'test_zero.gsd'), mode='rb')) as f:
         assert f.nframes == 1
         data_read = f.read_chunk(frame=0, name='data')
         assert data_read.shape == (0,)
         assert data_read.dtype == numpy.float32
 
 
 @pytest.mark.skipif(sys.version_info < (3, 7),
@@ -898,47 +895,47 @@
 def test_utf8(tmp_path):
     """Test that the API handles UTF-8 encoding for the filename."""
     data = numpy.array([1, 2, 3, 4, 5, 10012], dtype=numpy.int64)
 
     fname = '中文.gsd'
 
     with gsd.fl.open(name=tmp_path / fname,
-                     mode='xb',
+                     mode='x',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='chunk1', data=data)
         f.end_frame()
 
     dir_list = os.listdir(tmp_path)
     print(dir_list)
     assert fname in dir_list
 
     with gsd.fl.open(name=tmp_path / fname,
-                     mode='wb',
+                     mode='w',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='chunk1', data=data)
         f.end_frame()
 
     with gsd.fl.open(name=tmp_path / fname,
-                     mode='rb',
+                     mode='r',
                      application='test_open',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.read_chunk(0, name='chunk1')
 
 
-@pytest.mark.parametrize('mode', ['wb', 'wb+', 'ab', 'rb+', 'xb', 'xb+'])
+@pytest.mark.parametrize('mode', ['w', 'x', 'a', 'r+'])
 def test_read_write(tmp_path, mode):
     """Test that data chunks can read from files opened in all write modes."""
     if mode[0] == 'r' or mode[0] == 'a':
         with gsd.fl.open(name=tmp_path / 'test_read_write.gsd',
-                         mode='wb',
+                         mode='w',
                          application='test_read_write',
                          schema='none',
                          schema_version=[1, 2]):
             pass
 
     data = numpy.array([10], dtype=numpy.int64)
     nframes = 1024
```

### Comparing `gsd-2.8.1/gsd/test/test_gsd_v1.gsd` & `gsd-2.9.0/gsd/test/test_gsd_v1.gsd`

 * *Files identical despite different names*

### Comparing `gsd-2.8.1/gsd/test/test_hoomd.py` & `gsd-2.9.0/gsd/test/test_hoomd.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy
 import pickle
 import pytest
 
 
 def test_create(tmp_path):
     """Test that gsd files can be created."""
-    with gsd.hoomd.open(name=tmp_path / "test_create.gsd", mode='wb') as hf:
+    with gsd.hoomd.open(name=tmp_path / "test_create.gsd", mode='w') as hf:
         assert hf.file.schema == 'hoomd'
         assert hf.file.schema_version >= (1, 0)
 
 
 def test_append(tmp_path, open_mode):
     """Test that gsd files can be appended to."""
     frame = gsd.hoomd.Frame()
@@ -666,15 +666,15 @@
         assert view[0].configuration.step == view[0].configuration.step
         assert view[len(view)
                     - 1].configuration.step == view[-1].configuration.step
 
 
 def test_truncate(tmp_path):
     """Test the truncate API."""
-    with gsd.hoomd.open(name=tmp_path / "test_iteration.gsd", mode='wb') as hf:
+    with gsd.hoomd.open(name=tmp_path / "test_iteration.gsd", mode='w') as hf:
         hf.extend((create_frame(i) for i in range(20)))
 
         assert len(hf) == 20
         s = hf[10]  # noqa
         assert hf._initial_frame is not None
 
         hf.truncate()
@@ -762,34 +762,32 @@
         # specified entries are different in frame 1
         numpy.testing.assert_array_equal(s.log['particles/pair_lj_energy'],
                                          frame1.log['particles/pair_lj_energy'])
         numpy.testing.assert_array_equal(s.log['value/pressure'],
                                          frame1.log['value/pressure'])
 
 
-def test_pickle(tmp_path, open_mode):
+def test_pickle(tmp_path):
     """Test that hoomd trajectory objects can be pickled."""
-    with gsd.hoomd.open(name=tmp_path / "test_pickling.gsd",
-                        mode=open_mode.write) as traj:
+    with gsd.hoomd.open(name=tmp_path / "test_pickling.gsd", mode='w') as traj:
         traj.extend((create_frame(i) for i in range(20)))
         with pytest.raises(pickle.PickleError):
             pkl = pickle.dumps(traj)
-    with gsd.hoomd.open(name=tmp_path / "test_pickling.gsd",
-                        mode=open_mode.read) as traj:
+    with gsd.hoomd.open(name=tmp_path / "test_pickling.gsd", mode='r') as traj:
         pkl = pickle.dumps(traj)
         with pickle.loads(pkl) as hf:
             assert len(hf) == 20
 
 
 @pytest.mark.parametrize(
     'container',
     ['particles', 'bonds', 'angles', 'dihedrals', 'impropers', 'pairs'])
 def test_no_duplicate_types(tmp_path, container):
     """Test that duplicate types raise an error."""
-    with gsd.hoomd.open(name=tmp_path / "test_create.gsd", mode='wb') as hf:
+    with gsd.hoomd.open(name=tmp_path / "test_create.gsd", mode='w') as hf:
 
         frame = gsd.hoomd.Frame()
 
         getattr(frame, container).types = ['A', 'B', 'B', 'C']
 
         with pytest.raises(ValueError):
             hf.append(frame)
@@ -815,15 +813,15 @@
         (1, 1, 1),
         (2, 2, 2),
         (3, 3, 3),
         (4, 4, 4),
     ]
     frame1.log['value/pressure'] = [5]
 
-    with gsd.hoomd.open(name=tmp_path / "test_log.gsd", mode='wb') as hf:
+    with gsd.hoomd.open(name=tmp_path / "test_log.gsd", mode='w') as hf:
         hf.extend([frame0, frame1])
 
     # Test scalar_only = False
     logged_data_dict = gsd.hoomd.read_log(name=tmp_path / "test_log.gsd",
                                           scalar_only=False)
 
     assert len(logged_data_dict) == 5
@@ -873,14 +871,14 @@
         [*frame0.log['value/pressure'], *frame1.log['value/pressure']])
 
 
 def test_read_log_warning(tmp_path):
     """Test that read_log issues a warning."""
     frame = gsd.hoomd.Frame()
 
-    with gsd.hoomd.open(name=tmp_path / "test_log.gsd", mode='wb') as hf:
+    with gsd.hoomd.open(name=tmp_path / "test_log.gsd", mode='w') as hf:
         hf.extend([frame])
 
     with pytest.warns(RuntimeWarning):
         log = gsd.hoomd.read_log(tmp_path / "test_log.gsd")
 
     assert list(log.keys()) == ['configuration/step']
```

### Comparing `gsd-2.8.1/gsd/test/test_largefile.py` & `gsd-2.9.0/gsd/test/test_largefile.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 @pytest.mark.parametrize("N", [2**27, 2**28, 2**29 + 1])
 def test_large_n(tmp_path, N):
     """Test data chunks and files larger than 2 GB."""
     gc.collect()
 
     data = numpy.linspace(0, N, num=N, endpoint=False, dtype=numpy.uint32)
     with gsd.fl.open(name=tmp_path / 'test_large_N.gsd',
-                     mode='xb',
+                     mode='x',
                      application='test_large_N',
                      schema='none',
                      schema_version=[1, 2]) as f:
         f.write_chunk(name='data', data=data)
         f.end_frame()
 
     with gsd.fl.open(name=tmp_path / 'test_large_N.gsd',
-                     mode='rb',
+                     mode='r',
                      application='test_large_N',
                      schema='none',
                      schema_version=[1, 2]) as f:
         read_data = f.read_chunk(frame=0, name='data')
 
         # compare the array with memory usage so this test can pass on CI
         # platforms
```

### Comparing `gsd-2.8.1/gsd.egg-info/PKG-INFO` & `gsd-2.9.0/gsd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: gsd
-Version: 2.8.1
+Version: 2.9.0
 Summary: General simulation data file format.
-Home-page: https://gsd.readthedocs.io
-Author: Joshua A. Anderson
-Author-email: joaander@umich.edu
-License: BSD - 2 clause
-Download-URL: https://github.com/glotzerlab/gsd/releases/download/v2.8.1/gsd-v2.8.1.tar.gz
+Author-email: "Joshua A. Anderson" <joaander@umich.edu>
+License: BSD-2-Clause
+Project-URL: Homepage, https://gsd.readthedocs.io
 Project-URL: Documentation, https://gsd.readthedocs.io
-Project-URL: Source Code, https://github.com/glotzerlab/gsd
-Project-URL: Issue Tracker, https://github.com/glotzerlab/gsd/issues
-Platform: UNKNOWN
+Project-URL: Download, https://github.com/glotzerlab/gsd/releases/download/v2.9.0/gsd-v2.9.0.tar.gz
+Project-URL: Source, https://github.com/glotzerlab/gsd
+Project-URL: Issues, https://github.com/glotzerlab/gsd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -48,15 +46,15 @@
 ```python
 >>> s = gsd.hoomd.Frame()
 >>> s.particles.N = 4
 >>> s.particles.types = ['A', 'B']
 >>> s.particles.typeid = [0,0,1,1]
 >>> s.particles.position = [[0,0,0],[1,1,1], [-1,-1,-1], [1,-1,-1]]
 >>> s.configuration.box = [3, 3, 3, 0, 0, 0]
->>> traj = gsd.hoomd.open(name='test.gsd', mode='wb')
+>>> traj = gsd.hoomd.open(name='test.gsd', mode='w')
 >>> traj.append(s)
 ```
 
 Append frames to a gsd file:
 ```python
 >>> def create_frame(i):
 ...     s = gsd.hoomd.Frame();
@@ -68,15 +66,15 @@
 ...     t.extend( (create_frame(i) for i in range(10)) )
 ...     print(len(t))
 11
 ```
 
 Randomly index frames:
 ```python
->>> with gsd.hoomd.open('test.gsd', 'rb') as t:
+>>> with gsd.hoomd.open('test.gsd', 'r') as t:
 ...     frame = t[5]
 ...     print(frame.configuration.step)
 4
 ...     print(frame.particles.N)
 8
 ...     print(frame.particles.position)
 [[ 0.56993282  0.42243481  0.5502916 ]
@@ -87,31 +85,29 @@
  [ 0.13724308  0.14253527  0.02505   ]
  [ 0.39287439  0.82519054  0.01613089]
  [ 0.23150323  0.95167434  0.7715748 ]]
 ```
 
 Slice frames:
 ```python
->>> with gsd.hoomd.open('test.gsd', 'rb') as t:
+>>> with gsd.hoomd.open('test.gsd', 'r') as t:
 ...     for s in t[5:-2]:
 ...         print(s.configuration.step, end=' ')
 4 5 6 7
 ```
 
 ## File layer examples
 
 ```python
-with gsd.fl.open(name='file.gsd', mode='wb') as f:
+with gsd.fl.open(name='file.gsd', mode='w') as f:
     f.write_chunk(name='position', data=numpy.array([[1,2,3],[4,5,6]], dtype=numpy.float32));
     f.write_chunk(name='angle', data=numpy.array([0, 1], dtype=numpy.float32));
     f.write_chunk(name='box', data=numpy.array([10, 10, 10], dtype=numpy.float32));
     f.end_frame()
 ```
 
 ```python
-with gsd.fl.open(name='file.gsd', mode='rb') as f:
+with gsd.fl.open(name='file.gsd', mode='r') as f:
     for i in range(1,f.nframes):
         position = f.read_chunk(frame=i, name='position');
         do_something(position);
 ```
-
-
```

### Comparing `gsd-2.8.1/gsd.egg-info/SOURCES.txt` & `gsd-2.9.0/gsd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 gsd/__init__.py
```

### Comparing `gsd-2.8.1/setup.cfg` & `gsd-2.9.0/setup.cfg`

 * *Files identical despite different names*

