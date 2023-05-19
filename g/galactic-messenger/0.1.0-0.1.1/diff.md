# Comparing `tmp/galactic-messenger-0.1.0.tar.gz` & `tmp/galactic-messenger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galactic-messenger-0.1.0.tar", last modified: Fri May 19 03:07:52 2023, max compression
+gzip compressed data, was "galactic-messenger-0.1.1.tar", last modified: Fri May 19 03:41:51 2023, max compression
```

## Comparing `galactic-messenger-0.1.0.tar` & `galactic-messenger-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 03:07:52.585173 galactic-messenger-0.1.0/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     1059 2023-05-19 03:05:50.000000 galactic-messenger-0.1.0/LICENSE
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4880 2023-05-19 03:07:52.585326 galactic-messenger-0.1.0/PKG-INFO
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4146 2023-05-18 11:48:15.000000 galactic-messenger-0.1.0/README.md
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 03:07:52.584859 galactic-messenger-0.1.0/galactic_messenger.egg-info/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4880 2023-05-19 03:07:52.000000 galactic-messenger-0.1.0/galactic_messenger.egg-info/PKG-INFO
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      260 2023-05-19 03:07:52.000000 galactic-messenger-0.1.0/galactic_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)        1 2023-05-19 03:07:52.000000 galactic-messenger-0.1.0/galactic_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-19 03:07:52.000000 galactic-messenger-0.1.0/galactic_messenger.egg-info/requires.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)        1 2023-05-19 03:07:52.000000 galactic-messenger-0.1.0/galactic_messenger.egg-info/top_level.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      442 2023-05-12 09:46:57.000000 galactic-messenger-0.1.0/pyproject.toml
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      495 2023-05-19 03:07:52.585870 galactic-messenger-0.1.0/setup.cfg
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      919 2023-05-19 03:04:19.000000 galactic-messenger-0.1.0/setup.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 03:41:51.540562 galactic-messenger-0.1.1/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     1059 2023-05-19 03:05:50.000000 galactic-messenger-0.1.1/LICENSE
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4880 2023-05-19 03:41:51.541170 galactic-messenger-0.1.1/PKG-INFO
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4146 2023-05-18 11:48:15.000000 galactic-messenger-0.1.1/README.md
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 03:41:51.530745 galactic-messenger-0.1.1/galactic_messenger/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      113 2023-05-19 03:39:39.000000 galactic-messenger-0.1.1/galactic_messenger/__init__.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      291 2023-05-19 02:56:12.000000 galactic-messenger-0.1.1/galactic_messenger/config.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 03:41:51.539412 galactic-messenger-0.1.1/galactic_messenger.egg-info/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4880 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      320 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)        1 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/requires.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)       19 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/top_level.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      442 2023-05-12 09:46:57.000000 galactic-messenger-0.1.1/pyproject.toml
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      495 2023-05-19 03:41:51.542878 galactic-messenger-0.1.1/setup.cfg
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      919 2023-05-19 03:39:24.000000 galactic-messenger-0.1.1/setup.py
```

### Comparing `galactic-messenger-0.1.0/LICENSE` & `galactic-messenger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.0/PKG-INFO` & `galactic-messenger-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galactic-messenger
-Version: 0.1.0
+Version: 0.1.1
 Summary: Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.
 Home-page: https://github.com/Invigilo-AI/galactic-messenger
 Author: InvigiloAI
 Author-email: contact@invigilo.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `galactic-messenger-0.1.0/README.md` & `galactic-messenger-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.0/galactic_messenger.egg-info/PKG-INFO` & `galactic-messenger-0.1.1/galactic_messenger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galactic-messenger
-Version: 0.1.0
+Version: 0.1.1
 Summary: Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.
 Home-page: https://github.com/Invigilo-AI/galactic-messenger
 Author: InvigiloAI
 Author-email: contact@invigilo.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `galactic-messenger-0.1.0/setup.py` & `galactic-messenger-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="galactic-messenger",
-    version="0.1.0",
+    version="0.1.1",
     author="InvigiloAI",
     author_email="contact@invigilo.ai",
     description="Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Invigilo-AI/galactic-messenger",
     packages=find_packages(),
```

