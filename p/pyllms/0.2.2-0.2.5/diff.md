# Comparing `tmp/pyllms-0.2.2.tar.gz` & `tmp/pyllms-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.2.2.tar", last modified: Sat May 13 02:07:11 2023, max compression
+gzip compressed data, was "pyllms-0.2.5.tar", last modified: Fri May 19 21:49:26 2023, max compression
```

## Comparing `pyllms-0.2.2.tar` & `pyllms-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-13 02:07:11.011228 pyllms-0.2.2/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.2.2/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    16541 2023-05-13 02:07:11.010860 pyllms-0.2.2/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    15228 2023-04-29 05:43:17.000000 pyllms-0.2.2/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-13 02:07:11.006742 pyllms-0.2.2/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.2.2/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    18384 2023-05-07 04:00:58.000000 pyllms-0.2.2/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-13 02:07:11.009199 pyllms-0.2.2/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      228 2023-04-23 02:39:46.000000 pyllms-0.2.2/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2159 2023-05-07 04:00:58.000000 pyllms-0.2.2/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3769 2023-05-07 04:00:58.000000 pyllms-0.2.2/llms/providers/aleph.py
--rw-r--r--   0 prelovac   (502) staff       (20)     9195 2023-05-13 01:46:47.000000 pyllms-0.2.2/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1565 2023-05-07 04:00:58.000000 pyllms-0.2.2/llms/providers/base_provider.py
--rw-r--r--   0 prelovac   (502) staff       (20)     4701 2023-05-07 04:00:58.000000 pyllms-0.2.2/llms/providers/cohere.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3517 2023-05-13 02:04:37.000000 pyllms-0.2.2/llms/providers/huggingface.py
--rw-r--r--   0 prelovac   (502) staff       (20)     7943 2023-05-07 04:00:58.000000 pyllms-0.2.2/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-13 02:07:11.010495 pyllms-0.2.2/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    16541 2023-05-13 02:07:10.000000 pyllms-0.2.2/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      419 2023-05-13 02:07:11.000000 pyllms-0.2.2/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-05-13 02:07:10.000000 pyllms-0.2.2/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)      109 2023-05-13 02:07:10.000000 pyllms-0.2.2/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-05-13 02:07:10.000000 pyllms-0.2.2/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-05-13 02:07:11.011315 pyllms-0.2.2/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1917 2023-05-13 02:06:48.000000 pyllms-0.2.2/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 21:49:26.306997 pyllms-0.2.5/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.2.5/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    38271 2023-05-19 21:49:26.306713 pyllms-0.2.5/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    36916 2023-05-19 21:24:06.000000 pyllms-0.2.5/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 21:49:26.301324 pyllms-0.2.5/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.2.5/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    20934 2023-05-19 21:40:32.000000 pyllms-0.2.5/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 21:49:26.304687 pyllms-0.2.5/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      263 2023-05-13 02:47:09.000000 pyllms-0.2.5/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2108 2023-05-13 03:43:25.000000 pyllms-0.2.5/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3970 2023-05-19 21:15:15.000000 pyllms-0.2.5/llms/providers/aleph.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     8999 2023-05-13 10:20:16.000000 pyllms-0.2.5/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1618 2023-05-13 03:43:25.000000 pyllms-0.2.5/llms/providers/base_provider.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     4582 2023-05-19 21:16:49.000000 pyllms-0.2.5/llms/providers/cohere.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2632 2023-05-17 23:38:37.000000 pyllms-0.2.5/llms/providers/google.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3465 2023-05-13 03:43:25.000000 pyllms-0.2.5/llms/providers/huggingface.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     7452 2023-05-13 08:50:17.000000 pyllms-0.2.5/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 21:49:26.306323 pyllms-0.2.5/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    38271 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      444 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)      109 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-05-19 21:49:26.000000 pyllms-0.2.5/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-05-19 21:49:26.307068 pyllms-0.2.5/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1962 2023-05-19 21:48:21.000000 pyllms-0.2.5/setup.py
```

### Comparing `pyllms-0.2.2/LICENSE` & `pyllms-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.2.2/llms/llms.py` & `pyllms-0.2.5/llms/llms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
 import os
+import re
 import statistics
 from prettytable import PrettyTable
 from .providers import OpenAIProvider
 from .providers import AnthropicProvider
 from .providers import AI21Provider
 from .providers import CohereProvider
 from .providers import AlephAlphaProvider
 from .providers import HuggingfaceHubProvider
+from .providers import GoogleProvider
 import concurrent.futures
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import List, Optional, Tuple
 
 
 class Result:
     def __init__(self, results):
@@ -105,14 +107,16 @@
                 and single_model in HuggingfaceHubProvider.MODEL_INFO
             ):
                 self._providers.append(
                     HuggingfaceHubProvider(
                         api_key=huggingfacehub_api_key, model=single_model
                     )
                 )
