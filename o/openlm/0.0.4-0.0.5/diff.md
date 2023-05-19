# Comparing `tmp/openlm-0.0.4.tar.gz` & `tmp/openlm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlm-0.0.4.tar", max compression
+gzip compressed data, was "openlm-0.0.5.tar", max compression
```

## Comparing `openlm-0.0.4.tar` & `openlm-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-05-08 15:56:49.714425 openlm-0.0.4/LICENSE
--rw-r--r--   0        0        0     5054 2023-05-09 01:15:21.729839 openlm-0.0.4/README.md
--rw-r--r--   0        0        0      132 2023-05-08 21:54:25.618285 openlm-0.0.4/openlm/__init__.py
--rw-r--r--   0        0        0      119 2023-05-08 19:53:27.996546 openlm-0.0.4/openlm/llm/__init__.py
--rw-r--r--   0        0        0     1472 2023-05-08 18:39:43.818023 openlm-0.0.4/openlm/llm/base.py
--rw-r--r--   0        0        0     3051 2023-05-08 22:27:11.789761 openlm-0.0.4/openlm/llm/cohere.py
--rw-r--r--   0        0        0     3876 2023-05-19 15:25:08.749904 openlm-0.0.4/openlm/llm/huggingface.py
--rw-r--r--   0        0        0     3374 2023-05-08 22:25:22.904394 openlm-0.0.4/openlm/llm/openai.py
--rw-r--r--   0        0        0     7734 2023-05-08 22:26:26.647266 openlm-0.0.4/openlm/openlm.py
--rw-r--r--   0        0        0     1176 2023-05-19 15:49:24.673960 openlm-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 openlm-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 15:56:49.714425 openlm-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5054 2023-05-09 01:15:21.729839 openlm-0.0.5/README.md
+-rw-r--r--   0        0        0      132 2023-05-08 21:54:25.618285 openlm-0.0.5/openlm/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-08 19:53:27.996546 openlm-0.0.5/openlm/llm/__init__.py
+-rw-r--r--   0        0        0     1472 2023-05-19 16:41:33.933694 openlm-0.0.5/openlm/llm/base.py
+-rw-r--r--   0        0        0     3051 2023-05-08 22:27:11.789761 openlm-0.0.5/openlm/llm/cohere.py
+-rw-r--r--   0        0        0     3876 2023-05-19 15:25:08.749904 openlm-0.0.5/openlm/llm/huggingface.py
+-rw-r--r--   0        0        0     3374 2023-05-19 16:23:16.635132 openlm-0.0.5/openlm/llm/openai.py
+-rw-r--r--   0        0        0     7785 2023-05-19 16:40:52.825662 openlm-0.0.5/openlm/openlm.py
+-rw-r--r--   0        0        0     1176 2023-05-19 16:42:06.457673 openlm-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 openlm-0.0.5/PKG-INFO
```

### Comparing `openlm-0.0.4/LICENSE` & `openlm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openlm-0.0.4/README.md` & `openlm-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `openlm-0.0.4/openlm/llm/base.py` & `openlm-0.0.5/openlm/llm/base.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.4/openlm/llm/cohere.py` & `openlm-0.0.5/openlm/llm/cohere.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.4/openlm/llm/huggingface.py` & `openlm-0.0.5/openlm/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.4/openlm/llm/openai.py` & `openlm-0.0.5/openlm/llm/openai.py`

 * *Files identical despite different names*

### Comparing `openlm-0.0.4/openlm/openlm.py` & `openlm-0.0.5/openlm/openlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
                                 echo: Optional[bool] = None,
                                 stop: Optional[Union[str, List[str]]] = None,
                                 presence_penalty: Optional[float] = None,
                                 frequency_penalty: Optional[float] = None,
                                 best_of: Optional[int] = None,
                                 logit_bias: Optional[Dict[str, float]] = None,
                                 user: Optional[str] = None,
-                                api_keys: Optional[Dict[str, str]] = None) -> Dict[str, Any]:
+                                api_keys: Optional[Dict[str, str]] = None,
+                                request_timeout=0) -> Dict[str, Any]:
         """
         Creates a completion request for the OpenAI API.
 
         :param model: The ID(s) of the model to use.
         :param prompt: The prompt(s) to generate completions for.
         :param suffix: A string to append to the completion(s).
         :param max_tokens: The maximum number of tokens to generate in the completion(s).
```

### Comparing `openlm-0.0.4/pyproject.toml` & `openlm-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlm"
-version = "0.0.4"
+version = "0.0.5"
 description = "Drop-in OpenAI-compatible that can call LLMs from other providers"
 authors = ["Matt Rickard <pypi@matt-rickard.com>"]
 maintainers = ["Matt Rickard <pypi@matt-rickard.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = [
   "llm",
```

### Comparing `openlm-0.0.4/PKG-INFO` & `openlm-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Drop-in OpenAI-compatible that can call LLMs from other providers
 License: MIT
 Keywords: llm,ai,prompt,large language models,gpt-3,chatgpt
 Author: Matt Rickard
 Author-email: pypi@matt-rickard.com
 Maintainer: Matt Rickard
 Maintainer-email: pypi@matt-rickard.com
```

