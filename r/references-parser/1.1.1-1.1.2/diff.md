# Comparing `tmp/references_parser-1.1.1.tar.gz` & `tmp/references_parser-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "references_parser-1.1.1.tar", last modified: Thu May 18 07:17:37 2023, max compression
+gzip compressed data, was "references_parser-1.1.2.tar", last modified: Fri May 19 04:17:01 2023, max compression
```

## Comparing `references_parser-1.1.1.tar` & `references_parser-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:17:37.104461 references_parser-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-18 07:17:37.104461 references_parser-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-18 07:17:26.000000 references_parser-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 07:17:26.000000 references_parser-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:17:37.100460 references_parser-1.1.1/references_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:17:26.000000 references_parser-1.1.1/references_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 07:17:26.000000 references_parser-1.1.1/references_parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-18 07:17:26.000000 references_parser-1.1.1/references_parser/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:17:37.104461 references_parser-1.1.1/references_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-18 07:17:26.000000 references_parser-1.1.1/references_parser/parsers/IeeeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-18 07:17:26.000000 references_parser-1.1.1/references_parser/parsers/SsauParser.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 07:17:26.000000 references_parser-1.1.1/references_parser/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:17:37.100460 references_parser-1.1.1/references_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-18 07:17:37.000000 references_parser-1.1.1/references_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 07:17:37.000000 references_parser-1.1.1/references_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:17:37.000000 references_parser-1.1.1/references_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 07:17:37.000000 references_parser-1.1.1/references_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 07:17:37.000000 references_parser-1.1.1/references_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 07:17:37.000000 references_parser-1.1.1/references_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 07:17:37.104461 references_parser-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 07:17:26.000000 references_parser-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.795235 references_parser-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-19 04:17:01.795235 references_parser-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-19 04:16:39.000000 references_parser-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 04:16:39.000000 references_parser-1.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.791235 references_parser-1.1.2/references_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.795235 references_parser-1.1.2/references_parser/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/converters/url_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.795235 references_parser-1.1.2/references_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/parsers/IeeeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/parsers/SsauParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 04:16:39.000000 references_parser-1.1.2/references_parser/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 04:17:01.795235 references_parser-1.1.2/references_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 04:17:01.000000 references_parser-1.1.2/references_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 04:17:01.795235 references_parser-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-19 04:16:39.000000 references_parser-1.1.2/setup.py
```

### Comparing `references_parser-1.1.1/PKG-INFO` & `references_parser-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: references_parser
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tool for parsing bibtex in ssau's format
 Home-page: https://github.com/Banayaki/ReferencesParser
 Author: Mukhin Artem
 Author-email: artemmukhinssau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `references_parser-1.1.1/README.md` & `references_parser-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `references_parser-1.1.1/references_parser/cli.py` & `references_parser-1.1.2/references_parser/cli.py`

 * *Files identical despite different names*

### Comparing `references_parser-1.1.1/references_parser/parsers/IeeeParser.py` & `references_parser-1.1.2/references_parser/parsers/IeeeParser.py`

 * *Files identical despite different names*

### Comparing `references_parser-1.1.1/references_parser/parsers/SsauParser.py` & `references_parser-1.1.2/references_parser/parsers/SsauParser.py`

 * *Files identical despite different names*

### Comparing `references_parser-1.1.1/references_parser.egg-info/PKG-INFO` & `references_parser-1.1.2/references_parser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: references-parser
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tool for parsing bibtex in ssau's format
 Home-page: https://github.com/Banayaki/ReferencesParser
 Author: Mukhin Artem
 Author-email: artemmukhinssau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `references_parser-1.1.1/setup.py` & `references_parser-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='references_parser',
     packages=setuptools.find_packages(),
-    version='1.1.1',
+    version='1.1.2',
     description="Tool for parsing bibtex in ssau's format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mukhin Artem',
     author_email='artemmukhinssau@gmail.com',
     url='https://github.com/Banayaki/ReferencesParser',
     include_package_data=True,
```

