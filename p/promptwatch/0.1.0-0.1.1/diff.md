# Comparing `tmp/promptwatch-0.1.0.tar.gz` & `tmp/promptwatch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.1.0.tar", last modified: Fri May 19 08:45:05 2023, max compression
+gzip compressed data, was "promptwatch-0.1.1.tar", last modified: Fri May 19 13:00:54 2023, max compression
```

## Comparing `promptwatch-0.1.0.tar` & `promptwatch-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.064271 promptwatch-0.1.0/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-19 08:45:05.064060 promptwatch-0.1.0/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.1.0/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.1.0/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-19 08:45:05.064449 promptwatch-0.1.0/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-15 10:58:25.000000 promptwatch-0.1.0/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.054496 promptwatch-0.1.0/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.058188 promptwatch-0.1.0/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      317 2023-05-18 20:35:02.000000 promptwatch-0.1.0/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11928 2023-05-12 11:33:50.000000 promptwatch-0.1.0/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5392 2023-05-18 23:34:53.000000 promptwatch-0.1.0/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-14 23:06:27.000000 promptwatch-0.1.0/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.1.0/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1605 2023-05-19 07:02:23.000000 promptwatch-0.1.0/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.060692 promptwatch-0.1.0/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      153 2023-05-15 14:16:53.000000 promptwatch-0.1.0/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11067 2023-05-19 07:08:20.000000 promptwatch-0.1.0/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    25660 2023-05-19 07:10:20.000000 promptwatch-0.1.0/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-18 23:13:38.000000 promptwatch-0.1.0/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17876 2023-05-19 07:34:33.000000 promptwatch-0.1.0/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.063626 promptwatch-0.1.0/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-12 12:27:23.000000 promptwatch-0.1.0/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12091 2023-05-18 20:39:07.000000 promptwatch-0.1.0/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-17 23:04:57.000000 promptwatch-0.1.0/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13583 2023-05-18 23:34:47.000000 promptwatch-0.1.0/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.1.0/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 08:45:05.059424 promptwatch-0.1.0/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.1.0/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-19 08:45:05.000000 promptwatch-0.1.0/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.453308 promptwatch-0.1.1/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-19 13:00:54.453150 promptwatch-0.1.1/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.1.1/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.1.1/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-19 13:00:54.453353 promptwatch-0.1.1/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-19 10:25:10.000000 promptwatch-0.1.1/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.448601 promptwatch-0.1.1/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.450230 promptwatch-0.1.1/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      317 2023-05-19 13:00:45.000000 promptwatch-0.1.1/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11928 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5392 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.1.1/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1605 2023-05-19 07:02:23.000000 promptwatch-0.1.1/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.452032 promptwatch-0.1.1/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      153 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11067 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    25660 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17876 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.452921 promptwatch-0.1.1/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-19 12:57:26.000000 promptwatch-0.1.1/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13583 2023-05-19 10:25:10.000000 promptwatch-0.1.1/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.1.1/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-19 13:00:54.451377 promptwatch-0.1.1/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.1.1/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-19 13:00:54.000000 promptwatch-0.1.1/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.1.0/PKG-INFO` & `promptwatch-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: promptwatch
-Version: 0.1.0
-Summary: promptwatch.io python client to trace langchain sessions
-Home-page: https://github.com/blip-solutions/promptwatch-client
-Author: Juraj Bezdek
-Author-email: juraj.bezdek@blip.solutions
-License: MIT License
-Keywords: promptwatch prompt monitoring
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # PromptWatch.io ... session tracking for LangChain 
 
 It enables you to:
 - track all the chain executions
 - track LLM Prompts and **re-play the LLM runs** with the same input parameters and model settings to tweak your prompt template
 - track your costs per **project** and per **tenant** (your customer)
 