+            elif single_model in GoogleProvider.MODEL_INFO:
+                self._providers.append(GoogleProvider(model=single_model))
             else:
                 raise ValueError("Invalid API key and model combination", single_model)
 
     def __repr__(self) -> str:
         return f"LLMS({self.model})"
 
     @property
@@ -125,14 +129,15 @@
         all_providers = [
             OpenAIProvider,
             AI21Provider,
             AnthropicProvider,
             CohereProvider,
             AlephAlphaProvider,
             HuggingfaceHubProvider,
+            GoogleProvider,
         ]
 
         for provider in all_providers:
             for model, cost in provider.MODEL_INFO.items():
                 if query and (
                     (query.lower() not in model.lower())
                     and (query.lower() not in provider.__name__.lower())
@@ -181,87 +186,143 @@
 
     async def acomplete(
         self,
         prompt: str,
         **kwargs,
     ):
         if self.n_provider > 1:
-            tasks = [provider.acomplete(prompt, **kwargs) for provider in self._providers]
+            tasks = [
+                provider.acomplete(prompt, **kwargs) for provider in self._providers
+            ]
             results = await asyncio.gather(*tasks, return_exceptions=False)
             return Result(results)
 
         else:
             provider = self._providers[0]
             result = await provider.acomplete(prompt, **kwargs)
             return Result(result)
 
     def complete_stream(self, prompt, **kwargs):
         if len(self._providers) > 1:
             raise ValueError("Streaming is possible only with a single model")
 
         yield from self._providers[0].complete_stream(prompt, **kwargs)
 
-    def benchmark(self, prompts=None, evaluator=None, show_outputs=False, html=False):
-        if not prompts:
-            prompts = [
-                "What is the capital of the country where Christopher Columbus was born?",
-                "A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?",
-                "Solve the quadratic equation: x^2 - 5x + 6 = 0",
-                "How much is 7! * 3! -1234.5 ?",
-                'translate this sentence by alternating words in gemran and french "it was a beautiful day that thursday and I want skiing outside. it started raining soon although they said it won\'t be until friday, so I went to the pool instead"',
-                "Convert December 21 · 1:00 – 1:50pm pacific to asia/taipei time",
-                "In my kitchen there's a table with a cup with a ball inside. I moved the cup to my bed in my bedroom and turned the cup upside down. I grabbed the cup again and moved to the main room. Where's the ball now?",
-                'Capture the essence of this in exactly 7 words: "There’s much that divides us in Northern Ireland though one thing is guaranteed to bring us together: local phrases. Call it slang, call it colloquialisms, we all know only too well how important words are to where we’re from . . . and when it comes to the phrases that make us ‘us,’ we’ve got a lot to say. While you don’t need advance knowledge of the words to fit in, well, it helps. How else will you know where ‘foundered’ sits on the scale of warm to freezing? Or deciding whether that new car purchase is more ‘clinker’ than ‘beezer’? Or appreciating that ‘grand’ can mean exactly that or anything but? If the best way to get to know a nation is to understand their language, then surely tourists must be at times confused about what comes out of our mouths. Throughout the island of Ireland, we have utterly brilliant ways to verbally express ourselves.“I think it’s really important,” says Dr Frank Ferguson, research director for English Language and Literature at Ulster University, about the vitality of slang as part of language."',
-                "Write a Python function that takes a list of integers as input and returns the length of the longest increasing subsequence. An increasing subsequence is a subsequence of the given list where the elements are in strictly increasing order. Your function should have an efficient solution with a time complexity better than O(n^2), where n is the length of the input list. Output only code with no explainations and provide example usage.",
-                "Write a Python function that takes a list of integers as input and returns the maximum sum of non-adjacent elements in the list. The function should return 0 if the input list is empty. Your function should have an efficient solution with a time complexity of O(n), where n is the length of the input list. Output only code with no explainations and provide example usage.",
-                "You are given a 2D binary matrix filled with 0's and 1's. Your task is to write a JavaScript function that finds the largest rectangle containing only 1's and returns its area. Your function should have an efficient solution with a time complexity better than O(n^3), where n is the total number of elements in the input matrix. Output only code with no explainations and provide example usage.",
-                "Given the following messy and unstructured data, extract the names, email addresses, and phone numbers of the individuals listed:\
+    def benchmark(self, problems=None, evaluator=None, show_outputs=False, html=False):
+        if not problems:
+          
+            problems = [
+               
+                (
+                    "A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?",
+                    "pull",
+                ),
+                ("Solve the quadratic equation: x^2 - 5x + 6 = 0", "x=2, x=3"),
+                ("How much is 7! * 3! -1234.5 ?", "29005.5"),
+                (
+                    'translate this sentence by alternating words in gemran and french "it was a beautiful day that thursday and I want skiing outside. it started raining soon although they said it won\'t be until friday, so I went to the pool instead"',
+                    "",
+                ),
+                ("Convert December 21 1:50pm pacific to taipei time", "5:50 am"),
+                (
+                    "In my kitchen there's a table with a cup with a ball inside. I moved the cup to my bed in my bedroom and turned the cup upside down. I grabbed the cup again and moved to the main room. Where's the ball now?",
+                    "on the bed in the bedroom",
+                ),
+                (
+                    'Capture the essence of this in exactly 7 words: "There’s much that divides us in Northern Ireland though one thing is guaranteed to bring us together: local phrases. Call it slang, call it colloquialisms, we all know only too well how important words are to where we’re from . . . and when it comes to the phrases that make us ‘us,’ we’ve got a lot to say. While you don’t need advance knowledge of the words to fit in, well, it helps. How else will you know where ‘foundered’ sits on the scale of warm to freezing? Or deciding whether that new car purchase is more ‘clinker’ than ‘beezer’? Or appreciating that ‘grand’ can mean exactly that or anything but? If the best way to get to know a nation is to understand their language, then surely tourists must be at times confused about what comes out of our mouths. Throughout the island of Ireland, we have utterly brilliant ways to verbally express ourselves.“I think it’s really important,” says Dr Frank Ferguson, research director for English Language and Literature at Ulster University, about the vitality of slang as part of language."',
+                    "Make sure the answer has exactly 7 words",
+                ),
+                (
+                    "Write a Python function that takes a list of integers as input and returns the length of the longest increasing subsequence. An increasing subsequence is a subsequence of the given list where the elements are in strictly increasing order. Your function should have an efficient solution with a time complexity better than O(n^2), where n is the length of the input list. Output only code with no explainations and provide example usage.",
+                    "",
+                ),
+                (
+                    "Write a Python function that takes a list of integers as input and returns the maximum sum of non-adjacent elements in the list. The function should return 0 if the input list is empty. Your function should have an efficient solution with a time complexity of O(n), where n is the length of the input list. Output only code with no explainations and provide example usage.",
+                    "",
+                ),
+                (
+                    "You are given a 2D binary matrix filled with 0's and 1's. Your task is to write a JavaScript function that finds the largest rectangle containing only 1's and returns its area. Your function should have an efficient solution with a time complexity better than O(n^3), where n is the total number of elements in the input matrix. Output only code with no explainations and provide example usage.",
+                    "",
+                ),
+                (
+                    "Given the following messy and unstructured data, extract the clean names, email addresses, and phone numbers (as digits) of the individuals listed:\
 John Doe - johndoe (at) email.com (five-five-five) one-two-three-four-five-six-seven\
 random text not a phone 123 4468888\
 Jane Smith\
 random text 2, cinque-cinque-cinque-\
 nove-otto-sette-sei-quattro-tre\
 janesmith en email punto com\
 texto aleatorio 3\
 Bob Johnson - first name dot last name dot wild🐻@email.com\
 texto aleatorio 4 código de área five-five-five teléfono: eins-eins-eins-zwei-zwei-zwei-zwei",
+                    "Name: John Doe\
+Email: johndoe@email.com \
+Phone: 5551234567\
+\
+Name: Jane Smith \
+Email: janesmith@email.com\
+Phone: 5559876432\
+\
+Name: Bob Johnson\
+Email: first.name.wild🐻@email.com\
+Phone: 5551112222\
+",
+                ),
+                ("write three sentences each ending with the word apple", ""),
+                ("Please count the number of t in eeooeotetto", "3"),
+                (
+                    "Use m to substitute p, a to substitute e, n to substitute a, g to substitute c, o to substitute h,\
+how to spell peach under this rule?",
+                    "mango",
+                ),
+                (
+                    "two workers paint the fence in 8 hours. how long will it take one worker paint the same fence if they are injured and need to take a 30 min break after every hour of work?",
+                    "5.5 hours",
+                ),
+                ("5+55+555+5555+55555-1725=", "60000"),
+                ("-2-2-2-2-2-2*-2*-2=", "-18"),
+                ('what is the 13th letter of the word "supralapsarian"', 'a'),
+                ('Vlad\'s uncle can still beat him in sprinting although he is 30 years younger. who is "he" referring to?', 'Vlad'),
+                ("Belgium uses 160 million litres of petrol each day. Three is enough petrol stored to last 60 days. how much more petrol does Belgium need to buy to have enough stored for 90 days. A) 4 million litres, B) 4,8 million litres, C) 480 million litres D) 160 million litres E) 4800 million litres", "E) 4800 million litres"),
+                ("The sum of three numbers is 96. The first number is 6 times the third number, and the third number is 40 less than the second number. What is the absolute value of the difference between the first and second numbers?", "5"),
+                ("The least common multiple of a positive integer n and 18 is 180, and the greatest common divisor of n and 45 is 15. What is the sum of the digits of n?", "n = 60 thus the answer is 6"),
+                ("what square is the black king on in this chess position: 1Bb3BN/R2Pk2r/1Q5B/4q2R/2bN4/4Q1BK/1p6/1bq1R1rb w - - 0 1", "e7")
+
             ]
 
         def evaluate_answers(
             evaluator, query_answer_pairs: List[Tuple[str, str]]
         ) -> List[int]:
             system = """
-            You are a truthful evaluator of the capabilties of other AI models.
-
-You are given a list of queries and answers by an AI model. For each query first think about  the solution yourself, then score the reply of the other AI, compared to yours on a scale 0 to 5 (5 being great).
-
-For example:
-
-Query: What is the capital of the country where Christopher Columbus was born?
-Answer: Christopher Columbus was born in Genoa, Italy.
-
-Query : A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?
-Answer: You should push the door. The reason for this is that the mirror writing is intended for people on the other side of the door to read, not for you. So, if you push the door, you will be pushing it in the direction that the people on the other side are expecting it to move.
-
-
-Christopher Columbus was born in the Republic of Genoa, which is now part of Italy. The capital of Italy is Rome. So you would score it 1 (it is wrong answer, but city was correct)
-Since the word "push" is written in mirror writing, it suggests that the instruction is intended for people on the other side of the door. Therefore, you should pull the door to open it. You would score this 0 (it is wrong)
-
-
-Your only output should be a list of comma seperated integers representing your evaluation score for each answer. No other output is allowed. For example above your output will be:
-0, 1
+You are given a problem and answer by a student. Sometimes the correct solution will be provided with the problem as a hint, but if it is not, then first think about the solution yourself, then score the solution of the student's solution with one of these scores:
+0 - Incorrect solution
+3 - Correct solution
 
+Your output should be using this template:
+Score: #
 """
+            scores = []
+            for i, (query, hint, answer) in enumerate(query_answer_pairs, start=1):
+                if not len(hint):
+                    prompt = f"Problem: {query}\nStudent solution: {answer}"
+                else:
+                    prompt = f"Problem: {query}\nHint (correct answer): {hint}\nStudent solution: {answer}"
+#                print(prompt)
+                evaluator_result = evaluator.complete(
+                    prompt, system_message=system
+                ).text
+#                print(evaluator_result)
+                found = re.search(r"Score: (\d+)", evaluator_result)
+                if found:
+                    scores.append(int(found.group(1)))
+                else:
+                    print("No score found!", evaluator_result)
 
-            prompt = "".join(f"Query #{i}: {query}\nAnswer #{i}: {answer}\n\n"
-                             for i, (query, answer) in enumerate(query_answer_pairs, start=1))
-
-            evaluator_result = evaluator.complete(prompt, system_message=system).text
-            scores = evaluator_result.split(",")
-            return [int(score.strip()) for score in scores]
+#            print(scores)
+            return scores
 
         model_results = {}
 
         def process_prompt(model, prompt, index):
             print(model, index)
             result = model.complete(prompt, max_tokens=1000, temperature=0)
             output_data = {
@@ -273,25 +334,25 @@
             }
             return output_data
 
         def process_prompts_sequentially(model, prompts):
             results = []
             with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
                 futures = [
-                    executor.submit(process_prompt, model, prompt, index)
+                    executor.submit(process_prompt, model, prompt[0], index)
                     for index, prompt in enumerate(prompts)
                 ]
                 for future in concurrent.futures.as_completed(futures):
                     results.append(future.result())
             return model, results
 
         # Run completion tasks in parallel for each model, but sequentially for each prompt within a model
         with ThreadPoolExecutor() as executor:
             futures = [
-                executor.submit(process_prompts_sequentially, model, prompts)
+                executor.submit(process_prompts_sequentially, model, problems)
                 for model in self._providers
             ]
 
             for future in as_completed(futures):
                 model, outputs = future.result()
                 model_results[model] = {
                     "outputs": outputs,
@@ -316,23 +377,27 @@
         if evaluator:
             for model in model_results:
                 all_query_answer_pairs = []
                 model_data = model_results[model]
                 for output_data in model_data["outputs"]:
                     prompt_index = output_data["prompt_index"]
                     all_query_answer_pairs.append(
-                        (prompts[prompt_index], output_data["text"])
+                        (
+                            problems[prompt_index][0],
+                            problems[prompt_index][1],
+                            output_data["text"],
+                        )
                     )
 
                 evaluation = evaluate_answers(evaluator, all_query_answer_pairs)
                 # Add evaluation to results
                 model_results[model]["evaluation"] = []
                 for i in range(len(model_results[model]["outputs"])):
                     model_results[model]["evaluation"].append(evaluation[i])
-
+            print(model_results)
             sorted_models = sorted(
                 model_results,
                 key=lambda x: model_results[x]["aggregated_speed"]
                 * sum(model_results[x]["evaluation"]),
                 reverse=True,
             )
         else:
@@ -398,15 +463,16 @@
                     str(model),
                     f"Total Tokens: {total_tokens}",
                     f"Total Cost: {model_data['total_cost']:.5f}",
                     f"Median Latency: {model_data['median_latency']:.2f}",
                     f"Aggregated speed: {total_tokens/model_data['total_latency']:.2f}",
                 ]
             if evaluator:
-                row_data.append(f"Total Score: {total_score}")
+                acc=100*total_score/(3*len(model_data["evaluation"]))
+                row_data.append(f"Accuracy: {acc:.2f}%")
 
             table.add_row(row_data)
 
         if not html:
             return table
         else:
             return table.get_html_string()
```

### Comparing `pyllms-0.2.2/llms/providers/ai21.py` & `pyllms-0.2.5/llms/providers/ai21.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,31 +43,31 @@
     ):
         model_input = self._prepare_model_input(
             prompt=prompt,
             temperature=temperature,
             max_tokens=max_tokens,
             **kwargs,
         )
-        with self.track_latency() as latency:
+        with self.track_latency():
             response = ai21.Completion.execute(model=self.model, **model_input)
 
         completion = response.completions[0].data.text.strip()
         prompt_tokens = len(response.prompt.tokens)
         completion_tokens = len(response.completions[0].data.tokens)
         total_tokens = prompt_tokens + completion_tokens
 
-        cost = self.compute_cost(prompt_tokens=prompt_tokens,
-                                 completion_tokens=completion_tokens
-                                 )
+        cost = self.compute_cost(
+            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        )
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
```

### Comparing `pyllms-0.2.2/llms/providers/aleph.py` & `pyllms-0.2.5/llms/providers/aleph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # llms/providers/aleph.py
 
 import os
 
 from aleph_alpha_client import AsyncClient, Client, CompletionRequest, Prompt
 
 from .base_provider import BaseProvider
-
+import tiktoken
 
 class AlephAlphaProvider(BaseProvider):
     MODEL_INFO = {
         "luminous-base": {"prompt": 6.6, "completion": 7.6, "token_limit": 2048},
         "luminous-extended": {"prompt": 9.9, "completion": 10.9, "token_limit": 2048},
         "luminous-supreme": {"prompt": 38.5, "completion": 42.5, "token_limit": 2048},
         "luminous-supreme-control": {
@@ -25,14 +25,18 @@
         self.client = Client(api_key)
         self.async_client = AsyncClient(api_key)
 
         if model is None:
             model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
+    def count_tokens(self, content: str):
+        enc = tiktoken.encoding_for_model("gpt-3.5-turbo")
+        return len(enc.encode(content))
+
     def _prepare_model_input(
         self,
         prompt: str,
         temperature: float = 0,
         max_tokens: int = 300,
         **kwargs,
     ) -> CompletionRequest:
@@ -53,22 +57,22 @@
         temperature: float = 0,
         max_tokens: int = 300,
         **kwargs,
     ):
         model_input = self._prepare_model_input(
             prompt=prompt, temperature=temperature, max_tokens=max_tokens, **kwargs
         )
-        with self.track_latency() as latency:
+        with self.track_latency():
             response = self.client.complete(request=model_input, model=self.model)
 
         completion = response.completions[0].completion.strip()
 
         # Calculate tokens and cost
-        prompt_tokens = -1
-        completion_tokens = -1
+        prompt_tokens = self.count_tokens(prompt)
+        completion_tokens = self.count_tokens(completion)
 
         total_tokens = prompt_tokens + completion_tokens
 
         cost = self.compute_cost(
             prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
         )
 
@@ -76,15 +80,15 @@
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
 
     async def acomplete(
         self,
         prompt: str,
```

### Comparing `pyllms-0.2.2/llms/providers/anthropic.py` & `pyllms-0.2.5/llms/providers/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,51 +48,52 @@
                 return json_body
 
     async def acompletion(self, **kwargs):
         # Override original method which pass kwargs as params.
         # We will pass kwargs in
         # _arequest_as_json will strips-off the keyword arguments that it needs
         # and pass the rest as params
-        return await self._arequest_as_json(
-            "post",
-            "/v1/complete",
-            **kwargs
-        )
+        return await self._arequest_as_json("post", "/v1/complete", **kwargs)
 
 
 class AnthropicProvider(BaseProvider):
     MODEL_INFO = {
-        "claude-instant-v1.1": {"prompt": 1.63, "completion": 5.51, "token_limit": 9000},
+        "claude-instant-v1.1": {
+            "prompt": 1.63,
+            "completion": 5.51,
+            "token_limit": 9000,
+        },
         "claude-instant-v1": {"prompt": 1.63, "completion": 5.51, "token_limit": 9000},
         "claude-v1": {"prompt": 11.02, "completion": 32.68, "token_limit": 9000},
+        "claude-v1-100k": {"prompt": 11.02, "completion": 32.68, "token_limit": 100000},
     }
 
     def __init__(self, api_key=None, model=None):
         if model is None:
             model = list(self.MODEL_INFO.keys())[0]
         self.model = model
 
         if api_key is None:
             api_key = os.getenv("ANTHROPIC_API_KEY")
         self.client = AnthropicClient(api_key)
 
     def count_tokens(self, content: str):
         return anthropic.count_tokens(content)
 
-    def _prepare_model_input(self,
-                             prompt: str,
-                             history: Optional[List[dict]] = None,
-                             temperature: float = 0,
-                             max_tokens: int = 300,
-                             stop_sequences: Optional[List[str]] = None,
-                             ai_prompt: str = "",
-                             stream: bool = False,
-                             **kwargs,
-                             ):
-
+    def _prepare_model_input(
+        self,
+        prompt: str,
+        history: Optional[List[dict]] = None,
+        temperature: float = 0,
+        max_tokens: int = 300,
+        stop_sequences: Optional[List[str]] = None,
+        ai_prompt: str = "",
+        stream: bool = False,
+        **kwargs,
+    ):
         formatted_prompt = (
             f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}{ai_prompt}"
         )
 
         if history is not None:
             history_text_list = []
             for message in history:
@@ -119,15 +120,15 @@
             stop_sequences = [anthropic.HUMAN_PROMPT]
         model_input = {
             "prompt": formatted_prompt,
             "temperature": temperature,
             "max_tokens_to_sample": max_tokens_to_sample,
             "stop_sequences": stop_sequences,
             "stream": stream,
-            **kwargs
+            **kwargs,
         }
         return model_input
 
     def complete(
         self,
         prompt: str,
         history: Optional[List[dict]] = None,
@@ -150,36 +151,36 @@
             temperature=temperature,
             max_tokens=max_tokens,
             stop_sequences=stop_sequences,
             ai_prompt=ai_prompt,
             **kwargs,
         )
 
-        with self.track_latency() as latency:
+        with self.track_latency():
             response = self.client.completion(model=self.model, **model_input)
 
         completion = response["completion"].strip()
 
         # Calculate tokens and cost
         prompt_tokens = anthropic.count_tokens(model_input["prompt"])
         completion_tokens = anthropic.count_tokens(response["completion"])
         total_tokens = prompt_tokens + completion_tokens
-        cost = self.compute_cost(prompt_tokens=prompt_tokens,
-                                 completion_tokens=completion_tokens
-                                 )
+        cost = self.compute_cost(
+            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        )
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
 
     async def acomplete(
         self,
         prompt: str,
@@ -201,35 +202,35 @@
             history=history,
             temperature=temperature,
             max_tokens=max_tokens,
             stop_sequences=stop_sequences,
             ai_prompt=ai_prompt,
             **kwargs,
         )
-        with self.track_latency() as latency:
+        with self.track_latency():
             response = await self.client.acompletion(model=self.model, **model_input)
         completion = response["completion"].strip()
 
         # Calculate tokens and cost
         prompt_tokens = anthropic.count_tokens(model_input["prompt"])
         completion_tokens = anthropic.count_tokens(response["completion"])
         total_tokens = prompt_tokens + completion_tokens
 
-        cost = self.compute_cost(prompt_tokens=prompt_tokens,
-                                 completion_tokens=completion_tokens
-                                 )
+        cost = self.compute_cost(
+            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        )
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
 
     def complete_stream(
         self,
         prompt: str,
```

### Comparing `pyllms-0.2.2/llms/providers/base_provider.py` & `pyllms-0.2.5/llms/providers/base_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,32 +3,36 @@
 
 
 class BaseProvider:
     """Base class for all providers.
     Methods will raise NotImplementedError if they are not overwritten.
     """
 
+    def __init__(self):
+        self.latency = None
+
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} ({self.model})"
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.model})"
 
     @contextmanager
