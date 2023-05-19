# Comparing `tmp/lambdaprompt-0.5.3.tar.gz` & `tmp/lambdaprompt-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-s7mnpc4l/lambdaprompt-0.5.3.tar", last modified: Tue May 16 06:57:26 2023, max compression
+gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-502lzvwh/lambdaprompt-0.5.4.tar", last modified: Fri May 19 21:34:18 2023, max compression
```

## Comparing `lambdaprompt-0.5.3.tar` & `lambdaprompt-0.5.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/examples/one.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/examples/two.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/examples/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/server/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/server/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/tests/library/serverexamples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/tests/test_gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/examples/one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/examples/two.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/examples/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/server/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/server/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/tests/library/serverexamples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/tests/test_gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/tests/test_server.py
```

### Comparing `lambdaprompt-0.5.3/.github/workflows/publish-to-pypi.yml` & `lambdaprompt-0.5.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/.gitignore` & `lambdaprompt-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/LICENSE` & `lambdaprompt-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/PKG-INFO` & `lambdaprompt-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.5.3
+Version: 0.5.4
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lambdaprompt-0.5.3/README.md` & `lambdaprompt-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/lambdaprompt/__init__.py` & `lambdaprompt-0.5.4/lambdaprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/lambdaprompt/backends.py` & `lambdaprompt-0.5.4/lambdaprompt/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,35 +217,40 @@
         top_p: float = 0.92
         top_k: int = 0
         repetition_penalty: float = 1.1
         stop: Optional[Union[str, List[str]]]
 
     def __init__(self, model_name, torch_dtype=None, trust_remote_code=True, use_auth_token=None, **param_override):
         import torch
-        from transformers import AutoModelForCausalLM, AutoTokenizer
+        from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
         torch_dtype = torch_dtype or torch.bfloat16
         super().__init__(**param_override)
+        config = AutoConfig.from_pretrained(
+            model_name,
+            trust_remote_code=True
+        )
         self.model = AutoModelForCausalLM.from_pretrained(
             model_name,
             torch_dtype=torch_dtype,
             trust_remote_code=trust_remote_code,
             use_auth_token=use_auth_token,
+            config=config,
+            device_map="auto"
         )
         tokenizer = AutoTokenizer.from_pretrained(
             model_name,
             trust_remote_code=trust_remote_code,
             use_auth_token=use_auth_token,
+            device_map="auto"
         )
         if tokenizer.pad_token_id is None:
             tokenizer.pad_token = tokenizer.eos_token
         tokenizer.padding_side = "left"
         self.tokenizer = tokenizer
-        device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.model.eval()
-        self.model.to(device=device, dtype=torch_dtype)
 
     def preprocess(self, prompt):
         return prompt
 
     async def __call__(self, prompt, **kwargs):
         import torch
         from transformers import StoppingCriteriaList
```

### Comparing `lambdaprompt-0.5.3/lambdaprompt/gpt3.py` & `lambdaprompt-0.5.4/lambdaprompt/gpt3.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/lambdaprompt/prompt.py` & `lambdaprompt-0.5.4/lambdaprompt/prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/lambdaprompt/server/data.py` & `lambdaprompt-0.5.4/lambdaprompt/server/data.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/lambdaprompt/server/main.py` & `lambdaprompt-0.5.4/lambdaprompt/server/main.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/lambdaprompt.egg-info/PKG-INFO` & `lambdaprompt-0.5.4/lambdaprompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.5.3
+Version: 0.5.4
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lambdaprompt-0.5.3/lambdaprompt.egg-info/SOURCES.txt` & `lambdaprompt-0.5.4/lambdaprompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/pyproject.toml` & `lambdaprompt-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "requests", "aiohttp", "python-dotenv", "jinja2", "nest_asyncio", "pyyaml", "tenacity", "pydantic"
 ]
 urls = {homepage = "https://github.com/approximatelabs/lambdaprompt"}
 dynamic = ["version"]
 
 [project.optional-dependencies]
 server = ["fastapi", "uvicorn", "aiosqlite"]
-local = ["transformers"]
+local = ["transformers", "accelerate"]
 all = ["lambdaprompt[server,local]"]
 
 [tool.setuptools_scm]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
```

### Comparing `lambdaprompt-0.5.3/tests/test_gpt3.py` & `lambdaprompt-0.5.4/tests/test_gpt3.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/tests/test_prompt.py` & `lambdaprompt-0.5.4/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.3/tests/test_server.py` & `lambdaprompt-0.5.4/tests/test_server.py`

 * *Files identical despite different names*

