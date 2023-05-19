# Comparing `tmp/prompt_optimizer-0.1.0.tar.gz` & `tmp/prompt_optimizer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_optimizer-0.1.0.tar", max compression
+gzip compressed data, was "prompt_optimizer-0.2.0.tar", max compression
```

## Comparing `prompt_optimizer-0.1.0.tar` & `prompt_optimizer-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-04-09 00:01:22.989764 prompt_optimizer-0.1.0/LICENSE
--rw-r--r--   0        0        0     4302 2023-05-18 07:34:33.987684 prompt_optimizer-0.1.0/README.md
--rw-r--r--   0        0        0      472 2023-05-17 23:15:55.921964 prompt_optimizer-0.1.0/prompt_optimizer/__init__.py
--rw-r--r--   0        0        0      234 2023-04-08 22:38:34.428079 prompt_optimizer-0.1.0/prompt_optimizer/metric/__init__.py
--rw-r--r--   0        0        0     3070 2023-05-18 07:18:34.646759 prompt_optimizer-0.1.0/prompt_optimizer/metric/base.py
--rw-r--r--   0        0        0     1821 2023-05-16 21:01:33.834335 prompt_optimizer-0.1.0/prompt_optimizer/metric/bertscore_metric.py
--rw-r--r--   0        0        0     1672 2023-05-16 21:01:31.280863 prompt_optimizer-0.1.0/prompt_optimizer/metric/token_metric.py
--rw-r--r--   0        0        0     1197 2023-05-17 23:15:48.057206 prompt_optimizer-0.1.0/prompt_optimizer/poptim/__init__.py
--rw-r--r--   0        0        0     1362 2023-05-17 22:33:26.389519 prompt_optimizer-0.1.0/prompt_optimizer/poptim/autocorrect_optim.py
--rw-r--r--   0        0        0     5817 2023-05-18 07:20:14.758428 prompt_optimizer-0.1.0/prompt_optimizer/poptim/base.py
--rw-r--r--   0        0        0     4310 2023-05-17 22:38:32.536567 prompt_optimizer-0.1.0/prompt_optimizer/poptim/entropy_optim.py
--rw-r--r--   0        0        0     1817 2023-05-17 22:33:40.183305 prompt_optimizer-0.1.0/prompt_optimizer/poptim/lemmatizer_optim.py
--rw-r--r--   0        0        0      550 2023-04-08 22:37:20.803999 prompt_optimizer-0.1.0/prompt_optimizer/poptim/logger.py
--rw-r--r--   0        0        0     4690 2023-05-17 22:55:00.605397 prompt_optimizer-0.1.0/prompt_optimizer/poptim/name_replace_optim.py
--rw-r--r--   0        0        0     2331 2023-05-17 22:34:03.105862 prompt_optimizer-0.1.0/prompt_optimizer/poptim/pulp_optim.py
--rw-r--r--   0        0        0     1117 2023-05-17 22:07:26.149628 prompt_optimizer-0.1.0/prompt_optimizer/poptim/punctuation_optim.py
--rw-r--r--   0        0        0     1376 2023-05-17 22:54:59.573788 prompt_optimizer-0.1.0/prompt_optimizer/poptim/sequential.py
--rw-r--r--   0        0        0     1629 2023-05-17 22:34:11.859961 prompt_optimizer-0.1.0/prompt_optimizer/poptim/stemmer_optim.py
--rw-r--r--   0        0        0     1892 2023-05-17 22:34:15.632495 prompt_optimizer-0.1.0/prompt_optimizer/poptim/stop_word_optim.py
--rw-r--r--   0        0        0     3414 2023-05-17 22:34:19.734542 prompt_optimizer-0.1.0/prompt_optimizer/poptim/synonym_replace_optim.py
--rw-r--r--   0        0        0     2657 2023-05-17 23:03:52.834747 prompt_optimizer-0.1.0/prompt_optimizer/poptim/utils.py
--rw-r--r--   0        0        0     1668 2023-05-18 07:12:10.082147 prompt_optimizer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5054 1970-01-01 00:00:00.000000 prompt_optimizer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-09 00:01:22.989764 prompt_optimizer-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5307 2023-05-19 19:11:38.420996 prompt_optimizer-0.2.0/README.md
+-rw-r--r--   0        0        0      609 2023-05-19 03:03:11.410726 prompt_optimizer-0.2.0/prompt_optimizer/__init__.py
+-rw-r--r--   0        0        0      234 2023-04-08 22:38:34.428079 prompt_optimizer-0.2.0/prompt_optimizer/metric/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-18 08:41:28.963678 prompt_optimizer-0.2.0/prompt_optimizer/metric/base.py
+-rw-r--r--   0        0        0     2007 2023-05-19 02:42:52.321714 prompt_optimizer-0.2.0/prompt_optimizer/metric/bertscore_metric.py
+-rw-r--r--   0        0        0     1925 2023-05-19 03:03:01.423169 prompt_optimizer-0.2.0/prompt_optimizer/metric/token_metric.py
+-rw-r--r--   0        0        0     1027 2023-05-18 23:02:51.540434 prompt_optimizer-0.2.0/prompt_optimizer/poptim/__init__.py
+-rw-r--r--   0        0        0     1709 2023-05-19 03:03:01.415647 prompt_optimizer-0.2.0/prompt_optimizer/poptim/autocorrect_optim.py
+-rw-r--r--   0        0        0     5997 2023-05-18 23:01:02.911660 prompt_optimizer-0.2.0/prompt_optimizer/poptim/base.py
+-rw-r--r--   0        0        0     5122 2023-05-19 03:03:01.454647 prompt_optimizer-0.2.0/prompt_optimizer/poptim/entropy_optim.py
+-rw-r--r--   0        0        0     2109 2023-05-19 03:03:01.455363 prompt_optimizer-0.2.0/prompt_optimizer/poptim/lemmatizer_optim.py
+-rw-r--r--   0        0        0      550 2023-05-18 22:59:18.835561 prompt_optimizer-0.2.0/prompt_optimizer/poptim/logger.py
+-rw-r--r--   0        0        0     5180 2023-05-19 03:03:01.459575 prompt_optimizer-0.2.0/prompt_optimizer/poptim/name_replace_optim.py
+-rw-r--r--   0        0        0     2583 2023-05-19 03:03:01.433793 prompt_optimizer-0.2.0/prompt_optimizer/poptim/pulp_optim.py
+-rw-r--r--   0        0        0     1397 2023-05-19 03:03:01.427258 prompt_optimizer-0.2.0/prompt_optimizer/poptim/punctuation_optim.py
+-rw-r--r--   0        0        0     1447 2023-05-18 23:01:02.902907 prompt_optimizer-0.2.0/prompt_optimizer/poptim/sequential.py
+-rw-r--r--   0        0        0     1427 2023-05-19 03:03:01.438454 prompt_optimizer-0.2.0/prompt_optimizer/poptim/stemmer_optim.py
+-rw-r--r--   0        0        0     1683 2023-05-19 03:03:01.444802 prompt_optimizer-0.2.0/prompt_optimizer/poptim/stop_word_optim.py
+-rw-r--r--   0        0        0     3162 2023-05-19 03:03:01.465816 prompt_optimizer-0.2.0/prompt_optimizer/poptim/synonym_replace_optim.py
+-rw-r--r--   0        0        0     6164 2023-05-18 23:01:03.800340 prompt_optimizer-0.2.0/prompt_optimizer/poptim/utils.py
+-rw-r--r--   0        0        0       93 2023-05-18 08:28:30.775249 prompt_optimizer-0.2.0/prompt_optimizer/visualize/__init__.py
+-rw-r--r--   0        0        0     1033 2023-05-18 08:36:23.277116 prompt_optimizer-0.2.0/prompt_optimizer/visualize/stringdiffer.py
+-rw-r--r--   0        0        0     1691 2023-05-19 19:33:43.305769 prompt_optimizer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 prompt_optimizer-0.2.0/PKG-INFO
```

### Comparing `prompt_optimizer-0.1.0/LICENSE` & `prompt_optimizer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.1.0/README.md` & `prompt_optimizer-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-# PromptOptimizer
-Minimize LLM token complexity to save API costs and model computations.
+<div align="center">
 
