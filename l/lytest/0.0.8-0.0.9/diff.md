# Comparing `tmp/lytest-0.0.8.tar.gz` & `tmp/lytest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lytest-0.0.8.tar", last modified: Thu Nov 15 05:03:06 2018, max compression
+gzip compressed data, was "dist/lytest-0.0.9.tar", last modified: Thu Nov 15 05:38:12 2018, max compression
```

## Comparing `lytest-0.0.8.tar` & `lytest-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-15 05:03:06.000000 lytest-0.0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12395 2018-11-15 05:02:17.000000 lytest-0.0.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      638 2018-11-15 05:02:17.000000 lytest-0.0.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-15 05:03:06.000000 lytest-0.0.8/lytest.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2018-11-15 05:03:06.000000 lytest-0.0.8/lytest.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2018-11-15 05:03:06.000000 lytest-0.0.8/lytest.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    14396 2018-11-15 05:03:06.000000 lytest-0.0.8/lytest.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-11-15 05:03:06.000000 lytest-0.0.8/lytest.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2018-11-15 05:03:06.000000 lytest-0.0.8/lytest.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      302 2018-11-15 05:03:06.000000 lytest-0.0.8/lytest.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-11-15 05:03:06.000000 lytest-0.0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    14396 2018-11-15 05:03:06.000000 lytest-0.0.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-15 05:03:06.000000 lytest-0.0.8/lytest/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3693 2018-11-15 05:02:17.000000 lytest-0.0.8/lytest/kdb_xor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2473 2018-11-15 05:02:17.000000 lytest-0.0.8/lytest/utest_buds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2018-11-15 05:02:17.000000 lytest-0.0.8/lytest/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3094 2018-11-15 05:02:17.000000 lytest-0.0.8/lytest/containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7488 2018-11-15 05:02:17.000000 lytest-0.0.8/lytest/command_line.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-15 05:38:12.000000 lytest-0.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12395 2018-11-15 05:37:25.000000 lytest-0.0.9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      638 2018-11-15 05:37:25.000000 lytest-0.0.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-15 05:38:12.000000 lytest-0.0.9/lytest.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2018-11-15 05:38:12.000000 lytest-0.0.9/lytest.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       31 2018-11-15 05:38:12.000000 lytest-0.0.9/lytest.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14396 2018-11-15 05:38:12.000000 lytest-0.0.9/lytest.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-11-15 05:38:12.000000 lytest-0.0.9/lytest.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2018-11-15 05:38:12.000000 lytest-0.0.9/lytest.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      302 2018-11-15 05:38:12.000000 lytest-0.0.9/lytest.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-11-15 05:38:12.000000 lytest-0.0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14396 2018-11-15 05:38:12.000000 lytest-0.0.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-11-15 05:38:12.000000 lytest-0.0.9/lytest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5332 2018-11-15 05:37:25.000000 lytest-0.0.9/lytest/kdb_xor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2473 2018-11-15 05:37:25.000000 lytest-0.0.9/lytest/utest_buds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2018-11-15 05:37:25.000000 lytest-0.0.9/lytest/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3094 2018-11-15 05:37:25.000000 lytest-0.0.9/lytest/containers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7488 2018-11-15 05:37:25.000000 lytest-0.0.9/lytest/command_line.py
```

### Comparing `lytest-0.0.8/README.md` & `lytest-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lytest-0.0.8/setup.py` & `lytest-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def readme():
     with open('README.md', 'r') as fx:
       return fx.read()
 
 
 setup(name='lytest',
-      version='0.0.8',
+      version='0.0.9',
       description='Regression testing for klayout and phidl',
       long_description=readme(),
       author='Alex Tait, Adam McCaughan, Sonia Buckley, Jeff Chiles, Jeff Shainline, Rich Mirin, Sae Woo Nam',
       author_email='alexander.tait@nist.gov',
       license='MIT',
       packages=['lytest'],
       install_requires=['klayout', 'pytest', 'lygadgets', 'lyipc'],
```

### Comparing `lytest-0.0.8/lytest.egg-info/PKG-INFO` & `lytest-0.0.9/lytest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: lytest
-Version: 0.0.8
+Version: 0.0.9
 Summary: Regression testing for klayout and phidl
 Home-page: UNKNOWN
 Author: Alex Tait, Adam McCaughan, Sonia Buckley, Jeff Chiles, Jeff Shainline, Rich Mirin, Sae Woo Nam
 Author-email: alexander.tait@nist.gov
 License: MIT
 Description: [![Build Status](https://travis-ci.org/atait/lytest.svg?branch=master)](https://travis-ci.org/atait/lytest)
```

### Comparing `lytest-0.0.8/PKG-INFO` & `lytest-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: lytest
-Version: 0.0.8
+Version: 0.0.9
 Summary: Regression testing for klayout and phidl
 Home-page: UNKNOWN
 Author: Alex Tait, Adam McCaughan, Sonia Buckley, Jeff Chiles, Jeff Shainline, Rich Mirin, Sae Woo Nam
 Author-email: alexander.tait@nist.gov
 License: MIT
 Description: [![Build Status](https://travis-ci.org/atait/lytest.svg?branch=master)](https://travis-ci.org/atait/lytest)
```

### Comparing `lytest-0.0.8/lytest/utest_buds.py` & `lytest-0.0.9/lytest/utest_buds.py`

 * *Files identical despite different names*

### Comparing `lytest-0.0.8/lytest/__init__.py` & `lytest-0.0.9/lytest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 # quickplotters so you can debug more easily
 try:
     import lyipc.client as ipc
     kqp = ipc.generate_display_function(None, 'debugging.gds')
 except ImportError:
     def kqp(*args, **kwargs):
```

### Comparing `lytest-0.0.8/lytest/containers.py` & `lytest-0.0.9/lytest/containers.py`

 * *Files identical despite different names*

### Comparing `lytest-0.0.8/lytest/command_line.py` & `lytest-0.0.9/lytest/command_line.py`

 * *Files identical despite different names*

