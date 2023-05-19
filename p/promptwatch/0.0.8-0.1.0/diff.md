# Comparing `tmp/promptwatch-0.0.8.tar.gz` & `tmp/promptwatch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.0.8.tar", last modified: Wed May 10 08:33:26 2023, max compression
+gzip compressed data, was "promptwatch-0.1.0.tar", last modified: Fri May 19 08:45:05 2023, max compression
```

## Comparing `promptwatch-0.0.8.tar` & `promptwatch-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.401004 promptwatch-0.0.8/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-10 08:33:26.400827 promptwatch-0.0.8/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.0.8/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.8/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-10 08:33:26.401050 promptwatch-0.0.8/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 21:26:09.000000 promptwatch-0.0.8/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.395406 promptwatch-0.0.8/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.397796 promptwatch-0.0.8/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-10 08:33:10.000000 promptwatch-0.0.8/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11922 2023-05-10 08:27:00.000000 promptwatch-0.0.8/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 21:26:09.000000 promptwatch-0.0.8/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.8/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1605 2023-05-07 09:39:06.000000 promptwatch-0.0.8/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.400402 promptwatch-0.0.8/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-03 12:40:47.000000 promptwatch-0.0.8/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    34257 2023-05-10 08:30:37.000000 promptwatch-0.0.8/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    14278 2023-05-08 08:14:57.000000 promptwatch-0.0.8/src/promptwatch/promptwatch_context.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.0.8/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.399787 promptwatch-0.0.8/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.8/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.064271 promptwatch-0.1.0/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-19 08:45:05.064060 promptwatch-0.1.0/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.1.0/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.1.0/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-19 08:45:05.064449 promptwatch-0.1.0/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-15 10:58:25.000000 promptwatch-0.1.0/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.054496 promptwatch-0.1.0/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.058188 promptwatch-0.1.0/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      317 2023-05-18 20:35:02.000000 promptwatch-0.1.0/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11928 2023-05-12 11:33:50.000000 promptwatch-0.1.0/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5392 2023-05-18 23:34:53.000000 promptwatch-0.1.0/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-14 23:06:27.000000 promptwatch-0.1.0/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.1.0/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1605 2023-05-19 07:02:23.000000 promptwatch-0.1.0/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.060692 promptwatch-0.1.0/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      153 2023-05-15 14:16:53.000000 promptwatch-0.1.0/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11067 2023-05-19 07:08:20.000000 promptwatch-0.1.0/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    25660 2023-05-19 07:10:20.000000 promptwatch-0.1.0/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-18 23:13:38.000000 promptwatch-0.1.0/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17876 2023-05-19 07:34:33.000000 promptwatch-0.1.0/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.063626 promptwatch-0.1.0/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-12 12:27:23.000000 promptwatch-0.1.0/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12091 2023-05-18 20:39:07.000000 promptwatch-0.1.0/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-17 23:04:57.000000 promptwatch-0.1.0/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13583 2023-05-18 23:34:47.000000 promptwatch-0.1.0/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.1.0/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.059424 promptwatch-0.1.0/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.1.0/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.0.8/PKG-INFO` & `promptwatch-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.8
+Version: 0.1.0
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.8/README.md` & `promptwatch-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.8/setup.py` & `promptwatch-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 
                 classifiers=[
                 ],
                 python_requires='>=3.8',
                 install_requires=[
                     "langchain",
                     "pydantic",
-                    "tiktoken"
+                    "tiktoken",
+                    "tqdm",
                 ]
                 )
```

### Comparing `promptwatch-0.0.8/src/promptwatch/caching.py` & `promptwatch-0.1.0/src/promptwatch/caching.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         return self.client.get_from_cache(self.cache_namespace_key, prompt_embedding, min_similarity=similarity_limit)
     
     
     def add(self, prompt_hash:UUID, prompt_embedding:List[float],result:str):
         self.client.add_into_cache(self.cache_namespace_key, str(prompt_hash), prompt_embedding, result)
 
     def clear(self):
-        self.client.clear(self.cache_namespace_key)
+        self.client.clear_cache(self.cache_namespace_key)
 
 
 def num_tokens_from_string(string: str, encoding_name: str="cl100k_base") -> int:
     """Returns the number of tokens in a text string."""
     encoding = tiktoken.get_encoding(encoding_name)
     num_tokens = len(encoding.encode(string))
     return num_tokens
```

### Comparing `promptwatch-0.0.8/src/promptwatch/client.py` & `promptwatch-0.1.0/src/promptwatch/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,113 @@
 from .data_model import Session, ActivityBase, ActivityList
 import requests
 from typing import List, Optional,Tuple
 import os
 import logging
 from datetime import datetime
-
+from .unit_tests.schema import TestCase,  PromptUnitTestRun, TestCaseResult, TestCaseResultsList
+from pydantic.json import pydantic_encoder
 
 
 class Client:
 
-    def __init__(self, api_key:str) -> None:
+    def __init__(self, api_key:str=None) -> None:
         if not api_key:
             api_key=os.environ.get("PROMPTWATCH_API_KEY")
         if not api_key:
             raise Exception("Unable to find PromptWatch API key. Either set api key as a parameter to PromptWatch(api_key='<your api key>') or set it up as an env. variable PROMPTWATCH_API_KEY. You can generate your API key here: https://app.promptwatch.io/get-api-key")
         self.api_key=api_key    
         self.logger = logging.getLogger("PromptWatchClient")
         self.tracker_api_host_url = os.environ.get("PROMPTWATCH_HOST_URL","https://api.promptwatch.io").rstrip("/")
         self.headers={
                             "x-api-key":self.api_key, 
                             "Content-Type":"application/json"
                             }
                         
