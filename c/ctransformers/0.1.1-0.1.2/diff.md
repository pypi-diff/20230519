# Comparing `tmp/ctransformers-0.1.1.tar.gz` & `tmp/ctransformers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctransformers-0.1.1.tar", last modified: Thu May 18 20:26:08 2023, max compression
+gzip compressed data, was "ctransformers-0.1.2.tar", last modified: Fri May 19 21:44:18 2023, max compression
```

## Comparing `ctransformers-0.1.1.tar` & `ctransformers-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.126294 ctransformers-0.1.1/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    16975 2023-05-18 20:26:08.126294 ctransformers-0.1.1/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    12435 2023-05-18 20:14:09.000000 ctransformers-0.1.1/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.106294 ctransformers-0.1.1/ctransformers/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.1.1/ctransformers/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5875 2023-05-18 15:44:53.000000 ctransformers-0.1.1/ctransformers/hub.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1759 2023-05-17 19:24:39.000000 ctransformers-0.1.1/ctransformers/langchain.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.106294 ctransformers-0.1.1/ctransformers/lib/
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.116294 ctransformers-0.1.1/ctransformers/lib/avx/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   402432 2023-05-17 20:01:06.000000 ctransformers-0.1.1/ctransformers/lib/avx/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   905907 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/avx/libctransformers.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   545536 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/avx/libctransformers.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.116294 ctransformers-0.1.1/ctransformers/lib/avx2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   388608 2023-05-17 20:01:06.000000 ctransformers-0.1.1/ctransformers/lib/avx2/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   905907 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/avx2/libctransformers.dylib
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   545536 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/avx2/libctransformers.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.126294 ctransformers-0.1.1/ctransformers/lib/basic/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   394752 2023-05-17 20:01:06.000000 ctransformers-0.1.1/ctransformers/lib/basic/ctransformers.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   889523 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/basic/libctransformers.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   512768 2023-05-14 22:26:24.000000 ctransformers-0.1.1/ctransformers/lib/basic/libctransformers.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1033 2023-05-12 14:01:41.000000 ctransformers-0.1.1/ctransformers/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13074 2023-05-18 20:09:31.000000 ctransformers-0.1.1/ctransformers/llm.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-18 20:26:08.106294 ctransformers-0.1.1/ctransformers.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    16975 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      744 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-18 20:26:08.000000 ctransformers-0.1.1/ctransformers.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-18 20:26:08.126294 ctransformers-0.1.1/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1451 2023-05-18 20:21:47.000000 ctransformers-0.1.1/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-19 21:44:18.413481 ctransformers-0.1.2/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    17255 2023-05-19 21:44:18.413481 ctransformers-0.1.2/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    12691 2023-05-19 21:31:10.000000 ctransformers-0.1.2/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-19 21:44:18.383481 ctransformers-0.1.2/ctransformers/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.1.2/ctransformers/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5866 2023-05-19 19:43:30.000000 ctransformers-0.1.2/ctransformers/hub.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2616 2023-05-19 21:43:11.000000 ctransformers-0.1.2/ctransformers/langchain.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-19 21:44:18.383481 ctransformers-0.1.2/ctransformers/lib/
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-19 21:44:18.393481 ctransformers-0.1.2/ctransformers/lib/avx/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   402432 2023-05-17 20:01:06.000000 ctransformers-0.1.2/ctransformers/lib/avx/ctransformers.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   905907 2023-05-14 22:26:24.000000 ctransformers-0.1.2/ctransformers/lib/avx/libctransformers.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   545536 2023-05-14 22:26:24.000000 ctransformers-0.1.2/ctransformers/lib/avx/libctransformers.so
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-19 21:44:18.403481 ctransformers-0.1.2/ctransformers/lib/avx2/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   388608 2023-05-17 20:01:06.000000 ctransformers-0.1.2/ctransformers/lib/avx2/ctransformers.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   905907 2023-05-14 22:26:24.000000 ctransformers-0.1.2/ctransformers/lib/avx2/libctransformers.dylib
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)   545536 2023-05-14 22:26:24.000000 ctransformers-0.1.2/ctransformers/lib/avx2/libctransformers.so
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-19 21:44:18.403481 ctransformers-0.1.2/ctransformers/lib/basic/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   394752 2023-05-17 20:01:06.000000 ctransformers-0.1.2/ctransformers/lib/basic/ctransformers.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   889523 2023-05-14 22:26:24.000000 ctransformers-0.1.2/ctransformers/lib/basic/libctransformers.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   512768 2023-05-14 22:26:24.000000 ctransformers-0.1.2/ctransformers/lib/basic/libctransformers.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1033 2023-05-12 14:01:41.000000 ctransformers-0.1.2/ctransformers/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13306 2023-05-19 21:04:15.000000 ctransformers-0.1.2/ctransformers/llm.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-19 21:44:18.383481 ctransformers-0.1.2/ctransformers.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    17255 2023-05-19 21:44:18.000000 ctransformers-0.1.2/ctransformers.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      744 2023-05-19 21:44:18.000000 ctransformers-0.1.2/ctransformers.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-19 21:44:18.000000 ctransformers-0.1.2/ctransformers.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-19 21:44:18.000000 ctransformers-0.1.2/ctransformers.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-19 21:44:18.000000 ctransformers-0.1.2/ctransformers.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-19 21:44:18.000000 ctransformers-0.1.2/ctransformers.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-19 21:44:18.413481 ctransformers-0.1.2/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1451 2023-05-19 21:35:27.000000 ctransformers-0.1.2/setup.py
```

### Comparing `ctransformers-0.1.1/PKG-INFO` & `ctransformers-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
@@ -158,31 +158,32 @@
         llm_chain = LLMChain(prompt=prompt, llm=llm)
         
         print(llm_chain.run('What is AI?'))
         ```
         
         ## Documentation
         
-        ### Parameters
+        <!-- API_DOCS -->
+        
+        ### Config
         
-        | Name                 | Type        | Description                                              | Default |
+        | Parameter            | Type        | Description                                              | Default |
         | :------------------- | :---------- | :------------------------------------------------------- | :------ |
         | `top_k`              | `int`       | The top-k value to use for sampling.                     | `40`    |
         | `top_p`              | `float`     | The top-p value to use for sampling.                     | `0.95`  |
         | `temperature`        | `float`     | The temperature to use for sampling.                     | `0.8`   |
         | `repetition_penalty` | `float`     | The repetition penalty to use for sampling.              | `1.0`   |
         | `last_n_tokens`      | `int`       | The number of last tokens to use for repetition penalty. | `64`    |
-        | `seed`               | `int`       | The seed value to use for sampling tokens.               | Random  |
+        | `seed`               | `int`       | The seed value to use for sampling tokens.               | `-1`    |
         | `max_new_tokens`     | `int`       | The maximum number of new tokens to generate.            | `256`   |
-        | `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `[]`    |
+        | `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `None`  |
+        | `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
         | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
         | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
