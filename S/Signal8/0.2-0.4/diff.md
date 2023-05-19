# Comparing `tmp/Signal8-0.2.tar.gz` & `tmp/Signal8-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-0.2.tar", last modified: Wed May 17 21:25:47 2023, max compression
+gzip compressed data, was "Signal8-0.4.tar", last modified: Fri May 19 04:45:15 2023, max compression
```

## Comparing `Signal8-0.2.tar` & `Signal8-0.4.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 21:25:47.464644 Signal8-0.2/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-0.2/LICENSE
--rw-rw-rw-   0        0        0     4371 2023-05-17 21:25:47.454646 Signal8-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-05-17 21:23:57.000000 Signal8-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 21:25:47.452645 Signal8-0.2/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4371 2023-05-17 21:25:47.000000 Signal8-0.2/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-05-17 21:25:47.000000 Signal8-0.2/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 21:25:47.000000 Signal8-0.2/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 21:25:47.000000 Signal8-0.2/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 21:25:47.464644 Signal8-0.2/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-05-17 21:24:54.000000 Signal8-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 04:45:15.940734 Signal8-0.4/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-0.4/LICENSE
+-rw-rw-rw-   0        0        0     4371 2023-05-19 04:45:15.938732 Signal8-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3881 2023-05-17 21:23:57.000000 Signal8-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 04:45:15.912732 Signal8-0.4/Signal8/
+-rw-rw-rw-   0        0        0     6675 2023-05-19 04:12:41.000000 Signal8-0.4/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 04:32:59.000000 Signal8-0.4/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      117 2023-05-19 04:35:05.000000 Signal8-0.4/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-19 04:45:15.934733 Signal8-0.4/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4371 2023-05-19 04:45:15.000000 Signal8-0.4/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-19 04:45:15.000000 Signal8-0.4/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 04:45:15.000000 Signal8-0.4/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 04:45:15.000000 Signal8-0.4/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 04:45:15.940734 Signal8-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-05-19 04:40:52.000000 Signal8-0.4/setup.py
```

### Comparing `Signal8-0.2/LICENSE` & `Signal8-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-0.2/PKG-INFO` & `Signal8-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 0.2
+Version: 0.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-0.2/README.md` & `Signal8-0.4/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-0.2/Signal8.egg-info/PKG-INFO` & `Signal8-0.4/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 0.2
+Version: 0.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-0.2/setup.py` & `Signal8-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="0.2",
+    version="0.4",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic adversaries.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

