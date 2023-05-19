# Comparing `tmp/openlm-0.0.2.tar.gz` & `tmp/openlm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlm-0.0.2.tar", max compression
+gzip compressed data, was "openlm-0.0.3.tar", max compression
```

## Comparing `openlm-0.0.2.tar` & `openlm-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-05-08 15:56:49.714425 openlm-0.0.2/LICENSE
--rw-r--r--   0        0        0     1518 2023-05-08 22:18:45.011135 openlm-0.0.2/README.md
--rw-r--r--   0        0        0      132 2023-05-08 21:54:25.618285 openlm-0.0.2/openlm/__init__.py
--rw-r--r--   0        0        0      119 2023-05-08 19:53:27.996546 openlm-0.0.2/openlm/llm/__init__.py
--rw-r--r--   0        0        0     1472 2023-05-08 18:39:43.818023 openlm-0.0.2/openlm/llm/base.py
--rw-r--r--   0        0        0     3051 2023-05-08 22:27:11.789761 openlm-0.0.2/openlm/llm/cohere.py
--rw-r--r--   0        0        0     3526 2023-05-08 22:27:16.866957 openlm-0.0.2/openlm/llm/huggingface.py
--rw-r--r--   0        0        0     3374 2023-05-08 22:25:22.904394 openlm-0.0.2/openlm/llm/openai.py
--rw-r--r--   0        0        0     7734 2023-05-08 22:26:26.647266 openlm-0.0.2/openlm/openlm.py
--rw-r--r--   0        0        0     1174 2023-05-08 22:27:44.245701 openlm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 openlm-0.0.2/setup.py
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 openlm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 15:56:49.714425 openlm-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5054 2023-05-09 01:15:21.729839 openlm-0.0.3/README.md
+-rw-r--r--   0        0        0      132 2023-05-08 21:54:25.618285 openlm-0.0.3/openlm/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-08 19:53:27.996546 openlm-0.0.3/openlm/llm/__init__.py
+-rw-r--r--   0        0        0     1472 2023-05-08 18:39:43.818023 openlm-0.0.3/openlm/llm/base.py
+-rw-r--r--   0        0        0     3051 2023-05-08 22:27:11.789761 openlm-0.0.3/openlm/llm/cohere.py
+-rw-r--r--   0        0        0     3876 2023-05-19 15:25:08.749904 openlm-0.0.3/openlm/llm/huggingface.py
+-rw-r--r--   0        0        0     3374 2023-05-08 22:25:22.904394 openlm-0.0.3/openlm/llm/openai.py
+-rw-r--r--   0        0        0     7734 2023-05-08 22:26:26.647266 openlm-0.0.3/openlm/openlm.py
+-rw-r--r--   0        0        0     1181 2023-05-19 15:35:29.657555 openlm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6382 1970-01-01 00:00:00.000000 openlm-0.0.3/PKG-INFO
```

### Comparing `openlm-0.0.2/LICENSE` & `openlm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openlm-0.0.2/openlm/llm/base.py` & `openlm-0.0.3/openlm/llm/base.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.2/openlm/llm/cohere.py` & `openlm-0.0.3/openlm/llm/cohere.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.2/openlm/llm/huggingface.py` & `openlm-0.0.3/openlm/llm/huggingface.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from typing import Any, Dict, List, Optional, Union
 import json
 import requests
 
 hf_models = [
     'gpt2',
     'distilgpt2',
+    'gpt2-large',
+    'gpt2-medium',
+    'gpt2-xl',
 
     'bigscience/bloom-560m',
     'bigscience/bloom-1b',
     'bigscience/bloom-3b',
     'bigscience/bloom-7b1',
 
     'decapoda-research/llama-7b-hf',
@@ -38,14 +41,30 @@
     'bigcode/santacoder',
     
     'Salesforce/codegen-350M-multi',
     'Salesforce/codegen-2b-multi',
     
     'stabilityai/stablelm-tuned-alpha-3b',
     'stabilityai/stablelm-tuned-alpha-7b',
+
+    'facebook/opt-125m',
+    'facebook/opt-350m',
+    'facebook/opt-1.3b',
+    'facebook/opt-2.7b',
+    'facebook/opt-6.7b',
+    'facebook/opt-13b',
+    'facebook/opt-30b',
+
+    'mosaicml/mpt-7b',
+    'mosaicml/mpt-7b-instruct',
+    
+    'databricks/dolly-v2-7b',
+    'databricks/dolly-v2-12b',
+
+
 ]
 
 class Huggingface(BaseModel):
     def __init__(self,
                  api_key = os.environ.get("HF_API_TOKEN"),
                  model_list = hf_models,
                  namespace = 'huggingface.co',
```

### Comparing `openlm-0.0.2/openlm/llm/openai.py` & `openlm-0.0.3/openlm/llm/openai.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.2/openlm/openlm.py` & `openlm-0.0.3/openlm/openlm.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.2/pyproject.toml` & `openlm-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlm"
-version = "0.0.2"
+version = "0.0.3"
 description = "Drop-in OpenAI-compatible that can call LLMs from other providers"
 authors = ["Matt Rickard <pypi@matt-rickard.com>"]
 maintainers = ["Matt Rickard <pypi@matt-rickard.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = [
   "llm",
@@ -28,14 +28,14 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Linguistic",
 ]
 urls = { repository = "https://github.com/r2d4/openlm" }
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.8.1,<4.0"
 requests = "^2.30.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