-    def track_latency(self) -> float:
+    def track_latency(self):
         start = time.perf_counter()
-        elapsed = time.perf_counter() - start
-        elapsed = round(elapsed, 2)
-        yield elapsed
+        try:
+            yield
+        finally:
+            self.latency = round(time.perf_counter() - start, 2)
 
     def compute_cost(self, prompt_tokens: int, completion_tokens: int) -> float:
         cost_per_token = self.MODEL_INFO[self.model]
         cost = (
-            (prompt_tokens * cost_per_token["prompt"]) +
-            (completion_tokens * cost_per_token["completion"])
+            (prompt_tokens * cost_per_token["prompt"])
+            + (completion_tokens * cost_per_token["completion"])
         ) / 1_000_000
         cost = round(cost, 5)
         return cost
 
     def count_tokens(self):
         raise NotImplementedError(
             f"Count tokens is currently not supported with {self.__name__}"
```

### Comparing `pyllms-0.2.2/llms/providers/cohere.py` & `pyllms-0.2.5/llms/providers/cohere.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,41 +57,41 @@
     ):
         model_input = self._prepare_model_input(
             prompt=prompt,
             temperature=temperature,
             max_tokens=max_tokens,
             **kwargs,
         )
-        with self.track_latency() as latency:
+        with self.track_latency():
             response = self.client.generate(
                 model=self.model,
                 **model_input,
             )
 
         completion = response.generations[0].text.strip()
 
         # Calculate tokens and cost