-    def _request(self, method:str, endpoint:str, data:Optional[str]=None,json:Optional[dict]=None, params:Optional[dict]=None, timeout=5)-> requests.Response:
+    def _request(self, method:str, endpoint:str, data_str:Optional[str]=None,json_dict:Optional[dict]=None, params:Optional[dict]=None, timeout=5, ignore_errors=True)-> requests.Response:
 
         try:
-            response = requests.request(method, f"{self.tracker_api_host_url}{endpoint}", json=json, data=data, params=params, headers=self.headers, timeout=timeout)
+            response = requests.request(method, f"{self.tracker_api_host_url}{endpoint}", json=json_dict, data=data_str, params=params, headers=self.headers, timeout=timeout)
             if response.status_code>300:
+                if not ignore_errors:
+                    raise Exception(f"Error sending data to the server: Error {response.status_code} - {response.reason} ({response.text})")
                 self.logger.error(f"Error sending data to the server: Error {response.status_code} - {response.reason} ({response.text})")
+                return None
             return response
         except Exception as ex:
             self.logger.exception(ex)
+            if not ignore_errors:
+                raise ex
 
     
     def start_session(self, session:Session):
-       self._request("POST", f"/sessions/start", data=session.json())
+       self._request("POST", f"/sessions/start", data_str=session.json())
     def finish_session(self, session:Session):
-       self._request("POST", f"/sessions/finish", data=session.json())
+       self._request("POST", f"/sessions/finish", data_str=session.json())
 
     def restore_session(self, session_id:str):
        response = self._request("POST", f"/sessions/{session_id}/restore")
        data = response.json()
        session_data = data.get("session")
        if session_data:
            return Session(**session_data)
        
 
     def save_activities(self, session_id:str,   activities:List[ActivityBase]):
     
         payload = ActivityList(activities)
-        self._request("POST",f"/sessions/{session_id}/activities", data=payload.json())
+        self._request("POST",f"/sessions/{session_id}/activities", data_str=payload.json(), ignore_errors=True)
         
         
     def get_session(self, session_id:str)-> Session:
         response = requests.get(f"{self.tracker_api_host_url}/sessions/{session_id}", headers=self.headers)
         
     
         if response.status_code==200:
             return Session(**response.json())
         else:
             raise Exception(f"Error response from server: {response.status_code}: {response.text}")
         
 
     def get_from_cache(self, cache_namespace_key:str,  query_embedding:List[float], min_similarity:float)-> Tuple[str,float]:
-        response = self._request("POST", f"/prompt-cache/{cache_namespace_key}/get", json={"embedding":query_embedding},params={ "min_similarity":min_similarity})
+        response = self._request("POST", f"/prompt-cache/{cache_namespace_key}/get", json_dict={"embedding":query_embedding},params={ "min_similarity":min_similarity})
         if response:
             data = response.json()
             if data:
                 result = data.get("result")
                 similarity = data.get("similarity")
                 return result, similarity
         
     def add_into_cache(self, cache_namespace_key:str, id:str, embedding:List[float], result:str):
-       response = self._request("POST", f"/prompt-cache/{cache_namespace_key}", json={"embedding":embedding, "id":id,"result":result})
+       response = self._request("POST", f"/prompt-cache/{cache_namespace_key}", json_dict={"embedding":embedding, "id":id,"result":result})
     
-    def clear(self, cache_namespace_key:str, until:Optional[datetime]=None):
+    def clear_cache(self, cache_namespace_key:str, until:Optional[datetime]=None):
        response = self._request("POST", f"/prompt-cache/{cache_namespace_key}/clear", params={ "until":until})
+    
+
+    
+    def get_test_cases(self, for_tracking_project=None, for_template_name=None, skip=0, limit=1000)->TestCase:
+        
+        query_params = {
+            "for_tracking_project": for_tracking_project,
+            "for_template_name": for_template_name,
+            "skp": skip,
+            "limit": limit
+        }
+        response = self._request("GET", f"/test-cases", params=query_params,  timeout=None, ignore_errors=False)
+        if response:
+            data = response.json()
+            if data:
+                return [TestCase(**item) for item in data]
+            else:
+                return []
+        
+    def save_unit_test_run(self, unit_test_run: PromptUnitTestRun, timeout=None):
+        
+      
+        response = self._request("POST", f"/tests/{unit_test_run.test_name}/runs", data_str=unit_test_run.json(), timeout=None, ignore_errors=False)
+       
+
+    def save_unit_test_cases_result(self, test_name, run_id, test_case_results:List[TestCaseResult]):
+        response = self._request("POST", f"/tests/{test_name}/runs/{run_id}/result-details", data_str=TestCaseResultsList(__root__=test_case_results).json(), timeout=None, ignore_errors=False)
+
```

### Comparing `promptwatch-0.0.8/src/promptwatch/data_model.py` & `promptwatch-0.1.0/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.8/src/promptwatch/decorators.py` & `promptwatch-0.1.0/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.8/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.1.0/src/promptwatch/langchain/langchain_support.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 """A Tracer implementation that records to LangChain endpoint."""
 from __future__ import annotations
 import re
 from abc import ABC
-from typing import Any, Dict, Optional, Union, Callable
+from typing import Any, Dict, Optional, Union
 import datetime
-from pydantic import root_validator
 from langchain.prompts.base import BasePromptTemplate
-from langchain.prompts.chat import ChatPromptValue, ChatPromptTemplate, HumanMessagePromptTemplate, AIMessagePromptTemplate, SystemMessagePromptTemplate, MessagesPlaceholder, BaseMessagePromptTemplate
-from langchain.llms.base import LLM, BaseLLM
+from langchain.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate, AIMessagePromptTemplate, SystemMessagePromptTemplate, MessagesPlaceholder, BaseMessagePromptTemplate
+from langchain.llms.base import LLM
 from langchain.chat_models.base import BaseChatModel
 from langchain.chains import LLMChain
 from langchain.embeddings.base import Embeddings
