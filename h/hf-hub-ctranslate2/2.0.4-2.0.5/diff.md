# Comparing `tmp/hf_hub_ctranslate2-2.0.4.tar.gz` & `tmp/hf_hub_ctranslate2-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-2.0.4.tar", last modified: Thu May 18 23:39:07 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-2.0.5.tar", last modified: Thu May 18 23:47:47 2023, max compression
```

## Comparing `hf_hub_ctranslate2-2.0.4.tar` & `hf_hub_ctranslate2-2.0.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:47:47.727764 hf_hub_ctranslate2-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 23:47:38.000000 hf_hub_ctranslate2-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:47:47.727764 hf_hub_ctranslate2-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 23:47:38.000000 hf_hub_ctranslate2-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:47:47.723764 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:47:47.727764 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:47:47.000000 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-18 23:47:47.000000 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:47:47.000000 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 23:47:47.000000 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 23:47:47.000000 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/hf_hub_ctranslate2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:47:47.727764 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-18 23:47:38.000000 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-18 23:47:38.000000 hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 23:47:38.000000 hf_hub_ctranslate2-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:47:47.727764 hf_hub_ctranslate2-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-18 23:47:38.000000 hf_hub_ctranslate2-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:47:47.727764 hf_hub_ctranslate2-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-18 23:47:38.000000 hf_hub_ctranslate2-2.0.5/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 23:47:38.000000 hf_hub_ctranslate2-2.0.5/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-2.0.4/LICENSE` & `hf_hub_ctranslate2-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.4/PKG-INFO` & `hf_hub_ctranslate2-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf_hub_ctranslate2
-Version: 2.0.4
+Version: 2.0.5
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.4/README.md` & `hf_hub_ctranslate2-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-2.0.5/hf_hub_ctranslate2/hf_hub_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-hub-ctranslate2
-Version: 2.0.4
+Version: 2.0.5
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.4/setup.py` & `hf_hub_ctranslate2-2.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,18 @@
             break
 if len(version.split(".")) != 3:
     raise ValueError(f"Version incorrect: {version}")
 
 
 setup(
     name="hf_hub_ctranslate2",
-    packages=["hf_hub_ctranslate2"],
+    packages=find_packages(where="hf_hub_ctranslate2"),
+    package_dir={
+        '': 'hf_hub_ctranslate2',
+    },
     version=version,
     description=("Connecting Transfromers on HuggingfaceHub with Ctranslate2 "),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Michael Feil",
     license="MIT",
     url="https://github.com/michaelfeil/hf-hub-ctranslate2",
```

### Comparing `hf_hub_ctranslate2-2.0.4/tests/test_translate.py` & `hf_hub_ctranslate2-2.0.5/tests/test_translate.py`

 * *Files identical despite different names*

