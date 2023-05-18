# Comparing `tmp/mdforest-1.3.1.tar.gz` & `tmp/mdforest-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-1.3.1.tar", last modified: Thu May 18 19:16:34 2023, max compression
+gzip compressed data, was "mdforest-1.3.2.tar", last modified: Thu May 18 22:05:30 2023, max compression
```

## Comparing `mdforest-1.3.1.tar` & `mdforest-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 19:16:34.304007 mdforest-1.3.1/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 mdforest-1.3.1/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3006 2023-05-18 19:16:34.304007 mdforest-1.3.1/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2457 2023-05-15 12:14:38.000000 mdforest-1.3.1/README.md
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 19:16:34.304007 mdforest-1.3.1/mdforest/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      425 2023-05-18 14:40:51.000000 mdforest-1.3.1/mdforest/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3789 2023-05-18 19:08:48.000000 mdforest-1.3.1/mdforest/mdforest.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 19:16:34.304007 mdforest-1.3.1/mdforest/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 14:40:51.000000 mdforest-1.3.1/mdforest/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-18 19:08:48.000000 mdforest-1.3.1/mdforest/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     5710 2023-05-18 19:14:07.000000 mdforest-1.3.1/mdforest/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 19:16:34.304007 mdforest-1.3.1/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3006 2023-05-18 19:16:34.000000 mdforest-1.3.1/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      313 2023-05-18 19:16:34.000000 mdforest-1.3.1/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-18 19:16:34.000000 mdforest-1.3.1/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-18 19:16:34.000000 mdforest-1.3.1/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-18 19:16:34.000000 mdforest-1.3.1/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 12:19:37.000000 mdforest-1.3.1/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-18 19:16:34.304007 mdforest-1.3.1/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      983 2023-05-18 19:16:32.000000 mdforest-1.3.1/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 mdforest-1.3.2/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-18 22:05:30.952523 mdforest-1.3.2/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2592 2023-05-18 19:10:43.000000 mdforest-1.3.2/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/mdforest/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      457 2023-05-18 21:56:16.000000 mdforest-1.3.2/mdforest/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3877 2023-05-18 21:58:45.000000 mdforest-1.3.2/mdforest/mdforest.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/mdforest/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 14:40:51.000000 mdforest-1.3.2/mdforest/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-18 19:08:48.000000 mdforest-1.3.2/mdforest/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-18 19:23:23.000000 mdforest-1.3.2/mdforest/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-18 22:05:30.000000 mdforest-1.3.2/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 12:19:37.000000 mdforest-1.3.2/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-18 22:05:30.952523 mdforest-1.3.2/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      926 2023-05-18 22:02:43.000000 mdforest-1.3.2/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 22:05:30.952523 mdforest-1.3.2/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-18 14:40:51.000000 mdforest-1.3.2/tests/test_mdtree.py
```

### Comparing `mdforest-1.3.1/LICENSE` & `mdforest-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-1.3.1/PKG-INFO` & `mdforest-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
-Home-page: http://github.com/kj3moraes/markdown-tree
-Download-URL: https://github.com/kj3moraes/markdown-tree/archive/1.3.1.zip
+Home-page: http://github.com/kj3moraes/mdforest
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.3.2.zip
+Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 mdforest - Markdown Forest
 ==========================
 
 A library to convert Markdown documents into tree data structures and
@@ -108,7 +109,9 @@
 
 License
 -------
 
 The `original project <https://github.com/alvinwan/md2py>`__ was
 licensed under the Apache 2.0 License and a copy is provided in this
 repo as well. All the files changed are listed in the CHANGELOG.
+
+
```

### Comparing `mdforest-1.3.1/README.md` & `mdforest-1.3.2/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,102 @@
-![icon](media/forest-icon-display.png)
+mdforest - Markdown Forest
+==========================
 
-# mdforest - Markdown Forest
+A library to convert Markdown documents into tree data structures and
+vice versa. There is greater functionality available to modify, prune,
+add and delete parts of documents when there are in the MarkdownTree
+structure.
+
+markdown-tree is a fork of `md2py <https://github.com/alvinwan/md2py>`__
+which is no longer maintained. This library adds far more functionality
+and broadens the scope of the older libary. The full list of features
+can be found under `Features <##%20Features>`__
 
