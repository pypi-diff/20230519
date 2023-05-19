# Comparing `tmp/gentrace_py-0.7.3.tar.gz` & `tmp/gentrace_py-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.7.3.tar", max compression
+gzip compressed data, was "gentrace_py-0.7.4.tar", max compression
```

## Comparing `gentrace_py-0.7.3.tar` & `gentrace_py-0.7.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1058 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-05-01 13:29:09.179503 gentrace_py-0.7.3/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      229 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/__init__.py
--rw-r--r--   0        0        0     1134 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    26684 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6400 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/step_run.py
--rw-r--r--   0        0        0     3706 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    12262 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/gentrace/schemas.py
--rw-r--r--   0        0        0     1571 2023-05-01 13:29:09.183503 gentrace_py-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      229 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0     1134 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    27820 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6400 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0     3706 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    12262 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/schemas.py
+-rw-r--r--   0        0        0     1571 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.7.4/PKG-INFO
```

### Comparing `gentrace_py-0.7.3/gentrace/__init__.py` & `gentrace_py-0.7.4/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/api_client.py` & `gentrace_py-0.7.4/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/configuration.py` & `gentrace_py-0.7.4/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/exceptions.py` & `gentrace_py-0.7.4/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/model/feedback_request.py` & `gentrace_py-0.7.4/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/model/feedback_request.pyi` & `gentrace_py-0.7.4/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/model/feedback_response.py` & `gentrace_py-0.7.4/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/model/feedback_response.pyi` & `gentrace_py-0.7.4/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.7.4/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.7.4/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.7.4/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.7.4/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/models/__init__.py` & `gentrace_py-0.7.4/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.7.4/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.7.4/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/providers/getters.py` & `gentrace_py-0.7.4/gentrace/providers/getters.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/providers/llms/openai.py` & `gentrace_py-0.7.4/gentrace/providers/llms/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 completion["pipelineRunId"] = (
                     submit_result["pipelineRunId"]
                     if "pipelineRunId" in submit_result
                     else None
                 )
 
 
-def create_stream_response(stream_list):
+def create_completion_stream_response(stream_list):
     final_response_string = ""
     for value in stream_list:
         if "choices" in value and value["choices"]:
             first_choice = value["choices"][0]
             if "text" in first_choice:
                 final_response_string += first_choice["text"]
             elif (
@@ -128,14 +128,46 @@
             }
         ]
     }
 
     return final_response
 
 
+def create_chat_completion_stream_response(stream_list):
+    final_response_string = ""
+    for value in stream_list:
+        if "choices" in value and value["choices"]:
+            first_choice = value["choices"][0]
+            if "text" in first_choice:
+                final_response_string += first_choice["text"]
+            elif (
+                "delta" in first_choice
+                and first_choice["delta"]
+                and "content" in first_choice["delta"]
+            ):
+                final_response_string += first_choice["delta"]["content"]
+            elif (
+                "finish_reason" in first_choice
+                and first_choice["finish_reason"] == "stop"
+            ):
+                break
+
+    final_response = {
+        "choices": [
+            {
+                "finish_reason": None,
+                "index": 0,
+                "message": {"content": final_response_string, "role": "assistant"},
+            }
+        ]
+    }
+
+    return final_response
+
+
 def intercept_completion(original_fn, gentrace_config: Configuration):
     @classmethod
     def wrapper(cls, *args, **kwargs):
         prompt_template = kwargs.get("prompt_template")
         prompt_inputs = kwargs.get("prompt_inputs")
         prompt = kwargs.get("prompt")
         pipeline_id = kwargs.pop("pipeline_id", None)
@@ -173,15 +205,15 @@
                     if value and is_self_contained:
                         value["pipelineRunId"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
-                full_response = create_stream_response(modified_response)
+                full_response = create_completion_stream_response(modified_response)
 
                 create_completion_step_run(
                     cls,
                     pipeline_id,
                     gentrace_config,
                     start_time,
                     end_time,
@@ -273,15 +305,15 @@
                     if value and is_self_contained:
                         value["pipelineRunId"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
-                full_response = create_stream_response(modified_response)
+                full_response = create_completion_stream_response(modified_response)
 
                 create_completion_step_run(
                     cls,
                     pipeline_id,
                     gentrace_config,
                     start_time,
                     end_time,
@@ -381,16 +413,17 @@
 
                 elapsed_time = int((end_time - start_time) * 1000)
 
                 pipeline_run = (
                     cls.pipeline_run if hasattr(cls, "pipeline_run") else None
                 )
 
-                full_response = create_stream_response(modified_response)
-
+                full_response = create_chat_completion_stream_response(
+                    modified_response
+                )
                 if is_self_contained:
                     pipeline = Pipeline(
                         id=pipeline_id,
                         api_key=gentrace_config.access_token,
                         host=gentrace_config.host,
                     )
 
@@ -490,15 +523,17 @@
                     if value and is_self_contained:
                         value["pipelineRunId"] = pipeline_run_id
                     modified_response.append(value)
                     yield value
 
                 end_time = time.time()
 
-                full_response = create_stream_response(modified_response)
+                full_response = create_chat_completion_stream_response(
+                    modified_response
+                )
 
                 elapsed_time = int((end_time - start_time) * 1000)
 
                 pipeline_run = (
                     cls.pipeline_run if hasattr(cls, "pipeline_run") else None
                 )
```

### Comparing `gentrace_py-0.7.3/gentrace/providers/pipeline.py` & `gentrace_py-0.7.4/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/providers/pipeline_run.py` & `gentrace_py-0.7.4/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/providers/step_run.py` & `gentrace_py-0.7.4/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/providers/utils.py` & `gentrace_py-0.7.4/gentrace/providers/utils.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.7.4/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/rest.py` & `gentrace_py-0.7.4/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/gentrace/schemas.py` & `gentrace_py-0.7.4/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.3/pyproject.toml` & `gentrace_py-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.7.3"
+version = "0.7.4"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 openai = {version = "^0.27.4", optional = true}
 pinecone-client = {version = "^2.2.1", optional = true}
 pydantic = ">=1.10.2"
```

### Comparing `gentrace_py-0.7.3/PKG-INFO` & `gentrace_py-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

