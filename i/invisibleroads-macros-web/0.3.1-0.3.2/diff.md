# Comparing `tmp/invisibleroads-macros-web-0.3.1.tar.gz` & `tmp/invisibleroads-macros-web-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invisibleroads-macros-web-0.3.1.tar", last modified: Wed Apr 26 17:24:02 2023, max compression
+gzip compressed data, was "invisibleroads-macros-web-0.3.2.tar", last modified: Fri May 19 16:58:21 2023, max compression
```

## Comparing `invisibleroads-macros-web-0.3.1.tar` & `invisibleroads-macros-web-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:24:02.819001 invisibleroads-macros-web-0.3.1/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      288 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/CHANGES.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/MANIFEST.in
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-04-26 17:24:02.818001 invisibleroads-macros-web-0.3.1/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1086 2023-02-04 11:58:00.000000 invisibleroads-macros-web-0.3.1/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:24:02.814000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      846 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/browser.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      290 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/escape.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1263 2023-02-08 13:47:12.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/jinja.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      652 2023-04-25 11:27:49.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/markdown.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/port.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1117 2023-04-05 01:08:22.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/starlette.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:24:02.816001 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      667 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      163 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       32 2023-04-26 17:24:02.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-02-04 12:09:21.000000 invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2023-04-26 17:24:02.819001 invisibleroads-macros-web-0.3.1/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1374 2023-04-26 17:18:20.000000 invisibleroads-macros-web-0.3.1/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:24:02.817000 invisibleroads-macros-web-0.3.1/tests/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-26 17:22:15.000000 invisibleroads-macros-web-0.3.1/tests/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      344 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/tests/test_escape.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      549 2023-02-04 11:54:56.000000 invisibleroads-macros-web-0.3.1/tests/test_markdown.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-04-26 17:17:57.000000 invisibleroads-macros-web-0.3.1/tests/test_port.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 16:58:21.125714 invisibleroads-macros-web-0.3.2/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      288 2022-12-16 04:15:30.000000 invisibleroads-macros-web-0.3.2/CHANGES.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2022-09-23 03:10:37.000000 invisibleroads-macros-web-0.3.2/MANIFEST.in
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-05-19 16:58:21.124714 invisibleroads-macros-web-0.3.2/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1086 2023-02-08 16:42:52.000000 invisibleroads-macros-web-0.3.2/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 16:58:21.122714 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-09-23 04:08:50.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      846 2022-09-23 04:13:04.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/browser.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      290 2022-09-23 04:08:43.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/escape.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1263 2023-02-08 16:42:52.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/jinja.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      637 2023-05-19 16:53:17.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/markdown.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2022-09-23 04:13:41.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/port.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1117 2023-04-01 12:03:48.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/starlette.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 16:58:21.123714 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-05-19 16:58:21.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      667 2023-05-19 16:58:21.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-19 16:58:21.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      163 2023-05-19 16:58:21.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       32 2023-05-19 16:58:21.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-09-23 04:23:43.000000 invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2023-05-19 16:58:21.125714 invisibleroads-macros-web-0.3.2/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1374 2023-05-19 16:56:50.000000 invisibleroads-macros-web-0.3.2/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-19 16:58:21.124714 invisibleroads-macros-web-0.3.2/tests/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-04-26 18:11:44.000000 invisibleroads-macros-web-0.3.2/tests/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      344 2022-09-23 04:17:46.000000 invisibleroads-macros-web-0.3.2/tests/test_escape.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      784 2023-05-19 16:49:25.000000 invisibleroads-macros-web-0.3.2/tests/test_markdown.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-04-26 18:11:44.000000 invisibleroads-macros-web-0.3.2/tests/test_port.py
```

### Comparing `invisibleroads-macros-web-0.3.1/PKG-INFO` & `invisibleroads-macros-web-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invisibleroads-macros-web
-Version: 0.3.1
+Version: 0.3.2
 Summary: Shortcut functions for web operations
 Home-page: https://github.com/invisibleroads/invisibleroads-macros-web
 Author: Roy Hyunjin Han
 Author-email: rhh@crosscompute.com
 Keywords: invisibleroads
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `invisibleroads-macros-web-0.3.1/README.md` & `invisibleroads-macros-web-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/browser.py` & `invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/browser.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/jinja.py` & `invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/jinja.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/port.py` & `invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/port.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web/starlette.py` & `invisibleroads-macros-web-0.3.2/invisibleroads_macros_web/starlette.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/PKG-INFO` & `invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invisibleroads-macros-web
-Version: 0.3.1
+Version: 0.3.2
 Summary: Shortcut functions for web operations
 Home-page: https://github.com/invisibleroads/invisibleroads-macros-web
 Author: Roy Hyunjin Han
 Author-email: rhh@crosscompute.com
 Keywords: invisibleroads
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `invisibleroads-macros-web-0.3.1/invisibleroads_macros_web.egg-info/SOURCES.txt` & `invisibleroads-macros-web-0.3.2/invisibleroads_macros_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.1/setup.py` & `invisibleroads-macros-web-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 FOLDER = dirname(abspath(__file__))
 DESCRIPTION = '\n\n'.join(open(join(FOLDER, _)).read().strip() for _ in [
     'README.md', 'CHANGES.md'])
 
 
 setup(
     name='invisibleroads-macros-web',
-    version='0.3.1',
+    version='0.3.2',
     description='Shortcut functions for web operations',
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python',
         'License :: OSI Approved :: MIT License',
     ],
```

### Comparing `invisibleroads-macros-web-0.3.1/tests/test_port.py` & `invisibleroads-macros-web-0.3.2/tests/test_port.py`

 * *Files identical despite different names*

