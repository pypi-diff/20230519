# Comparing `tmp/Enumerator_linux-3.0.tar.gz` & `tmp/Enumerator_linux-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Enumerator_linux-3.0.tar", last modified: Fri May 19 05:15:17 2023, max compression
+gzip compressed data, was "dist/Enumerator_linux-4.0.tar", last modified: Fri May 19 05:40:44 2023, max compression
```

## Comparing `Enumerator_linux-3.0.tar` & `Enumerator_linux-4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 sulthan   (1001) sulthan   (1001)        0 2023-05-19 05:15:17.000000 Enumerator_linux-3.0/
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)       38 2023-05-19 05:15:17.000000 Enumerator_linux-3.0/setup.cfg
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)    11605 2023-05-19 05:13:08.000000 Enumerator_linux-3.0/Enumerator_linux.cpp
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      231 2023-05-19 05:15:17.000000 Enumerator_linux-3.0/PKG-INFO
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)     1646 2023-05-19 05:13:42.000000 Enumerator_linux-3.0/setup.py
-drwxrwxr-x   0 sulthan   (1001) sulthan   (1001)        0 2023-05-19 05:15:17.000000 Enumerator_linux-3.0/Enumerator_linux.egg-info/
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)        1 2023-05-19 05:15:17.000000 Enumerator_linux-3.0/Enumerator_linux.egg-info/dependency_links.txt
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      231 2023-05-19 05:15:17.000000 Enumerator_linux-3.0/Enumerator_linux.egg-info/PKG-INFO
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)        1 2023-05-19 04:59:22.000000 Enumerator_linux-3.0/Enumerator_linux.egg-info/not-zip-safe
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)       17 2023-05-19 05:15:17.000000 Enumerator_linux-3.0/Enumerator_linux.egg-info/top_level.txt
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      228 2023-05-19 05:15:17.000000 Enumerator_linux-3.0/Enumerator_linux.egg-info/SOURCES.txt
+drwxrwxr-x   0 sulthan   (1001) sulthan   (1001)        0 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)       38 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/setup.cfg
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)    11605 2023-05-19 05:13:08.000000 Enumerator_linux-4.0/Enumerator_linux.cpp
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      231 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/PKG-INFO
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)     1646 2023-05-19 05:40:00.000000 Enumerator_linux-4.0/setup.py
+drwxrwxr-x   0 sulthan   (1001) sulthan   (1001)        0 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/Enumerator_linux.egg-info/
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)        1 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/Enumerator_linux.egg-info/dependency_links.txt
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      231 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/Enumerator_linux.egg-info/PKG-INFO
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)        1 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/Enumerator_linux.egg-info/not-zip-safe
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)       17 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/Enumerator_linux.egg-info/top_level.txt
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      228 2023-05-19 05:40:44.000000 Enumerator_linux-4.0/Enumerator_linux.egg-info/SOURCES.txt
```

### Comparing `Enumerator_linux-3.0/Enumerator_linux.cpp` & `Enumerator_linux-4.0/Enumerator_linux.cpp`

 * *Files identical despite different names*

### Comparing `Enumerator_linux-3.0/setup.py` & `Enumerator_linux-4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         for ext in self.extensions:
             ext.extra_compile_args = extra_compile_args
         build_ext.build_extensions(self)
 
 # Setup configuration
 setup(
     name='Enumerator_linux',
-    version='3.0',
+    version='4.0',
     description='Enumerator Linux Extension Module',
     author='Your Name',
     author_email='your_email@example.com',
     ext_modules=[ext_module],
     cmdclass={'build_ext': BuildExt},
     zip_safe=False
 )
```