-        | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | Auto    |
-        
-        <!-- API_DOCS -->
+        | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
         
         ### <kbd>class</kbd> `AutoModelForCausalLM`
         
         ---
         
         #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
         
@@ -410,16 +411,17 @@
             temperature: Optional[float] = None,
             repetition_penalty: Optional[float] = None,
             last_n_tokens: Optional[int] = None,
             seed: Optional[int] = None,
             batch_size: Optional[int] = None,
             threads: Optional[int] = None,
             stop: Optional[Sequence[str]] = None,
+            stream: Optional[bool] = None,
             reset: Optional[bool] = None
-        ) → str
+        ) → Union[str, Generator[str, NoneType, NoneType]]
         ```
         
         Generates text from a prompt.
         
         **Args:**
         
         - <b>`prompt`</b>: The prompt to generate text from.
@@ -429,14 +431,15 @@
         - <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
         - <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
         - <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
         - <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
         - <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
         - <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
         - <b>`stop`</b>: A list of sequences to stop generation when encountered. Default: `None`
+        - <b>`stream`</b>: Whether to stream the generated text. Default: `False`
         - <b>`reset`</b>: Whether to reset the model state before generating text. Default: `True`
         
         **Returns:**
         The generated text.
         
         <!-- API_DOCS -->
```

