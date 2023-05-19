# Comparing `tmp/openlm-0.0.3.tar.gz` & `tmp/openlm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlm-0.0.3.tar", max compression
+gzip compressed data, was "openlm-0.0.4.tar", max compression
```

## Comparing `openlm-0.0.3.tar` & `openlm-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-05-08 15:56:49.714425 openlm-0.0.3/LICENSE
--rw-r--r--   0        0        0     5054 2023-05-09 01:15:21.729839 openlm-0.0.3/README.md
--rw-r--r--   0        0        0      132 2023-05-08 21:54:25.618285 openlm-0.0.3/openlm/__init__.py
--rw-r--r--   0        0        0      119 2023-05-08 19:53:27.996546 openlm-0.0.3/openlm/llm/__init__.py
--rw-r--r--   0        0        0     1472 2023-05-08 18:39:43.818023 openlm-0.0.3/openlm/llm/base.py
--rw-r--r--   0        0        0     3051 2023-05-08 22:27:11.789761 openlm-0.0.3/openlm/llm/cohere.py
--rw-r--r--   0        0        0     3876 2023-05-19 15:25:08.749904 openlm-0.0.3/openlm/llm/huggingface.py
--rw-r--r--   0        0        0     3374 2023-05-08 22:25:22.904394 openlm-0.0.3/openlm/llm/openai.py
--rw-r--r--   0        0        0     7734 2023-05-08 22:26:26.647266 openlm-0.0.3/openlm/openlm.py
--rw-r--r--   0        0        0     1181 2023-05-19 15:35:29.657555 openlm-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6382 1970-01-01 00:00:00.000000 openlm-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 15:56:49.714425 openlm-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5054 2023-05-09 01:15:21.729839 openlm-0.0.4/README.md
+-rw-r--r--   0        0        0      132 2023-05-08 21:54:25.618285 openlm-0.0.4/openlm/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-08 19:53:27.996546 openlm-0.0.4/openlm/llm/__init__.py
+-rw-r--r--   0        0        0     1472 2023-05-08 18:39:43.818023 openlm-0.0.4/openlm/llm/base.py
+-rw-r--r--   0        0        0     3051 2023-05-08 22:27:11.789761 openlm-0.0.4/openlm/llm/cohere.py
+-rw-r--r--   0        0        0     3876 2023-05-19 15:25:08.749904 openlm-0.0.4/openlm/llm/huggingface.py
+-rw-r--r--   0        0        0     3374 2023-05-08 22:25:22.904394 openlm-0.0.4/openlm/llm/openai.py
+-rw-r--r--   0        0        0     7734 2023-05-08 22:26:26.647266 openlm-0.0.4/openlm/openlm.py
+-rw-r--r--   0        0        0     1176 2023-05-19 15:49:24.673960 openlm-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 openlm-0.0.4/PKG-INFO
```

### Comparing `openlm-0.0.3/LICENSE` & `openlm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openlm-0.0.3/README.md` & `openlm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `openlm-0.0.3/openlm/llm/base.py` & `openlm-0.0.4/openlm/llm/base.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.3/openlm/llm/cohere.py` & `openlm-0.0.4/openlm/llm/cohere.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.3/openlm/llm/huggingface.py` & `openlm-0.0.4/openlm/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.3/openlm/llm/openai.py` & `openlm-0.0.4/openlm/llm/openai.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.3/openlm/openlm.py` & `openlm-0.0.4/openlm/openlm.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.3/pyproject.toml` & `openlm-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlm"
-version = "0.0.3"
+version = "0.0.4"
 description = "Drop-in OpenAI-compatible that can call LLMs from other providers"
 authors = ["Matt Rickard <pypi@matt-rickard.com>"]
 maintainers = ["Matt Rickard <pypi@matt-rickard.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = [
   "llm",
@@ -29,13 +29,13 @@
     "Topic :: Text Processing :: Linguistic",
 ]
 urls = { repository = "https://github.com/r2d4/openlm" }
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-requests = "^2.30.0"
+requests = "^2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openlm-0.0.3/PKG-INFO` & `openlm-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Drop-in OpenAI-compatible that can call LLMs from other providers
 License: MIT
 Keywords: llm,ai,prompt,large language models,gpt-3,chatgpt
 Author: Matt Rickard
 Author-email: pypi@matt-rickard.com
 Maintainer: Matt Rickard
 Maintainer-email: pypi@matt-rickard.com
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: requests (>=2,<3)
 Project-URL: repository, https://github.com/r2d4/openlm
 Description-Content-Type: text/markdown
 
 # OpenLM
 
 Drop-in OpenAI-compatible library that can call LLMs from other providers (e.g., HuggingFace, Cohere, and more).
```