-        # prompt_tokens = len(self.client.tokenize(prompt)) # too slow for normal use
-        # completion_tokens =len(self.client.tokenize(completion))
-        prompt_tokens = -1
-        completion_tokens = -1
+        prompt_tokens = self.count_tokens(prompt) # too slow for normal use
+        completion_tokens = self.count_tokens(completion)
+        #prompt_tokens = -1
+        #completion_tokens = -1
         total_tokens = prompt_tokens + completion_tokens
-        cost = self.compute_cost(prompt_tokens=prompt_tokens,
-                                 completion_tokens=completion_tokens
-                                 )
+        cost = self.compute_cost(
+            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        )
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
 
     async def acomplete(
         self,
         prompt: str,
@@ -101,42 +101,42 @@
     ):
         model_input = self._prepare_model_input(
             prompt=prompt,
             temperature=temperature,
             max_tokens=max_tokens,
             **kwargs,
         )
-        with self.track_latency() as latency:
+        with self.track_latency():
             async with self.async_client() as client:
                 response = await client.generate(
                     model=self.model,
                     **model_input,
                 )
 
         completion = response.generations[0].text.strip()
 
         # Calculate tokens and cost
         # prompt_tokens = len(self.client.tokenize(prompt)) # too slow for normal use
         # completion_tokens =len(self.client.tokenize(completion))
         prompt_tokens = -1
         completion_tokens = -1
         total_tokens = prompt_tokens + completion_tokens
