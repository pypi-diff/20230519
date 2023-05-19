# Comparing `tmp/verse-core-0.0.6.tar.gz` & `tmp/verse-core-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verse-core-0.0.6.tar", last modified: Thu May 11 01:25:16 2023, max compression
+gzip compressed data, was "verse-core-0.0.7.tar", last modified: Fri May 19 03:26:23 2023, max compression
```

## Comparing `verse-core-0.0.6.tar` & `verse-core-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 01:25:16.818259 verse-core-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verse-core-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      593 2023-05-11 01:25:16.817284 verse-core-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-26 23:13:54.000000 verse-core-0.0.6/README.md
--rw-rw-rw-   0        0        0      660 2023-05-11 01:24:50.000000 verse-core-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 01:25:16.818259 verse-core-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 01:25:16.777029 verse-core-0.0.6/verse/
-drwxrwxrwx   0        0        0        0 2023-05-11 01:25:16.801334 verse-core-0.0.6/verse/core/
--rw-rw-rw-   0        0        0      125 2023-04-27 20:54:44.000000 verse-core-0.0.6/verse/core/__init__.py
--rw-rw-rw-   0        0        0      162 2023-04-26 23:17:00.000000 verse-core-0.0.6/verse/core/async_helper.py
--rw-rw-rw-   0        0        0      402 2023-04-26 23:17:08.000000 verse-core-0.0.6/verse/core/import_helper.py
--rw-rw-rw-   0        0        0      463 2023-05-08 23:41:13.000000 verse-core-0.0.6/verse/core/model.py
--rw-rw-rw-   0        0        0       28 2023-05-11 01:18:44.000000 verse-core-0.0.6/verse/core/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-11 01:25:16.816291 verse-core-0.0.6/verse_core.egg-info/
--rw-rw-rw-   0        0        0      593 2023-05-11 01:25:16.000000 verse-core-0.0.6/verse_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-11 01:25:16.000000 verse-core-0.0.6/verse_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 01:25:16.000000 verse-core-0.0.6/verse_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 01:25:16.000000 verse-core-0.0.6/verse_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 03:26:23.986869 verse-core-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verse-core-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      593 2023-05-19 03:26:23.986869 verse-core-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-26 23:13:54.000000 verse-core-0.0.7/README.md
+-rw-rw-rw-   0        0        0      660 2023-05-19 03:26:04.000000 verse-core-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 03:26:23.987827 verse-core-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 03:26:23.951904 verse-core-0.0.7/verse/
+drwxrwxrwx   0        0        0        0 2023-05-19 03:26:23.974347 verse-core-0.0.7/verse/core/
+-rw-rw-rw-   0        0        0      125 2023-04-27 20:54:44.000000 verse-core-0.0.7/verse/core/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-04-26 23:17:00.000000 verse-core-0.0.7/verse/core/_async_helper.py
+-rw-rw-rw-   0        0        0      402 2023-04-26 23:17:08.000000 verse-core-0.0.7/verse/core/_import_helper.py
+-rw-rw-rw-   0        0        0      463 2023-05-08 23:41:13.000000 verse-core-0.0.7/verse/core/_model.py
+-rw-rw-rw-   0        0        0      430 2023-05-19 03:25:38.000000 verse-core-0.0.7/verse/core/decorators.py
+-rw-rw-rw-   0        0        0      296 2023-05-19 03:25:19.000000 verse-core-0.0.7/verse/core/exceptions.py
+-rw-rw-rw-   0        0        0       26 2023-05-11 01:27:41.000000 verse-core-0.0.7/verse/core/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-19 03:26:23.985866 verse-core-0.0.7/verse_core.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-05-19 03:26:23.000000 verse-core-0.0.7/verse_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-19 03:26:23.000000 verse-core-0.0.7/verse_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 03:26:23.000000 verse-core-0.0.7/verse_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-19 03:26:23.000000 verse-core-0.0.7/verse_core.egg-info/top_level.txt
```

### Comparing `verse-core-0.0.6/LICENSE` & `verse-core-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `verse-core-0.0.6/PKG-INFO` & `verse-core-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verse-core
-Version: 0.0.6
+Version: 0.0.7
 Summary: Core Verse package shared by all Verse packages
 Author-email: Rapidverse <admin@rapidverse.com>
 Project-URL: Homepage, https://github.com/rapidverse/verse
 Project-URL: Bug Tracker, https://github.com/rapidverse/verse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `verse-core-0.0.6/pyproject.toml` & `verse-core-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "verse-core"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name = "Rapidverse", email = "admin@rapidverse.com" }]
 description = "Core Verse package shared by all Verse packages"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `verse-core-0.0.6/verse_core.egg-info/PKG-INFO` & `verse-core-0.0.7/verse_core.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verse-core
-Version: 0.0.6
+Version: 0.0.7
 Summary: Core Verse package shared by all Verse packages
 Author-email: Rapidverse <admin@rapidverse.com>
 Project-URL: Homepage, https://github.com/rapidverse/verse
 Project-URL: Bug Tracker, https://github.com/rapidverse/verse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

