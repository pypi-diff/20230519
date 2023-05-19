# Comparing `tmp/gpt_json-0.1.6.tar.gz` & `tmp/gpt_json-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_json-0.1.6.tar", max compression
+gzip compressed data, was "gpt_json-0.1.7.tar", max compression
```

## Comparing `gpt_json-0.1.6.tar` & `gpt_json-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-05-18 20:56:17.170380 gpt_json-0.1.6/LICENSE
--rw-r--r--   0        0        0     8612 2023-05-18 20:56:17.170380 gpt_json-0.1.6/README.md
--rw-r--r--   0        0        0       63 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/enums.py
--rw-r--r--   0        0        0      145 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/exceptions.py
--rw-r--r--   0        0        0    11841 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/gpt.py
--rw-r--r--   0        0        0      792 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/models.py
--rw-r--r--   0        0        0     1483 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/parsers.py
--rw-r--r--   0        0        0     1860 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      256 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/tests/shared.py
--rw-r--r--   0        0        0     8767 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0      656 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/tests/test_models.py
--rw-r--r--   0        0        0     1037 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1189 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     3455 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/tests/test_transformations.py
--rw-r--r--   0        0        0     2808 2023-05-18 20:56:17.174380 gpt_json-0.1.6/gpt_json/transformations.py
--rw-r--r--   0        0        0      534 2023-05-18 20:56:17.174380 gpt_json-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 gpt_json-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-19 05:39:50.697158 gpt_json-0.1.7/LICENSE
+-rw-r--r--   0        0        0     8612 2023-05-19 05:39:50.697158 gpt_json-0.1.7/README.md
+-rw-r--r--   0        0        0       63 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/enums.py
+-rw-r--r--   0        0        0      145 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/exceptions.py
+-rw-r--r--   0        0        0    11846 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/gpt.py
+-rw-r--r--   0        0        0      792 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/models.py
+-rw-r--r--   0        0        0     1483 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/parsers.py
+-rw-r--r--   0        0        0     1860 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0     8767 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0      656 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_models.py
+-rw-r--r--   0        0        0     1037 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1189 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     3455 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/tests/test_transformations.py
+-rw-r--r--   0        0        0     2808 2023-05-19 05:39:50.697158 gpt_json-0.1.7/gpt_json/transformations.py
+-rw-r--r--   0        0        0      534 2023-05-19 05:39:50.697158 gpt_json-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 gpt_json-0.1.7/PKG-INFO
```

### Comparing `gpt_json-0.1.6/LICENSE` & `gpt_json-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/README.md` & `gpt_json-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/gpt.py` & `gpt_json-0.1.7/gpt_json/gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from gpt_json.models import (FixTransforms, GPTMessage, GPTModelVersion,
                              ResponseType)
 from gpt_json.parsers import find_json_response
 from gpt_json.prompts import generate_schema_prompt
 from gpt_json.transformations import fix_bools, fix_truncated_json
 
-logger = logging.getLogger('my_logger')
+logger = logging.getLogger('gptjson_logger')
 handler = logging.StreamHandler()
 formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
 
 def handle_backoff(details):
```

### Comparing `gpt_json-0.1.6/gpt_json/models.py` & `gpt_json-0.1.7/gpt_json/models.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/parsers.py` & `gpt_json-0.1.7/gpt_json/parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/prompts.py` & `gpt_json-0.1.7/gpt_json/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/tests/test_gpt.py` & `gpt_json-0.1.7/gpt_json/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/tests/test_models.py` & `gpt_json-0.1.7/gpt_json/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/tests/test_parsers.py` & `gpt_json-0.1.7/gpt_json/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/tests/test_prompts.py` & `gpt_json-0.1.7/gpt_json/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/tests/test_transformations.py` & `gpt_json-0.1.7/gpt_json/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/gpt_json/transformations.py` & `gpt_json-0.1.7/gpt_json/transformations.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.6/pyproject.toml` & `gpt_json-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-json"
-version = "0.1.6"
+version = "0.1.7"
 description = "Structured and typehinted GPT responses in Python."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 packages = [{include = "gpt_json"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gpt_json-0.1.6/PKG-INFO` & `gpt_json-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-json
-Version: 0.1.6
+Version: 0.1.7
 Summary: Structured and typehinted GPT responses in Python.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

