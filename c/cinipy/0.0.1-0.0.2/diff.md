# Comparing `tmp/cinipy-0.0.1.tar.gz` & `tmp/cinipy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cinipy-0.0.1.tar", last modified: Fri May 19 19:24:12 2023, max compression
+gzip compressed data, was "cinipy-0.0.2.tar", last modified: Fri May 19 19:41:03 2023, max compression
```

## Comparing `cinipy-0.0.1.tar` & `cinipy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jr        (1000) jr        (1000)        0 2023-05-19 19:24:12.197026 cinipy-0.0.1/
--rw-r--r--   0 jr        (1000) jr        (1000)      909 2023-05-19 19:24:12.197026 cinipy-0.0.1/PKG-INFO
--rw-r--r--   0 jr        (1000) jr        (1000)      335 2023-05-19 19:17:52.000000 cinipy-0.0.1/README.md
-drwxr-xr-x   0 jr        (1000) jr        (1000)        0 2023-05-19 19:24:12.197026 cinipy-0.0.1/cinipy/
--rw-r--r--   0 jr        (1000) jr        (1000)       53 2023-05-19 19:23:40.000000 cinipy-0.0.1/cinipy/__init__.py
--rw-r--r--   0 jr        (1000) jr        (1000)     1741 2023-05-19 19:08:08.000000 cinipy-0.0.1/cinipy/cinipy.py
-drwxr-xr-x   0 jr        (1000) jr        (1000)        0 2023-05-19 19:24:12.197026 cinipy-0.0.1/cinipy.egg-info/
--rw-r--r--   0 jr        (1000) jr        (1000)      909 2023-05-19 19:24:12.000000 cinipy-0.0.1/cinipy.egg-info/PKG-INFO
--rw-r--r--   0 jr        (1000) jr        (1000)      203 2023-05-19 19:24:12.000000 cinipy-0.0.1/cinipy.egg-info/SOURCES.txt
--rw-r--r--   0 jr        (1000) jr        (1000)        1 2023-05-19 19:24:12.000000 cinipy-0.0.1/cinipy.egg-info/dependency_links.txt
--rw-r--r--   0 jr        (1000) jr        (1000)        9 2023-05-19 19:24:12.000000 cinipy-0.0.1/cinipy.egg-info/requires.txt
--rw-r--r--   0 jr        (1000) jr        (1000)        7 2023-05-19 19:24:12.000000 cinipy-0.0.1/cinipy.egg-info/top_level.txt
--rw-r--r--   0 jr        (1000) jr        (1000)       38 2023-05-19 19:24:12.197026 cinipy-0.0.1/setup.cfg
--rw-r--r--   0 jr        (1000) jr        (1000)      794 2023-05-19 19:22:48.000000 cinipy-0.0.1/setup.py
+drwxr-xr-x   0 jr        (1000) jr        (1000)        0 2023-05-19 19:41:03.912157 cinipy-0.0.2/
+-rw-r--r--   0 jr        (1000) jr        (1000)     1122 2023-05-19 19:41:03.912157 cinipy-0.0.2/PKG-INFO
+-rw-r--r--   0 jr        (1000) jr        (1000)      547 2023-05-19 19:37:27.000000 cinipy-0.0.2/README.md
+drwxr-xr-x   0 jr        (1000) jr        (1000)        0 2023-05-19 19:41:03.908824 cinipy-0.0.2/cinipy/
+-rw-r--r--   0 jr        (1000) jr        (1000)       53 2023-05-19 19:23:40.000000 cinipy-0.0.2/cinipy/__init__.py
+-rw-r--r--   0 jr        (1000) jr        (1000)     1741 2023-05-19 19:08:08.000000 cinipy-0.0.2/cinipy/cinipy.py
+drwxr-xr-x   0 jr        (1000) jr        (1000)        0 2023-05-19 19:41:03.912157 cinipy-0.0.2/cinipy.egg-info/
+-rw-r--r--   0 jr        (1000) jr        (1000)     1122 2023-05-19 19:41:03.000000 cinipy-0.0.2/cinipy.egg-info/PKG-INFO
+-rw-r--r--   0 jr        (1000) jr        (1000)      203 2023-05-19 19:41:03.000000 cinipy-0.0.2/cinipy.egg-info/SOURCES.txt
+-rw-r--r--   0 jr        (1000) jr        (1000)        1 2023-05-19 19:41:03.000000 cinipy-0.0.2/cinipy.egg-info/dependency_links.txt
+-rw-r--r--   0 jr        (1000) jr        (1000)        9 2023-05-19 19:41:03.000000 cinipy-0.0.2/cinipy.egg-info/requires.txt
+-rw-r--r--   0 jr        (1000) jr        (1000)        7 2023-05-19 19:41:03.000000 cinipy-0.0.2/cinipy.egg-info/top_level.txt
+-rw-r--r--   0 jr        (1000) jr        (1000)       38 2023-05-19 19:41:03.912157 cinipy-0.0.2/setup.cfg
+-rw-r--r--   0 jr        (1000) jr        (1000)      794 2023-05-19 19:39:00.000000 cinipy-0.0.2/setup.py
```

### Comparing `cinipy-0.0.1/PKG-INFO` & `cinipy-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 Metadata-Version: 2.1
 Name: cinipy
