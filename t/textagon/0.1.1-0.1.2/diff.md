# Comparing `tmp/textagon-0.1.1.tar.gz` & `tmp/textagon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textagon-0.1.1.tar", last modified: Fri May 19 17:14:33 2023, max compression
+gzip compressed data, was "textagon-0.1.2.tar", last modified: Fri May 19 19:54:08 2023, max compression
```

## Comparing `textagon-0.1.1.tar` & `textagon-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 17:14:33.039585 textagon-0.1.1/
--rw-rw-rw-   0        0        0      181 2023-05-19 17:14:33.038575 textagon-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-19 17:14:33.039585 textagon-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-05-19 17:14:28.000000 textagon-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 17:14:33.025820 textagon-0.1.1/textagon/
--rw-rw-rw-   0        0        0       70 2023-05-19 17:12:16.000000 textagon-0.1.1/textagon/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.1/textagon/install-dependencies.py
--rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.1/textagon/process-text.py
--rw-rw-rw-   0        0        0     3428 2023-05-19 17:12:02.000000 textagon-0.1.1/textagon/textagon.py
-drwxrwxrwx   0        0        0        0 2023-05-19 17:14:33.038575 textagon-0.1.1/textagon.egg-info/
--rw-rw-rw-   0        0        0      181 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 17:14:32.000000 textagon-0.1.1/textagon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 19:54:08.089343 textagon-0.1.2/
+-rw-rw-rw-   0        0        0      181 2023-05-19 19:54:08.088326 textagon-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:54:08.089343 textagon-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-05-19 19:54:02.000000 textagon-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:54:08.084329 textagon-0.1.2/textagon/
+-rw-rw-rw-   0        0        0      105 2023-05-19 19:46:12.000000 textagon-0.1.2/textagon/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.2/textagon/install-dependencies.py
+-rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.2/textagon/process-text.py
+-rw-rw-rw-   0        0        0     5377 2023-05-19 19:50:47.000000 textagon-0.1.2/textagon/textagon.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:54:08.087327 textagon-0.1.2/textagon.egg-info/
+-rw-rw-rw-   0        0        0      181 2023-05-19 19:54:07.000000 textagon-0.1.2/textagon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-19 19:54:08.000000 textagon-0.1.2/textagon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:54:07.000000 textagon-0.1.2/textagon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-05-19 19:54:07.000000 textagon-0.1.2/textagon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 19:54:07.000000 textagon-0.1.2/textagon.egg-info/top_level.txt
```

### Comparing `textagon-0.1.1/setup.py` & `textagon-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'textagon',
-    version = '0.1.1',
+    version = '0.1.2',
     packages = find_packages(),
     description = 'Start building textagon',
     author = 'Mendoza',
     classifiers=[
         "License :: OSI Approved :: Python Software Foundation License"
     ],
     install_requires=[
```

### Comparing `textagon-0.1.1/textagon/process-text.py` & `textagon-0.1.2/textagon/process-text.py`

 * *Files identical despite different names*