-from langchain.schema import HumanMessage, ChatMessage as LangChainChatMessage, AIMessage, SystemMessage, BaseMessage, ChatGeneration, ChatResult
+from langchain.schema import HumanMessage, ChatMessage as LangChainChatMessage, AIMessage, SystemMessage, BaseMessage
 from langchain.callbacks.base import BaseCallbackHandler
 
-from langchain.schema import PromptValue
 from langchain.schema import AgentAction, AgentFinish, LLMResult,  Document
 from ..client import Client
 from ..data_model import NamedPromptTemplateDescription,PromptTemplateDescription, LlmPrompt, ParallelPrompt, ChainSequence, ChatMessage, Answer, Action, Question, RetrievedDocuments, DocumentSnippet, ChatMessagePromptTemplate
 from ..utils import find_the_caller_in_the_stack, is_primitive_type, wrap_a_method
-
+from .caching import CachedLLM, CachedChatLLM
 from ..decorators import FORMATTED_PROMPT_CONTEXT_KEY, TEMPLATE_NAME_CONTEXT_KEY, LLM_CHAIN_CONTEXT_KEY
 
 from typing import List, Dict
-from .. import PromptWatch
-from langchain.cache import BaseCache
-from langchain.schema import Generation
-from collections import OrderedDict
+from ..promptwatch_context import PromptWatch, ContextTrackerSingleton
 
 
 class LangChainSupport:
 
     def __init__(self, promptwatch_context:PromptWatch) -> None:
         self.promptwatch_context=promptwatch_context
         self.langchain_callback_handler=None
@@ -43,15 +38,14 @@
 
         """
         self.langchain_callback_handler = LangChainCallbackHandler(self.promptwatch_context)
 
         try:
             # this will 
             #for langchain >0.0.153
-            from langchain.callbacks.manager import _configure
             import langchain.callbacks.manager as langchain_callback_manager_module
             def promptwatch_callback_configure_decorator(func):
                 def configure_with_promptwatch(*args, **kwargs):
                     callback_manager = func(*args, **kwargs)
                     if callback_manager and not any(isinstance(handler, LangChainCallbackHandler) for handler in callback_manager.handlers):
                         pw = PromptWatch.get_active_instance()
                         if pw:
@@ -109,23 +103,29 @@
 
     def __init__(self, 
                  prompt_watch:PromptWatch
 
             ) -> None:
         self.current_llm_chain:Optional[LLMChain]=None
         self.tracing_handlers={}
+        self.prompt_watch_session_id=prompt_watch.session_id
         #we keep these in order to reverse
         self.monkey_patched_functions=[]
         
         super().__init__()
+
         
     @property
     def prompt_watch(self) -> PromptWatch:
         """Whether to call verbose callbacks even if verbose is False."""
-        return PromptWatch.get_active_instance()
+        
+        prompt_watch_context = ContextTrackerSingleton.get_current(self.prompt_watch_session_id)
+        if not prompt_watch_context:
+            raise Exception("PromptWatch context could not be resolved")
+        return prompt_watch_context
 
 
     @property
     def always_verbose(self) -> bool:
         """Whether to call verbose callbacks even if verbose is False."""
         return True
     
@@ -187,14 +187,17 @@
                 prompt_input_values = {k:v for k,v in prompt_input_values.items() if k in prompt_template.prompt_input_params and (isinstance(v,str) )}
             else:
                 prompt_input_values={k:v for k,v in prompt_input_values.items() if isinstance(v,str)}
 
             if  prompt_template and isinstance(prompt_template.prompt_template,list):
                 non_text_input = {k:v for k,v in  self.prompt_watch.current_activity.inputs.items() if not isinstance(v,str)}
                 for k, v in non_text_input.items():
+                    if v and isinstance(v,list) and isinstance(v[0],ChatMessage):
+                        prompt_input_values[k] = v
+                    # this should be necessary anymore... keeping it just in case
                     if v and isinstance(v,list) and isinstance(v[0],BaseMessage):
                         prompt_input_values[k] = convert_chat_messages(v)
                         
 
         else:
             info_message="Could not retrieve all the additional information needed to for reproducible prompt execution. Consider registering the prompt template."
 
@@ -225,15 +228,14 @@
             )
 
 
 
     
     def on_llm_new_token(self, token: str, **kwargs: Any) -> Any:
         """Run on new LLM token. Only available when streaming is enabled."""
-        pass
 
     
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
         """Run when LLM ends running."""
         if len(response.generations)>1:
             thoughts =  self.prompt_watch.current_activity.thoughts
         else:
@@ -287,31 +289,28 @@
 
         if  question and not self.prompt_watch.chain_hierarchy:
             self.prompt_watch._add_activity(Question(text=question))
         if not self.prompt_watch.current_session.session_name:
             self.prompt_watch.current_session.session_name=question
             if not self.prompt_watch.current_session.start_time:
                 self.prompt_watch.current_session.start_time=datetime.datetime.now(tz=datetime.timezone.utc)
-            #self.prompt_watch.client.start_session(self.prompt_watch.current_session)
-
+            
+        
+        
         current_chain=ChainSequence(
-                inputs=inputs,
+                inputs=serialize_chain_inputs(inputs),
                 metadata={},
                 sequence_type=serialized.get("name") or "others"
             )
                                      
         if kwargs:
             current_chain.metadata["input_kwargs"]=kwargs
         self.prompt_watch._open_activity(current_chain)
         
 
-    # def _trace_function_call(self, handler_key:str, function_name:str, args, kwargs, result):
-    #     handler = self.tracing_handlers.get(handler_key)
-    #     if handler:
-    #         handler(function_name, args, kwargs, result)
         
 
         
     def try_get_retrieved_documents(self, inputs:dict):
         retrieved_documents = next((val for key,val in inputs.items() if isinstance(val,list) and val and isinstance(val[0], Document)),None)
         if retrieved_documents:
             docs=[]
@@ -379,21 +378,19 @@
     ) -> Any:
         """Run when tool errors."""
         self.prompt_watch._on_error(error, kwargs)
 
     
     def on_text(self, text: str, **kwargs: Any) -> Any:
         """Run on arbitrary text."""
-        pass
 
     
     def on_agent_action(self, action: AgentAction, **kwargs: Any) -> Any:
         """Run on agent action."""
         
-        pass
         
 
 
 
     
     def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
         """Run on agent end."""
@@ -401,71 +398,69 @@
         answer_activity = Answer(text=answer_text)
         self.prompt_watch._add_activity(answer_activity, as_root=True)
         if finish.return_values:
             answer_activity.metadata["outputs"]:finish.return_values
         
         
     
-    
-        
 
+        
 
 
-class PromptWatchLlmCache(BaseCache):
 
-    def __init__(self, cache_namespace_key:str=None, cache_embeddings:Embeddings = None, token_limit:int=None, similarity_limit:float=0.97) -> None:
-        
-        self.cache_namespace_key = cache_namespace_key
-        self.cache_embeddings = cache_embeddings
-        self.similarity_limit=similarity_limit
-        
-        self.embed_func = self.cache_embeddings.embed_query if self.cache_embeddings else None
-
-        self.token_limit=token_limit
+def register_prompt_template(template_name:str,prompt_template, version:Optional[str]=None):
+        """
+        Register prompt template into context for more detailed tracking, versioning and evaluation
 