-        cost = self.compute_cost(prompt_tokens=prompt_tokens,
-                                 completion_tokens=completion_tokens
-                                 )
+        cost = self.compute_cost(
+            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        )
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
 
     def complete_stream(
         self,
         prompt: str,
```

### Comparing `pyllms-0.2.2/llms/providers/huggingface.py` & `pyllms-0.2.5/llms/providers/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         },
         "hf_llava": {
             "full": "liuhaotian/LLaVA-Lightning-MPT-7B-preview",
             "prompt": 0,
             "completion": 0,
             "token_limit": 2048,
         },
-
         "hf_dolly": {
             "full": "databricks/dolly-v2-12b",
             "prompt": 0,
             "completion": 0,
             "token_limit": -1,
         },
     }
@@ -82,43 +81,43 @@
     ):
         prompt, params = self._prepare_model_input(
             prompt=prompt,
             temperature=temperature,
             max_tokens=max_tokens,
             **kwargs,
         )
-        with self.track_latency() as latency:
+        with self.track_latency():
             response = self.client(inputs=prompt, params=params)
 
         if "error" in response:
             print("Error: ", response["error"])
             return {}
 
         completion = response[0]["generated_text"][len(prompt) :]
 
         # Calculate tokens and cost
         prompt_tokens = -1
         completion_tokens = -1
 
         total_tokens = prompt_tokens + completion_tokens
 