### Comparing `ctransformers-0.1.1/README.md` & `ctransformers-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -150,31 +150,32 @@
 llm_chain = LLMChain(prompt=prompt, llm=llm)
 
 print(llm_chain.run('What is AI?'))
 ```
 
 ## Documentation
 
-### Parameters
+<!-- API_DOCS -->
+
+### Config
 
-| Name                 | Type        | Description                                              | Default |
+| Parameter            | Type        | Description                                              | Default |
 | :------------------- | :---------- | :------------------------------------------------------- | :------ |
 | `top_k`              | `int`       | The top-k value to use for sampling.                     | `40`    |
 | `top_p`              | `float`     | The top-p value to use for sampling.                     | `0.95`  |
 | `temperature`        | `float`     | The temperature to use for sampling.                     | `0.8`   |
 | `repetition_penalty` | `float`     | The repetition penalty to use for sampling.              | `1.0`   |
 | `last_n_tokens`      | `int`       | The number of last tokens to use for repetition penalty. | `64`    |
-| `seed`               | `int`       | The seed value to use for sampling tokens.               | Random  |
+| `seed`               | `int`       | The seed value to use for sampling tokens.               | `-1`    |
 | `max_new_tokens`     | `int`       | The maximum number of new tokens to generate.            | `256`   |
-| `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `[]`    |
+| `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `None`  |
+| `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
 | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
 | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
-| `threads`            | `int`       | The number of threads to use for evaluating tokens.      | Auto    |
-
-<!-- API_DOCS -->
+| `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
 
 ### <kbd>class</kbd> `AutoModelForCausalLM`
 
 ---
 
 #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
 
@@ -402,16 +403,17 @@
     temperature: Optional[float] = None,
     repetition_penalty: Optional[float] = None,
     last_n_tokens: Optional[int] = None,
     seed: Optional[int] = None,
     batch_size: Optional[int] = None,
     threads: Optional[int] = None,
     stop: Optional[Sequence[str]] = None,
+    stream: Optional[bool] = None,
     reset: Optional[bool] = None
-) → str
+) → Union[str, Generator[str, NoneType, NoneType]]
 ```
 
 Generates text from a prompt.
 
 **Args:**
 
 - <b>`prompt`</b>: The prompt to generate text from.
@@ -421,14 +423,15 @@
 - <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
 - <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
 - <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
 - <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
 - <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
 - <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
 - <b>`stop`</b>: A list of sequences to stop generation when encountered. Default: `None`
+- <b>`stream`</b>: Whether to stream the generated text. Default: `False`
 - <b>`reset`</b>: Whether to reset the model state before generating text. Default: `True`
 
 **Returns:**
 The generated text.
 
 <!-- API_DOCS -->
```

### Comparing `ctransformers-0.1.1/ctransformers/hub.py` & `ctransformers-0.1.2/ctransformers/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,15 @@
         *,
         model_type: Optional[str] = None,
         model_file: Optional[str] = None,
         config: Optional[AutoConfig] = None,
         lib: Optional[str] = None,
         **kwargs,
     ) -> LLM:
-        """
-        Loads the language model from a local file or remote repo.
+        """Loads the language model from a local file or remote repo.
 
         Args:
             model_path_or_repo_id: The path to a model file or directory or the
             name of a Hugging Face Hub model repo.
             model_type: The model type.
             model_file: The name of the model file in repo or directory.
             config: `AutoConfig` object.
