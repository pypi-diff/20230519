# Comparing `tmp/textagon-0.1.3.tar.gz` & `tmp/textagon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textagon-0.1.3.tar", last modified: Fri May 19 20:02:36 2023, max compression
+gzip compressed data, was "textagon-0.1.4.tar", last modified: Fri May 19 20:09:52 2023, max compression
```

## Comparing `textagon-0.1.3.tar` & `textagon-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 20:02:36.721469 textagon-0.1.3/
--rw-rw-rw-   0        0        0      181 2023-05-19 20:02:36.719481 textagon-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-19 20:02:36.721469 textagon-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      528 2023-05-19 20:02:27.000000 textagon-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 20:02:36.712460 textagon-0.1.3/textagon/
--rw-rw-rw-   0        0        0      105 2023-05-19 19:46:12.000000 textagon-0.1.3/textagon/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.3/textagon/install-dependencies.py
--rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.3/textagon/process-text.py
--rw-rw-rw-   0        0        0     5377 2023-05-19 19:50:47.000000 textagon-0.1.3/textagon/textagon.py
-drwxrwxrwx   0        0        0        0 2023-05-19 20:02:36.719481 textagon-0.1.3/textagon.egg-info/
--rw-rw-rw-   0        0        0      181 2023-05-19 20:02:36.000000 textagon-0.1.3/textagon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-19 20:02:36.000000 textagon-0.1.3/textagon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 20:02:36.000000 textagon-0.1.3/textagon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-19 20:02:36.000000 textagon-0.1.3/textagon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 20:02:36.000000 textagon-0.1.3/textagon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 20:09:52.800000 textagon-0.1.4/
+-rw-rw-rw-   0        0        0      181 2023-05-19 20:09:52.800000 textagon-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-19 20:09:52.800000 textagon-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      528 2023-05-19 20:09:43.000000 textagon-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:09:52.789987 textagon-0.1.4/textagon/
+-rw-rw-rw-   0        0        0      105 2023-05-19 19:46:12.000000 textagon-0.1.4/textagon/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.4/textagon/install-dependencies.py
+-rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.4/textagon/process-text.py
+-rw-rw-rw-   0        0        0     5377 2023-05-19 20:09:35.000000 textagon-0.1.4/textagon/textagon.py
+drwxrwxrwx   0        0        0        0 2023-05-19 20:09:52.799000 textagon-0.1.4/textagon.egg-info/
+-rw-rw-rw-   0        0        0      181 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/top_level.txt
```

### Comparing `textagon-0.1.3/setup.py` & `textagon-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'textagon',
-    version = '0.1.3',
+    version = '0.1.4',
     packages = find_packages(),
     description = 'Start building textagon',
     author = 'Mendoza',
     classifiers=[
         "License :: OSI Approved :: Python Software Foundation License"
     ],
     install_requires=[
```

### Comparing `textagon-0.1.3/textagon/process-text.py` & `textagon-0.1.4/textagon/process-text.py`

 * *Files identical despite different names*

### Comparing `textagon-0.1.3/textagon/textagon.py` & `textagon-0.1.4/textagon/textagon.py`

 * *Files identical despite different names*