-Version: 0.0.1
+Version: 0.0.2
 Summary: An app for custom logging
 Author: jonasrdl
 Author-email: jonasriedel@pm.me
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# cini
+# cinipy
 
-cini is an app for custom logging.
+cinipy is an app for custom logging.
 
 ## Installation
 
 You can install the app using pip:
-
-**Coming soon**   
-~~pip install cini~~ 
+  
+`pip install cinipy`
 
 ## Usage
 
 ```python
-from cini import log_info, log_warning, log_error
+from cinipy import log_info, log_warning, log_error
 
 log_info("This is an info message.")
 log_warning({"key": "value", "key2": [1, 2, 3]})
 log_error(["error", {"key": "value"}])
+```
+
+### Future features
+
+- [ ] Custom Formatting
+- [ ] Log handlers
+  - [ ] Write logs to a file
+  - [ ] Send logs to remote server
+  - [ ] Stream to Elasticsearch, logstash, ...
+- [ ] More configure options
+- [ ] Filtering
```

### Comparing `cinipy-0.0.1/cinipy/cinipy.py` & `cinipy-0.0.2/cinipy/cinipy.py`

 * *Files identical despite different names*

### Comparing `cinipy-0.0.1/cinipy.egg-info/PKG-INFO` & `cinipy-0.0.2/cinipy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 Metadata-Version: 2.1
 Name: cinipy
-Version: 0.0.1
+Version: 0.0.2
 Summary: An app for custom logging
 Author: jonasrdl
 Author-email: jonasriedel@pm.me
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# cini
+# cinipy
 
-cini is an app for custom logging.
+cinipy is an app for custom logging.
 
 ## Installation
 
 You can install the app using pip:
-
-**Coming soon**   
-~~pip install cini~~ 
+  
+`pip install cinipy`
 
 ## Usage
 
 ```python
-from cini import log_info, log_warning, log_error
+from cinipy import log_info, log_warning, log_error
 
 log_info("This is an info message.")
 log_warning({"key": "value", "key2": [1, 2, 3]})
 log_error(["error", {"key": "value"}])
+```
+
+### Future features
+
+- [ ] Custom Formatting
+- [ ] Log handlers
+  - [ ] Write logs to a file
+  - [ ] Send logs to remote server
+  - [ ] Stream to Elasticsearch, logstash, ...
+- [ ] More configure options
+- [ ] Filtering
```

### Comparing `cinipy-0.0.1/setup.py` & `cinipy-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cinipy',
-    version='0.0.1',
+    version='0.0.2',
     author='jonasrdl',
     author_email='jonasriedel@pm.me',
     description='An app for custom logging',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