@@ -39,92 +27,54 @@
 
 ```
 
 Here you can get your API key: http://www.promptwatch.io/get-api-key (no registration needed)
 
 You can set it directly into `PromptWatch` constructor, or set is as an *ENV variable* `PROMPTWATCH_API_KEY`
 
-### Project and Tenant costs tracking
-
-You can assign a **project** and **tenant** id to your session by setting the constructor parameter:
-
-This will allow you to track costs per OpenAI request per customer and as well as your dev project.
-
-```python
-
-...
-
-with PromptWatch(tracking_project="my-project", tracking_tenant="my-tenant",) as pw:
-    my_chain("The quick brown fox jumped over")
-
-```
-### What is being tracked
-
-PromptWatch tracks all the details that LangChain exposes via its tracking "API" and more.
-
-👉 Chain execution inputs, outputs, execution time
+## Comprehensive Chain Execution Tracking
 
-👉 Tools input output
+With PromptWatch.io, you can track all chains, actions, retrieved documents, and more to gain complete visibility into your system. This makes it easy to identify issues with your prompts and quickly fix them for optimal performance.
 
-👉 **retrieved documents from retrieval vector DB**
+What sets PromptWatch.io apart is its intuitive and visual interface. You can easily drill down into the chains to find the root cause of any problems and get a clear understanding of what's happening in your system.
 
-👉 Details about LLM runs like:
+![](https://docs.promptwatch.io/assets/images/sessions_optimized.gif)
 
-  - final prompt text
-  - generated text
-  - execution details like model, temperature, etc. (everything you need to re-run the prompt with the same exact setup)
-  - total used tokens
-  - **costs (based on OpenAI price list per model)**
-  - **prompt template and its parameters**
-  
- 
+Read more here:
+[Chain tracing documentation](https://docs.promptwatch.io/docs/category/chain-tracing)
 
-### Custom logging
+## LLM Prompt caching
+It is often tha case that some of the prompts are repeated over an over. It is costly and slow. 
+With PromptWatch you just wrap your LLM model into our CachedLLM interface and it will automatically reuse previously generated values.
 
-PromptWatch tracks quite extensively standard LangChain tools, but if you have some custom code you'd like to track you can do so.
+Read more here:
+[Prompt caching documentation](https://docs.promptwatch.io/docs/caching)
 
-```python
-...
-with PromptWatch(api_key=invalid_api_key):
-    PromptWatch.log_activity(Question(text="What did the president say about Ketanji Brown Jackson"))
-    PromptWatch.log("my arbitrary log message")
-```
-
-All the logs are associated with to opened session. You can't log outside the session.
-
-```python
-...
-with PromptWatch(api_key=invalid_api_key):
-    PromptWatch.log_activity(Question(text="What did the president say about Ketanji Brown Jackson"))
-    #end of session   
-PromptWatch.log("this will raise an exception!")
-```
+## LLM Prompt Template Tweaking
 
+Tweaking prompt templates to find the optimal variation can be a time-consuming and challenging process, especially when dealing with multi-stage LLM chains. Fortunately, PromptWatch.io can help simplify the process!
 
-## Prompt template tracking
+With PromptWatch.io, you can easily experiment with different prompt variants by replaying any given LLM chain with the exact same inputs used in real scenarios. This allows you to fine-tune your prompts until you find the variation that works best for your needs.
 
-You can register any LangChain prompt template for detailed monitoring
+![](https://docs.promptwatch.io/assets/images/prompt_templates_optmized.gif)
 
-```python
-from promptwatch import PromptWatch, register_prompt_template
-from langchain import OpenAI, LLMChain, PromptTemplate
+Read more here:
+[Prompt tweaking documentation](https://docs.promptwatch.io/docs/prompt_tweaking)
 
-prompt_template = PromptTemplate.from_template("Finish this sentence {input}")
-my_chain = LLMChain(llm=OpenAI(), prompt=prompt_template)
 
-register_prompt_template("your_template_name",prompt_template) 
+## Keep Track of Your Prompt Template Changes
 
-with PromptWatch() as pw:
-    
-    #execute the chain
-    my_chain("The quick brown fox jumped over")
+Making changes to your prompt templates can be a delicate process, and it's not always easy to know what impact those changes will have on your system. Version control platforms like GIT are great for tracking code changes, but they're not always the best solution for tracking prompt changes.
 
-```
+![](https://docs.promptwatch.io/assets/images/prompt_templates_optmized.gif)
 
-This will allow you to associate the prompt template with a custom name (and function) and track it independently... 
+Read more here:
+[Prompt template versioning documentation](https://docs.promptwatch.io/docs/prompt_template_versioning)
 
-Any change of that template text will cause an automatic version change (with automatic version number increment)
 
-**Warning**
-The registration just assigns the template a custom name and is only done when the LLM actually executes the LLM prompt with that template. Therefore is has no additional performance costs, on the contrary it can even speed up the execution a bit if the same template is used multiple times.
 
+## Unit testing
+Unit tests will help you understand what impact your changes in Prompt templates and your code can have on representative sessions examples.
 
+![](https://docs.promptwatch.io/assets/images/unit_tests.png)
+Read more here:
+[Unit tests documentation](https://docs.promptwatch.io/docs/category/unit-testing)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `promptwatch-0.1.0/setup.py` & `promptwatch-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/caching.py` & `promptwatch-0.1.1/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/client.py` & `promptwatch-0.1.1/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/data_model.py` & `promptwatch-0.1.1/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/decorators.py` & `promptwatch-0.1.1/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/langchain/caching.py` & `promptwatch-0.1.1/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.1.1/src/promptwatch/langchain/langchain_support.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.1.1/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/promptwatch_context.py` & `promptwatch-0.1.1/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.1.1/src/promptwatch/unit_tests/evaluation.py`

 * *Files 12% similar despite different names*

```diff
@@ -184,14 +184,15 @@
 class TestCaseEvaluationWrapper:
 
     def __init__(self, test_session: "UnitTestSession", test_case:"TestCase") -> None:
         self.unit_test_session:UnitTestSession=test_session
         self.inner_test_case=test_case
         self.llm_prompt=None
         self.activity_id=None
+        self.iterations=0
         
         
         
     @property
     def inputs(self)->dict:
         return self.inner_test_case.inputs
     
@@ -221,28 +222,53 @@
         with UnitTest("my_test").for_template_name("my_template_name") as test:
             for example in test.test_cases():
                 example.evaluate(llmChain)
             
         ```
         
         """
+        if self.iterations==0:
+            # sanity checks
+            try:
+                from langchain import LLMChain
+                if self.unit_test_session.unit_test_run.conditions and self.unit_test_session.unit_test_run.conditions.for_template_name:
+                    # if we are running test for template, we expect to evaluate llm_chain.run method, not the instance itself
+                    if isinstance(result_generator, LLMChain):
+                        result_generator=result_generator.run
+                    
+            except ImportError as e:
+                # we ignore error if langchain cant be imported
+                pass
+
+
         try:
             generated = result_generator(self.inputs)
+            if self.unit_test_session.unit_test_run.conditions and self.unit_test_session.unit_test_run.conditions.for_template_name and not isinstance(generated, str):
+                raise Exception(f"we expect that the evaluated method/object to return a string for 'for_template_name' unit test, but got: {type(generated)}")
+                
+
             if hasattr(result_generator,"output_keys") and isinstance(generated,dict):
                 # langchain chains have input / output_keys and also options for return more than output. (return intermediate results, return only outputs etc.)
                 # we want to compare ONLY outputs
                 output_keys = result_generator.output_keys
                 #filter out the results
                 generated = {k:v for k,v in generated.items() if k in output_keys}
 
             self.evaluate_result(generated)
         except Exception as e:
+                
             self.mark_as_failed(str(e))
+            if "Missing some input keys:" in str(e):
+                # this is likely due to missing test memory...
+                raise Exception(f"Got exception {str(e)}. \nThis is likely due to missing test memory. Please see: docs.promptwatch.com/docs/unit_testing/unit_tests_reference_guide#langchain-test-memory")
+            
             if not continue_on_error:
                 raise e
+            
+        self.iterations+=1
 
     def skip(self):
         self.unit_test_session.skip()
 
     def mark_as_failed(self, error_description:str):
         """ Useful to log an error during the generation.
         Generally speaking, if you handle generation on your own, you should wrap it into try catch block so the test could continue. You can use this method to log the error and mark the results for this example as failed.
```

### Comparing `promptwatch-0.1.0/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.1.1/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.1.1/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch/utils.py` & `promptwatch-0.1.1/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.1.0/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.1.1/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

