# Comparing `tmp/galactic-messenger-0.1.1.tar.gz` & `tmp/galactic-messenger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galactic-messenger-0.1.1.tar", last modified: Fri May 19 03:41:51 2023, max compression
+gzip compressed data, was "galactic-messenger-0.1.2.tar", last modified: Fri May 19 04:32:01 2023, max compression
```

## Comparing `galactic-messenger-0.1.1.tar` & `galactic-messenger-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,34 @@
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 03:41:51.540562 galactic-messenger-0.1.1/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     1059 2023-05-19 03:05:50.000000 galactic-messenger-0.1.1/LICENSE
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4880 2023-05-19 03:41:51.541170 galactic-messenger-0.1.1/PKG-INFO
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4146 2023-05-18 11:48:15.000000 galactic-messenger-0.1.1/README.md
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 03:41:51.530745 galactic-messenger-0.1.1/galactic_messenger/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      113 2023-05-19 03:39:39.000000 galactic-messenger-0.1.1/galactic_messenger/__init__.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      291 2023-05-19 02:56:12.000000 galactic-messenger-0.1.1/galactic_messenger/config.py
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 03:41:51.539412 galactic-messenger-0.1.1/galactic_messenger.egg-info/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4880 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/PKG-INFO
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      320 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)        1 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/requires.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)       19 2023-05-19 03:41:51.000000 galactic-messenger-0.1.1/galactic_messenger.egg-info/top_level.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      442 2023-05-12 09:46:57.000000 galactic-messenger-0.1.1/pyproject.toml
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      495 2023-05-19 03:41:51.542878 galactic-messenger-0.1.1/setup.cfg
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      919 2023-05-19 03:39:24.000000 galactic-messenger-0.1.1/setup.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 04:32:01.759343 galactic-messenger-0.1.2/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     1059 2023-05-19 03:05:50.000000 galactic-messenger-0.1.2/LICENSE
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      232 2023-05-19 04:30:41.000000 galactic-messenger-0.1.2/MANIFEST.in
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4880 2023-05-19 04:32:01.759627 galactic-messenger-0.1.2/PKG-INFO
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4146 2023-05-18 11:48:15.000000 galactic-messenger-0.1.2/README.md
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 04:32:01.740908 galactic-messenger-0.1.2/galactic_messenger/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      113 2023-05-19 03:39:39.000000 galactic-messenger-0.1.2/galactic_messenger/__init__.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      291 2023-05-19 02:56:12.000000 galactic-messenger-0.1.2/galactic_messenger/config.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 04:32:01.750953 galactic-messenger-0.1.2/galactic_messenger/env/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      564 2023-05-18 07:28:08.000000 galactic-messenger-0.1.2/galactic_messenger/env/env.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 04:32:01.753800 galactic-messenger-0.1.2/galactic_messenger/src/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3310 2023-05-18 07:29:34.000000 galactic-messenger-0.1.2/galactic_messenger/src/mail.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     6303 2023-05-18 09:42:17.000000 galactic-messenger-0.1.2/galactic_messenger/src/telegram.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      476 2023-05-15 09:17:23.000000 galactic-messenger-0.1.2/galactic_messenger/src/utils.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     6274 2023-05-18 07:34:12.000000 galactic-messenger-0.1.2/galactic_messenger/src/whatsapp.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 04:32:01.736413 galactic-messenger-0.1.2/galactic_messenger/tests/
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 04:32:01.756593 galactic-messenger-0.1.2/galactic_messenger/tests/end_to_end/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4972 2023-05-18 07:32:48.000000 galactic-messenger-0.1.2/galactic_messenger/tests/end_to_end/test_mail.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     2138 2023-05-18 07:36:47.000000 galactic-messenger-0.1.2/galactic_messenger/tests/end_to_end/test_telegram.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     2135 2023-05-18 07:34:01.000000 galactic-messenger-0.1.2/galactic_messenger/tests/end_to_end/test_whatsapp.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 04:32:01.758855 galactic-messenger-0.1.2/galactic_messenger/tests/unit/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3534 2023-05-19 04:03:29.000000 galactic-messenger-0.1.2/galactic_messenger/tests/unit/test_mail.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      493 2023-05-19 04:04:02.000000 galactic-messenger-0.1.2/galactic_messenger/tests/unit/test_utils.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3002 2023-05-19 04:04:34.000000 galactic-messenger-0.1.2/galactic_messenger/tests/unit/test_whatsapp.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-19 04:32:01.750023 galactic-messenger-0.1.2/galactic_messenger.egg-info/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4880 2023-05-19 04:32:01.000000 galactic-messenger-0.1.2/galactic_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      801 2023-05-19 04:32:01.000000 galactic-messenger-0.1.2/galactic_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)        1 2023-05-19 04:32:01.000000 galactic-messenger-0.1.2/galactic_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-19 04:32:01.000000 galactic-messenger-0.1.2/galactic_messenger.egg-info/requires.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)       19 2023-05-19 04:32:01.000000 galactic-messenger-0.1.2/galactic_messenger.egg-info/top_level.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      442 2023-05-12 09:46:57.000000 galactic-messenger-0.1.2/pyproject.toml
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-19 03:07:47.000000 galactic-messenger-0.1.2/requirements.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      495 2023-05-19 04:32:01.760896 galactic-messenger-0.1.2/setup.cfg
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      919 2023-05-19 04:31:33.000000 galactic-messenger-0.1.2/setup.py
```

### Comparing `galactic-messenger-0.1.1/LICENSE` & `galactic-messenger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.1/PKG-INFO` & `galactic-messenger-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galactic-messenger
-Version: 0.1.1
+Version: 0.1.2
 Summary: Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.
 Home-page: https://github.com/Invigilo-AI/galactic-messenger
 Author: InvigiloAI
 Author-email: contact@invigilo.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `galactic-messenger-0.1.1/README.md` & `galactic-messenger-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.1/galactic_messenger.egg-info/PKG-INFO` & `galactic-messenger-0.1.2/galactic_messenger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galactic-messenger
-Version: 0.1.1
+Version: 0.1.2
 Summary: Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.
 Home-page: https://github.com/Invigilo-AI/galactic-messenger
 Author: InvigiloAI
 Author-email: contact@invigilo.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `galactic-messenger-0.1.1/setup.py` & `galactic-messenger-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="galactic-messenger",
-    version="0.1.1",
+    version="0.1.2",
     author="InvigiloAI",
     author_email="contact@invigilo.ai",
     description="Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Invigilo-AI/galactic-messenger",
     packages=find_packages(),
```