-    def lookup(self, prompt: str, llm_string: str) -> Optional[List[Generation]]:
-        """Look up based on prompt and llm_string."""
-        promptwatch_context = PromptWatch.get_active_instance()
-        cache_prompt_key = f"{llm_string}\n:{prompt}"
-        
-        if promptwatch_context:
-            cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, self.embed_func, self.token_limit, self.similarity_limit)
-            cached_res=cache.get(cache_prompt_key)
-            
-            if cached_res:         
-                return  [Generation(text=cached_res.result, generation_info={"cached":True, **cached_res.metadata, "_cached_result":cached_res})]
-       
-            else:
-                return None
 
-    
-    def update(self, prompt: str, llm_string: str, return_val: List[Generation]) -> None:
-        """Update cache based on prompt and llm_string."""
-        
-        cached_res = return_val[0].generation_info.get("_cached_result")
+        Args:
+            template_name (str): arbitrary unique template name (should not contain white spaces, max 126 chars)
+            prompt_template (Union[BasePromptTemplate,BaseChatPromptTemplate]): Any langchain prompt template
+            version (Optional[str], optional): Optional - (major) (SemVer) version of the template. Minor changes are tracked incrementally automatically. Useful if you are going to make a major change in the template, and you with to dive the version a distinct version number.
 
+        ## Examples:
         
-        promptwatch_context = PromptWatch.get_active_instance()
-        cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, self.embed_func, self.token_limit, self.similarity_limit)
-        cache.add(cached_res)
-
+        ### Registering regular prompt (completion)
 
+        ```
+        from promptwatch import PromptWatch
+        from langchain import OpenAI, LLMChain, PromptTemplate
 
+        prompt_template = PromptTemplate.from_template("Finish this sentence {input}")
+        my_chain = LLMChain(llm=OpenAI(), prompt=prompt_template)
 
-    
-    def clear(self, until:datetime=None) -> None:
-        promptwatch_context = PromptWatch.get_active_instance()
-        if promptwatch_context:
-            cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, self.embed_func, self.token_limit, self.similarity_limit)
-            cache.clear()
-        else:
-            Client().clear(self.cache_namespace_key,until=until)
+        with PromptWatch() as pw:
+            pw.register_prompt_template("simple_completion_template",prompt_template, version="1.0")
+            my_chain("The quick brown fox jumped over")
+        ```
 
+        ### Registering chat messages template (completion)
+        ...
 
