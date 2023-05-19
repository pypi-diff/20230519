# Comparing `tmp/lkmlfmt-0.0.5.tar.gz` & `tmp/lkmlfmt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkmlfmt-0.0.5.tar", max compression
+gzip compressed data, was "lkmlfmt-0.0.6.tar", max compression
```

## Comparing `lkmlfmt-0.0.5.tar` & `lkmlfmt-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2647 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/README.md
--rw-r--r--   0        0        0       53 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/__init__.py
--rw-r--r--   0        0        0       70 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/__main__.py
--rw-r--r--   0        0        0     2546 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/command.py
--rw-r--r--   0        0        0      100 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/exception.py
--rw-r--r--   0        0        0    11101 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/formatter.py
--rw-r--r--   0        0        0      757 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/lkml.lark
--rw-r--r--   0        0        0       64 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/logger.py
--rw-r--r--   0        0        0     2292 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/parser.py
--rw-r--r--   0        0        0     4806 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/lkmlfmt/template.py
--rw-r--r--   0        0        0      552 2023-04-22 06:39:17.111472 lkmlfmt-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 lkmlfmt-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2647 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/README.md
+-rw-r--r--   0        0        0       53 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/__main__.py
+-rw-r--r--   0        0        0     2546 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/command.py
+-rw-r--r--   0        0        0      100 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/exception.py
+-rw-r--r--   0        0        0    11101 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/formatter.py
+-rw-r--r--   0        0        0      757 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/lkml.lark
+-rw-r--r--   0        0        0       64 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/logger.py
+-rw-r--r--   0        0        0     2292 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/parser.py
+-rw-r--r--   0        0        0     4806 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/template.py
+-rw-r--r--   0        0        0      552 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 lkmlfmt-0.0.6/PKG-INFO
```

### Comparing `lkmlfmt-0.0.5/README.md` & `lkmlfmt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.5/lkmlfmt/command.py` & `lkmlfmt-0.0.6/lkmlfmt/command.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.5/lkmlfmt/formatter.py` & `lkmlfmt-0.0.6/lkmlfmt/formatter.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.5/lkmlfmt/lkml.lark` & `lkmlfmt-0.0.6/lkmlfmt/lkml.lark`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.5/lkmlfmt/parser.py` & `lkmlfmt-0.0.6/lkmlfmt/parser.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.5/lkmlfmt/template.py` & `lkmlfmt-0.0.6/lkmlfmt/template.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.5/pyproject.toml` & `lkmlfmt-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "lkmlfmt"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["dr666m1 <skndr666m1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 lkmlfmt = "lkmlfmt.command:run"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 lark = "^1.1.5"
-shandy-sqlfmt = "^0.17.0"
 click = "^8.1.3"
 djhtml = "^3.0.6"
+shandy-sqlfmt = "^0.18.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.1"
 isort = "^5.12.0"
```

### Comparing `lkmlfmt-0.0.5/PKG-INFO` & `lkmlfmt-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lkmlfmt
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: dr666m1
 Author-email: skndr666m1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: djhtml (>=3.0.6,<4.0.0)
 Requires-Dist: lark (>=1.1.5,<2.0.0)
-Requires-Dist: shandy-sqlfmt (>=0.17.0,<0.18.0)
+Requires-Dist: shandy-sqlfmt (>=0.18.1,<0.19.0)
 Description-Content-Type: text/markdown
 
 # lkmlfmt
 lkmlfmt formats your LookML files including embedded SQL and HTML.
 
 ## Installation
 ```sh
```

