# Comparing `tmp/mdforest-1.3.2.tar.gz` & `tmp/mdforest-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-1.3.2.tar", last modified: Thu May 18 22:05:30 2023, max compression
+gzip compressed data, was "mdforest-1.3.3.tar", last modified: Thu May 18 22:29:58 2023, max compression
```

## Comparing `mdforest-1.3.2.tar` & `mdforest-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 mdforest-1.3.2/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-18 22:05:30.952523 mdforest-1.3.2/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2592 2023-05-18 19:10:43.000000 mdforest-1.3.2/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/mdforest/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      457 2023-05-18 21:56:16.000000 mdforest-1.3.2/mdforest/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3877 2023-05-18 21:58:45.000000 mdforest-1.3.2/mdforest/mdforest.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/mdforest/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 14:40:51.000000 mdforest-1.3.2/mdforest/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-18 19:08:48.000000 mdforest-1.3.2/mdforest/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-18 19:23:23.000000 mdforest-1.3.2/mdforest/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 12:19:37.000000 mdforest-1.3.2/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-18 22:05:30.952523 mdforest-1.3.2/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      926 2023-05-18 22:02:43.000000 mdforest-1.3.2/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-18 14:40:51.000000 mdforest-1.3.2/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:29:58.214568 mdforest-1.3.3/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 mdforest-1.3.3/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-18 22:29:58.214568 mdforest-1.3.3/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2592 2023-05-18 19:10:43.000000 mdforest-1.3.3/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:29:58.214568 mdforest-1.3.3/mdforest/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      457 2023-05-18 22:28:45.000000 mdforest-1.3.3/mdforest/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3165 2023-05-18 22:27:59.000000 mdforest-1.3.3/mdforest/mdforest.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:29:58.214568 mdforest-1.3.3/mdforest/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 14:40:51.000000 mdforest-1.3.3/mdforest/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-18 19:08:48.000000 mdforest-1.3.3/mdforest/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-18 19:23:23.000000 mdforest-1.3.3/mdforest/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:29:58.214568 mdforest-1.3.3/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-18 22:29:58.000000 mdforest-1.3.3/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-18 22:29:58.000000 mdforest-1.3.3/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-18 22:29:58.000000 mdforest-1.3.3/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-18 22:29:58.000000 mdforest-1.3.3/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-18 22:29:58.000000 mdforest-1.3.3/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 12:19:37.000000 mdforest-1.3.3/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-18 22:29:58.214568 mdforest-1.3.3/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      943 2023-05-18 22:29:08.000000 mdforest-1.3.3/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:29:58.214568 mdforest-1.3.3/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-18 14:40:51.000000 mdforest-1.3.3/tests/test_mdtree.py
```

### Comparing `mdforest-1.3.2/LICENSE` & `mdforest-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-1.3.2/PKG-INFO` & `mdforest-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.3.2
+Version: 1.3.3
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.3.2.zip
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.3.3.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 mdforest - Markdown Forest
 ==========================
```

### Comparing `mdforest-1.3.2/README.rst` & `mdforest-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `mdforest-1.3.2/mdforest/tree/types.py` & `mdforest-1.3.3/mdforest/tree/types.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.3.2/mdforest/treebuild.py` & `mdforest-1.3.3/mdforest/treebuild.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.3.2/mdforest.egg-info/PKG-INFO` & `mdforest-1.3.3/mdforest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.3.2
+Version: 1.3.3
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.3.2.zip
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.3.3.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 mdforest - Markdown Forest
 ==========================
```

### Comparing `mdforest-1.3.2/setup.py` & `mdforest-1.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.3.2'
+VERSION = '1.3.3'
 DESCRIPTION = 'A package to convert between Markdown and a forest data structure for efficient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     readme="README.rst",
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/mdforest",
-    packages = ['mdforest'],
+    packages = ['mdforest', 'mdforest.tree'],
     tests_require = ['unittest'],
     install_requires = ['markdown', 'beautifulsoup4', 'python-frontmatter'],
     download_url = 'https://github.com/kj3moraes/mdforest/archive/%s.zip' % VERSION,
     classifiers = [
         "Topic :: Utilities",
     ],
 )
```

### Comparing `mdforest-1.3.2/tests/test_mdtree.py` & `mdforest-1.3.3/tests/test_mdtree.py`

 * *Files identical despite different names*