-[![lint](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/lint.yml/badge.svg)](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/lint.yml) [![test](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/test.yml/badge.svg)](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/test.yml) [![linkcheck](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/linkcheck.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+  ## PromptOptimizer
+  
+  <img width="200" src="evaluations/artifacts/logo.png" alt="kevin inspired logo" />
+
+  Minimize LLM token complexity to save API costs and model computations.
+
+</div>
+<div align="center">
+
+[![lint](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/lint.yml/badge.svg)](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/lint.yml) 
+[![test](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/test.yml/badge.svg)](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/test.yml) 
+[![linkcheck](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/linkcheck.yml) 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+[Docs](https://promptoptimizer.readthedocs.io/en/latest/)
+
+</div>
 
 
 # Features
 - **Plug and Play Optimizers:** Minimize token complexity using optimization methods without any access to weights, logits or decoding algorithm. Directly applicable to virtually all NLU systems.
 - **Protected Tags:** Special protected tags to mark important sections of prompt that should not be removed/modified.
-- **Multiple Input Format Support:** Optmization of string, batches of strings and JSON prompt data with an option to skip system prompts.
 - **Sequential Optimization:** Chain different optimizers together sequentially.
 - **Optimization Metrics:** Number of tokens reduced and semantic similarity before and after optimization.
-- **Langhcain Support:** Supports langchain style prompt chains.
+- **Langhcain and JSON Support:** Supports langchain style prompt chains and OpenAI request JSON Object.
  
 # Why?
 - **Minimize Token Complexity:** Token Complexity is the amount of prompt tokens required to achieve a given task. Reducing token complexity corresponds to linearly reducing API costs and quadratically reducing computational complexity of usual transformer models.
 - **Save Money:** For large businesses, saving 10% on token count can lead to saving 100k USD per 1M USD.
 - **Extend Limitations:** Some models have small context lengths, prompt optimizers can help them process larger than context documents.
 
-# Why does it work?
-1. LLMs are powerful, they can infill missing information.
-2. Natural language is bulky, large words and phrases can be replaced by smaller ones.
-
 | Prompt | # Tokens | Correct Response? |  
 | ------------------------------------------------------- | ---------- | ------------------- |  
 | Who is the president of the United States of America? | 11 | ✅ |  
 | Who president US | 3  (-72%) | ✅ |
 
 # Installation
 ### Quick Installation
 ```pip install prompt-optimizer```
 
 ### Install from source
 ```bash
-git clone https://github.com/TimeTraveller-San/prompt-optimizer.git;
+git clone https://github.com/vaibkumr/prompt-optimizer.git;
 cd prompt-optimizer;
 pip install -e .
 ```
 
 # Disclaimer
 There is a compression vs performance tradeoff -- the increase in compression comes at the cost of loss in model performance. The tradeoff can be greatly mitigated by chosing the right optimize for a given task. There is no single optimizer for all cases. There is no Adam here.
 
@@ -50,24 +60,45 @@
 prompt = """The Belle Tout Lighthouse is a decommissioned lighthouse and British landmark located at Beachy Head, East Sussex, close to the town of Eastbourne."""
 p_optimizer = EntropyOptim(verbose=True, p=0.1)
 optimized_prompt = p_optimizer(prompt)
 print(optimized_prompt)
 
 ```
 # Evaluations
-Following are the results for [logiqa](https://github.com/openai/evals/blob/main/evals/registry/evals/logiqa.yaml) OpenAI evals task. It is only performed for first 100 samples. Please note the results over this task are not true for all other tasks, more thorough testing and domain knowledge is needed to choose the optimal optimizer.
+Following are the results for [logiqa](https://github.com/openai/evals/blob/main/evals/registry/evals/logiqa.yaml) OpenAI evals task. It is only performed for a subset of first 100 samples. Please note the optimizer performance over this task should not be generalized to other tasks, more thorough testing and domain knowledge is needed to choose the optimal optimizer.
 
 | Name | % Tokens Reduced | LogiQA Accuracy | USD Saved Per $100 |
 | --- | --- | --- | --- |
 | Default | 0.0 | 0.32 | 0.0 |
 | Entropy_Optim_p_0.05 | 0.06 | 0.3 | 6.35 |
 | Entropy_Optim_p_0.1 | 0.11 | 0.28 | 11.19 |
 | Entropy_Optim_p_0.25 | 0.26 | 0.22 | 26.47 |
 | Entropy_Optim_p_0.5 | 0.5 | 0.08 | 49.65 |
 | SynonymReplace_Optim_p_1.0 | 0.01 | 0.33 | 1.06 |
 | Lemmatizer_Optim | 0.01 | 0.33 | 1.01 |
-| Stemmer_Optim | -0.06 | 0.09 | -5.91 |
 | NameReplace_Optim | 0.01 | 0.34 | 1.13 |
 | Punctuation_Optim | 0.13 | 0.35 | 12.81 |
 | Autocorrect_Optim | 0.01 | 0.3 | 1.14 |
 | Pulp_Optim_p_0.05 | 0.05 | 0.31 | 5.49 |
 | Pulp_Optim_p_0.1 | 0.1 | 0.25 | 9.52 |
+
+# Cost-Performance Tradeoff
+The reduction in cost often comes with a loss in LLM performance. Almost every optimizer have hyperparameters that control this tradeoff. 
+
+For example, in `EntropyOptim` the hyperparamter `p`, a floating point number between 0 and 1 controls the ratio of tokens to remove. `p=1.0` corresponds to removing all tokens while `p=0.0` corresponds to removing none. 
+
+The following chart shows the trade-off for different values of `p` as evaluated on the OpenAI evals [logiqa](https://github.com/openai/evals/blob/main/evals/registry/evals/logiqa.yaml) task for a subset of first 100 samples.
+
+<div align="center">
+  <img src="evaluations/artifacts/tradeoff.png" alt="tradeoff" />
+</div>
+
+# Contributing
+There are several directions to contribute to. Please see [CONTRIBUTING.md](.github/CONTRIBUTING.md) for contribution guidelines and possible future directions.
+
+# Social
+Contact us on twitter [Vaibhav Kumar](https://twitter.com/vaibhavk1o1) and [Vaibhav Kumar](https://twitter.com/vaibhavk97).
+
+# Inspiration
+<div align="center">
+  <img src="evaluations/artifacts/kevin.gif" alt="Image" />
+</div>
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/metric/base.py` & `prompt_optimizer-0.2.0/prompt_optimizer/metric/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         n = 0
         for pb, pa in zip(prompts_before, prompts_after):
             if json:
                 if skip_system and pb["role"] == "system":
                     continue
                 else:
                     res = self.run_json(pb, pa)
+                    n += 1
 
             elif langchain:
                 if skip_system and pb.role == "system":
                     continue
                 else:
                     res = self.run(pb.content, pa.content)
                     n += 1
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/metric/bertscore_metric.py` & `prompt_optimizer-0.2.0/prompt_optimizer/metric/bertscore_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from prompt_optimizer.metric.base import Metric
 
 
 class BERTScoreMetric(Metric):
     """
     BERTScoreMetric is a metric that calculates precision, recall, and F1 score based on BERT embeddings.
     It inherits from the Metric base class.
+
+    Example:
+        >>> from prompt_optimizer.metric import BERTScoreMetric
+        >>> metric = BERTScoreMetric()
+        >>> res = metric("default prompt...", "optimized prompt...")
     """
 
     def __init__(self):
         super().__init__()
         self.tokenizer = AutoTokenizer.from_pretrained("bert-base-uncased")
         self.model = AutoModelForSequenceClassification.from_pretrained(
             "bert-base-uncased", num_labels=2
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/metric/token_metric.py` & `prompt_optimizer-0.2.0/prompt_optimizer/metric/token_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 
 from prompt_optimizer.metric.base import Metric
 
 
 class TokenMetric(Metric):
     """
     TokenMetric is a metric that calculates the optimization ratio based on the number of tokens reduced.
+    It uses `tiktoken` to tokenize strings and count the number of tokens.
 
     It inherits from the Metric base class.
+
+    Example:
+        >>> from prompt_optimizer.metric import TokenMetric
+        >>> metric = TokenMetric()
+        >>> res = metric("default prompt...", "optimized prompt...")
     """
 
     def __init__(self, tokenizer: str = "cl100k_base"):
         """
         Initializes the TokenMetric.
 
         Args:
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/__init__.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 import logging
 
-import nltk
-
 from prompt_optimizer.poptim.autocorrect_optim import AutocorrectOptim
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 from prompt_optimizer.poptim.entropy_optim import EntropyOptim
 from prompt_optimizer.poptim.lemmatizer_optim import LemmatizerOptim
 from prompt_optimizer.poptim.name_replace_optim import NameReplaceOptim
 from prompt_optimizer.poptim.pulp_optim import PulpOptim
 from prompt_optimizer.poptim.punctuation_optim import PunctuationOptim
 from prompt_optimizer.poptim.sequential import Sequential
 from prompt_optimizer.poptim.stemmer_optim import StemmerOptim
 from prompt_optimizer.poptim.stop_word_optim import StopWordOptim
 from prompt_optimizer.poptim.synonym_replace_optim import SynonymReplaceOptim
 
-nltk.download("wordnet")
-nltk.download("punkt")
-nltk.download("averaged_perceptron_tagger")
-nltk.download("maxent_ne_chunker")
-nltk.download("words")
-
 __all__ = [
     "Sequential",
-    "PromptOptimize",
+    "PromptOptim",
     "LemmatizerOptim",
     "StopWordOptim",
     "NameReplaceOptim",
     "PunctuationOptim",
     "PulpOptim",
     "StemmerOptim",
     "AutocorrectOptim",
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/autocorrect_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/autocorrect_optim.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from autocorrect import Speller
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class AutocorrectOptim(PromptOptimize):
+class AutocorrectOptim(PromptOptim):
     """
     AutocorrectOptim is a prompt optimization technique that applies autocorrection to the prompt text.
+    Correctly spelled words have less token count than incorrect ones. This is useful in scenarios where
+    human client types the text.
 
-    It inherits from the PromptOptimize base class.
+    It inherits from the PromptOptim base class.
+
+    Example:
+        >>> from prompt_optimizer.poptim import AutocorrectOptim
+        >>> p_optimizer = AutocorrectOptim()
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
     """
 
     def __init__(self, fast: bool = False, verbose: bool = False, metrics: list = []):
         """
         Initializes the AutocorrectOptim.
 
         Args:
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/base.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import copy
 from abc import ABC, abstractmethod
 
 from .logger import logger
-from .utils import protected_runner
+from .utils import DotDict, protected_runner
 
 
-class PromptOptimize(ABC):
+class PromptOptim(ABC):
     """
-    PromptOptimize is an abstract base class for prompt optimization techniques.
+    PromptOptim is an abstract base class for prompt optimization techniques.
 
     It defines the common structure and interface for prompt optimization.
 
     This class inherits from ABC (Abstract Base Class).
     """
 
     def __init__(
         self, verbose: bool = False, metrics: list = [], protect_tag: str = None
     ):
         """
-        Initializes the PromptOptimize.
+        Initializes the PromptOptim.
 
         Args:
             verbose (bool, optional): Flag indicating whether to enable verbose output. Defaults to False.
             metrics (list, optional): A list of metric names to evaluate during optimization. Defaults to an empty list.
             protect_tag (str, optional): markup style tag string to indicate protected content that can't be deleted or modified. Defaults to `None`.
         """
         self.verbose = verbose
@@ -63,41 +63,43 @@
 
         Args:
             json_data (dict): The JSON data object.
 
         Returns:
             dict: The JSON data object with the content field replaced by the optimized prompt text.
         """
-        for data in json_data:
+        optim_json_data = copy.deepcopy(json_data)
+
+        for data in optim_json_data:
             if skip_system and data["role"] == "system":
                 continue
             data["content"] = self.run(data["content"])
-        return json_data
-    
+        return optim_json_data
+
     def run_langchain(self, langchain_data: list, skip_system: bool = False):
         """
         Runs the prompt optimizer on langchain chat data.
 
         Args:
             langchain_data (list): The langchain data containing 'type' and 'content' fields.
             skip_system (bool, optional): Whether to skip data with type 'system'. Defaults to False.
 
         Returns:
             list: The modified langchain data.
 
-        """        
+        """
 
         optim_langchain_data = copy.deepcopy(langchain_data)
 
         for data in optim_langchain_data:
             if skip_system and data.type == "system":
                 continue
             data.content = self.run(data.content)
 
-        return optim_langchain_data    
+        return optim_langchain_data
 
     # def batch_run(
     #     self, data: list, skip_system: bool = False, json: bool = True
     # ) -> list:
     #     """
     #     Applies prompt optimization to a batch of data.
 
@@ -140,15 +142,17 @@
             AssertionError: If skip_system is True and json is False.
 
         """
 
         assert not (json and langchain), "Data type can't be both json and langchain"
 
         if skip_system:
-            assert json or langchain, "Can't skip system prompts without batched json format"
+            assert (
+                json or langchain
+            ), "Can't skip system prompts without batched json format"
 
         if json:
             opti_prompt_data = self.run_json(prompt_data, skip_system)
         elif langchain:
             opti_prompt_data = self.run_langchain(prompt_data, skip_system)
         else:
             opti_prompt_data = self.run(prompt_data)
@@ -167,8 +171,12 @@
         if self.verbose:
             logger.info(f"Prompt Data Before: {prompt_data}")
             logger.info(f"Prompt Data After: {opti_prompt_data}")
             for metric_result in metric_results:
                 for key in metric_result:
                     logger.info(f"{key}: {metric_result[key]:.3f}")
 
-        return opti_prompt_data
+        result = DotDict()
+        result.content = opti_prompt_data
+        result.metrics = metric_results
+
+        return result
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/entropy_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/entropy_optim.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 import numpy as np
 import torch
 from transformers import AutoModelForMaskedLM, AutoTokenizer
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class EntropyOptim(PromptOptimize):
+class EntropyOptim(PromptOptim):
     """
-    EntropyOptim is a prompt optimization technique based on entropy values.
+    EntropyOptim is a prompt optimization technique based on entropy values of tokens.
+    A masked language model (`bert-base-cased` by default) is used to compute probabilities
+    of observing the current token based on right and left context. These probability values
+    are further used to compute the entropy values. Optimizer then moves on to remove the
+    tokens corresponding to lowest `p` percentile entropies.
+
+    The intuition of this method is that the model can infill low entropy i.e. low surprise
+    or highly probable tokens through the context. I will probably write a paper to explain
+    this in more detail.
+
+    `EntropyOptim` inherits from the PromptOptim base class.
+
+    Example:
+        >>> from prompt_optimizer.poptim import EntropyOptim
+        >>> p_optimizer = EntropyOptim(p=0.1)
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
 
-    It inherits from the PromptOptimize base class.
     """
 
     def __init__(
         self,
         model_name: str = "bert-base-cased",
-        p: float = 0.9,
+        p: float = 0.1,
         verbose: bool = False,
         metrics: list = [],
         **kwargs,
     ):
         """
         Initializes the EntropyOptim.
 
         Args:
             model_name (str, optional): The name of the pretrained masked language model. Defaults to "bert-base-cased".
-            p (float, optional): The percentile cutoff value for selecting tokens. Defaults to 0.9.
+            p (float, optional): The percentile cutoff value for selecting tokens. Defaults to `0.1`. Higher `p` means more compression.
             verbose (bool, optional): Flag indicating whether to enable verbose output. Defaults to False.
             metrics (list, optional): A list of metric names to evaluate during optimization. Defaults to an empty list.
         """
         super().__init__(verbose, metrics, **kwargs)
         self.p = p * 100
         self.model_name = model_name
         self.load_mlm_model_tokenizer()
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/lemmatizer_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/lemmatizer_optim.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import nltk
 from nltk.corpus import wordnet
 from nltk.stem import WordNetLemmatizer
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class LemmatizerOptim(PromptOptimize):
+class LemmatizerOptim(PromptOptim):
     """
     LemmatizerOptim is a prompt optimization technique based on lemmatization.
 
-    It inherits from the PromptOptimize base class.
+    It inherits from the PromptOptim base class.
+
+    Example:
+        >>> from prompt_optimizer.poptim import LemmatizerOptim
+        >>> p_optimizer = LemmatizerOptim()
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
     """
 
     def __init__(self, verbose: bool = False, metrics: list = []):
         """
         Initializes the LemmatizerOptim.
 
         Args:
             verbose (bool, optional): Flag indicating whether to enable verbose output. Defaults to False.
             metrics (list, optional): A list of metric names to evaluate during optimization. Defaults to an empty list.
         """
         super().__init__(verbose, metrics)
         self.lemmatizer = WordNetLemmatizer()
+        nltk.download("averaged_perceptron_tagger")
+        nltk.download("wordnet")
 
     def get_wordnet_pos(self, word: str) -> str:
         """
         Maps the POS tag from NLTK to WordNet POS tags.
 
         Args:
             word (str): The word to determine the POS tag.
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/logger.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/logger.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/name_replace_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/name_replace_optim.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 import nltk
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class NameReplaceOptim(PromptOptimize):
+class NameReplaceOptim(PromptOptim):
     """
     NameReplaceOptim is a prompt optimization technique based on replacing names in the prompt.
-
-    It inherits from the PromptOptimize base class.
+    Some names have lower token count (1) than others. Higher token count names can be replaced by
+    such names to reduce token complexity. `self.opti_names` contains the pre-made list of such names
+    for `tiktokenizer`. The list will need to be modified for other tokenizers.
+
+    It inherits from the PromptOptim base class.
+
+    Example:
+        >>> from prompt_optimizer.poptim import NameReplaceOptim
+        >>> p_optimizer = NameReplaceOptim()
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
     """
 
     def __init__(self, verbose: bool = False, metrics: list = []):
         """
         Initializes the NameReplaceOptim.
 
         Args:
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/pulp_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/pulp_optim.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from pulp import LpBinary, LpMinimize, LpProblem, LpVariable, lpSum
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class PulpOptim(PromptOptimize):
+class PulpOptim(PromptOptim):
     """
     PulpOptim is a prompt optimization technique based on integer linear programming using the Pulp library.
 
-    It inherits from the PromptOptimize base class.
+    It inherits from the PromptOptim base class.
+
+    Example:
+        >>> from prompt_optimizer.poptim import PulpOptim
+        >>> p_optimizer = PulpOptim(p=0.1)
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
     """
 
-    def __init__(self, p: float = 0.4, verbose: bool = False, metrics: list = []):
+    def __init__(self, p: float = 0.1, verbose: bool = False, metrics: list = []):
         """
         Initializes the PulpOptim.
 
         Args:
-            p (float, optional): The aggression factor controlling the reduction in the number of tokens. Defaults to 0.4.
+            p (float, optional): The aggression factor controlling the reduction in the number of tokens. Defaults to 0.1. Higher `p` corresponds to lower token output count.
             verbose (bool, optional): Flag indicating whether to enable verbose output. Defaults to False.
             metrics (list, optional): A list of metric names to evaluate during optimization. Defaults to an empty list.
         """
         super().__init__(verbose, metrics)
         self.aggression = p  # will reduce num tokens by aggression*100%
 
     def optimize(self, prompt: str) -> str:
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/punctuation_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/punctuation_optim.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import string
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class PunctuationOptim(PromptOptimize):
+class PunctuationOptim(PromptOptim):
     """
     PunctuationOptim is a prompt optimization technique that removes punctuation marks from the prompt.
+    LLMs can infer punctuations themselves in most cases, remove them.
 
-    It inherits from the PromptOptimize base class.
+    It inherits from the PromptOptim base class.
+
+    Example:
+        >>> from prompt_optimizer.poptim import PunctuationOptim
+        >>> p_optimizer = PunctuationOptim()
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
     """
 
     def __init__(self, verbose: bool = False, metrics: list = [], **kwargs):
         """
         Initializes the PunctuationOptim.
 
         Args:
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/sequential.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/sequential.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, List
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
+
+from .utils import DotDict
 
 
 class Sequential:
     """
     Sequential is a class that represents a sequential composition of prompt optimization techniques.
 
     It applies a series of optimization techniques in sequence to the prompt.
@@ -21,29 +23,31 @@
         *optims: Variable-length argument list of prompt optimization techniques.
 
     Attributes:
         optims (list): A list of prompt optimization techniques.
 
     """
 
-    def __init__(self, *optims: PromptOptimize):
+    def __init__(self, *optims: PromptOptim):
         """
         Initializes the Sequential object with the specified prompt optimization techniques.
 
         Args:
             *optims: Variable-length argument list of prompt optimization techniques.
         """
-        self.optims: List[PromptOptimize] = list(optims)
+        self.optims: List[PromptOptim] = list(optims)
 
     def __call__(self, x: Any) -> Any:
         """
         Applies the sequential composition of prompt optimization techniques to the prompt.
 
         Args:
             x (Any): The input prompt.
 
         Returns:
             Any: The optimized prompt after applying the sequential optimizations.
         """
+        d = DotDict()
+        d.content = x
         for optim in self.optims:
-            x = optim(x)
-        return x
+            d = optim(d.content)
+        return d
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/stemmer_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/stemmer_optim.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 from nltk.stem import PorterStemmer
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class StemmerOptim(PromptOptimize):
+class StemmerOptim(PromptOptim):
     """
     StemmerOptim is a prompt optimization technique that applies stemming to the prompt.
 
     Stemming reduces words to their base or root form, removing suffixes and prefixes.
 
-    Usage:
-    ```
-    stemmer = StemmerOptim()
-    optimized_prompt = stemmer(prompt)
-    ```
-
-    Args:
-        verbose (bool, optional): If True, print verbose information during optimization. Defaults to False.
-        metrics (list, optional): List of metrics to evaluate the optimization. Defaults to [].
-
-    Attributes:
-        stemmer (PorterStemmer): The stemmer object used for stemming words.
+    Example:
+        >>> from prompt_optimizer.poptim import StemmerOptim
+        >>> p_optimizer = StemmerOptim()
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
 
     """
 
     def __init__(self, verbose: bool = False, metrics: list = []):
         """
         Initializes the StemmerOptim object with the specified parameters.
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/stop_word_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/stop_word_optim.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 import nltk
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class StopWordOptim(PromptOptimize):
+class StopWordOptim(PromptOptim):
     """
     StopWordOptim is a prompt optimization technique that removes stop words from the prompt.
 
     Stop words are commonly used words (e.g., "the", "is", "in") that are often considered insignificant in natural language processing tasks.
 
-    Usage:
-    ```
-    stopword_optim = StopWordOptim()
-    optimized_prompt = stopword_optim(prompt)
-    ```
-
-    Args:
-        verbose (bool, optional): If True, print verbose information during optimization. Defaults to False.
-        metrics (list, optional): List of metrics to evaluate the optimization. Defaults to [].
-
-    Attributes:
-        stop_words (set): A set of stop words in the English language.
+    Example:
+        >>> from prompt_optimizer.poptim import StopWordOptim
+        >>> p_optimizer = StopWordOptim()
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
 
     """
 
     def __init__(self, verbose: bool = False, metrics: list = []):
         """
         Initializes the StopWordOptim object with the specified parameters.
```

### Comparing `prompt_optimizer-0.1.0/prompt_optimizer/poptim/synonym_replace_optim.py` & `prompt_optimizer-0.2.0/prompt_optimizer/poptim/synonym_replace_optim.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 import random
 
+import nltk
 import tiktoken
 from nltk.corpus import wordnet
 
-from prompt_optimizer.poptim.base import PromptOptimize
+from prompt_optimizer.poptim.base import PromptOptim
 
 
-class SynonymReplaceOptim(PromptOptimize):
+class SynonymReplaceOptim(PromptOptim):
     """
     SynonymReplaceOptim is a prompt optimization technique that replaces words in the prompt with their synonyms.
 
-    Synonyms are words that have similar meanings to the original word. This technique aims to diversify the language used in the prompt.
+    Synonyms are words that have similar meanings to the original word. Sometimes a synonym has lower token count
+    than the original word.
 
-    Usage:
-    ```
-    synonym_optim = SynonymReplaceOptim(p=0.5)
-    optimized_prompt = synonym_optim(prompt)
-    ```
-
-    Args:
-        verbose (bool, optional): If True, print verbose information during optimization. Defaults to False.
-        metrics (list, optional): List of metrics to evaluate the optimization. Defaults to [].
-        p (float, optional): Probability of replacing a word with a synonym. Defaults to 0.5.
-
-    Attributes:
-        tokenizer (tiktoken.Tokenizer): A tokenizer for encoding words.
+    Example:
+        >>> from prompt_optimizer.poptim import SynonymReplaceOptim
+        >>> p_optimizer = SynonymReplaceOptim()
+        >>> res = p_optimizer("example prompt...")
+        >>> optimized_prompt = res.content
     """
 
     def __init__(self, verbose: bool = False, metrics: list = [], p: float = 0.5):
         """
         Initializes the SynonymReplaceOptim object with the specified parameters.
 
         Args:
             verbose (bool, optional): If True, print verbose information during optimization. Defaults to False.
             metrics (list, optional): List of metrics to evaluate the optimization. Defaults to [].
             p (float, optional): Probability of replacing a word with a synonym. Defaults to 0.5.
         """
         super().__init__(verbose, metrics)
         self.p = p
+        nltk.download("wordnet")
         self.tokenizer = tiktoken.get_encoding("cl100k_base")
 
     def get_word_pos(self, word: str) -> str:
         """
         Get the part of speech of a word.
 
         Args:
```

### Comparing `prompt_optimizer-0.1.0/pyproject.toml` & `prompt_optimizer-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prompt-optimizer"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Vaibhav Kumar <34630911+TimeTraveller-San@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "prompt_optimizer"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
@@ -21,14 +21,15 @@
 sphinx = "^6.1.3"
 sphinx-book-theme = "^1.0.1"
 ruff = "^0.0.261"
 mypy = "^1.2.0"
 pytest = "^7.3.0"
 black = "^23.3.0"
 langchain = "^0.0.173"
+myst-parser = "^1.0.0"
 
 [tool.poetry.group.docs.dependencies]
 autodoc_pydantic = "^1.8.0"
 nbsphinx = "^0.8.9"
 sphinx-autobuild = "^2021.3.14"
 sphinx_rtd_theme = "^1.0.0"
 sphinx-typlog-theme = "^0.8.0"
```

### Comparing `prompt_optimizer-0.1.0/PKG-INFO` & `prompt_optimizer-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-optimizer
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Vaibhav Kumar
 Author-email: 34630911+TimeTraveller-San@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,49 +15,59 @@
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pulp (>=2.7.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: transformers (>=4.27.4,<5.0.0)
 Description-Content-Type: text/markdown
 
-# PromptOptimizer
-Minimize LLM token complexity to save API costs and model computations.
+<div align="center">
 
-[![lint](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/lint.yml/badge.svg)](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/lint.yml) [![test](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/test.yml/badge.svg)](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/test.yml) [![linkcheck](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/TimeTraveller-San/prompt-optimizer/actions/workflows/linkcheck.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+  ## PromptOptimizer
+  
+  <img width="200" src="evaluations/artifacts/logo.png" alt="kevin inspired logo" />
+
+  Minimize LLM token complexity to save API costs and model computations.
+
+</div>
+<div align="center">
+
+[![lint](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/lint.yml/badge.svg)](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/lint.yml) 
+[![test](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/test.yml/badge.svg)](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/test.yml) 
+[![linkcheck](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/linkcheck.yml/badge.svg)](https://github.com/vaibkumr/prompt-optimizer/actions/workflows/linkcheck.yml) 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+[Docs](https://promptoptimizer.readthedocs.io/en/latest/)
+
+</div>
 
 
 # Features
 - **Plug and Play Optimizers:** Minimize token complexity using optimization methods without any access to weights, logits or decoding algorithm. Directly applicable to virtually all NLU systems.
 - **Protected Tags:** Special protected tags to mark important sections of prompt that should not be removed/modified.
-- **Multiple Input Format Support:** Optmization of string, batches of strings and JSON prompt data with an option to skip system prompts.
 - **Sequential Optimization:** Chain different optimizers together sequentially.
 - **Optimization Metrics:** Number of tokens reduced and semantic similarity before and after optimization.
-- **Langhcain Support:** Supports langchain style prompt chains.
+- **Langhcain and JSON Support:** Supports langchain style prompt chains and OpenAI request JSON Object.
  
 # Why?
 - **Minimize Token Complexity:** Token Complexity is the amount of prompt tokens required to achieve a given task. Reducing token complexity corresponds to linearly reducing API costs and quadratically reducing computational complexity of usual transformer models.
 - **Save Money:** For large businesses, saving 10% on token count can lead to saving 100k USD per 1M USD.
 - **Extend Limitations:** Some models have small context lengths, prompt optimizers can help them process larger than context documents.
 
-# Why does it work?
-1. LLMs are powerful, they can infill missing information.
-2. Natural language is bulky, large words and phrases can be replaced by smaller ones.
-
 | Prompt | # Tokens | Correct Response? |  
 | ------------------------------------------------------- | ---------- | ------------------- |  
 | Who is the president of the United States of America? | 11 | ✅ |  
 | Who president US | 3  (-72%) | ✅ |
 
 # Installation
 ### Quick Installation
 ```pip install prompt-optimizer```
 
 ### Install from source
 ```bash
-git clone https://github.com/TimeTraveller-San/prompt-optimizer.git;
+git clone https://github.com/vaibkumr/prompt-optimizer.git;
 cd prompt-optimizer;
 pip install -e .
 ```
 
 # Disclaimer
 There is a compression vs performance tradeoff -- the increase in compression comes at the cost of loss in model performance. The tradeoff can be greatly mitigated by chosing the right optimize for a given task. There is no single optimizer for all cases. There is no Adam here.
 
@@ -71,25 +81,45 @@
 prompt = """The Belle Tout Lighthouse is a decommissioned lighthouse and British landmark located at Beachy Head, East Sussex, close to the town of Eastbourne."""
 p_optimizer = EntropyOptim(verbose=True, p=0.1)
 optimized_prompt = p_optimizer(prompt)
 print(optimized_prompt)
 
 ```
 # Evaluations
-Following are the results for [logiqa](https://github.com/openai/evals/blob/main/evals/registry/evals/logiqa.yaml) OpenAI evals task. It is only performed for first 100 samples. Please note the results over this task are not true for all other tasks, more thorough testing and domain knowledge is needed to choose the optimal optimizer.
+Following are the results for [logiqa](https://github.com/openai/evals/blob/main/evals/registry/evals/logiqa.yaml) OpenAI evals task. It is only performed for a subset of first 100 samples. Please note the optimizer performance over this task should not be generalized to other tasks, more thorough testing and domain knowledge is needed to choose the optimal optimizer.
 
 | Name | % Tokens Reduced | LogiQA Accuracy | USD Saved Per $100 |
 | --- | --- | --- | --- |
 | Default | 0.0 | 0.32 | 0.0 |
 | Entropy_Optim_p_0.05 | 0.06 | 0.3 | 6.35 |
 | Entropy_Optim_p_0.1 | 0.11 | 0.28 | 11.19 |
 | Entropy_Optim_p_0.25 | 0.26 | 0.22 | 26.47 |
 | Entropy_Optim_p_0.5 | 0.5 | 0.08 | 49.65 |
 | SynonymReplace_Optim_p_1.0 | 0.01 | 0.33 | 1.06 |
 | Lemmatizer_Optim | 0.01 | 0.33 | 1.01 |
-| Stemmer_Optim | -0.06 | 0.09 | -5.91 |
 | NameReplace_Optim | 0.01 | 0.34 | 1.13 |
 | Punctuation_Optim | 0.13 | 0.35 | 12.81 |
 | Autocorrect_Optim | 0.01 | 0.3 | 1.14 |
 | Pulp_Optim_p_0.05 | 0.05 | 0.31 | 5.49 |
 | Pulp_Optim_p_0.1 | 0.1 | 0.25 | 9.52 |
 
+# Cost-Performance Tradeoff
+The reduction in cost often comes with a loss in LLM performance. Almost every optimizer have hyperparameters that control this tradeoff. 
+
+For example, in `EntropyOptim` the hyperparamter `p`, a floating point number between 0 and 1 controls the ratio of tokens to remove. `p=1.0` corresponds to removing all tokens while `p=0.0` corresponds to removing none. 
+
+The following chart shows the trade-off for different values of `p` as evaluated on the OpenAI evals [logiqa](https://github.com/openai/evals/blob/main/evals/registry/evals/logiqa.yaml) task for a subset of first 100 samples.
+
+<div align="center">
+  <img src="evaluations/artifacts/tradeoff.png" alt="tradeoff" />
+</div>
+
+# Contributing
+There are several directions to contribute to. Please see [CONTRIBUTING.md](.github/CONTRIBUTING.md) for contribution guidelines and possible future directions.
+
+# Social
+Contact us on twitter [Vaibhav Kumar](https://twitter.com/vaibhavk1o1) and [Vaibhav Kumar](https://twitter.com/vaibhavk97).
+
+# Inspiration
+<div align="center">
+  <img src="evaluations/artifacts/kevin.gif" alt="Image" />
+</div>
```

