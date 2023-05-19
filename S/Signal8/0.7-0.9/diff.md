# Comparing `tmp/Signal8-0.7.tar.gz` & `tmp/Signal8-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-0.7.tar", last modified: Fri May 19 05:14:13 2023, max compression
+gzip compressed data, was "Signal8-0.9.tar", last modified: Fri May 19 15:47:57 2023, max compression
```

## Comparing `Signal8-0.7.tar` & `Signal8-0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 05:14:13.571059 Signal8-0.7/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-0.7/LICENSE
--rw-rw-rw-   0        0        0     4371 2023-05-19 05:14:13.569055 Signal8-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-05-17 21:23:57.000000 Signal8-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 05:14:13.505056 Signal8-0.7/Signal8/
--rw-rw-rw-   0        0        0     6682 2023-05-19 05:13:45.000000 Signal8-0.7/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-05-19 05:04:09.000000 Signal8-0.7/Signal8/__init__.py
--rw-rw-rw-   0        0        0      136 2023-05-19 05:13:31.000000 Signal8-0.7/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:14:13.564059 Signal8-0.7/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-0.7/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7891 2023-05-17 20:35:42.000000 Signal8-0.7/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2459 2023-05-17 19:04:54.000000 Signal8-0.7/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-0.7/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12585 2023-05-19 05:11:53.000000 Signal8-0.7/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:14:13.540056 Signal8-0.7/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4371 2023-05-19 05:14:13.000000 Signal8-0.7/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-19 05:14:13.000000 Signal8-0.7/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 05:14:13.000000 Signal8-0.7/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 05:14:13.000000 Signal8-0.7/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 05:14:13.575056 Signal8-0.7/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-05-19 05:13:57.000000 Signal8-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 15:47:57.140470 Signal8-0.9/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-0.9/LICENSE
+-rw-rw-rw-   0        0        0     4371 2023-05-19 15:47:57.138468 Signal8-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-05-17 21:23:57.000000 Signal8-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 15:47:57.063468 Signal8-0.9/Signal8/
+-rw-rw-rw-   0        0        0     6682 2023-05-19 05:13:45.000000 Signal8-0.9/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-0.9/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-05-19 05:13:31.000000 Signal8-0.9/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 15:47:57.133469 Signal8-0.9/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-0.9/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     7891 2023-05-17 20:35:42.000000 Signal8-0.9/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2459 2023-05-17 19:04:54.000000 Signal8-0.9/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-0.9/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12585 2023-05-19 05:11:53.000000 Signal8-0.9/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-19 15:47:57.109470 Signal8-0.9/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4371 2023-05-19 15:47:56.000000 Signal8-0.9/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-19 15:47:56.000000 Signal8-0.9/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 15:47:56.000000 Signal8-0.9/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 15:47:56.000000 Signal8-0.9/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 15:47:57.141469 Signal8-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-05-19 15:47:47.000000 Signal8-0.9/setup.py
```

### Comparing `Signal8-0.7/LICENSE` & `Signal8-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-0.7/PKG-INFO` & `Signal8-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 0.7
+Version: 0.9
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-0.7/README.md` & `Signal8-0.9/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-0.7/Signal8/Signal8.py` & `Signal8-0.9/Signal8/Signal8.py`

 * *Files identical despite different names*

### Comparing `Signal8-0.7/Signal8/utils/core.py` & `Signal8-0.9/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-0.7/Signal8/utils/problems.py` & `Signal8-0.9/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-0.7/Signal8/utils/simple_env.py` & `Signal8-0.9/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-0.7/Signal8.egg-info/PKG-INFO` & `Signal8-0.9/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 0.7
+Version: 0.9
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-0.7/setup.py` & `Signal8-0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="0.7",
+    version="0.9",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