-        cost = self.compute_cost(prompt_tokens=prompt_tokens,
-                                 completion_tokens=completion_tokens
-                                 )
+        cost = self.compute_cost(
+            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        )
         cost_per_token = self.MODEL_INFO[self.model]
         cost = (
             (prompt_tokens * cost_per_token["prompt"])
             + (completion_tokens * cost_per_token["completion"])
         ) / 1_000_000
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
```

### Comparing `pyllms-0.2.2/llms/providers/openai.py` & `pyllms-0.2.5/llms/providers/openai.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from .base_provider import BaseProvider
 
 
 class OpenAIProvider(BaseProvider):
     # cost is per million tokens
     MODEL_INFO = {
-        "gpt-3.5-turbo": {"prompt": 2.0, "completion": 2.0, "token_limit": 4000},
-        "gpt-4": {"prompt": 30.0, "completion": 60.0, "token_limit": 8000},
-        "text-davinci-003": {"prompt": 20.0, "completion": 20.0, "token_limit": 4097}
+        "gpt-3.5-turbo": {"prompt": 2.0, "completion": 2.0, "token_limit": 4096},
+        "gpt-4": {"prompt": 30.0, "completion": 60.0, "token_limit": 8192},
+        "text-davinci-003": {"prompt": 20.0, "completion": 20.0, "token_limit": 4096},
     }
 
     def __init__(self, api_key, model=None):
         openai.api_key = api_key
         if model is None:
             model = list(self.MODEL_INFO.keys())[0]
         self.model = model
