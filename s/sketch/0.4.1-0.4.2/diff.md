# Comparing `tmp/sketch-0.4.1.tar.gz` & `tmp/sketch-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketch-0.4.1.tar", last modified: Tue May 16 07:00:25 2023, max compression
+gzip compressed data, was "sketch-0.4.2.tar", last modified: Fri May 19 21:36:46 2023, max compression
```

## Comparing `sketch-0.4.1.tar` & `sketch-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:00:25.768469 sketch-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:00:25.764469 sketch-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:00:25.764469 sketch-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-16 07:00:16.000000 sketch-0.4.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-16 07:00:16.000000 sketch-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 07:00:16.000000 sketch-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-16 07:00:25.768469 sketch-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-16 07:00:16.000000 sketch-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 07:00:16.000000 sketch-0.4.1/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-16 07:00:16.000000 sketch-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:00:25.768469 sketch-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:00:16.000000 sketch-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:00:25.768469 sketch-0.4.1/sketch/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 07:00:16.000000 sketch-0.4.1/sketch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-16 07:00:16.000000 sketch-0.4.1/sketch/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-16 07:00:16.000000 sketch-0.4.1/sketch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-16 07:00:16.000000 sketch-0.4.1/sketch/pandas_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-16 07:00:16.000000 sketch-0.4.1/sketch/references.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-05-16 07:00:16.000000 sketch-0.4.1/sketch/sketches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:00:25.768469 sketch-0.4.1/sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-16 07:00:25.000000 sketch-0.4.1/sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-16 07:00:25.000000 sketch-0.4.1/sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:00:25.000000 sketch-0.4.1/sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-16 07:00:25.000000 sketch-0.4.1/sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 07:00:25.000000 sketch-0.4.1/sketch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:00:25.768469 sketch-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 07:00:16.000000 sketch-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 07:00:16.000000 sketch-0.4.1/tests/test_calculate_sketches.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-16 07:00:16.000000 sketch-0.4.1/tests/test_metrics_from_sketchpads.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-16 07:00:16.000000 sketch-0.4.1/tests/test_pandas_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:36:46.706156 sketch-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:36:46.702156 sketch-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:36:46.702156 sketch-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-19 21:36:37.000000 sketch-0.4.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 21:36:37.000000 sketch-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 21:36:37.000000 sketch-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-19 21:36:46.706156 sketch-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-19 21:36:37.000000 sketch-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 21:36:37.000000 sketch-0.4.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-19 21:36:37.000000 sketch-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:36:46.706156 sketch-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:36:37.000000 sketch-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:36:46.702156 sketch-0.4.2/sketch/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 21:36:37.000000 sketch-0.4.2/sketch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-19 21:36:37.000000 sketch-0.4.2/sketch/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-19 21:36:37.000000 sketch-0.4.2/sketch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-19 21:36:37.000000 sketch-0.4.2/sketch/pandas_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-19 21:36:37.000000 sketch-0.4.2/sketch/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-05-19 21:36:37.000000 sketch-0.4.2/sketch/sketches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:36:46.702156 sketch-0.4.2/sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-19 21:36:46.000000 sketch-0.4.2/sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-19 21:36:46.000000 sketch-0.4.2/sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:36:46.000000 sketch-0.4.2/sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-19 21:36:46.000000 sketch-0.4.2/sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 21:36:46.000000 sketch-0.4.2/sketch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:36:46.706156 sketch-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-19 21:36:37.000000 sketch-0.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-19 21:36:37.000000 sketch-0.4.2/tests/test_calculate_sketches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-19 21:36:37.000000 sketch-0.4.2/tests/test_metrics_from_sketchpads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-19 21:36:37.000000 sketch-0.4.2/tests/test_pandas_extension.py
```

### Comparing `sketch-0.4.1/.github/workflows/publish-to-pypi.yml` & `sketch-0.4.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/.gitignore` & `sketch-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/LICENSE` & `sketch-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/PKG-INFO` & `sketch-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketch
-Version: 0.4.1
+Version: 0.4.2
 Summary: Compute, store and operate on data sketches
 License: MIT License
         
         Copyright (c) 2023 Justin Waugh, Mike Biven
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `sketch-0.4.1/README.md` & `sketch-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/pyproject.toml` & `sketch-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "pandas>=1.3.0",
     "datasketch>=1.5.8",
     "datasketches>=4.0.0",
     "ipython",
-    "lambdaprompt>=0.5.3",
+    "lambdaprompt>=0.5.4",
     "packaging"
 ]
 urls = {homepage = "https://github.com/approximatelabs/sketch"}
 dynamic = ["version"]
 
 [project.optional-dependencies]
 local = ["lambdaprompt[local]"]
```

### Comparing `sketch-0.4.1/sketch/core.py` & `sketch-0.4.2/sketch/core.py`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/sketch/metrics.py` & `sketch-0.4.2/sketch/metrics.py`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/sketch/pandas_extension.py` & `sketch-0.4.2/sketch/pandas_extension.py`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/sketch/references.py` & `sketch-0.4.2/sketch/references.py`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/sketch/sketches.py` & `sketch-0.4.2/sketch/sketches.py`

 * *Files identical despite different names*

### Comparing `sketch-0.4.1/sketch.egg-info/PKG-INFO` & `sketch-0.4.2/sketch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketch
-Version: 0.4.1
+Version: 0.4.2
 Summary: Compute, store and operate on data sketches
 License: MIT License
         
         Copyright (c) 2023 Justin Waugh, Mike Biven
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `sketch-0.4.1/tests/test_pandas_extension.py` & `sketch-0.4.2/tests/test_pandas_extension.py`

 * *Files identical despite different names*

