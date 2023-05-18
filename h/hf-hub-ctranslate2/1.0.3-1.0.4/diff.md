# Comparing `tmp/hf_hub_ctranslate2-1.0.3.tar.gz` & `tmp/hf_hub_ctranslate2-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-1.0.3.tar", last modified: Sat May 13 21:12:44 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-1.0.4.tar", last modified: Thu May 18 22:34:55 2023, max compression
```

## Comparing `hf_hub_ctranslate2-1.0.3.tar` & `hf_hub_ctranslate2-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:12:44.740648 hf_hub_ctranslate2-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-13 21:12:30.000000 hf_hub_ctranslate2-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-13 21:12:44.740648 hf_hub_ctranslate2-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-13 21:12:30.000000 hf_hub_ctranslate2-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:12:44.740648 hf_hub_ctranslate2-1.0.3/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-13 21:12:44.000000 hf_hub_ctranslate2-1.0.3/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-13 21:12:44.000000 hf_hub_ctranslate2-1.0.3/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 21:12:44.000000 hf_hub_ctranslate2-1.0.3/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-13 21:12:44.000000 hf_hub_ctranslate2-1.0.3/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 21:12:44.000000 hf_hub_ctranslate2-1.0.3/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-13 21:12:30.000000 hf_hub_ctranslate2-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 21:12:44.740648 hf_hub_ctranslate2-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-13 21:12:30.000000 hf_hub_ctranslate2-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:12:44.740648 hf_hub_ctranslate2-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-13 21:12:30.000000 hf_hub_ctranslate2-1.0.3/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-13 21:12:30.000000 hf_hub_ctranslate2-1.0.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:34:55.451240 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 22:34:55.000000 hf_hub_ctranslate2-1.0.4/hf_hub_ctranslate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:34:55.455241 hf_hub_ctranslate2-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 22:34:45.000000 hf_hub_ctranslate2-1.0.4/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-1.0.3/LICENSE` & `hf_hub_ctranslate2-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-1.0.3/PKG-INFO` & `hf_hub_ctranslate2-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: hf_hub_ctranslate2
-Version: 1.0.3
-Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
-Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
-Author: Michael Feil
-License: MIT
-Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 hf_hub_ctranslate2
 ==============================
 
 Connecting Transfromers on HuggingfaceHub with Ctranslate2 - a small utility for keeping tokenizer and model around Huggingface Hub.
 
 [![codecov](https://codecov.io/gh/michaelfeil/hf-hub-ctranslate2/branch/main/graph/badge.svg?token=U9VIEFEELS)](https://codecov.io/gh/michaelfeil/hf-hub-ctranslate2)![CI pytest](https://github.com/michaelfeil/hf-hub-ctranslate2/actions/workflows/test_release.yml/badge.svg)
 
@@ -27,28 +13,31 @@
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 --------
 ## Usage:
+#### Decoder-only Transformer:
 ```python
 # download ctranslate.Generator repos from Huggingface Hub (GPT-J, ..)
 from hf_hub_ctranslate2 import TranslatorCT2fromHfHub, GeneratorCT2fromHfHub
 
 model_name_1="michaelfeil/ct2fast-pythia-160m"
 model = GeneratorCT2fromHfHub(
     # load in int8 on CPU
     model_name_or_path=model_name_1, device="cpu", compute_type="int8"
 )
 outputs = model.generate(
     text=["How do you call a fast Flan-ingo?", "User: How are you doing?"]
     # add arguments specifically to ctranslate2.Generator here
 )
-
+```
+#### Encoder-Decoder:
+```python
 # download ctranslate.Translator repos from Huggingface Hub (T5, ..)
 model_name_2 = "michaelfeil/ct2fast-flan-alpaca-base"
 model = TranslatorCT2fromHfHub(
         # load in int8 on CUDA
         model_name_or_path=model_name_2, device="cuda", compute_type="int8_float16"
 )
 outputs = model.generate(
@@ -57,14 +46,27 @@
     min_decoding_length=8,
     max_decoding_length=16,
     max_input_length=512,
     beam_size=3
 )
 print(outputs)
 ```
+#### Encoder-Decoder for multilingual translations (m2m-100):
+```python
+model = MultiLingualTranslatorCT2fromHfHub(
+    model_name_or_path="michaelfeil/ct2fast-m2m100_418M", device="cpu", compute_type="int8",
+    tokenizer=AutoTokenizer.from_pretrained(f"facebook/m2m100_418M")
+)
+
+outputs = model.generate(
+    ["How do you call a fast Flamingo?", "Wie geht es dir?"],
+    src_lang=["en", "de"],
+    tgt_lang=["de", "fr"]
+)
+```
 
 --------
 ## PYPI Install
 ```bash
 pip install hf-hub-ctranslate2
 ```
 --------
```

### Comparing `hf_hub_ctranslate2-1.0.3/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hf-hub-ctranslate2
-Version: 1.0.3
+Name: hf_hub_ctranslate2
+Version: 1.0.4
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -27,28 +27,31 @@
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 --------
 ## Usage:
+#### Decoder-only Transformer:
 ```python
 # download ctranslate.Generator repos from Huggingface Hub (GPT-J, ..)
 from hf_hub_ctranslate2 import TranslatorCT2fromHfHub, GeneratorCT2fromHfHub
 
 model_name_1="michaelfeil/ct2fast-pythia-160m"
 model = GeneratorCT2fromHfHub(
     # load in int8 on CPU
     model_name_or_path=model_name_1, device="cpu", compute_type="int8"
 )
 outputs = model.generate(
     text=["How do you call a fast Flan-ingo?", "User: How are you doing?"]
     # add arguments specifically to ctranslate2.Generator here
 )
-
+```
+#### Encoder-Decoder:
+```python
 # download ctranslate.Translator repos from Huggingface Hub (T5, ..)
 model_name_2 = "michaelfeil/ct2fast-flan-alpaca-base"
 model = TranslatorCT2fromHfHub(
         # load in int8 on CUDA
         model_name_or_path=model_name_2, device="cuda", compute_type="int8_float16"
 )
 outputs = model.generate(
@@ -57,14 +60,27 @@
     min_decoding_length=8,
     max_decoding_length=16,
     max_input_length=512,
     beam_size=3
 )
 print(outputs)
 ```
+#### Encoder-Decoder for multilingual translations (m2m-100):
+```python
+model = MultiLingualTranslatorCT2fromHfHub(
+    model_name_or_path="michaelfeil/ct2fast-m2m100_418M", device="cpu", compute_type="int8",
+    tokenizer=AutoTokenizer.from_pretrained(f"facebook/m2m100_418M")
+)
+
+outputs = model.generate(
+    ["How do you call a fast Flamingo?", "Wie geht es dir?"],
+    src_lang=["en", "de"],
+    tgt_lang=["de", "fr"]
+)
+```
 
 --------
 ## PYPI Install
 ```bash
 pip install hf-hub-ctranslate2
 ```
 --------
```

### Comparing `hf_hub_ctranslate2-1.0.3/setup.py` & `hf_hub_ctranslate2-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             break
 if len(version.split(".")) != 3:
     raise ValueError(f"Version incorrect: {version}")
 
 
 setup(
     name="hf_hub_ctranslate2",
-    packages=find_packages(include="hf_hub_ctranslate2"),
+    packages=["hf_hub_ctranslate2"],
     version=version,
     description=("Connecting Transfromers on HuggingfaceHub with Ctranslate2 "),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Michael Feil",
     license="MIT",
     url="https://github.com/michaelfeil/hf-hub-ctranslate2",
```

### Comparing `hf_hub_ctranslate2-1.0.3/tests/test_translate.py` & `hf_hub_ctranslate2-1.0.4/tests/test_translate.py`

 * *Files identical despite different names*

