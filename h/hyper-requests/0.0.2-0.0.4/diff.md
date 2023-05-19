# Comparing `tmp/hyper_requests-0.0.2.tar.gz` & `tmp/hyper-requests-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper_requests-0.0.2.tar", last modified: Fri May 19 15:51:21 2023, max compression
+gzip compressed data, was "hyper-requests-0.0.4.tar", last modified: Fri May 19 16:34:36 2023, max compression
```

## Comparing `hyper_requests-0.0.2.tar` & `hyper-requests-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 edward.jones   (503) staff       (20)        0 2023-05-19 15:51:21.593645 hyper_requests-0.0.2/
--rw-r--r--   0 edward.jones   (503) staff       (20)     1066 2023-05-19 15:00:38.000000 hyper_requests-0.0.2/LICENSE
--rw-r--r--   0 edward.jones   (503) staff       (20)       34 2023-05-19 15:03:25.000000 hyper_requests-0.0.2/MANIFEST.in
--rw-r--r--   0 edward.jones   (503) staff       (20)     1881 2023-05-19 15:51:21.593708 hyper_requests-0.0.2/PKG-INFO
--rw-r--r--   0 edward.jones   (503) staff       (20)     1485 2023-05-19 14:49:36.000000 hyper_requests-0.0.2/README.md
--rw-r--r--   0 edward.jones   (503) staff       (20)      162 2023-05-19 15:51:21.593988 hyper_requests-0.0.2/setup.cfg
--rw-r--r--   0 edward.jones   (503) staff       (20)      665 2023-05-19 15:50:50.000000 hyper_requests-0.0.2/setup.py
-drwxr-xr-x   0 edward.jones   (503) staff       (20)        0 2023-05-19 15:51:21.592329 hyper_requests-0.0.2/src/
-drwxr-xr-x   0 edward.jones   (503) staff       (20)        0 2023-05-19 15:51:21.593520 hyper_requests-0.0.2/src/hyper_requests.egg-info/
--rw-r--r--   0 edward.jones   (503) staff       (20)     1881 2023-05-19 15:51:21.000000 hyper_requests-0.0.2/src/hyper_requests.egg-info/PKG-INFO
--rw-r--r--   0 edward.jones   (503) staff       (20)      216 2023-05-19 15:51:21.000000 hyper_requests-0.0.2/src/hyper_requests.egg-info/SOURCES.txt
--rw-r--r--   0 edward.jones   (503) staff       (20)        1 2023-05-19 15:51:21.000000 hyper_requests-0.0.2/src/hyper_requests.egg-info/dependency_links.txt
--rw-r--r--   0 edward.jones   (503) staff       (20)        1 2023-05-19 15:51:21.000000 hyper_requests-0.0.2/src/hyper_requests.egg-info/top_level.txt
+drwxr-xr-x   0 edward.jones   (503) staff       (20)        0 2023-05-19 16:34:36.997229 hyper-requests-0.0.4/
+-rw-r--r--   0 edward.jones   (503) staff       (20)     1066 2023-05-19 15:00:38.000000 hyper-requests-0.0.4/LICENSE
+-rw-r--r--   0 edward.jones   (503) staff       (20)       34 2023-05-19 15:03:25.000000 hyper-requests-0.0.4/MANIFEST.in
+-rw-r--r--   0 edward.jones   (503) staff       (20)     1881 2023-05-19 16:34:36.997289 hyper-requests-0.0.4/PKG-INFO
+-rw-r--r--   0 edward.jones   (503) staff       (20)     1485 2023-05-19 14:49:36.000000 hyper-requests-0.0.4/README.md
+-rw-r--r--   0 edward.jones   (503) staff       (20)      162 2023-05-19 16:34:36.997514 hyper-requests-0.0.4/setup.cfg
+-rw-r--r--   0 edward.jones   (503) staff       (20)      584 2023-05-19 16:34:34.000000 hyper-requests-0.0.4/setup.py
+drwxr-xr-x   0 edward.jones   (503) staff       (20)        0 2023-05-19 16:34:36.996505 hyper-requests-0.0.4/src/
+-rw-r--r--   0 edward.jones   (503) staff       (20)        0 2023-05-19 16:28:41.000000 hyper-requests-0.0.4/src/__init__.py
+drwxr-xr-x   0 edward.jones   (503) staff       (20)        0 2023-05-19 16:34:36.997114 hyper-requests-0.0.4/src/hyper_requests.egg-info/
+-rw-r--r--   0 edward.jones   (503) staff       (20)     1881 2023-05-19 16:34:36.000000 hyper-requests-0.0.4/src/hyper_requests.egg-info/PKG-INFO
+-rw-r--r--   0 edward.jones   (503) staff       (20)      271 2023-05-19 16:34:36.000000 hyper-requests-0.0.4/src/hyper_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 edward.jones   (503) staff       (20)        1 2023-05-19 16:34:36.000000 hyper-requests-0.0.4/src/hyper_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 edward.jones   (503) staff       (20)       34 2023-05-19 16:34:36.000000 hyper-requests-0.0.4/src/hyper_requests.egg-info/top_level.txt
+-rw-r--r--   0 edward.jones   (503) staff       (20)     1090 2023-05-19 14:26:56.000000 hyper-requests-0.0.4/src/request_builder.py
+-rw-r--r--   0 edward.jones   (503) staff       (20)     2173 2023-05-19 14:33:41.000000 hyper-requests-0.0.4/src/threader.py
```

### Comparing `hyper_requests-0.0.2/LICENSE` & `hyper-requests-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.2/PKG-INFO` & `hyper-requests-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyper_requests
-Version: 0.0.2
+Name: hyper-requests
+Version: 0.0.4
 Summary: Concurrent request HTTP execution library
 Author: Edward Jones
 Author-email: ejones84@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `hyper_requests-0.0.2/README.md` & `hyper-requests-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.2/setup.py` & `hyper-requests-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import setuptools
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="hyper_requests",
-    version="0.0.2",
+    name="hyper-requests",
+    version="0.0.4",
     author="Edward Jones",
     author_email="ejones84@icloud.com",
     description="Concurrent request HTTP execution library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

### Comparing `hyper_requests-0.0.2/src/hyper_requests.egg-info/PKG-INFO` & `hyper-requests-0.0.4/src/hyper_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-requests
-Version: 0.0.2
+Version: 0.0.4
 Summary: Concurrent request HTTP execution library
 Author: Edward Jones
 Author-email: ejones84@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

