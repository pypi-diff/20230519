# Comparing `tmp/sybil-5.0.1.tar.gz` & `tmp/sybil-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-5.0.1.tar", last modified: Tue May  9 06:59:47 2023, max compression
+gzip compressed data, was "sybil-5.0.2.tar", last modified: Fri May 19 07:44:54 2023, max compression
```

## Comparing `sybil-5.0.1.tar` & `sybil-5.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-09 06:59:35.000000 sybil-5.0.1/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-05-09 06:59:47.863063 sybil-5.0.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-05-09 06:59:35.000000 sybil-5.0.1/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-09 06:59:47.867063 sybil-5.0.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-05-09 06:59:35.000000 sybil-5.0.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.859063 sybil-5.0.1/sybil/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8523 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/document.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.859063 sybil-5.0.1/sybil/evaluators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1600 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/python.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1775 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/example.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.859063 sybil-5.0.1/sybil/integration/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/integration/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3911 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/integration/pytest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/integration/unittest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/sybil/parsers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/sybil/parsers/abstract/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1915 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2145 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/doctest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/sybil/parsers/myst/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2784 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      989 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5747 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/skip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/sybil/parsers/rest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2862 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1465 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2688 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/python.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3288 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/region.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6439 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/sybil.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/text.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/typing.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.859063 sybil-5.0.1/sybil.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-19 07:44:42.000000 sybil-5.0.2/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-05-19 07:44:54.212619 sybil-5.0.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-05-19 07:44:42.000000 sybil-5.0.2/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-19 07:44:54.216619 sybil-5.0.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1136 2023-05-19 07:44:42.000000 sybil-5.0.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.208618 sybil-5.0.2/sybil/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8309 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/document.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/evaluators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1882 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/python.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1775 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/evaluators/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/example.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/integration/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/integration/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3911 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/integration/pytest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/integration/unittest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/parsers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/parsers/abstract/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1915 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2145 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/abstract/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/doctest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/parsers/myst/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2784 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      989 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5747 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/myst/skip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.212619 sybil-5.0.2/sybil/parsers/rest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2862 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1465 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2690 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/rest/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/parsers/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/python.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3299 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/region.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6442 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/sybil.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-19 07:44:42.000000 sybil-5.0.2/sybil/typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 07:44:54.208618 sybil-5.0.2/sybil.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-19 07:44:54.000000 sybil-5.0.2/sybil.egg-info/top_level.txt
```

### Comparing `sybil-5.0.1/LICENSE.txt` & `sybil-5.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/PKG-INFO` & `sybil-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil
-Version: 5.0.1
+Version: 5.0.2
 Summary: Automated testing for the examples in your code and documentation.
 Home-page: https://github.com/simplistix/sybil
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `sybil-5.0.1/README.rst` & `sybil-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/setup.py` & `sybil-5.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup, find_packages
 
 base_dir = os.path.dirname(__file__)
 
 setup(
     name='sybil',
-    version='5.0.1',
+    version='5.0.2',
     author='Chris Withers',
     author_email='chris@withers.org',
     license='MIT',
     description="Automated testing for the examples in your code and documentation.",
     long_description=open('README.rst').read(),
     url='https://github.com/simplistix/sybil',
     classifiers=[
@@ -27,10 +27,16 @@
         test=[
             'myst_parser',
             'pytest>=7.1.0',
             'pytest-cov',
             'seedir',
             'testfixtures',
             ],
-        build=['furo', 'sphinx', 'twine', 'wheel']
+        build=[
+            'furo',
+            'sphinx',
+            'twine',
+            'urllib3<2',  # workaround for RTD builds failing with old SSL
+            'wheel',
+        ]
     ),
 )
```