```

### Comparing `ctransformers-0.1.1/ctransformers/lib/avx/ctransformers.dll` & `ctransformers-0.1.2/ctransformers/lib/avx/ctransformers.dll`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib/avx/libctransformers.dylib` & `ctransformers-0.1.2/ctransformers/lib/avx/libctransformers.dylib`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib/avx/libctransformers.so` & `ctransformers-0.1.2/ctransformers/lib/avx/libctransformers.so`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib/avx2/ctransformers.dll` & `ctransformers-0.1.2/ctransformers/lib/avx2/ctransformers.dll`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib/avx2/libctransformers.dylib` & `ctransformers-0.1.2/ctransformers/lib/avx2/libctransformers.dylib`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib/avx2/libctransformers.so` & `ctransformers-0.1.2/ctransformers/lib/avx2/libctransformers.so`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib/basic/ctransformers.dll` & `ctransformers-0.1.2/ctransformers/lib/basic/ctransformers.dll`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib/basic/libctransformers.dylib` & `ctransformers-0.1.2/ctransformers/lib/basic/libctransformers.dylib`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib/basic/libctransformers.so` & `ctransformers-0.1.2/ctransformers/lib/basic/libctransformers.so`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/lib.py` & `ctransformers-0.1.2/ctransformers/lib.py`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/ctransformers/llm.py` & `ctransformers-0.1.2/ctransformers/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import re
+from collections import OrderedDict
 from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 from ctypes import (
     CDLL,
     c_bool,
     c_int,
@@ -15,14 +16,15 @@
 from typing import (
     Any,
     Callable,
     Generator,
     List,
     Optional,
     Sequence,
+    Union,
 )
 
 from .lib import find_library
 
 c_int_p = POINTER(c_int)
 llm_p = c_void_p
 
@@ -40,40 +42,40 @@
     # eval
     batch_size: int = 8
     threads: int = -1
 
     # generate
     max_new_tokens: int = 256
     stop: Optional[Sequence[str]] = None
+    stream: bool = False
     reset: bool = True
 
 
-docs = dict(
+docs = OrderedDict(
     top_k='The top-k value to use for sampling.',
     top_p='The top-p value to use for sampling.',
     temperature='The temperature to use for sampling.',
     repetition_penalty='The repetition penalty to use for sampling.',
     last_n_tokens='The number of last tokens to use for repetition penalty.',
     seed='The seed value to use for sampling tokens.',
     max_new_tokens='The maximum number of new tokens to generate.',
     stop='A list of sequences to stop generation when encountered.',
+    stream='Whether to stream the generated text.',
     reset='Whether to reset the model state before generating text.',
     batch_size='The batch size to use for evaluating tokens.',
     threads='The number of threads to use for evaluating tokens.',
 )
 
-for k in docs:
-    docs[k] = f'{k}: {docs[k]} Default: `{getattr(Config, k)}`'
-
 
 def doc(fn):
     doc = []
     for param in inspect.signature(fn).parameters:
         if param in docs:
-            doc.append(docs[param])
+            default = getattr(Config, param)
+            doc.append(f'{param}: {docs[param]} Default: `{default}`')
     doc = ('\n' + ' ' * 12).join(doc)
     fn.__doc__ = fn.__doc__.format(params=doc)
     return fn
 
 
 def get(*values):
     for value in values:
@@ -126,16 +128,15 @@
         self,
         model_path: str,
         model_type: str,
         *,
         config: Optional[Config] = None,
         lib: Optional[str] = None,
     ):
-        """
-        Loads the language model from a local file.
+        """Loads the language model from a local file.
 
         Args:
             model_path: The path to a model file.
             model_type: The model type.
             config: `Config` object.
             lib: The path to a shared library or one of `avx2`, `avx`, `basic`.
         """
@@ -173,30 +174,28 @@
     def __getattr__(self, name: str) -> Callable:
         lib, llm = self._lib, self._llm
         if name.startswith('ctransformers_llm_') and hasattr(lib, name):
             return partial(getattr(lib, name), llm)
         raise AttributeError(f"'LLM' object has no attribute '{name}'")
 
     def tokenize(self, text: str) -> List[int]:
-        """
-        Converts a text into list of tokens.
+        """Converts a text into list of tokens.
 
         Args:
             text: The text to tokenize.
 
         Returns:
             The list of tokens.
         """
         tokens = (c_int * len(text))()
         n_tokens = self.ctransformers_llm_tokenize(text.encode(), tokens)
         return tokens[:n_tokens]
 
     def detokenize(self, tokens: Sequence[int]) -> str:
-        """
-        Converts a list of tokens to text.
+        """Converts a list of tokens to text.
 
         Args:
             tokens: The list of tokens.
 
         Returns:
             The combined text of all tokens.
         """
@@ -205,16 +204,15 @@
         texts = []
         for token in tokens:
             text = self.ctransformers_llm_detokenize(token)
             texts.append(text.decode())
         return ''.join(texts)
 
     def is_eos_token(self, token: int) -> bool:
-        """
-        Checks if a token is an end-of-sequence token.
+        """Checks if a token is an end-of-sequence token.
 
         Args:
             token: The token to check.
 
         Returns:
             `True` if the token is an end-of-sequence token else `False`.
         """
@@ -224,16 +222,15 @@
     def eval(
         self,
         tokens: Sequence[int],
         *,
         batch_size: Optional[int] = None,
         threads: Optional[int] = None,
     ) -> None:
-        """
-        Evaluates a list of tokens.
+        """Evaluates a list of tokens.
 
         Args:
             tokens: The list of tokens to evaluate.
             {params}
         """
         config = self.config
         batch_size = get(batch_size, config.batch_size)
@@ -253,16 +250,15 @@
         top_k: Optional[int] = None,
         top_p: Optional[float] = None,
         temperature: Optional[float] = None,
         repetition_penalty: Optional[float] = None,
         last_n_tokens: Optional[int] = None,
         seed: Optional[int] = None,
     ) -> int:
-        """
-        Samples a token from the model.
+        """Samples a token from the model.
 
         Args:
             {params}
 
         Returns:
             The sampled token.
         """
@@ -280,17 +276,15 @@
             temperature,
             repetition_penalty,
             last_n_tokens,
             seed,
         )
 
     def reset(self) -> None:
