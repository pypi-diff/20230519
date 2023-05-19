# Comparing `tmp/guten-0.1.9.tar.gz` & `tmp/guten-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guten-0.1.9.tar", max compression
+gzip compressed data, was "guten-0.2.0.tar", max compression
```

## Comparing `guten-0.1.9.tar` & `guten-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0       54 2022-12-25 18:53:57.314870 guten-0.1.9/README.md
--rw-r--r--   0        0        0        0 2022-12-24 11:32:16.552571 guten-0.1.9/guten/__init__.py
--rw-r--r--   0        0        0      876 2022-12-26 05:13:17.812880 guten-0.1.9/guten/__main__.py
--rw-r--r--   0        0        0     1207 2022-12-26 04:57:45.933337 guten-0.1.9/guten/backend.py
--rw-r--r--   0        0        0     4930 2023-04-08 17:27:57.778085 guten-0.1.9/guten/backends/html.py
--rw-r--r--   0        0        0     2443 2022-12-27 06:42:31.641999 guten-0.1.9/guten/backends/text.py
--rw-r--r--   0        0        0     3272 2022-12-26 05:15:30.047264 guten-0.1.9/guten/config.py
--rw-r--r--   0        0        0     3383 2023-04-08 16:56:06.506470 guten-0.1.9/guten/press.py
--rw-r--r--   0        0        0      184 2022-12-25 03:46:23.026388 guten-0.1.9/guten/source.py
--rw-r--r--   0        0        0      362 2022-12-25 18:33:08.012285 guten-0.1.9/guten/utils.py
--rw-r--r--   0        0        0      376 2023-04-08 17:33:39.210665 guten-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 guten-0.1.9/setup.py
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 guten-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       54 2022-12-25 18:53:57.314870 guten-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-24 11:32:16.552571 guten-0.2.0/guten/__init__.py
+-rw-r--r--   0        0        0      876 2022-12-26 05:13:17.812880 guten-0.2.0/guten/__main__.py
+-rw-r--r--   0        0        0     1207 2023-05-18 19:01:48.564705 guten-0.2.0/guten/backend.py
+-rw-r--r--   0        0        0     3022 2023-05-18 19:39:25.218152 guten-0.2.0/guten/backends/html.py
+-rw-r--r--   0        0        0     2443 2022-12-27 06:42:31.641999 guten-0.2.0/guten/backends/text.py
+-rw-r--r--   0        0        0     3272 2022-12-26 05:15:30.047264 guten-0.2.0/guten/config.py
+-rw-r--r--   0        0        0     1158 2023-05-18 19:38:39.309147 guten-0.2.0/guten/filters.py
+-rw-r--r--   0        0        0     2378 2023-05-18 19:37:32.140056 guten-0.2.0/guten/metadata.py
+-rw-r--r--   0        0        0     3383 2023-04-08 16:56:06.506470 guten-0.2.0/guten/press.py
+-rw-r--r--   0        0        0      184 2022-12-25 03:46:23.026388 guten-0.2.0/guten/source.py
+-rw-r--r--   0        0        0      362 2022-12-25 18:33:08.012285 guten-0.2.0/guten/utils.py
+-rw-r--r--   0        0        0      376 2023-05-18 19:51:46.469020 guten-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 guten-0.2.0/setup.py
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 guten-0.2.0/PKG-INFO
```

### Comparing `guten-0.1.9/guten/__main__.py` & `guten-0.2.0/guten/__main__.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.9/guten/backend.py` & `guten-0.2.0/guten/backend.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.9/guten/backends/text.py` & `guten-0.2.0/guten/backends/text.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.9/guten/config.py` & `guten-0.2.0/guten/config.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.9/guten/press.py` & `guten-0.2.0/guten/press.py`

 * *Files identical despite different names*

### Comparing `guten-0.1.9/setup.py` & `guten-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pandas>=1.5.2,<2.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'pytz>=2022.7,<2023.0',
  'toml==0.10.2']
 
 setup_kwargs = {
     'name': 'guten',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': '',
     'long_description': '# guten\n\nCompile RSS/Atom feeds into a combined feed.\n',
     'author': 'Elton',
     'author_email': 'eltonp3103@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `guten-0.1.9/PKG-INFO` & `guten-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guten
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: Elton
 Author-email: eltonp3103@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

