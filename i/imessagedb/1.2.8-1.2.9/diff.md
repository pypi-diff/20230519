# Comparing `tmp/imessagedb-1.2.8.tar.gz` & `tmp/imessagedb-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.2.8.tar", max compression
+gzip compressed data, was "imessagedb-1.2.9.tar", max compression
```

## Comparing `imessagedb-1.2.8.tar` & `imessagedb-1.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1070 2023-05-18 02:57:53.956294 imessagedb-1.2.8/LICENSE
--rw-r--r--   0        0        0     8458 2023-05-18 02:57:53.956294 imessagedb-1.2.8/README.md
--rw-r--r--   0        0        0     1309 2023-05-18 02:58:25.356546 imessagedb-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     9342 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8476 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3055 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2133 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/chat.py
--rw-r--r--   0        0        0     2518 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3301 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/default.ini
--rw-r--r--   0        0        0      985 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/handle.py
--rw-r--r--   0        0        0     1640 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/handles.py
--rw-r--r--   0        0        0    23179 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/html.py
--rw-r--r--   0        0        0     4975 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/message.py
--rw-r--r--   0        0        0     4896 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/messages.py
--rw-r--r--   0        0        0     4182 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/text.py
--rw-r--r--   0        0        0      538 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/utils.py
--rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-18 03:16:08.542343 imessagedb-1.2.9/LICENSE
+-rw-r--r--   0        0        0     8509 2023-05-18 03:16:08.542343 imessagedb-1.2.9/README.md
+-rw-r--r--   0        0        0     1309 2023-05-18 03:16:52.974677 imessagedb-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     9342 2023-05-18 03:16:08.542343 imessagedb-1.2.9/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-18 03:16:08.542343 imessagedb-1.2.9/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8476 2023-05-18 03:16:08.542343 imessagedb-1.2.9/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3055 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2133 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     2518 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3301 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/default.ini
+-rw-r--r--   0        0        0      985 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     1640 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    23179 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/html.py
+-rw-r--r--   0        0        0     4975 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/message.py
+-rw-r--r--   0        0        0     4896 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     4182 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/text.py
+-rw-r--r--   0        0        0      538 2023-05-18 03:16:08.546342 imessagedb-1.2.9/src/imessagedb/utils.py
+-rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 imessagedb-1.2.9/PKG-INFO
```

### Comparing `imessagedb-1.2.8/LICENSE` & `imessagedb-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/README.md` & `imessagedb-1.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 **--no_copy**             Don't copy the attachments. This will make them inaccessible for 
 viewing
 
 **--no_attachments**      Do not show the attachments at all
 
 **-v, --verbose**         Turn on additional output
 
+**--version**  Shows the version number and exits
+
 
 ### Configuration File
 
 The configuration file is in configparser format. Here is the template that is created
 by default:
 
 ```python
```

### Comparing `imessagedb-1.2.8/pyproject.toml` & `imessagedb-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.2.8"
+version = "1.2.9"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.2.8/src/imessagedb/__init__.py` & `imessagedb-1.2.9/src/imessagedb/__init__.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/attachment.py` & `imessagedb-1.2.9/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/attachments.py` & `imessagedb-1.2.9/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/chat.py` & `imessagedb-1.2.9/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/chats.py` & `imessagedb-1.2.9/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/db.py` & `imessagedb-1.2.9/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/default.ini` & `imessagedb-1.2.9/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/handle.py` & `imessagedb-1.2.9/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/handles.py` & `imessagedb-1.2.9/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/html.py` & `imessagedb-1.2.9/src/imessagedb/html.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/message.py` & `imessagedb-1.2.9/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/messages.py` & `imessagedb-1.2.9/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/text.py` & `imessagedb-1.2.9/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/src/imessagedb/utils.py` & `imessagedb-1.2.9/src/imessagedb/utils.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.8/PKG-INFO` & `imessagedb-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.2.8
+Version: 1.2.9
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -131,14 +131,16 @@
 **--no_copy**             Don't copy the attachments. This will make them inaccessible for 
 viewing
 
 **--no_attachments**      Do not show the attachments at all
 
 **-v, --verbose**         Turn on additional output
 
+**--version**  Shows the version number and exits
+
 
 ### Configuration File
 
 The configuration file is in configparser format. Here is the template that is created
 by default:
 
 ```python
```