+        """
+        if not template_name:
+            raise Exception("template_name can't be empty")
+        if re.search(r"\s", template_name):
+            raise Exception("template_name can't contain white spaces")
+        if len(template_name)>126:
+            raise Exception("template_name must be less than 126 characters")
+        
+        #TODO: hardcoded langchain_callback_handler
+        converted_template =  create_prompt_template_description(prompt_template, template_name=template_name, template_version=version)
+        from ..decorators import format_prompt_decorator
+        decorator_func = format_prompt_decorator(template_name)
+        
+        
+        wrap_a_method(prompt_template, "format_prompt", decorator_func)
+        # we need to mark the prompt template somehow... keeping just the reference doesn't work since pydantic is creating copy of it when passed to the constructor
+        # that is why we add special field __template_name__ into it... also skipping setattr() since that might be blocked by pydantic as well (depending on the configuration)
+        prompt_template.__dict__["__template_name__"]=template_name
 
+        PromptWatch.prompt_template_register_cache[template_name] = converted_template
+        return prompt_template
 
 
 
 def convert_chat_messages( msg:Union[BaseMessage, List[BaseMessage]]):
         if isinstance(msg, BaseMessage):
                 if isinstance(msg,HumanMessage):
                     role="user"
@@ -475,15 +470,53 @@
                     role="assistant"
                 elif isinstance(msg,SystemMessage):
                     role="system"
                     
                 return (ChatMessage(role=role,text=msg.content))
         elif isinstance(msg, list):
             return [convert_chat_messages(msg) for msg in msg]
+        else:
+            raise ValueError("msg must be either BaseMessage or List[BaseMessage]")
         
+def reconstruct_langchain_chat_messages( msg:Union[ChatMessage, List[ChatMessage]]):
+        if isinstance(msg, ChatMessage):
+                if msg.role=="user":
+                    return HumanMessage( content=msg.text)
+                    
+                elif msg.role=="assistant":
+                    return AIMessage( content=msg.text)
+                    
+                elif msg.role=="system":
+                    return SystemMessage( content=msg.text)
+                    
+                else:    
+                    return (LangChainChatMessage(role=msg.role,content=msg.text))
+        elif isinstance(msg, list):
+            return [reconstruct_langchain_chat_messages(msg) for msg in msg]
+        else:
+            raise ValueError("msg must be either ChatMessage or List[ChatMessage]")
+        
+def serialize_chain_inputs(inputs:dict):
+    res = {}
+    for k,v in inputs.items():
+        if isinstance(v, BaseMessage):
+            res[k]=convert_chat_messages(v)
+        elif isinstance(v, dict):
+            res[k]=serialize_chain_inputs(v)
+        elif isinstance(v, list):
+            if v:
+                if isinstance(v[0], BaseMessage):
+                    res[k]=convert_chat_messages(v)
+                elif isinstance(v[0], dict):
+                    res[k]=[serialize_chain_inputs(item) for item in v]
+                else:
+                    res[k]=v
+        else:
+            res[k]=v
+    return res
 
 def create_prompt_template_description( langchain_prompt_template:BasePromptTemplate, template_name:str = None, template_version:str=None)->Union[PromptTemplateDescription,NamedPromptTemplateDescription, None ]:
         
     format=None
     prompt_template=None
     
     if hasattr(langchain_prompt_template,"messages") and  langchain_prompt_template.messages:
@@ -534,237 +567,7 @@
     if prompt_template:
         if template_name:
             return NamedPromptTemplateDescription(prompt_template=prompt_template, prompt_input_params=input_params, format=format, template_name=template_name ,template_version=template_version)
         else:
             return PromptTemplateDescription(prompt_template=prompt_template, prompt_input_params=input_params, format=format)
 
 
-
-def register_prompt_template(template_name:str,prompt_template, version:Optional[str]=None):
-        """
-        Register prompt template into context for more detailed tracking, versioning and evaluation
-
-
-        Args:
-            template_name (str): arbitrary unique template name (should not contain white spaces, max 126 chars)
-            prompt_template (Union[BasePromptTemplate,BaseChatPromptTemplate]): Any langchain prompt template
-            version (Optional[str], optional): Optional - (major) (SemVer) version of the template. Minor changes are tracked incrementally automatically. Useful if you are going to make a major change in the template, and you with to dive the version a distinct version number.
-
-        ## Examples:
-        
-        ### Registering regular prompt (completion)
-
-        ```
-        from promptwatch import PromptWatch
-        from langchain import OpenAI, LLMChain, PromptTemplate
-
-        prompt_template = PromptTemplate.from_template("Finish this sentence {input}")
-        my_chain = LLMChain(llm=OpenAI(), prompt=prompt_template)
-
-        with PromptWatch() as pw:
-            pw.register_prompt_template("simple_completion_template",prompt_template, version="1.0")
-            my_chain("The quick brown fox jumped over")
-        ```
-
-        ### Registering chat messages template (completion)
-        ...
-
-        """
-        if not template_name:
-            raise Exception("template_name can't be empty")
-        if re.search(r"\s", template_name):
-            raise Exception("template_name can't contain white spaces")
-        if len(template_name)>126:
-            raise Exception("template_name must be less than 126 characters")
-        
-        #TODO: hardcoded langchain_callback_handler
-        converted_template =  create_prompt_template_description(prompt_template, template_name=template_name, template_version=version)
-        from ..decorators import format_prompt_decorator
-        decorator_func = format_prompt_decorator(template_name)
-        
-        
-        wrap_a_method(prompt_template, "format_prompt", decorator_func)
-        # we need to mark the prompt template somehow... keeping just the reference doesn't work since pydantic is creating copy of it when passed to the constructor
-        # that is why we add special field __template_name__ into it... also skipping setattr() since that might be blocked by pydantic as well (depending on the configuration)
-        prompt_template.__dict__["__template_name__"]=template_name
-
-        PromptWatch.prompt_template_register_cache[template_name] = converted_template
-
-
-
-
-class CachedLLM(LLM):
-    """Cached LLM wrapper around the actual LLM."""
-    inner_llm:Any
-    cache_namespace_key:Optional[str]
-    cache_embeddings:Optional[Embeddings]
-    token_limit:Optional[int]
-    similarity_limit:Optional[float]
-
-       
-    def __init__(self, inner_llm:BaseLLM, cache_namespace_key:str=None, cache_embeddings:Embeddings = None, token_limit:int=None, similarity_limit:float=0.97) -> None:
-        super().__init__(inner_llm=inner_llm, cache_namespace_key=cache_namespace_key, cache_embeddings=cache_embeddings, token_limit=token_limit, similarity_limit=similarity_limit)
-       
-    @property
-    def _llm_type(self) -> str:
-        """Return type of llm."""
-        return "cached-llm"
-    
-    
-    
-    def _get_from_cache(self,prompt, stop: Optional[List[str]] = None):
-        promptwatch_context = PromptWatch.get_active_instance()
-
-        
-        if promptwatch_context:
-            
-            embed_func = self.cache_embeddings.embed_query if self.cache_embeddings else None
-            cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, embed_func, self.token_limit, self.similarity_limit)
-            
-            cache_prompt_req = f"Stop:[{','.join(stop)}]\n:{prompt}" if stop else prompt
-            cached_res = cache.get(cache_prompt_req)
-           
-           
-            return  cached_res, lambda cached_res,result : cache.add(cached_res, result) if cached_res is not None else None
-        else:
-            return None, None
-        
-    def _call(self, prompt:str, stop: Optional[List[str]] = None) -> str:
-        """ Implementing abstract call method."""
-        return self.generate([prompt], stop=stop).generations[0][0].text
-    
-      
-        
-    def _generate(
-        self, prompts: List[str], stop: Optional[List[str]] = None
-    ) -> LLMResult:
-        if prompts and len(prompts)==1:
-            # we do not support multiple prompts for now
-
-            cached_res,callback=self._get_from_cache(prompts[0], stop=stop)
-        
-            if not cached_res:
-
-                llmresult:ChatResult = self.inner_llm._generate(prompts, stop) 
-                if callback:
-                    callback(cached_res, llmresult.generations[0][0].text)
-                return llmresult
-            else:
-                generation = Generation(text=cached_res.result, generation_info={"cached":True, **cached_res.metadata,  "cache_namespace_key":cached_res.cache_namespace_key})
-                return LLMResult(generations=[[generation]], llm_output={"cached":True})
-            
-        else:
-            return self.inner_llm._generate(prompts, stop) 
-        
-    async def _agenerate(self, 
-                         prompts: List[str], stop: Optional[List[str]] = None
-        ) -> LLMResult:
-        if prompts and len(prompts)==1:
-            cached_res,callback=self._get_from_cache(prompts[0], stop=stop)
-            
-            if not cached_res:
-
-                chat_result:ChatResult = await self.inner_llm._agenerate(prompts, stop) 
-                if callback:
-                    callback(cached_res, chat_result.generations[0].text)
-                return chat_result
-            else:
-                generation = Generation(text=cached_res.result, generation_info={"cached":True, **cached_res.metadata,  "cache_namespace_key":cached_res.cache_namespace_key})
-                return LLMResult(generations=[[generation]], llm_output={"cached":True})
-        else:
-            return self.inner_llm._generate(prompts, stop) 
-
-
-class CachedChatLLM(BaseChatModel):
-    
-    inner_llm:Any
-    cache_namespace_key:Optional[str]
-    cache_embeddings:Optional[Embeddings]
-    token_limit:Optional[int]
-    similarity_limit:Optional[float]
-    def __init__(self, inner_llm:BaseLLM, cache_namespace_key:str=None, cache_embeddings:Embeddings = None, token_limit:int=None, similarity_limit:float=0.97) -> None:
-        
-        super().__init__(inner_llm=inner_llm, cache_namespace_key=cache_namespace_key, cache_embeddings=cache_embeddings, token_limit=token_limit, similarity_limit=similarity_limit)
-       
-    @property
-    def _llm_type(self) -> str:
-        """Return type of llm."""
-        return "cached-chat-llm"
-    
-    def generate_prompt(
-        self, prompts: List[PromptValue], stop: Optional[List[str]] = None, **kwargs
-    ) -> LLMResult:
-        # overriding generate_prompt because we want to pass down the prompts to the inner llm
-        promptwatch_context = PromptWatch.get_active_instance()
-        if promptwatch_context and len(prompts)==1 :
-            promptwatch_context.add_context(FORMATTED_PROMPT_CONTEXT_KEY, prompts[0])
-        return super().generate_prompt(prompts, stop=stop)
-        
-    
-    def _get_from_cache(self, messages: Union[str, List[BaseMessage]], stop: Optional[List[str]] = None):
-        promptwatch_context = PromptWatch.get_active_instance()
-        prompt = ChatPromptValue(messages=messages).to_string()
-        
-        if promptwatch_context:
-            
-            embed_func = self.cache_embeddings.embed_query if self.cache_embeddings else None
-            cache = promptwatch_context.caching.get_or_init_cache(self.cache_namespace_key, embed_func, self.token_limit, self.similarity_limit)
-            
-            cache_prompt_req = f"Stop:[{','.join(stop)}]\n:{prompt}" if stop else prompt
-            cached_res = cache.get(cache_prompt_req)
-           
-           
-            return  cached_res, lambda cached_res,result : cache.add(cached_res, result) 
-        else:
-            return None, None
-        
-    def _call(self, messages: List[BaseMessage], stop: Optional[List[str]] = None, **kwargs) -> str:
-        """ Implementing abstract call method."""
-        return self._generate(messages, stop=stop).generations[0].message
-    
-        
-        
-    async def _acall(self, messages: List[BaseMessage], stop: Optional[List[str]] = None) -> str:
-        """ Implementing abstract call method."""
-        return (await self._agenerate(messages, stop=stop)).generations[0].message
-        
-    async def _agenerate(
-       self, messages: List[BaseMessage], stop: Optional[List[str]] = None,**kwargs
-    ):
-        cached_res,callback=self._get_from_cache(messages, stop=stop)
-        
-        if not cached_res:
-
-            chat_result:ChatResult = await self.inner_llm._agenerate(messages, stop, **kwargs) 
-            if callback:
-                callback(cached_res, chat_result.generations[0].text)
-            return chat_result
-        else:
-            generated_msg = AIMessage(content=cached_res.result)
-            generation = ChatGeneration(message=generated_msg, generation_info={"cached":True, **cached_res.metadata, "cache_namespace_key":cached_res.cache_namespace_key})
-            return ChatResult(generations=[generation],llm_output={"cached":True})
-
-        
-    def _generate(
-        self, messages: List[BaseMessage], stop: Optional[List[str]] = None,**kwargs
-    ) -> ChatResult:
-        cached_res,callback=self._get_from_cache(messages, stop=stop)
-        
-        
-        if not cached_res:
-
-
-            chat_result:ChatResult = self.inner_llm._generate(messages, stop,**kwargs) 
-            if callback:
-                callback(cached_res, chat_result.generations[0].text)
-            return chat_result
-        else:
-            generated_msg = AIMessage(content=cached_res.result)
-            generation = ChatGeneration(message=generated_msg, generation_info={"cached":True, **cached_res.metadata, "cache_namespace_key":cached_res.cache_namespace_key})
-            return ChatResult(generations=[generation],llm_output={"cached":True})
-    
-    def _combine_llm_outputs(self, llm_outputs: List[Optional[dict]]) -> dict:
-        """Combine llm outputs."""
-        if llm_outputs and len(llm_outputs)==1 and llm_outputs[0].get("cached"):
-            return llm_outputs[0]
-        else:
-            return self.inner_llm._combine_llm_outputs(llm_outputs)
```

### Comparing `promptwatch-0.0.8/src/promptwatch/promptwatch_context.py` & `promptwatch-0.1.0/src/promptwatch/promptwatch_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,73 @@
 """A Tracer implementation that records to LangChain endpoint."""
 from __future__ import annotations
 import base64
 import threading
-from typing import Any, Dict, Optional,List, Union, Tuple
+from typing import Any, Dict, Optional,List, Union, Tuple, Callable,Any
 import datetime
 import os
 import re
 from .data_model import (ActivityBase, Log, Session)
 import logging
 from .data_model import Session, ActivityBase,  ChainSequence, Log, Answer, Action, Question, RetrievedDocuments, DocumentSnippet
-from .client import Client
 from uuid import uuid4
 import types
 from .utils import wrap_a_method, classproperty
 from .caching import PromptWatchCacheManager
+from .constants import EnvVariables
 from abc import ABCMeta
 
 
+
 class ContextTrackerSingleton(ABCMeta,type):
     """
     Singleton metaclass for ensuring only one instance of a class per thread
     """
 
     _thread_local = threading.local()
+    _cross_thread_storage = {}
 
     def __call__(cls, *args, **kwargs):
         """Call method for the singleton metaclass."""
         if not hasattr(ContextTrackerSingleton._thread_local, "_instance"):
-            ContextTrackerSingleton._thread_local._instance = super(ContextTrackerSingleton, cls).__call__(*args, **kwargs)
+            prompt_watch_context = super(ContextTrackerSingleton, cls).__call__(*args, **kwargs)
+            if not prompt_watch_context.session_id:
+                raise Exception("PromptWatch: Session ID was not initialized. Please report this as a bug.")
+            ContextTrackerSingleton._cross_thread_storage[prompt_watch_context.session_id] = prompt_watch_context
+            ContextTrackerSingleton._thread_local._instance = prompt_watch_context
        
         return ContextTrackerSingleton._thread_local._instance 
         
-    def get_current():
+    def get_current(session_id:str=None):
+        """ return the current instance
+        for sync context session_id is not required
+        for async context session_id is required, otherwise it the instance wont be found
+        """
         if hasattr(ContextTrackerSingleton._thread_local, "_instance"):
-            return ContextTrackerSingleton._thread_local._instance
+            # in thread context ... this will work unless async is used... then we loose track...
+            # it is OK for nesting context in single thread...
+            current_instance = ContextTrackerSingleton._thread_local._instance
+            if current_instance and session_id and current_instance.session_id != session_id:
+                logging.warn(f"PromptWatch: Session ID {session_id} is not the same as the current session ID {current_instance.session_id}.  Please report this as a bug, ignoring the current context.")
+            else:
+                return current_instance
+        
+        # in async context... we need to use cross thread storage    
+        if session_id and ContextTrackerSingleton._cross_thread_storage.get(session_id):
+            current_session_context =  ContextTrackerSingleton._cross_thread_storage[session_id]
+            # also introduce it to the thread local storage
+            ContextTrackerSingleton._thread_local._instance = current_session_context
+            return current_session_context
         else:
             return None
 
-
+    @classmethod
     def remove_active_instance(cls):
+        session_id = ContextTrackerSingleton._thread_local._instance.session_id
+        del ContextTrackerSingleton._cross_thread_storage[session_id]
         del ContextTrackerSingleton._thread_local._instance 
 
 class PromptWatch(metaclass=ContextTrackerSingleton):
     
     prompt_template_register_cache={}
 
     def __init__(self, session_id: Optional[str] = None, tracking_project: Optional[str] = None, tracking_tenant: Optional[str] = None, api_key: Optional[str] = None):
@@ -62,44 +87,53 @@
         with PromptWatch(tracking_tenant="myCustomerTenantId", tracking_project="nameOfThisTrackingProject", api_key="<your api key>"):
            agent.run(question) 
         ```
         """
         self.logger = logging.getLogger("PromptWatch")
         self.session_id = session_id
         self.tracking_project=tracking_project
