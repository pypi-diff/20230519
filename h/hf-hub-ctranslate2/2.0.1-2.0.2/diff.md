# Comparing `tmp/hf_hub_ctranslate2-2.0.1.tar.gz` & `tmp/hf_hub_ctranslate2-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-2.0.1.tar", last modified: Thu May 18 22:57:19 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-2.0.2.tar", last modified: Thu May 18 23:09:02 2023, max compression
```

## Comparing `hf_hub_ctranslate2-2.0.1.tar` & `hf_hub_ctranslate2-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:57:19.873623 hf_hub_ctranslate2-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 22:57:11.000000 hf_hub_ctranslate2-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 22:57:19.873623 hf_hub_ctranslate2-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 22:57:11.000000 hf_hub_ctranslate2-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:57:19.869623 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-18 22:57:11.000000 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-18 22:57:11.000000 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:57:19.869623 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 22:57:19.000000 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-18 22:57:19.000000 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:57:19.000000 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 22:57:19.000000 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 22:57:19.000000 hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 22:57:11.000000 hf_hub_ctranslate2-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:57:19.873623 hf_hub_ctranslate2-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 22:57:11.000000 hf_hub_ctranslate2-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:57:19.869623 hf_hub_ctranslate2-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-18 22:57:11.000000 hf_hub_ctranslate2-2.0.1/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 22:57:11.000000 hf_hub_ctranslate2-2.0.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:09:02.061629 hf_hub_ctranslate2-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 23:08:53.000000 hf_hub_ctranslate2-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:09:02.061629 hf_hub_ctranslate2-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 23:08:53.000000 hf_hub_ctranslate2-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:09:02.061629 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-18 23:08:53.000000 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-05-18 23:08:53.000000 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:09:02.061629 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:09:02.000000 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-18 23:09:02.000000 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:09:02.000000 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 23:09:02.000000 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 23:09:02.000000 hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 23:08:53.000000 hf_hub_ctranslate2-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:09:02.061629 hf_hub_ctranslate2-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 23:08:53.000000 hf_hub_ctranslate2-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:09:02.061629 hf_hub_ctranslate2-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-18 23:08:53.000000 hf_hub_ctranslate2-2.0.2/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 23:08:53.000000 hf_hub_ctranslate2-2.0.2/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-2.0.1/LICENSE` & `hf_hub_ctranslate2-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.1/PKG-INFO` & `hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hf_hub_ctranslate2
-Version: 2.0.1
+Name: hf-hub-ctranslate2
+Version: 2.0.2
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.1/README.md` & `hf_hub_ctranslate2-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2/translate.py` & `hf_hub_ctranslate2-2.0.2/hf_hub_ctranslate2/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from typing import Any, Union, List
 import os
 
-import hf_hub_ctranslate2._private.utils as utils
+import hf_hub_ctranslate2._private.utils as _utils
 
 
 class CTranslate2ModelfromHuggingfaceHub:
     """CTranslate2 compatibility class for Translator and Generator"""
 
     def __init__(
         self,
@@ -25,29 +25,33 @@
         hub_kwargs: dict = {},
     ):
         # adaptions from https://github.com/guillaumekln/faster-whisper
         if os.path.isdir(model_name_or_path):
             model_path = model_name_or_path
         else:
             try:
-                model_path = utils.download_model(model_name_or_path, hub_kwargs=hub_kwargs)
+                model_path = _utils.download_model(model_name_or_path, hub_kwargs=hub_kwargs)
             except:
                 hub_kwargs["local_files_only"] = True
-                model_path = utils.download_model(model_name_or_path, hub_kwargs=hub_kwargs)
+                model_path = _utils.download_model(model_name_or_path, hub_kwargs=hub_kwargs)
         self.model = self.ctranslate_class(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
         )
 
-        if tokenizer is None:
-            self.tokenizer = AutoTokenizer.from_pretrained(model_path, fast=True)
-        else:
+        if tokenizer is not None:
             self.tokenizer = tokenizer
+        else:
+            if "tokenizer.json" in os.listdir(model_path):
+                self.tokenizer = AutoTokenizer.from_pretrained(model_path, fast=True)
+            if "tokenizer.json" in os.listdir(model_path):
+                self.tokenizer = AutoTokenizer.from_pretrained(model_path, fast=True)
+                
 
     def _forward(self, *args: Any, **kwds: Any) -> Any:
         raise NotImplementedError
     
     def tokenize_encode(self, text, *args, **kwargs):
         return [
             self.tokenizer.convert_ids_to_tokens(self.tokenizer.encode(p)) for p in text
```

### Comparing `hf_hub_ctranslate2-2.0.1/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hf-hub-ctranslate2
-Version: 2.0.1
+Name: hf_hub_ctranslate2
+Version: 2.0.2
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.1/setup.py` & `hf_hub_ctranslate2-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.1/tests/test_translate.py` & `hf_hub_ctranslate2-2.0.2/tests/test_translate.py`

 * *Files identical despite different names*

