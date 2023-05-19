# Comparing `tmp/auto-eval-0.1.9.tar.gz` & `tmp/auto-eval-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.1.9.tar", last modified: Wed May 10 10:56:57 2023, max compression
+gzip compressed data, was "auto-eval-0.2.0.tar", last modified: Fri May 19 09:38:15 2023, max compression
```

## Comparing `auto-eval-0.1.9.tar` & `auto-eval-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.588708 auto-eval-0.1.9/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.9/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    13658 2023-05-10 10:56:57.588509 auto-eval-0.1.9/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    13232 2023-05-09 07:43:05.000000 auto-eval-0.1.9/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.585940 auto-eval-0.1.9/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    13658 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      480 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-10 10:56:57.000000 auto-eval-0.1.9/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.586349 auto-eval-0.1.9/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.1.9/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     7022 2023-05-10 10:54:05.000000 auto-eval-0.1.9/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.586742 auto-eval-0.1.9/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.9/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3928 2023-05-08 07:55:11.000000 auto-eval-0.1.9/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.587553 auto-eval-0.1.9/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.9/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      775 2023-05-06 02:34:00.000000 auto-eval-0.1.9/eval/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     3092 2023-05-08 13:10:10.000000 auto-eval-0.1.9/eval/prompt_template/prompter.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-10 10:56:57.588137 auto-eval-0.1.9/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.9/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3108 2023-05-08 13:22:30.000000 auto-eval-0.1.9/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-10 10:56:57.588756 auto-eval-0.1.9/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      950 2023-05-10 10:54:54.000000 auto-eval-0.1.9/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:38:15.150509 auto-eval-0.2.0/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.0/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13744 2023-05-19 09:38:15.150273 auto-eval-0.2.0/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13318 2023-05-12 08:18:35.000000 auto-eval-0.2.0/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:38:15.147517 auto-eval-0.2.0/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13744 2023-05-19 09:38:15.000000 auto-eval-0.2.0/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-05-19 09:38:15.000000 auto-eval-0.2.0/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-19 09:38:15.000000 auto-eval-0.2.0/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-19 09:38:15.000000 auto-eval-0.2.0/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-19 09:38:15.000000 auto-eval-0.2.0/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-19 09:38:15.000000 auto-eval-0.2.0/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:38:15.148035 auto-eval-0.2.0/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.0/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7995 2023-05-19 09:34:38.000000 auto-eval-0.2.0/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:38:15.148487 auto-eval-0.2.0/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.0/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     5552 2023-05-19 08:57:24.000000 auto-eval-0.2.0/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:38:15.149362 auto-eval-0.2.0/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.0/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.0/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2083 2023-05-19 09:31:53.000000 auto-eval-0.2.0/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-19 09:38:15.149871 auto-eval-0.2.0/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.0/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3422 2023-05-18 04:08:41.000000 auto-eval-0.2.0/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-19 09:38:15.150569 auto-eval-0.2.0/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-05-19 09:18:00.000000 auto-eval-0.2.0/setup.py
```

### Comparing `auto-eval-0.1.9/LICENSE` & `auto-eval-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.9/PKG-INFO` & `auto-eval-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.9
+Version: 0.2.0
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -251,9 +251,10 @@
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
 
 ## ToDo