-        self.tracking_tenant=tracking_tenant
+        self.tracking_tenant=tracking_tenant or os.environ.get(EnvVariables.PROMPTWATCH_TRACKING_PROJECT)
 
         if not api_key:
-            api_key=os.environ.get("PROMPTWATCH_API_KEY")
+            api_key=os.environ.get(EnvVariables.PROMPTWATCH_API_KEY)
         if not api_key:
             raise Exception("Unable to find PromptWatch API key. Either set api key as a parameter to PromptWatch(api_key='<your api key>') or set it up as an env. variable PROMPTWATCH_API_KEY. You can generate your API key here: https://app.promptwatch.io/get-api-key")
         else:
             tenant_id  = self._decode_tenant_from_api_key(api_key)
             if tenant_id.startswith("temp_"):
                 if session_id:
                     self.logger.warn("Setting up session_id with a temporary PromptWatch API Key is not allowed. You session_id will be ignored")
                 self.session_id = tenant_id[5:]
                 GREEN = '\033[32m'
                 RESET = '\033[0m'
                 print(f"{GREEN}You are using a temporary API key. Do not use in production.")
                 print(f"Visit the the detail of this session at https://www.promptwatch.io/sessions?temp-api-key={api_key} {RESET}")
                 
 
-
+        from .client import Client
         self.client = Client(api_key=api_key)
         
