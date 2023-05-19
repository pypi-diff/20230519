# Comparing `tmp/strip-tags-0.2.tar.gz` & `tmp/strip-tags-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strip-tags-0.2.tar", last modified: Thu May 18 16:26:58 2023, max compression
+gzip compressed data, was "strip-tags-0.3.tar", last modified: Fri May 19 05:20:18 2023, max compression
```

## Comparing `strip-tags-0.2.tar` & `strip-tags-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:26:58.024879 strip-tags-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 16:26:39.000000 strip-tags-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-18 16:26:58.024879 strip-tags-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-18 16:26:39.000000 strip-tags-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:26:58.024879 strip-tags-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-18 16:26:39.000000 strip-tags-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:26:58.020879 strip-tags-0.2/strip_tags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:26:39.000000 strip-tags-0.2/strip_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 16:26:39.000000 strip-tags-0.2/strip_tags/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-18 16:26:39.000000 strip-tags-0.2/strip_tags/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:26:58.024879 strip-tags-0.2/strip_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-18 16:26:58.000000 strip-tags-0.2/strip_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 16:26:58.000000 strip-tags-0.2/strip_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:26:58.000000 strip-tags-0.2/strip_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 16:26:58.000000 strip-tags-0.2/strip_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-18 16:26:58.000000 strip-tags-0.2/strip_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 16:26:58.000000 strip-tags-0.2/strip_tags.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:26:58.024879 strip-tags-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-18 16:26:39.000000 strip-tags-0.2/tests/test_strip_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:20:18.746920 strip-tags-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 05:19:55.000000 strip-tags-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-19 05:20:18.746920 strip-tags-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-19 05:19:55.000000 strip-tags-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 05:20:18.746920 strip-tags-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-19 05:19:55.000000 strip-tags-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:20:18.742920 strip-tags-0.3/strip_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 05:19:55.000000 strip-tags-0.3/strip_tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 05:19:55.000000 strip-tags-0.3/strip_tags/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-19 05:19:55.000000 strip-tags-0.3/strip_tags/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:20:18.746920 strip-tags-0.3/strip_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:20:18.746920 strip-tags-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-19 05:19:55.000000 strip-tags-0.3/tests/test_strip_tags.py
```

### Comparing `strip-tags-0.2/LICENSE` & `strip-tags-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strip-tags-0.2/PKG-INFO` & `strip-tags-0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,59 @@
-Metadata-Version: 2.1
-Name: strip-tags
-Version: 0.2
-Summary: Strip tags from HTML, optionally from areas identified by CSS selectors
-Home-page: https://github.com/simonw/strip-tags
-Author: Simon Willison
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.com/simonw/strip-tags/issues
-Project-URL: CI, https://github.com/simonw/strip-tags/actions
-Project-URL: Changelog, https://github.com/simonw/strip-tags/releases
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # strip-tags
 
 [![PyPI](https://img.shields.io/pypi/v/strip-tags.svg)](https://pypi.org/project/strip-tags/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/strip-tags?include_prereleases&label=changelog)](https://github.com/simonw/strip-tags/releases)
 [![Tests](https://github.com/simonw/strip-tags/workflows/Test/badge.svg)](https://github.com/simonw/strip-tags/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/strip-tags/blob/master/LICENSE)
 
 Strip tags from HTML, optionally from areas identified by CSS selectors
 
+See [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/) for more on this project.
+
 ## Installation
 
 Install this tool using `pip`:
-
-    pip install strip-tags
-
+```bash
+pip install strip-tags
+```
 ## Usage
 
 Pipe content into this tool to strip tags from it:
-
-    cat input.html | strip-tags > output.txt
-
+```bash
+cat input.html | strip-tags > output.txt
+````
 Or pass a filename:
-
-    strip-tags -i input.html > output.txt
-
+```bash
+strip-tags -i input.html > output.txt
+```
 To run against just specific areas identified by CSS selectors:
-
-    strip-tags '.content' -i input.html > output.txt
-
+```bash
+strip-tags '.content' -i input.html > output.txt
+```
 This can be called with multiple selectors:
-
-    cat input.html | strip-tags '.content' '.sidebar' > output.txt
-
-You can also use:
-
-    python -m strip_tags --help
-
+```bash
+cat input.html | strip-tags '.content' '.sidebar' > output.txt
+```
+To minify whitespace - reducing multiple space and tab characters to a single space, and multiple newlines and spaces to a maximum of two newlines - add `-m` or `--minify`:
+```bash
+cat input.html | strip-tags -m > output.txt
+```
+You can also run this command using `python -m` like this:
+```bash
+python -m strip_tags --help
+```
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
-
-    cd strip-tags
-    python -m venv venv
-    source venv/bin/activate
-
+```bash
+cd strip-tags
+python -m venv venv
+source venv/bin/activate
+```
 Now install the dependencies and test dependencies:
-
-    pip install -e '.[test]'
-
+```bash
+pip install -e '.[test]'
+```
 To run the tests:
-
-    pytest
+```bash
+pytest
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `strip-tags-0.2/setup.py` & `strip-tags-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2"
+VERSION = "0.3"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