@@ -25,32 +25,32 @@
     def is_chat_model(self):
         return self.model.startswith("gpt")
 
     def count_tokens(self, content: str):
         enc = tiktoken.encoding_for_model(self.model)
         return len(enc.encode(content))
 
-    def _prepapre_model_input(self,
-                              prompt: str,
-                              history: Optional[List[dict]] = None,
-                              system_message: Optional[List[dict]] = None,
-                              temperature: float = 0,
-                              max_tokens: int = 300,
-                              stream: bool = False,
-                              **kwargs,
-                              ):
-
+    def _prepapre_model_input(
+        self,
+        prompt: str,
+        history: Optional[List[dict]] = None,
+        system_message: str = None,
+        temperature: float = 0,
+        max_tokens: int = 300,
+        stream: bool = False,
+        **kwargs,
+    ):
         if self.is_chat_model:
             messages = [{"role": "user", "content": prompt}]
 
             if history:
                 messages = [*history, *messages]
 
             if system_message:
-                messages = [*system_message, *messages]
+                messages = [{"role": "system", "content": system_message}, *messages]
 
             model_input = {
                 "messages": messages,
                 "temperature": temperature,
                 "max_tokens": max_tokens,
                 "stream": stream,
                 **kwargs,
@@ -93,43 +93,43 @@
 
         model_input = self._prepapre_model_input(
             prompt=prompt,
             history=history,
             system_message=system_message,
             temperature=temperature,
             max_tokens=max_tokens,
-            **kwargs
+            **kwargs,
         )
 
-        with self.track_latency() as latency:
+        with self.track_latency():
             response = self.client.create(model=self.model, **model_input)
 
         if self.is_chat_model:
             completion = response.choices[0].message.content.strip()
         else:
             completion = response.choices[0].text.strip()
 
         usage = response.usage
         prompt_tokens = usage["prompt_tokens"]
         completion_tokens = usage["completion_tokens"]
         total_tokens = usage["total_tokens"]
 
-        cost = self.compute_cost(prompt_tokens=prompt_tokens,
-                                 completion_tokens=completion_tokens
-                                 )
+        cost = self.compute_cost(
+            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        )
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,  # Add tokens_prompt to meta
                 "tokens_completion": completion_tokens,  # Add tokens_completion to meta
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
 
     async def acomplete(
         self,
         prompt: str,
@@ -151,43 +151,43 @@
 
         model_input = self._prepapre_model_input(
             prompt=prompt,
             history=history,
             system_message=system_message,
             temperature=temperature,
             max_tokens=max_tokens,
-            **kwargs
+            **kwargs,
         )
 
-        with self.track_latency() as latency:
+        with self.track_latency():
             response = await self.client.acreate(model=self.model, **model_input)
 
         if self.is_chat_model:
             completion = response.choices[0].message.content.strip()
         else:
             completion = response.choices[0].text.strip()
 
         usage = response.usage
         prompt_tokens = usage["prompt_tokens"]
         completion_tokens = usage["completion_tokens"]
         total_tokens = usage["total_tokens"]
 
-        cost = self.compute_cost(prompt_tokens=prompt_tokens,
-                                 completion_tokens=completion_tokens
-                                 )
+        cost = self.compute_cost(
+            prompt_tokens=prompt_tokens, completion_tokens=completion_tokens
+        )
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,  # Add tokens_prompt to meta
                 "tokens_completion": completion_tokens,  # Add tokens_completion to meta
                 "cost": cost,
-                "latency": latency,
+                "latency": self.latency,
             },
             "provider": str(self),
         }
 
     def complete_stream(
         self,
         prompt: str,
@@ -199,27 +199,29 @@
     ):
         """
         Args:
             history: messages in OpenAI format, each dict must include role and content key.
             system_message: system messages in OpenAI format, must have role and content key.
               It can has name key to include few-shots examples.
         """