+        # assign session_id if not provided
+        # we will used to track the session across multiple threads
+        if not self.session_id:
+            self.session_id = str(uuid4())
         
         self.chain_hierarchy:List[ChainSequence]=[]
         self.pending_session_save=True
         self.pending_stack:List[ActivityBase]=[]
         
         self.current_session=None
         self.context={}
         self._cache_manager = PromptWatchCacheManager(self)
         self.tracing_handlers={}
+        self.session_entered=False
+
+        #event handlers that lasts only
+        self.on_activity_event_handlers=[]
+        
 
     @property
     def caching(self):
         return self._cache_manager
 
     @property
     def langchain(self):
@@ -110,36 +144,45 @@
         
         return self._langchain
     
 
 
     def __enter__(self):
         
-
         if not self.tracing_handlers:
             # lets enable tracing by default
             self.langchain.init_tracing()
             #raise Exception("PromptWatch: LangChain callback handler is not set. Please call langchain_tracing() before entering the context.")
 
         if not self.current_session:
             self.start_session()
         
         
+        
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         try:
             self.finish_session()
         except Exception as ex:
             self.logger.warn(f"Failed to persist the session: {ex}")
+        # we will clear the handlers because we don't want to keep them in memory since PromptWatch is a singleton and lives for the whole app lifecycle
+        self.on_activity_event_handlers.clear()
 