+- [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.1.9/README.md` & `auto-eval-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -239,9 +239,10 @@
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
 
 ## ToDo
+- [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.1.9/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.2.0/auto_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.9
+Version: 0.2.0
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -251,9 +251,10 @@
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
 
 ## ToDo
+- [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.1.9/eval/auto_llms_eval.py` & `auto-eval-0.2.0/eval/auto_llms_eval.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,67 +17,71 @@
 
 def eval_one_qa(
              api_tool: OneAPITool,
              eval_prompter: Prompter,
              question: str,
              candidate_answers: List[str],
              target: Union[str, None]='',
-             model: str='',
+             engine: str='',
              temperature=0.1,
              max_new_tokens=2048) -> Tuple[Union[List[float], None], str]:
     raw_response = ''
     eval_prompt = eval_prompter.generate_prompt(question, target,
                                                 candidate_answers)
     try:
         raw_response = api_tool.simple_chat(eval_prompt,
-                                      model=model,
+                                      model=engine,
                                       temperature=temperature,
                                       max_new_tokens=max_new_tokens)
         scores = eval_prompter.extract_result_from_response(raw_response)
         return scores, raw_response
     except Exception as e:
         print(f'error, request result:{raw_response}, exception:{e}')
         traceback.print_exc()
         return None, raw_response
 
 
 def eval_one_group(
     api_tool: OneAPITool,
     eval_prompter: Prompter,
     data_group: pd.DataFrame,
-    model: str='',
+    engine: str,
     temperature=0.1,
     max_new_tokens=2048,
 ) -> Union[pd.DataFrame, None]:
     group = data_group.reset_index()
+    valid_score_count = group['score'].map(lambda x: x if x != '' and x == x else None).count()
+    if 'score' in group.keys() and valid_score_count == len(group):
+        group['score'] = group['score'].map(float)
+        return group
     question = group['question'].unique()[0]
     candidate_answers = group['output']
     if 'target' in data_group.keys():
         target = group['target'].unique()[0]
     else:
         target = ''
     scores, raw_response = eval_one_qa(api_tool=api_tool,
                       eval_prompter=eval_prompter,
                       question=question,
                       candidate_answers=candidate_answers,
                       target=target,
-                      model=model,
+                      engine=engine,
                       temperature=temperature,
                       max_new_tokens=max_new_tokens)
     if scores is not None and len(scores) == len(candidate_answers):
         group.at[0, 'raw_response'] = raw_response
         for i in range(len(scores)):
             group.at[i, 'score'] = scores[i]
         return group
     else:
         return None
 
 
 
-def prepare_eval_data(eval_data_path: List[str], eval_categories: Optional[List[str]] = None, sample_num: int=0) -> List[pd.DataFrame]:
+def prepare_eval_data(eval_data_path: List[str], eval_categories: Optional[List[str]] = None, sample_num: int=0, eval_models: Optional[List[str]] = None) -> List[pd.DataFrame]:
     eval_data = df_reader(eval_data_path[0]) if len(eval_data_path) == 1 else pd.concat([df_reader(file_path) for file_path in eval_data_path])
     eval_data = eval_data.fillna('')
     if len({'instruction', 'input', 'output'} - set(eval_data.keys())) == 0:
         eval_data['question'] = eval_data['instruction'].str.cat(
             eval_data['input'], sep=' ')
     elif len({'prompt', 'output'} - set(eval_data.keys())) == 0:
         eval_data['quesion'] = eval_data['prompt'].copy()
@@ -89,85 +93,97 @@
         raise KeyError(
             f'Eval data columns must be either: ["instruction", "input", "output"] or ["prompt", "output"] or ["question", "output"]'
         )
     # filter specific categories
     if eval_categories is not None and len(
             eval_categories) > 0 and 'category' in eval_data.keys():
         eval_data = eval_data[eval_data['category'].isin(eval_categories)]
+    if eval_models is not None and len(
+            eval_models) > 0 and 'model' in eval_data.keys():
+        eval_data = eval_data[eval_data['model'].isin(eval_models)]
     grouped = eval_data.groupby(by=['question'])
     if sample_num > 0:
         sample_keys = random.sample(grouped.groups.keys(), sample_num)
     else:
         sample_keys = grouped.groups.keys()
     return [grouped.get_group(key) for key in sample_keys]
 
-def log_score_results(eval_results_df: pd.DataFrame):
+def log_score_results(eval_results_df: pd.DataFrame, score_by: List[str]):
     if 'model' in eval_results_df.keys():
-        print( eval_results_df.groupby('model')['score'])
         score_models = eval_results_df.groupby('model')['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}')
-        print(f'{"-"*20} Scores by Model {"-"*20}\n{score_models.to_markdown()}')
+        print(f'{"-"*20} Scores by \'model\' {"-"*20}\n{score_models.to_markdown()}')
         if 'category' in eval_results_df.keys():
             score_category = eval_results_df.groupby([
                 'model', 'category'
             ])['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').reset_index().sort_values(by=['category', 'model'])
             print(
-                f'\n{"-"*20} Scores by Model and Task Category {"-"*20}\n{score_category.to_markdown(index=False)}'
+                f'\n{"-"*20} Scores by [\'model\', \'category\'] {"-"*20}\n{score_category.to_markdown(index=False)}'
             )
+    if score_by is not None and len(score_by) > 0:
+        scores = eval_results_df.groupby(score_by)['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').reset_index().sort_values(by=score_by)
+        print(
+            f'\n{"-"*20} Scores by {score_by} {"-"*20}\n{scores.to_markdown(index=False)}'
+        )
+        
+def evaluation_prompt_acc(eval_result_df: pd.DataFrame):
+    if 'targe_score' in eval_result_df.keys():
+        pass
 
 def save_results(eval_results_df: pd.DataFrame, output_path: str):
     print(f'Saving evaluation results: {output_path}')
     df_saver(eval_results_df, output_path)
     print(f'Saved successfully.')
 
 @dataclass
 class EvalConfig:
     api_config_file: str
     eval_prompter: Prompter
     eval_data_path: str
     output_path: str = ''
-    model: str = ''
+    engine: str = ''
     eval_categories: Optional[List[str]] = None
+    eval_models: Optional[List[str]] = None
+    score_by: Optional[List[str]] = None
     sample_num: int = 0
     request_interval: int = 1
     retry: bool = True
-    verbose: bool = False
     temperature: float = 0.1
     max_new_tokens: int = 2048
 
 def eval_groups(
     eval_config: EvalConfig
 ):
     # Preparing data
-    eval_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.sample_num)
+    eval_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.sample_num, eval_config.eval_models)
 
     # Init api tool and prompter
     tool = OneAPITool.from_config_file(config_file=eval_config.api_config_file)
 
     eval_results = []
     failed_results = []
     for group in tqdm(eval_groups):
-        result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.model, eval_config.temperature, eval_config.max_new_tokens)
+        result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
         if result is not None:
             eval_results.append(result)
         else:
             failed_results.append(group)
         time.sleep(eval_config.request_interval)
 
     # Retry failed requests
     if len(failed_results) > 0 and eval_config.retry:
         for group in tqdm(failed_results.copy(), desc='RETRY'):
