# Comparing `tmp/async_pymongo-0.1.1.tar.gz` & `tmp/async_pymongo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_pymongo-0.1.1.tar", max compression
+gzip compressed data, was "async_pymongo-0.1.2.tar", max compression
```

## Comparing `async_pymongo-0.1.1.tar` & `async_pymongo-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-05-19 12:41:58.827361 async_pymongo-0.1.1/LICENSE
--rw-r--r--   0        0        0       33 2023-05-19 12:32:53.659374 async_pymongo-0.1.1/README.md
--rw-r--r--   0        0        0     1110 2023-05-19 12:35:12.219371 async_pymongo-0.1.1/async_pymongo/__init__.py
--rw-r--r--   0        0        0     1227 2023-05-19 12:35:34.141370 async_pymongo-0.1.1/async_pymongo/async_helper.py
--rw-r--r--   0        0        0     3383 2023-05-19 12:35:56.153370 async_pymongo-0.1.1/async_pymongo/base.py
--rw-r--r--   0        0        0     4419 2023-05-19 12:36:00.219370 async_pymongo-0.1.1/async_pymongo/change_stream.py
--rw-r--r--   0        0        0     8569 2023-05-19 12:36:04.453369 async_pymongo-0.1.1/async_pymongo/client.py
--rw-r--r--   0        0        0     6825 2023-05-19 12:36:08.703369 async_pymongo-0.1.1/async_pymongo/client_session.py
--rw-r--r--   0        0        0    17710 2023-05-19 12:36:15.287369 async_pymongo-0.1.1/async_pymongo/collection.py
--rw-r--r--   0        0        0     7482 2023-05-19 12:37:24.525368 async_pymongo-0.1.1/async_pymongo/command_cursor.py
--rw-r--r--   0        0        0     6533 2023-05-19 12:36:22.935369 async_pymongo-0.1.1/async_pymongo/cursor.py
--rw-r--r--   0        0        0     6977 2023-05-19 12:36:27.975369 async_pymongo-0.1.1/async_pymongo/cursor_base.py
--rw-r--r--   0        0        0     9347 2023-05-19 12:36:34.353369 async_pymongo-0.1.1/async_pymongo/db.py
--rw-r--r--   0        0        0      942 2023-05-19 12:36:43.745369 async_pymongo-0.1.1/async_pymongo/errors.py
--rw-r--r--   0        0        0     1338 2023-05-19 12:35:49.663370 async_pymongo-0.1.1/async_pymongo/typings.py
--rw-r--r--   0        0        0     1129 2023-05-19 13:00:35.259333 async_pymongo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 async_pymongo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-19 12:41:58.827361 async_pymongo-0.1.2/LICENSE
+-rw-r--r--   0        0        0       33 2023-05-19 12:32:53.659374 async_pymongo-0.1.2/README.md
+-rw-r--r--   0        0        0     1110 2023-05-19 12:35:12.219371 async_pymongo-0.1.2/async_pymongo/__init__.py
+-rw-r--r--   0        0        0     1227 2023-05-19 12:35:34.141370 async_pymongo-0.1.2/async_pymongo/async_helper.py
+-rw-r--r--   0        0        0     3383 2023-05-19 12:35:56.153370 async_pymongo-0.1.2/async_pymongo/base.py
+-rw-r--r--   0        0        0     4419 2023-05-19 12:36:00.219370 async_pymongo-0.1.2/async_pymongo/change_stream.py
+-rw-r--r--   0        0        0     8569 2023-05-19 12:36:04.453369 async_pymongo-0.1.2/async_pymongo/client.py
+-rw-r--r--   0        0        0     6825 2023-05-19 12:36:08.703369 async_pymongo-0.1.2/async_pymongo/client_session.py
+-rw-r--r--   0        0        0    17710 2023-05-19 12:36:15.287369 async_pymongo-0.1.2/async_pymongo/collection.py
+-rw-r--r--   0        0        0     7482 2023-05-19 12:37:24.525368 async_pymongo-0.1.2/async_pymongo/command_cursor.py
+-rw-r--r--   0        0        0     6533 2023-05-19 12:36:22.935369 async_pymongo-0.1.2/async_pymongo/cursor.py
+-rw-r--r--   0        0        0     6977 2023-05-19 12:36:27.975369 async_pymongo-0.1.2/async_pymongo/cursor_base.py
+-rw-r--r--   0        0        0     9347 2023-05-19 12:36:34.353369 async_pymongo-0.1.2/async_pymongo/db.py
+-rw-r--r--   0        0        0      942 2023-05-19 12:36:43.745369 async_pymongo-0.1.2/async_pymongo/errors.py
+-rw-r--r--   0        0        0     1338 2023-05-19 12:35:49.663370 async_pymongo-0.1.2/async_pymongo/typings.py
+-rw-r--r--   0        0        0     1040 2023-05-19 14:11:22.009226 async_pymongo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 async_pymongo-0.1.2/PKG-INFO
```

### Comparing `async_pymongo-0.1.1/LICENSE` & `async_pymongo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/__init__.py` & `async_pymongo-0.1.2/async_pymongo/__init__.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/async_helper.py` & `async_pymongo-0.1.2/async_pymongo/async_helper.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/base.py` & `async_pymongo-0.1.2/async_pymongo/base.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/change_stream.py` & `async_pymongo-0.1.2/async_pymongo/change_stream.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/client.py` & `async_pymongo-0.1.2/async_pymongo/client.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/client_session.py` & `async_pymongo-0.1.2/async_pymongo/client_session.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/collection.py` & `async_pymongo-0.1.2/async_pymongo/collection.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/command_cursor.py` & `async_pymongo-0.1.2/async_pymongo/command_cursor.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/cursor.py` & `async_pymongo-0.1.2/async_pymongo/cursor.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/cursor_base.py` & `async_pymongo-0.1.2/async_pymongo/cursor_base.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/db.py` & `async_pymongo-0.1.2/async_pymongo/db.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/errors.py` & `async_pymongo-0.1.2/async_pymongo/errors.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/async_pymongo/typings.py` & `async_pymongo-0.1.2/async_pymongo/typings.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.1/pyproject.toml` & `async_pymongo-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-pymongo"
-version = "0.1.1"
+version = "0.1.2"
 description = "Asynchronous wrapper for pymongo"
 license = "GPL-3.0-or-later"
 authors = [
     "Adek Maulana <adekzmaulana@gmail.com>",
     "Gaung Ramadhan <hi@mrmiss.my.id>",
     "wulan17 <wulan17@nusantararom.org>"
 ]
@@ -13,26 +13,24 @@
 keywords = ["async", "python", "pymongo"]
 classifiers = [
     "Environment :: Console",
     "Framework :: AsyncIO",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Database",
 ]
 
 packages = [{include = "async_pymongo"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "~=3.9"
 pymongo = "^4.3.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `async_pymongo-0.1.1/PKG-INFO` & `async_pymongo-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: async-pymongo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous wrapper for pymongo
 Home-page: https://github.com/Mayuri-Chan/async_pymongo
 License: GPL-3.0-or-later
 Keywords: async,python,pymongo
 Author: Adek Maulana
 Author-email: adekzmaulana@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Project-URL: Repository, https://github.com/Mayuri-Chan/async_pymongo
 Description-Content-Type: text/markdown
 
 Asynchronous wrapper for pymongo
```