-       
-
-
+    
+    def add_on_activity_callback(self, event_handler: Callable[[ActivityBase],Any]):
+        if event_handler not in self.on_activity_event_handlers:
+            self.on_activity_event_handlers.append(event_handler)
+
+    def set_session_name(self, name:str):
+        if self.current_session:
+            self.current_session.session_name=name
+        else:
+            raise Exception("No active session. Please call this method inside PromptWatch context")
 
     @classmethod
     def get_current_session(cls) -> Session:
         """_summary_
 
         Raises:
             Exception: If called outside PromptWatch context
@@ -301,28 +344,40 @@
 
         activity.end_time=datetime.datetime.now(tz=datetime.timezone.utc)
         if self.current_activity and not as_root:
             if isinstance(self.current_activity,ChainSequence):
                 activity.parent_activity_id=self.current_activity.id
             else:
                 activity.parent_activity_id=self.current_activity.parent_activity_id
+
+        for handler in self.on_activity_event_handlers:
+            try:
+                handler(activity)
+            except Exception as ex:
+                self.logger.exception(f"Failed to execute on_activity_event_handlers handler {handler.__name__}: {ex}")
+
         self.pending_stack.append(activity)
         
         
         
     
     def _close_current_activity(self):
         self._end_context_scope()
         self.current_activity.end_time=datetime.datetime.now(tz=datetime.timezone.utc)
         if self.chain_hierarchy and self.current_activity==self.current_activity:
             closing_chain = self.chain_hierarchy.pop()
             closing_chain.end_time = datetime.datetime.now(tz=datetime.timezone.utc)
             if closing_chain not in self.pending_stack:
                 self.pending_stack.append(closing_chain)
-        
+                
+        for handler in self.on_activity_event_handlers:
+            try:
+                handler(closing_chain)
+            except Exception as ex:
+                self.logger.exception(f"Failed to execute on_activity_event_handlers handler {handler.__name__}: {ex}")
         self._flush_stack()
 
     def _flush_stack(self):
         if  self.pending_session_save and self.current_session.steps_count:
             try:
                 self.client.start_session(self.current_session)
                 self.pending_session_save=False
@@ -336,29 +391,32 @@
                     if activity.end_time:
                         self.pending_stack.remove(activity)
             except Exception as ex:
                 self.logger.warn(f"Failed to persist activities to PromptWatch: {ex}")
 
 
     def start_session(self):
-        self.current_session=Session(start_time=datetime.datetime.now(tz=datetime.timezone.utc), tracking_project=self.tracking_project, tracking_tenant=self.tracking_tenant)
+        if self.current_session:
+            raise Exception("Session already started. Do not open PromptWatch context twice (probably nested with PromptWatch: ... calls)")
+        self.current_session=Session(id=self.session_id, start_time=datetime.datetime.now(tz=datetime.timezone.utc), tracking_project=self.tracking_project, tracking_tenant=self.tracking_tenant)
         self.logger.info(f"Starting PromptWatch session: {self.current_session.id}")
         self.current_session.start_time=self.current_session.start_time or datetime.datetime.now(tz=datetime.timezone.utc)
         self.pending_session_save=True
         
         
   
 
     def finish_session(self):
         
         self.current_session.end_time=datetime.datetime.now(tz=datetime.timezone.utc)
         self._flush_stack()
         if self.current_session.steps_count:
             self.client.finish_session(self.current_session)
         ContextTrackerSingleton.remove_active_instance()
+        self.current_session=None
 
     def _on_error(self, error, kwargs):
         self.current_activity.error=str(error)
         if kwargs:
             if not self.current_activity.metadata:
                 self.current_activity.metadata={}
             self.current_activity.metadata["error_kwargs"]=kwargs
```

### Comparing `promptwatch-0.0.8/src/promptwatch/utils.py` & `promptwatch-0.1.0/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.8/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.1.0/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.8
+Version: 0.1.0
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.8/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.1.0/src/promptwatch.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 README.md
 pyproject.toml
 setup.py
 src/promptwatch/__init__.py
 src/promptwatch/caching.py
 src/promptwatch/client.py
+src/promptwatch/constants.py
 src/promptwatch/data_model.py
 src/promptwatch/decorators.py
 src/promptwatch/promptwatch_context.py
 src/promptwatch/utils.py
 src/promptwatch.egg-info/PKG-INFO
 src/promptwatch.egg-info/SOURCES.txt
 src/promptwatch.egg-info/dependency_links.txt
 src/promptwatch.egg-info/not-zip-safe
 src/promptwatch.egg-info/requires.txt
 src/promptwatch.egg-info/top_level.txt
 src/promptwatch/langchain/__init__.py
-src/promptwatch/langchain/langchain_support.py
+src/promptwatch/langchain/caching.py
+src/promptwatch/langchain/langchain_support.py
+src/promptwatch/langchain/unit_tests.py
+src/promptwatch/unit_tests/__init__.py
+src/promptwatch/unit_tests/evaluation.py
+src/promptwatch/unit_tests/schema.py
+src/promptwatch/unit_tests/unit_tests.py
```