-        model_input = self._prepapre_model_input(prompt=prompt,
-                                                 history=history,
-                                                 system_message=system_message,
-                                                 temperature=temperature,
-                                                 max_tokens=max_tokens,
-                                                 stream=True,
-                                                 **kwargs
-                                                 )
+        model_input = self._prepapre_model_input(
+            prompt=prompt,
+            history=history,
+            system_message=system_message,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            stream=True,
+            **kwargs,
+        )
         response = self.client.create(model=self.model, **model_input)
 
         if self.is_chat_model:
             chunk_generator = (
-                chunk["choices"][0].get("delta", {}).get("content") for chunk in response
+                chunk["choices"][0].get("delta", {}).get("content")
+                for chunk in response
             )
         else:
             chunk_generator = (
                 chunk["choices"][0].get("text", "") for chunk in response
             )
 
         while not (first_text := next(chunk_generator)):
```

### Comparing `pyllms-0.2.2/setup.py` & `pyllms-0.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.2.2",
-    description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.",
+    version="0.2.5",
+    description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, Google Palm2/Vertex, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
         "openai",
@@ -38,14 +38,14 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Human Machine Interfaces",
         "Topic :: Text Processing",
     ],
     python_requires=">=3.7",
-    keywords="llm, llms, large language model, AI, NLP, natural language processing, gpt, chatgpt, openai, anthropic, ai21, cohere, aleph alpha, huggingface hub",
+    keywords="llm, llms, large language model, AI, NLP, natural language processing, gpt, chatgpt, openai, anthropic, ai21, cohere, aleph alpha, huggingface hub, vertex ai, palm, palm2",
     project_urls={
         "Documentation": _project_homepage,
         "Source Code": _project_homepage,
         "Issue Tracker": _project_homepage+"/issues",
     },
 )
```