-A library to convert Markdown documents into tree data structures and vice versa. There is greater functionality available to modify, prune, add and delete parts of documents when there are in the MarkdownTree structure.
-
-markdown-tree is a fork of [md2py](https://github.com/alvinwan/md2py) which is no longer maintained. This library adds far more functionality and broadens the scope of the older libary. The full list of features can be found under [Features](## Features)
-
-## Install
+Install
+-------
 
 Install via pip
 
-```bash
-pip install markdown-tree
-```
+.. code:: bash
 
-You can find the library page here [here](nil)
+   pip install markdown-tree
 
-## Quick Usage Guide
+You can find the library page here `here <nil>`__
 
-Markdown2Python offers only one function `md2py`, which generates a Python
-object from markdown text. This object is a navigable, "Tree of Contents"
-abstraction for the markdown file.
+Quick Usage Guide
+-----------------
+
+Markdown2Python offers only one function ``md2py``, which generates a
+Python object from markdown text. This object is a navigable, “Tree of
+Contents” abstraction for the markdown file.
 
 Take, for example, the following markdown file.
 
 [[ chikin.md ]]
 
-```markdown
-# Chikin Tales
-
-Once there was a chikin.
+.. code:: markdown
 
-## Chapter 1 : Chikin Fly
+   # Chikin Tales
 
-Chickens don't fly. They do only the following:
+   Once there was a chikin.
 
-- waddle
-- plop 
+   ## Chapter 1 : Chikin Fly
 
+   Chickens don't fly. They do only the following:
 
-### Waddling
+   - waddle
+   - plop 
 
-A waddle is what these birds do.
 
-## Chapter 2 : Chikin Scream
+   ### Waddling
 
-### Plopping
+   A waddle is what these birds do.
 
-Plopping involves three steps:
+   ## Chapter 2 : Chikin Scream
 
-1. squawk
-2. plop
-3. repeat, unless ordered to squat
+   ### Plopping
 
-```
+   Plopping involves three steps:
 
-Akin to a navigation bar, the `TreeOfContents` object allows you to expand a
-markdown file one level at a time. Running `md2py` on the above markdown file
-will generate a tree, abstracting the below structure.
+   1. squawk
+   2. plop
+   3. repeat, unless ordered to squat
 
-```text
-               Chikin Tales
-              /     \       \
-             /       \       \ 
-       (Once th..)    |       \
-                      |        \
-                  Chapter 1     \
-                  /     |     Chapter 2   
-                 /      |         |
-       (Chickens do..)  |       Plopping
-                        |         |
-                     Waddling   (Plopping...)
-                        |
-                    (A waddle...)
+Akin to a navigation bar, the ``TreeOfContents`` object allows you to
+expand a markdown file one level at a time. Running ``md2py`` on the
+above markdown file will generate a tree, abstracting the below
+structure.
 
+.. code:: text
 
-```
+                  Chikin Tales
+                 /     \       \
+                /       \       \ 
+          (Once th..)    |       \
+                         |        \
+                     Chapter 1     \
+                     /     |     Chapter 2   
+                    /      |         |
+          (Chickens do..)  |       Plopping
+                           |         |
+                        Waddling   (Plopping...)
+                           |
+                       (A waddle...)
 
 For the full usage guide, access the SAMPLES.md file.
 
-## Features
+Features
+--------
 
 Some of the features of this library are:
 
-1. Converts a markdown file to a manipulatable, light Python data structure.
+1. Converts a markdown file to a manipulatable, light Python data
+   structure.
 2. Converts the Python data structure back into a Markdown file.
 3. Traverse and edit the Python data structure.
 
-## License 
+License
+-------
 
-The [original project](https://github.com/alvinwan/md2py) was licensed under the Apache 2.0 License and a copy is provided in this repo as well. All the files changed are listed in the CHANGELOG.
+The `original project <https://github.com/alvinwan/md2py>`__ was
+licensed under the Apache 2.0 License and a copy is provided in this
+repo as well. All the files changed are listed in the CHANGELOG.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mdforest-1.3.1/mdforest/mdforest.py` & `mdforest-1.3.2/mdforest/mdforest.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,33 +99,40 @@
 # Some text here and there
 # ### Header 3
 # Some more text here and there
 # ## Header 2.2
 # Thats' all folks!
 # """
 
-# test2 = """
-# ---
-# tags: [test, test2, test3]
-# author: Keane Moraes
-# time: 2
-# ---
-# # Header 1
-# ## Header 2.1
-# Some [[text]] here and there #asd
-# ### Header 3
-# Some more text here and there
-# ## Header 2.2
-# Thats' all folks!
-# """
+test2 = """
+---
+author: Keane Moraes
+id: 1
+tags:
+- tag1
+- tag2
+---
 
-# print(find_tags(test2))
+# Appendices 
 
-# a = mdtreeify("test2", test2)
-# print(a)
+## Appendix I: The Ecology of Dune.
+
+## Appendix II: The Religion of Dune.
+
+## Appendix III: Report on Bene Gesserit Motives and Purposes.
+
+## Appendix IV: The Almanak eb-Ashraf (Selected Excerpts of the Noble Houses)
+
+# Terminology of the Imperium
+"""
+
+print(find_tags(test2))
+
+a = mdtreeify("test2", test2)
+print(a)
 # print(mdtextify(a))
 # print(a)
 # ret_test2 = mdtextify(a)
 
 # print(ret_test2)
 
 # print(a)
```

### Comparing `mdforest-1.3.1/mdforest/tree/types.py` & `mdforest-1.3.2/mdforest/tree/types.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.3.1/mdforest/treebuild.py` & `mdforest-1.3.2/mdforest/treebuild.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,28 @@
                 parsed.append({'root':branch.string, 'source':branch})
             else:
                 parsed[-1].setdefault('descendants', []).append(branch)
         if self.depth == None:
             return [TOC(depth=1, **kwargs) for kwargs in parsed]
         return [TOC(depth=self.depth+1, **kwargs) for kwargs in parsed]
 
+    def __getattr__(self, attr, *default):
+        """Check source for attributes"""
+        tag = attr[:-1]
+        if attr in self.allowed_attrs:
+            return getattr(self.source, attr, *default)
+        if attr in self.valid_tags:
+            return next(filter(lambda t: t.name == attr, self.branches), None)
+        if len(default):
+            return default[0]
+        if attr[-1] == 's' and tag in self.valid_tags:
+            condition = lambda t: t.name == tag
+            return filter(condition, self.branches)
+        raise AttributeError("'TreeOfContents' object has no attribute '%s'" % attr)
+
     def __repr__(self):
         """Display contents"""
         return str(self)
 
     def __str__(self):
         """Display contents"""
         return self.string or ''
```

### Comparing `mdforest-1.3.1/mdforest.egg-info/PKG-INFO` & `mdforest-1.3.2/mdforest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
-Home-page: http://github.com/kj3moraes/markdown-tree
-Download-URL: https://github.com/kj3moraes/markdown-tree/archive/1.3.1.zip
+Home-page: http://github.com/kj3moraes/mdforest
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.3.2.zip
+Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 mdforest - Markdown Forest
 ==========================
 
 A library to convert Markdown documents into tree data structures and
@@ -108,7 +109,9 @@
 
 License
 -------
 
 The `original project <https://github.com/alvinwan/md2py>`__ was
 licensed under the Apache 2.0 License and a copy is provided in this
 repo as well. All the files changed are listed in the CHANGELOG.
+
+
```

### Comparing `mdforest-1.3.1/setup.py` & `mdforest-1.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-import sys
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
-LONG_DESCRIPTION = (this_directory / "media" / "README.rst").read_text()
+LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.3.1'
+VERSION = '1.3.2'
 DESCRIPTION = 'A package to convert between Markdown and a forest data structure for efficient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    readme="README.md",
+    readme="README.rst",
     license = "Apache 2.0",
-    url = "http://github.com/kj3moraes/markdown-tree",
-    packages = ['mdforest', 'mdforest.tree'],
-    tests_require = ['unittest', 'pytest'],
+    url = "http://github.com/kj3moraes/mdforest",
+    packages = ['mdforest'],
+    tests_require = ['unittest'],
     install_requires = ['markdown', 'beautifulsoup4', 'python-frontmatter'],
-    download_url = 'https://github.com/kj3moraes/markdown-tree/archive/%s.zip' % VERSION,
+    download_url = 'https://github.com/kj3moraes/mdforest/archive/%s.zip' % VERSION,
     classifiers = [
         "Topic :: Utilities",
     ],
 )
```