-        """
-        Resets the model state.
-        """
+        """Resets the model state."""
         self.ctransformers_llm_reset()
 
     def __del__(self):
         if self._llm is not None:
             self.ctransformers_llm_delete()
 
     @doc
@@ -304,16 +298,15 @@
         repetition_penalty: Optional[float] = None,
         last_n_tokens: Optional[int] = None,
         seed: Optional[int] = None,
         batch_size: Optional[int] = None,
         threads: Optional[int] = None,
         reset: Optional[bool] = None,
     ) -> Generator[int, None, None]:
-        """
-        Generates new tokens from a list of tokens.
+        """Generates new tokens from a list of tokens.
 
         Args:
             tokens: The list of tokens to generate tokens from.
             {params}
 
         Returns:
             The generated tokens.
@@ -422,34 +415,39 @@
         temperature: Optional[float] = None,
         repetition_penalty: Optional[float] = None,
         last_n_tokens: Optional[int] = None,
         seed: Optional[int] = None,
         batch_size: Optional[int] = None,
         threads: Optional[int] = None,
         stop: Optional[Sequence[str]] = None,
+        stream: Optional[bool] = None,
         reset: Optional[bool] = None,
-    ) -> str:
-        """
-        Generates text from a prompt.
+    ) -> Union[str, Generator[str, None, None]]:
+        """Generates text from a prompt.
 
         Args:
             prompt: The prompt to generate text from.
             {params}
 
         Returns:
             The generated text.
         """
+        config = self.config
+        stream = get(stream, config.stream)
+
         text = self._stream(
             prompt,
             max_new_tokens=max_new_tokens,
             top_k=top_k,
             top_p=top_p,
             temperature=temperature,
             repetition_penalty=repetition_penalty,
             last_n_tokens=last_n_tokens,
             seed=seed,
             batch_size=batch_size,
             threads=threads,
             stop=stop,
             reset=reset,
         )
+        if stream:
+            return text
         return ''.join(text)
```

### Comparing `ctransformers-0.1.1/ctransformers.egg-info/PKG-INFO` & `ctransformers-0.1.2/ctransformers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
         
@@ -158,31 +158,32 @@
         llm_chain = LLMChain(prompt=prompt, llm=llm)
         
         print(llm_chain.run('What is AI?'))
         ```
         
         ## Documentation
         
-        ### Parameters
+        <!-- API_DOCS -->
+        
+        ### Config
         
-        | Name                 | Type        | Description                                              | Default |
+        | Parameter            | Type        | Description                                              | Default |
         | :------------------- | :---------- | :------------------------------------------------------- | :------ |
         | `top_k`              | `int`       | The top-k value to use for sampling.                     | `40`    |
         | `top_p`              | `float`     | The top-p value to use for sampling.                     | `0.95`  |
         | `temperature`        | `float`     | The temperature to use for sampling.                     | `0.8`   |
         | `repetition_penalty` | `float`     | The repetition penalty to use for sampling.              | `1.0`   |
         | `last_n_tokens`      | `int`       | The number of last tokens to use for repetition penalty. | `64`    |
-        | `seed`               | `int`       | The seed value to use for sampling tokens.               | Random  |
+        | `seed`               | `int`       | The seed value to use for sampling tokens.               | `-1`    |
         | `max_new_tokens`     | `int`       | The maximum number of new tokens to generate.            | `256`   |
-        | `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `[]`    |
+        | `stop`               | `List[str]` | A list of sequences to stop generation when encountered. | `None`  |
+        | `stream`             | `bool`      | Whether to stream the generated text.                    | `False` |
         | `reset`              | `bool`      | Whether to reset the model state before generating text. | `True`  |
         | `batch_size`         | `int`       | The batch size to use for evaluating tokens.             | `8`     |
-        | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | Auto    |
-        
-        <!-- API_DOCS -->
+        | `threads`            | `int`       | The number of threads to use for evaluating tokens.      | `-1`    |
         
         ### <kbd>class</kbd> `AutoModelForCausalLM`
         
         ---
         
         #### <kbd>classmethod</kbd> `AutoModelForCausalLM.from_pretrained`
         
@@ -410,16 +411,17 @@
             temperature: Optional[float] = None,
             repetition_penalty: Optional[float] = None,
             last_n_tokens: Optional[int] = None,
             seed: Optional[int] = None,
             batch_size: Optional[int] = None,
             threads: Optional[int] = None,
             stop: Optional[Sequence[str]] = None,
+            stream: Optional[bool] = None,
             reset: Optional[bool] = None
-        ) → str
+        ) → Union[str, Generator[str, NoneType, NoneType]]
         ```
         
         Generates text from a prompt.
         
         **Args:**
         
         - <b>`prompt`</b>: The prompt to generate text from.
@@ -429,14 +431,15 @@
         - <b>`temperature`</b>: The temperature to use for sampling. Default: `0.8`
         - <b>`repetition_penalty`</b>: The repetition penalty to use for sampling. Default: `1.0`
         - <b>`last_n_tokens`</b>: The number of last tokens to use for repetition penalty. Default: `64`
         - <b>`seed`</b>: The seed value to use for sampling tokens. Default: `-1`
         - <b>`batch_size`</b>: The batch size to use for evaluating tokens. Default: `8`
         - <b>`threads`</b>: The number of threads to use for evaluating tokens. Default: `-1`
         - <b>`stop`</b>: A list of sequences to stop generation when encountered. Default: `None`
+        - <b>`stream`</b>: Whether to stream the generated text. Default: `False`
         - <b>`reset`</b>: Whether to reset the model state before generating text. Default: `True`
         
         **Returns:**
         The generated text.
         
         <!-- API_DOCS -->
```

### Comparing `ctransformers-0.1.1/ctransformers.egg-info/SOURCES.txt` & `ctransformers-0.1.2/ctransformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctransformers-0.1.1/setup.py` & `ctransformers-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 name = 'ctransformers'
 
 setup(
     name=name,
-    version='0.1.1',
+    version='0.1.2',
     description=
     'Python bindings for the Transformer models implemented in C/C++ using GGML library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ravindra Marella',
     author_email='mv.ravindra007@gmail.com',
     url='https://github.com/marella/{}'.format(name),
```

