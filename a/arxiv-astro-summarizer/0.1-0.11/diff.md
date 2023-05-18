# Comparing `tmp/arxiv-astro-summarizer-0.1.tar.gz` & `tmp/arxiv-astro-summarizer-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-astro-summarizer-0.1.tar", last modified: Thu May 18 20:05:35 2023, max compression
+gzip compressed data, was "arxiv-astro-summarizer-0.11.tar", last modified: Thu May 18 21:07:30 2023, max compression
```

## Comparing `arxiv-astro-summarizer-0.1.tar` & `arxiv-astro-summarizer-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 20:05:35.345068 arxiv-astro-summarizer-0.1/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2021-09-01 21:31:50.000000 arxiv-astro-summarizer-0.1/LICENSE.txt
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-05-18 19:47:43.000000 arxiv-astro-summarizer-0.1/MANIFEST.in
--rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-18 20:05:35.344781 arxiv-astro-summarizer-0.1/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)      793 2023-05-18 19:47:32.000000 arxiv-astro-summarizer-0.1/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 20:05:35.341718 arxiv-astro-summarizer-0.1/arxiv-astro-summarizer/
--rwxr-xr-x   0 daniel     (501) staff       (20)       26 2021-09-01 21:31:50.000000 arxiv-astro-summarizer-0.1/arxiv-astro-summarizer/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    19473 2023-05-18 19:50:18.000000 arxiv-astro-summarizer-0.1/arxiv-astro-summarizer/astroph_summarizer.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 20:05:35.344283 arxiv-astro-summarizer-0.1/arxiv_astro_summarizer.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-18 20:05:35.000000 arxiv-astro-summarizer-0.1/arxiv_astro_summarizer.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      366 2023-05-18 20:05:35.000000 arxiv-astro-summarizer-0.1/arxiv_astro_summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-18 20:05:35.000000 arxiv-astro-summarizer-0.1/arxiv_astro_summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       93 2023-05-18 20:05:35.000000 arxiv-astro-summarizer-0.1/arxiv_astro_summarizer.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-18 20:05:35.000000 arxiv-astro-summarizer-0.1/arxiv_astro_summarizer.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)      283 2023-05-18 20:04:00.000000 arxiv-astro-summarizer-0.1/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-18 20:05:35.345154 arxiv-astro-summarizer-0.1/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)     1064 2023-05-18 19:43:14.000000 arxiv-astro-summarizer-0.1/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 21:07:30.356900 arxiv-astro-summarizer-0.11/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2021-09-01 21:31:50.000000 arxiv-astro-summarizer-0.11/LICENSE.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-05-18 19:47:43.000000 arxiv-astro-summarizer-0.11/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)      664 2023-05-18 21:07:30.356622 arxiv-astro-summarizer-0.11/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)      850 2023-05-18 21:05:03.000000 arxiv-astro-summarizer-0.11/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 21:07:30.354064 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer/
+-rwxr-xr-x   0 daniel     (501) staff       (20)       26 2021-09-01 21:31:50.000000 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    19473 2023-05-18 19:50:18.000000 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer/astroph_summarizer.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-18 21:07:30.356204 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      664 2023-05-18 21:07:30.000000 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      366 2023-05-18 21:07:30.000000 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-18 21:07:30.000000 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       93 2023-05-18 21:07:30.000000 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-18 21:07:30.000000 arxiv-astro-summarizer-0.11/arxiv_astro_summarizer.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      283 2023-05-18 20:04:00.000000 arxiv-astro-summarizer-0.11/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-18 21:07:30.357025 arxiv-astro-summarizer-0.11/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1065 2023-05-18 21:06:10.000000 arxiv-astro-summarizer-0.11/setup.py
```

### Comparing `arxiv-astro-summarizer-0.1/LICENSE.txt` & `arxiv-astro-summarizer-0.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-0.1/PKG-INFO` & `arxiv-astro-summarizer-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-astro-summarizer
-Version: 0.1
+Version: 0.11
 Summary: Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.
 Home-page: https://github.com/Professor-G/arxiv-astro-summarizer
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `arxiv-astro-summarizer-0.1/README.md` & `arxiv-astro-summarizer-0.11/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 
 ```
     $ pip install arxiv-astro-summarizer
 ```
 
 # Documentation
 
-For technical details and an example of how to implement arxiv-astro-summarizer, check out the Documentation.
+For technical details and an example of how to implement arxiv-astro-summarizer, check out the Documentation: https://arxiv-astro-summarizer.readthedocs.io/en/latest/
 
 
 # How to Contribute?
 
 Want to contribute? Bug detections? Comments? Suggestions? Please email: danielgodinez123@gmail.com
```

### Comparing `arxiv-astro-summarizer-0.1/arxiv-astro-summarizer/astroph_summarizer.py` & `arxiv-astro-summarizer-0.11/arxiv_astro_summarizer/astroph_summarizer.py`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-0.1/arxiv_astro_summarizer.egg-info/PKG-INFO` & `arxiv-astro-summarizer-0.11/arxiv_astro_summarizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-astro-summarizer
-Version: 0.1
+Version: 0.11
 Summary: Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.
 Home-page: https://github.com/Professor-G/arxiv-astro-summarizer
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `arxiv-astro-summarizer-0.1/setup.py` & `arxiv-astro-summarizer-0.11/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 
 setup(
     name="arxiv-astro-summarizer",
-    version="0.1",
+    version="0.11",
     author="Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/arxiv-astro-summarizer",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
```