-            result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.model, eval_config.temperature, eval_config.max_new_tokens)
+            result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
             if result is not None:
                 eval_results.append(result)
                 failed_results = [df for df in failed_results if not df.equals(group)]
             time.sleep(eval_config.request_interval)
 
     eval_results.extend(failed_results)
     eval_results_df = pd.concat(eval_results)
-    log_score_results(eval_results_df=eval_results_df)
+    log_score_results(eval_results_df=eval_results_df, score_by=eval_config.score_by)
     # Log score results
-    print(f'Eval model: {eval_config.model}')
+    print(f'Eval engine: {eval_config.engine}')
     print(f'Eval files: {eval_config.eval_data_path}')
     print(f'Failed requests: {len(failed_results)}/{len(eval_groups)}')
     # Save results
     if eval_config.output_path:
         save_results(eval_results_df=eval_results_df, output_path=eval_config.output_path)
```

### Comparing `auto-eval-0.1.9/eval/prompt_template/prompter.py` & `auto-eval-0.2.0/eval/prompt_template/prompter.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
     def generate_prompt(self, question: str, target: str,
                         candidate_answers: List[str]) -> str:
         """
         Generate a prompt based on the given question, target, and candidate answers.
         """
         candidate_answer_numbers = generate_letters(len(candidate_answers))
-        format_option_data = '\n'.join([
-            f'**{candidate_answer_numbers[i]}**. {candidate_answers[i]}'
+        format_option_data = '\n\n'.join([
+            f'{candidate_answer_numbers[i]}. {candidate_answers[i]}'
             for i in range(len(candidate_answers))
         ])
 
         if target:
             eval_prompt = self.eval_with_target_template.format(
                 question=question, target=target, answers=format_option_data)
         else:
```

### Comparing `auto-eval-0.1.9/eval/utils/data_utils.py` & `auto-eval-0.2.0/eval/utils/data_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
  # -*- coding: utf-8 -*-
 import re
 import os
 import json
 import pandas as pd
+from typing import Union, List
 
 
-def df_reader(data_path) -> pd.DataFrame:
+def df_reader(data_path, header: Union[int, None] = 0, usecols: Union[List[Union[str, int]], None] = None ,sep='\t', sheet_name=0) -> pd.DataFrame:
     if data_path.endswith('json'):
         df_data = pd.read_json(data_path)
     if data_path.endswith('jsonl'):
         df_data = pd.read_json(data_path, lines=True)
     elif data_path.endswith('xlsx'):
-        df_data = pd.read_excel(data_path)
+        df_data = pd.read_excel(data_path, header=header, usecols=usecols, sheet_name=sheet_name)
+    elif data_path.endswith('.pkl'):
+        df_data = pd.read_pickle(data_path)
     elif data_path.endswith('csv'):
-        df_data = pd.read_csv(data_path)
+        df_data = pd.read_csv(data_path, header=header, usecols=usecols, sep=sep)
     else:
         raise AssertionError(f'not supported file type:{data_path}, suport types: json, jsonl, xlsx, csv')
     return df_data
 
 def df_saver(df: pd.DataFrame, data_path):
     if data_path.endswith('json'):
         df.to_json(df, orient='records', force_ascii=False)
```

### Comparing `auto-eval-0.1.9/setup.py` & `auto-eval-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.1.9",
+    version="0.2.0",
     packages=find_packages(),
-    package_data={
-      "eval":["prompt_template/eval_prompt_template.json"]  
-    },
+    # package_data={
+    #   "eval":["prompt_template/eval_prompt_template.json"]  
+    # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
         "pandas",
         "openpyxl",
         "tabulate",
         "XlsxWriter"
```

