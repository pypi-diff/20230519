# Comparing `tmp/hf_hub_ctranslate2-1.0.4.tar.gz` & `tmp/hf_hub_ctranslate2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-1.0.4.tar", last modified: Thu May 18 22:34:55 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-2.0.0.tar", last modified: Thu May 18 22:47:31 2023, max compression
```

## Comparing `hf_hub_ctranslate2-1.0.4.tar` & `hf_hub_ctranslate2-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:34:55.451240 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:47:31.925488 hf_hub_ctranslate2-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 22:47:23.000000 hf_hub_ctranslate2-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 22:47:31.925488 hf_hub_ctranslate2-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 22:47:23.000000 hf_hub_ctranslate2-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:47:31.921487 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-18 22:47:23.000000 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-05-18 22:47:23.000000 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:47:31.925488 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 22:47:31.000000 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-18 22:47:31.000000 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:47:31.000000 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 22:47:31.000000 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 22:47:31.000000 hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 22:47:23.000000 hf_hub_ctranslate2-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:47:31.925488 hf_hub_ctranslate2-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 22:47:23.000000 hf_hub_ctranslate2-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:47:31.925488 hf_hub_ctranslate2-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-18 22:47:23.000000 hf_hub_ctranslate2-2.0.0/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 22:47:23.000000 hf_hub_ctranslate2-2.0.0/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-1.0.4/LICENSE` & `hf_hub_ctranslate2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-1.0.4/PKG-INFO` & `hf_hub_ctranslate2-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf_hub_ctranslate2
-Version: 1.0.4
+Version: 2.0.0
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-1.0.4/README.md` & `hf_hub_ctranslate2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2/translate.py` & `hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2/translate.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-2.0.0/hf_hub_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-hub-ctranslate2
-Version: 1.0.4
+Version: 2.0.0
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-1.0.4/setup.py` & `hf_hub_ctranslate2-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-1.0.4/tests/test_translate.py` & `hf_hub_ctranslate2-2.0.0/tests/test_translate.py`

 * *Files identical despite different names*

