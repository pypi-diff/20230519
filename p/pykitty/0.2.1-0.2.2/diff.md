# Comparing `tmp/pykitty-0.2.1.tar.gz` & `tmp/pykitty-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykitty-0.2.1.tar", max compression
+gzip compressed data, was "pykitty-0.2.2.tar", max compression
```

## Comparing `pykitty-0.2.1.tar` & `pykitty-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2202 2023-04-07 10:29:06.231169 pykitty-0.2.1/README.md
--rw-r--r--   0        0        0       21 2023-04-06 19:26:41.689694 pykitty-0.2.1/pykitty/__init__.py
--rw-r--r--   0        0        0     2943 2023-04-06 19:00:01.649008 pykitty-0.2.1/pykitty/cli.py
--rw-r--r--   0        0        0     6071 2023-04-07 10:29:06.231436 pykitty-0.2.1/pykitty/client.py
--rw-r--r--   0        0        0     3016 2023-04-07 10:29:06.231718 pykitty-0.2.1/pykitty/kitty_parser.py
--rw-r--r--   0        0        0      531 2023-04-07 10:29:06.231984 pykitty-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 pykitty-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-07 13:19:00.028271 pykitty-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2195 2023-04-07 13:14:15.727476 pykitty-0.2.2/README.md
+-rw-r--r--   0        0        0       34 2023-05-19 19:18:21.950507 pykitty-0.2.2/pykitty/__init__.py
+-rw-r--r--   0        0        0     2943 2023-04-06 19:00:01.649008 pykitty-0.2.2/pykitty/cli.py
+-rw-r--r--   0        0        0     6071 2023-04-07 10:29:06.231436 pykitty-0.2.2/pykitty/client.py
+-rw-r--r--   0        0        0     3016 2023-04-07 10:29:06.231718 pykitty-0.2.2/pykitty/kitty_parser.py
+-rw-r--r--   0        0        0      531 2023-05-19 19:19:50.306239 pykitty-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 pykitty-0.2.2/PKG-INFO
```

### Comparing `pykitty-0.2.1/README.md` & `pykitty-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -87,12 +87,12 @@
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Next Steps (TODO)
 
-- [x] Parse Kitty URL parser to extract `kitty_id` 
+- [x] Parse Kitty URL to extract `kitty_id` 
 - [x] Implement `get_expenses` method to retrieve all expenses.
 - [ ] Add support for updating and deleting expenses.
 - [ ] Document CLI usage.
 - [ ] Support for Kittysplit in other languages.
```

### Comparing `pykitty-0.2.1/pykitty/cli.py` & `pykitty-0.2.2/pykitty/cli.py`

 * *Files identical despite different names*

### Comparing `pykitty-0.2.1/pykitty/client.py` & `pykitty-0.2.2/pykitty/client.py`

 * *Files identical despite different names*

### Comparing `pykitty-0.2.1/pykitty/kitty_parser.py` & `pykitty-0.2.2/pykitty/kitty_parser.py`

 * *Files identical despite different names*

### Comparing `pykitty-0.2.1/pyproject.toml` & `pykitty-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykitty"
-version = "0.2.1"
+version = "0.2.2"
 description = "The unofficial Kittysplit wrapper for Python."
 authors = ["Lars Heinen"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.scripts]
 pykitty = "pykitty.cli:app"
```

### Comparing `pykitty-0.2.1/PKG-INFO` & `pykitty-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykitty
-Version: 0.2.1
+Version: 0.2.2
 Summary: The unofficial Kittysplit wrapper for Python.
 License: MIT
 Author: Lars Heinen
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -105,13 +105,13 @@
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Next Steps (TODO)
 
-- [x] Parse Kitty URL parser to extract `kitty_id` 
+- [x] Parse Kitty URL to extract `kitty_id` 
 - [x] Implement `get_expenses` method to retrieve all expenses.
 - [ ] Add support for updating and deleting expenses.
 - [ ] Document CLI usage.
 - [ ] Support for Kittysplit in other languages.
```

