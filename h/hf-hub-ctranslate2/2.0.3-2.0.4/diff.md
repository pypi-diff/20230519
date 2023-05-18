# Comparing `tmp/hf_hub_ctranslate2-2.0.3.tar.gz` & `tmp/hf_hub_ctranslate2-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-2.0.3.tar", last modified: Thu May 18 23:19:33 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-2.0.4.tar", last modified: Thu May 18 23:39:07 2023, max compression
```

## Comparing `hf_hub_ctranslate2-2.0.3.tar` & `hf_hub_ctranslate2-2.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:19:33.156879 hf_hub_ctranslate2-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 23:19:22.000000 hf_hub_ctranslate2-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:19:33.156879 hf_hub_ctranslate2-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 23:19:22.000000 hf_hub_ctranslate2-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:19:33.152879 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-18 23:19:22.000000 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-18 23:19:22.000000 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:19:33.152879 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:19:33.000000 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-18 23:19:33.000000 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:19:33.000000 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 23:19:33.000000 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 23:19:33.000000 hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 23:19:22.000000 hf_hub_ctranslate2-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:19:33.156879 hf_hub_ctranslate2-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 23:19:22.000000 hf_hub_ctranslate2-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:19:33.156879 hf_hub_ctranslate2-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-18 23:19:22.000000 hf_hub_ctranslate2-2.0.3/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 23:19:22.000000 hf_hub_ctranslate2-2.0.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 23:39:07.000000 hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:39:07.420043 hf_hub_ctranslate2-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 23:38:58.000000 hf_hub_ctranslate2-2.0.4/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-2.0.3/LICENSE` & `hf_hub_ctranslate2-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.3/PKG-INFO` & `hf_hub_ctranslate2-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf_hub_ctranslate2
-Version: 2.0.3
+Version: 2.0.4
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.3/README.md` & `hf_hub_ctranslate2-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2/translate.py` & `hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2/translate.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from typing import Any, Union, List
 import os
 
-from ._private import download_model as _download_model
+from hf_hub_ctranslate2.util import _download_model
 
 
 class CTranslate2ModelfromHuggingfaceHub:
     """CTranslate2 compatibility class for Translator and Generator"""
 
     def __init__(
         self,
```

### Comparing `hf_hub_ctranslate2-2.0.3/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-2.0.4/hf_hub_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-hub-ctranslate2
-Version: 2.0.3
+Version: 2.0.4
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.3/setup.py` & `hf_hub_ctranslate2-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.3/tests/test_translate.py` & `hf_hub_ctranslate2-2.0.4/tests/test_translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from hf_hub_ctranslate2 import TranslatorCT2fromHfHub, GeneratorCT2fromHfHub, MultiLingualTranslatorCT2fromHfHub
-import hf_hub_ctranslate2._private.utils as utils
+from hf_hub_ctranslate2.util import _download_model
 from transformers import AutoTokenizer
 
 
 def test_translator(model_name="michaelfeil/ct2fast-flan-alpaca-base"):
     model = TranslatorCT2fromHfHub(
         model_name_or_path=model_name, device="cpu", compute_type="int8"
     )
@@ -47,15 +47,15 @@
     assert len(outputs[0]) != len(outputs[1])
     assert "flan" in outputs[0].lower()
     for o in outputs:
         assert isinstance(o, str)
 
 
 def test_generator_single(model_name="michaelfeil/ct2fast-pythia-160m"):
-    model_path = utils.download_model(model_name)
+    model_path = _download_model(model_name)
     tokenizer = AutoTokenizer.from_pretrained(model_path)
 
     model = GeneratorCT2fromHfHub(
         model_name_or_path=model_path,
         device="cpu",
         compute_type="int8",
         tokenizer=tokenizer,
```

