# Comparing `tmp/djangocms-layouttools-0.1.3.tar.gz` & `tmp/djangocms-layouttools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-layouttools-0.1.3.tar", last modified: Fri May 19 16:54:51 2023, max compression
+gzip compressed data, was "djangocms-layouttools-0.1.4.tar", last modified: Fri May 19 17:31:42 2023, max compression
```

## Comparing `djangocms-layouttools-0.1.3.tar` & `djangocms-layouttools-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.601999 djangocms-layouttools-0.1.3/
--rw-r--r--   0 russmo     (501) staff       (20)     1090 2018-03-01 00:34:30.000000 djangocms-layouttools-0.1.3/LICENSE.txt
--rw-r--r--   0 russmo     (501) staff       (20)      166 2018-03-06 20:48:10.000000 djangocms-layouttools-0.1.3/MANIFEST.in
--rw-r--r--   0 russmo     (501) staff       (20)     3324 2023-05-19 16:54:51.602080 djangocms-layouttools-0.1.3/PKG-INFO
--rw-r--r--   0 russmo     (501) staff       (20)     1996 2021-01-12 06:57:13.000000 djangocms-layouttools-0.1.3/README.rst
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.591039 djangocms-layouttools-0.1.3/djangocms_layouttools/
--rw-r--r--   0 russmo     (501) staff       (20)       46 2023-05-19 16:50:16.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/__init__.py
--rw-r--r--   0 russmo     (501) staff       (20)      624 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/admin.py
--rw-r--r--   0 russmo     (501) staff       (20)      235 2023-05-19 16:47:54.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/apps.py
--rw-r--r--   0 russmo     (501) staff       (20)     1213 2018-03-06 20:40:22.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/cms_plugins.py
--rw-r--r--   0 russmo     (501) staff       (20)      240 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/fields.py
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.600253 djangocms-layouttools-0.1.3/djangocms_layouttools/migrations/
--rw-r--r--   0 russmo     (501) staff       (20)     3768 2018-03-13 17:56:36.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/migrations/0001_initial.py
--rw-r--r--   0 russmo     (501) staff       (20)        0 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/migrations/__init__.py
--rw-r--r--   0 russmo     (501) staff       (20)     4550 2021-01-12 06:32:31.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/models.py
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.585148 djangocms-layouttools-0.1.3/djangocms_layouttools/templates/
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.600415 djangocms-layouttools-0.1.3/djangocms_layouttools/templates/djangocms_layouttools/
--rw-r--r--   0 russmo     (501) staff       (20)      953 2018-03-05 20:05:37.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/templates/djangocms_layouttools/section.html
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.601835 djangocms-layouttools-0.1.3/djangocms_layouttools/tests/
--rw-r--r--   0 russmo     (501) staff       (20)       24 2018-03-01 20:48:06.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/tests/__init__.py
--rw-r--r--   0 russmo     (501) staff       (20)      460 2018-03-01 20:49:29.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/tests/settings.py
--rw-r--r--   0 russmo     (501) staff       (20)      673 2018-03-01 23:37:26.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/tests/tests_models.py
--rw-r--r--   0 russmo     (501) staff       (20)       63 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.3/djangocms_layouttools/views.py
-drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 16:54:51.599496 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/
--rw-r--r--   0 russmo     (501) staff       (20)     3324 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/PKG-INFO
--rw-r--r--   0 russmo     (501) staff       (20)      833 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/SOURCES.txt
--rw-r--r--   0 russmo     (501) staff       (20)        1 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/dependency_links.txt
--rw-r--r--   0 russmo     (501) staff       (20)        1 2018-03-06 20:50:50.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/not-zip-safe
--rw-r--r--   0 russmo     (501) staff       (20)       72 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/requires.txt
--rw-r--r--   0 russmo     (501) staff       (20)       22 2023-05-19 16:54:51.000000 djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/top_level.txt
--rw-r--r--   0 russmo     (501) staff       (20)      172 2023-05-19 16:54:51.603000 djangocms-layouttools-0.1.3/setup.cfg
--rw-r--r--   0 russmo     (501) staff       (20)     1753 2021-01-12 07:04:03.000000 djangocms-layouttools-0.1.3/setup.py
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 17:31:42.080859 djangocms-layouttools-0.1.4/
+-rw-r--r--   0 russmo     (501) staff       (20)     1090 2018-03-01 00:34:30.000000 djangocms-layouttools-0.1.4/LICENSE.txt
+-rw-r--r--   0 russmo     (501) staff       (20)      166 2018-03-06 20:48:10.000000 djangocms-layouttools-0.1.4/MANIFEST.in
+-rw-r--r--   0 russmo     (501) staff       (20)     3324 2023-05-19 17:31:42.080953 djangocms-layouttools-0.1.4/PKG-INFO
+-rw-r--r--   0 russmo     (501) staff       (20)     1996 2021-01-12 06:57:13.000000 djangocms-layouttools-0.1.4/README.rst
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 17:31:42.070550 djangocms-layouttools-0.1.4/djangocms_layouttools/
+-rw-r--r--   0 russmo     (501) staff       (20)       46 2023-05-19 17:31:11.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/__init__.py
+-rw-r--r--   0 russmo     (501) staff       (20)      624 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/admin.py
+-rw-r--r--   0 russmo     (501) staff       (20)      240 2023-05-19 17:27:49.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/apps.py
+-rw-r--r--   0 russmo     (501) staff       (20)     1213 2018-03-06 20:40:22.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/cms_plugins.py
+-rw-r--r--   0 russmo     (501) staff       (20)      240 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/fields.py
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 17:31:42.079080 djangocms-layouttools-0.1.4/djangocms_layouttools/migrations/
+-rw-r--r--   0 russmo     (501) staff       (20)     3768 2018-03-13 17:56:36.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/migrations/0001_initial.py
+-rw-r--r--   0 russmo     (501) staff       (20)        0 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/migrations/__init__.py
+-rw-r--r--   0 russmo     (501) staff       (20)     4550 2021-01-12 06:32:31.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/models.py
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 17:31:42.066455 djangocms-layouttools-0.1.4/djangocms_layouttools/templates/
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 17:31:42.079267 djangocms-layouttools-0.1.4/djangocms_layouttools/templates/djangocms_layouttools/
+-rw-r--r--   0 russmo     (501) staff       (20)      953 2018-03-05 20:05:37.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/templates/djangocms_layouttools/section.html
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 17:31:42.080644 djangocms-layouttools-0.1.4/djangocms_layouttools/tests/
+-rw-r--r--   0 russmo     (501) staff       (20)       24 2018-03-01 20:48:06.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/tests/__init__.py
+-rw-r--r--   0 russmo     (501) staff       (20)      460 2018-03-01 20:49:29.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/tests/settings.py
+-rw-r--r--   0 russmo     (501) staff       (20)      673 2018-03-01 23:37:26.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/tests/tests_models.py
+-rw-r--r--   0 russmo     (501) staff       (20)       63 2018-02-28 23:55:43.000000 djangocms-layouttools-0.1.4/djangocms_layouttools/views.py
+drwxr-xr-x   0 russmo     (501) staff       (20)        0 2023-05-19 17:31:42.078522 djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/
+-rw-r--r--   0 russmo     (501) staff       (20)     3324 2023-05-19 17:31:42.000000 djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/PKG-INFO
+-rw-r--r--   0 russmo     (501) staff       (20)      833 2023-05-19 17:31:42.000000 djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/SOURCES.txt
+-rw-r--r--   0 russmo     (501) staff       (20)        1 2023-05-19 17:31:42.000000 djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/dependency_links.txt
+-rw-r--r--   0 russmo     (501) staff       (20)        1 2018-03-06 20:50:50.000000 djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/not-zip-safe
+-rw-r--r--   0 russmo     (501) staff       (20)       72 2023-05-19 17:31:42.000000 djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/requires.txt
+-rw-r--r--   0 russmo     (501) staff       (20)       22 2023-05-19 17:31:42.000000 djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/top_level.txt
+-rw-r--r--   0 russmo     (501) staff       (20)      172 2023-05-19 17:31:42.081827 djangocms-layouttools-0.1.4/setup.cfg
+-rw-r--r--   0 russmo     (501) staff       (20)     1753 2021-01-12 07:04:03.000000 djangocms-layouttools-0.1.4/setup.py
```

### Comparing `djangocms-layouttools-0.1.3/LICENSE.txt` & `djangocms-layouttools-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/PKG-INFO` & `djangocms-layouttools-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-layouttools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Adds layout Section and other plugins to django CMS.
 Home-page: https://github.com/mci/djangocms-layouttools
 Author: Russell Moffitt, Marine Conservation Institute
 Author-email: Russell.Moffitt@marine-conservation.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `djangocms-layouttools-0.1.3/README.rst` & `djangocms-layouttools-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/djangocms_layouttools/admin.py` & `djangocms-layouttools-0.1.4/djangocms_layouttools/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/djangocms_layouttools/cms_plugins.py` & `djangocms-layouttools-0.1.4/djangocms_layouttools/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/djangocms_layouttools/migrations/0001_initial.py` & `djangocms-layouttools-0.1.4/djangocms_layouttools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/djangocms_layouttools/models.py` & `djangocms-layouttools-0.1.4/djangocms_layouttools/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/djangocms_layouttools/templates/djangocms_layouttools/section.html` & `djangocms-layouttools-0.1.4/djangocms_layouttools/templates/djangocms_layouttools/section.html`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/djangocms_layouttools/tests/tests_models.py` & `djangocms-layouttools-0.1.4/djangocms_layouttools/tests/tests_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/PKG-INFO` & `djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-layouttools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Adds layout Section and other plugins to django CMS.
 Home-page: https://github.com/mci/djangocms-layouttools
 Author: Russell Moffitt, Marine Conservation Institute
 Author-email: Russell.Moffitt@marine-conservation.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `djangocms-layouttools-0.1.3/djangocms_layouttools.egg-info/SOURCES.txt` & `djangocms-layouttools-0.1.4/djangocms_layouttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-layouttools-0.1.3/setup.py` & `djangocms-layouttools-0.1.4/setup.py`

 * *Files identical despite different names*

