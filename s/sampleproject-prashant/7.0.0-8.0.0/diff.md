# Comparing `tmp/sampleproject-prashant-7.0.0.tar.gz` & `tmp/sampleproject-prashant-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampleproject-prashant-7.0.0.tar", last modified: Fri May 19 18:45:12 2023, max compression
+gzip compressed data, was "sampleproject-prashant-8.0.0.tar", last modified: Fri May 19 18:46:44 2023, max compression
```

## Comparing `sampleproject-prashant-7.0.0.tar` & `sampleproject-prashant-8.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:45:12.311687 sampleproject-prashant-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 18:45:02.000000 sampleproject-prashant-7.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-19 18:45:12.311687 sampleproject-prashant-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-19 18:45:02.000000 sampleproject-prashant-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-19 18:45:02.000000 sampleproject-prashant-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:45:12.311687 sampleproject-prashant-7.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:45:12.307687 sampleproject-prashant-7.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:45:12.307687 sampleproject-prashant-7.0.0/src/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-19 18:45:02.000000 sampleproject-prashant-7.0.0/src/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 18:45:02.000000 sampleproject-prashant-7.0.0/src/sample/package_data.dat
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 18:45:02.000000 sampleproject-prashant-7.0.0/src/sample/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:45:12.311687 sampleproject-prashant-7.0.0/src/sampleproject_prashant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-19 18:45:12.000000 sampleproject-prashant-7.0.0/src/sampleproject_prashant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-19 18:45:12.000000 sampleproject-prashant-7.0.0/src/sampleproject_prashant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:45:12.000000 sampleproject-prashant-7.0.0/src/sampleproject_prashant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 18:45:12.000000 sampleproject-prashant-7.0.0/src/sampleproject_prashant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 18:45:12.000000 sampleproject-prashant-7.0.0/src/sampleproject_prashant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 18:45:12.000000 sampleproject-prashant-7.0.0/src/sampleproject_prashant.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:45:12.311687 sampleproject-prashant-7.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 18:45:02.000000 sampleproject-prashant-7.0.0/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:46:44.599497 sampleproject-prashant-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 18:46:33.000000 sampleproject-prashant-8.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-19 18:46:44.599497 sampleproject-prashant-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-19 18:46:33.000000 sampleproject-prashant-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-19 18:46:33.000000 sampleproject-prashant-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:46:44.599497 sampleproject-prashant-8.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:46:44.595497 sampleproject-prashant-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:46:44.599497 sampleproject-prashant-8.0.0/src/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-19 18:46:33.000000 sampleproject-prashant-8.0.0/src/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 18:46:33.000000 sampleproject-prashant-8.0.0/src/sample/package_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 18:46:33.000000 sampleproject-prashant-8.0.0/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:46:44.599497 sampleproject-prashant-8.0.0/src/sampleproject_prashant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-19 18:46:44.000000 sampleproject-prashant-8.0.0/src/sampleproject_prashant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-19 18:46:44.000000 sampleproject-prashant-8.0.0/src/sampleproject_prashant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:46:44.000000 sampleproject-prashant-8.0.0/src/sampleproject_prashant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 18:46:44.000000 sampleproject-prashant-8.0.0/src/sampleproject_prashant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 18:46:44.000000 sampleproject-prashant-8.0.0/src/sampleproject_prashant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 18:46:44.000000 sampleproject-prashant-8.0.0/src/sampleproject_prashant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:46:44.599497 sampleproject-prashant-8.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 18:46:33.000000 sampleproject-prashant-8.0.0/tests/test_simple.py
```

### Comparing `sampleproject-prashant-7.0.0/LICENSE.txt` & `sampleproject-prashant-8.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sampleproject-prashant-7.0.0/PKG-INFO` & `sampleproject-prashant-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampleproject-prashant
-Version: 7.0.0
+Version: 8.0.0
 Summary: A sample Python project
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -43,15 +43,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
-# 7.0.0
+# 8.0.0
 # A sample Python project...
 
 ![Python Logo](https://www.python.org/static/community_logos/python-logo.png "Sample inline image")
 
 A sample project that exists as an aid to the [Python Packaging User
 Guide][packaging guide]'s [Tutorial on Packaging and Distributing
 Projects][distribution tutorial].
```

### Comparing `sampleproject-prashant-7.0.0/README.md` & `sampleproject-prashant-8.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 7.0.0
+# 8.0.0
 # A sample Python project...
 
 ![Python Logo](https://www.python.org/static/community_logos/python-logo.png "Sample inline image")
 
 A sample project that exists as an aid to the [Python Packaging User
 Guide][packaging guide]'s [Tutorial on Packaging and Distributing
 Projects][distribution tutorial].
```

### Comparing `sampleproject-prashant-7.0.0/pyproject.toml` & `sampleproject-prashant-8.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "sampleproject-prashant"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "7.0.0"  # Required
+version = "8.0.0"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A sample Python project"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `sampleproject-prashant-7.0.0/src/sampleproject_prashant.egg-info/PKG-INFO` & `sampleproject-prashant-8.0.0/src/sampleproject_prashant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sampleproject-prashant
-Version: 7.0.0
+Version: 8.0.0
 Summary: A sample Python project
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -43,15 +43,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
-# 7.0.0
+# 8.0.0
 # A sample Python project...
 
 ![Python Logo](https://www.python.org/static/community_logos/python-logo.png "Sample inline image")
 
 A sample project that exists as an aid to the [Python Packaging User
 Guide][packaging guide]'s [Tutorial on Packaging and Distributing
 Projects][distribution tutorial].
```