### Comparing `sybil-5.0.1/sybil/document.py` & `sybil-5.0.2/sybil/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,17 +191,13 @@
         Read the text from the supplied path to a Python source file and parse any docstrings
         it contains into a document using the supplied parsers.
         """
         with open(path, encoding=encoding) as source:
             document = cls(source.read(), path)
             for start, end, text in cls.extract_docstrings(document.text):
                 docstring_document = cls(text, path)
-                print(repr(docstring_document.text))
-                print(docstring_document.text)
                 for parser in parsers:
                     for region in parser(docstring_document):
                         region.start += start
                         region.end += start
-                        print(region)
-                        print(repr(document.text[region.start:region.end]))
                         document.add(region)
         return document
```

### Comparing `sybil-5.0.1/sybil/evaluators/doctest.py` & `sybil-5.0.2/sybil/evaluators/doctest.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,22 @@
     def __init__(self, optionflags=0):
         self.runner = DocTestRunner(optionflags)
 
     def __call__(self, sybil_example: Example) -> str:
         example = sybil_example.parsed
         namespace = sybil_example.namespace
         output = []
-        self.runner.run(
-            DocTest([example], namespace, name=sybil_example.path,
-                    filename=None, lineno=example.lineno, docstring=None),
-            clear_globs=False,
-            out=output.append
-        )
+        remove_name = False
+        try:
+            if '__name__' not in namespace:
+                remove_name = True
+                namespace['__name__'] = '__test__'
+            self.runner.run(
+                DocTest([example], namespace, name=sybil_example.path,
+                        filename=None, lineno=example.lineno, docstring=None),
+                clear_globs=False,
+                out=output.append
+            )
+        finally:
+            if remove_name:
+                del namespace['__name__']
         return ''.join(output)
```

### Comparing `sybil-5.0.1/sybil/evaluators/python.py` & `sybil-5.0.2/sybil/evaluators/python.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/evaluators/skip.py` & `sybil-5.0.2/sybil/evaluators/skip.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/example.py` & `sybil-5.0.2/sybil/example.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/integration/pytest.py` & `sybil-5.0.2/sybil/integration/pytest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/integration/unittest.py` & `sybil-5.0.2/sybil/integration/unittest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/abstract/clear.py` & `sybil-5.0.2/sybil/parsers/abstract/clear.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/abstract/codeblock.py` & `sybil-5.0.2/sybil/parsers/abstract/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/abstract/doctest.py` & `sybil-5.0.2/sybil/parsers/abstract/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/abstract/lexers.py` & `sybil-5.0.2/sybil/parsers/abstract/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/abstract/skip.py` & `sybil-5.0.2/sybil/parsers/abstract/skip.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/myst/codeblock.py` & `sybil-5.0.2/sybil/parsers/myst/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/myst/doctest.py` & `sybil-5.0.2/sybil/parsers/myst/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/myst/lexers.py` & `sybil-5.0.2/sybil/parsers/myst/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/rest/capture.py` & `sybil-5.0.2/sybil/parsers/rest/capture.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/rest/codeblock.py` & `sybil-5.0.2/sybil/parsers/rest/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/rest/doctest.py` & `sybil-5.0.2/sybil/parsers/rest/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/parsers/rest/lexers.py` & `sybil-5.0.2/sybil/parsers/rest/lexers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     r'^(?P<prefix>[ \t]*)\.\.\s*(?P<directive>{directive})'
     r'({delimiter}\s*'
     r'(?P<arguments>[\w-]+\b)?'
     r'(?:\s*\:[\w-]+\:.*\n)*'
     r'(?:\s*\n)*\n)?'
 )
 
-END_PATTERN_TEMPLATE = '(\n\\Z|\n[ \t]{{0,{len_prefix}}}(?=\\S))'
+END_PATTERN_TEMPLATE = r'(\n\Z|\n[ \t]{{0,{len_prefix}}}(?=\S|\Z))'
 
 
 class DirectiveLexer(BlockLexer):
     """
     A :class:`~sybil.parsers.abstract.lexers.BlockLexer` for ReST directives that extracts the
     following lexemes:
```

### Comparing `sybil-5.0.1/sybil/python.py` & `sybil-5.0.2/sybil/python.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.1/sybil/region.py` & `sybil-5.0.2/sybil/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.end: int = end
         #: The lexemes extracted from the region.
         self.lexemes: Dict[str, Union[str, Lexeme]] = lexemes
 
     def __repr__(self):
         lexemes_for_repr = {}
         for name, lexeme in self.lexemes.items():
-            if len(lexeme) > 10:
+            if lexeme and len(lexeme) > 10:
                 lexeme = lexeme[:10]+'...'
             lexemes_for_repr[name] = lexeme
         return f'<LexedRegion start={self.start} end={self.end} {lexemes_for_repr}>'
 
 
 class Region:
     """
```

### Comparing `sybil-5.0.1/sybil/sybil.py` & `sybil-5.0.2/sybil/sybil.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       
     :param patterns:
       An optional sequence of :func:`patterns <fnmatch.fnmatch>` used to match source
       paths that will be parsed for examples.
 
     :param exclude:
       An optional :func:`pattern <fnmatch.fnmatch>` for source file names
-      that will excluded when looking for examples.
+      that will be excluded when looking for examples.
 
     :param excludes:
       An optional  sequence of :func:`patterns <fnmatch.fnmatch>` for source paths
       that will be excluded when looking for examples.
 
     :param filenames:
       An optional collection of file names that, if found anywhere within the
```

### Comparing `sybil-5.0.1/sybil.egg-info/PKG-INFO` & `sybil-5.0.2/sybil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil
-Version: 5.0.1
+Version: 5.0.2
 Summary: Automated testing for the examples in your code and documentation.
 Home-page: https://github.com/simplistix/sybil
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `sybil-5.0.1/sybil.egg-info/SOURCES.txt` & `sybil-5.0.2/sybil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

