# Comparing `tmp/scikit-llm-0.1.0b1.tar.gz` & `tmp/scikit-llm-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-llm-0.1.0b1.tar", last modified: Sat May 13 17:57:54 2023, max compression
+gzip compressed data, was "scikit-llm-0.1.0b2.tar", last modified: Fri May 19 20:03:18 2023, max compression
```

## Comparing `scikit-llm-0.1.0b1.tar` & `scikit-llm-0.1.0b2.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-13 17:57:54.379731 scikit-llm-0.1.0b1/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b1/LICENSE
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     4193 2023-05-13 17:57:54.379400 scikit-llm-0.1.0b1/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3660 2023-05-13 17:42:08.000000 scikit-llm-0.1.0b1/README.md
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      780 2023-05-13 17:57:13.000000 scikit-llm-0.1.0b1/pyproject.toml
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-13 17:57:54.376910 scikit-llm-0.1.0b1/scikit_llm.egg-info/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     4193 2023-05-13 17:57:54.000000 scikit-llm-0.1.0b1/scikit_llm.egg-info/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      404 2023-05-13 17:57:54.000000 scikit-llm-0.1.0b1/scikit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-05-13 17:57:54.000000 scikit-llm-0.1.0b1/scikit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       62 2023-05-13 17:57:54.000000 scikit-llm-0.1.0b1/scikit_llm.egg-info/requires.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-05-13 17:57:54.000000 scikit-llm-0.1.0b1/scikit_llm.egg-info/top_level.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-05-13 17:57:54.379810 scikit-llm-0.1.0b1/setup.cfg
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-13 17:57:54.377463 scikit-llm-0.1.0b1/skllm/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       97 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b1/skllm/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-05-13 17:42:03.000000 scikit-llm-0.1.0b1/skllm/config.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-13 17:57:54.378269 scikit-llm-0.1.0b1/skllm/datasets/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      142 2023-05-13 15:03:57.000000 scikit-llm-0.1.0b1/skllm/datasets/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.1.0b1/skllm/datasets/multi_class.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.1.0b1/skllm/datasets/multi_label.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-13 17:57:54.378536 scikit-llm-0.1.0b1/skllm/models/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5517 2023-05-13 17:55:02.000000 scikit-llm-0.1.0b1/skllm/models/gpt_zero_shot_clf.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-13 17:57:54.379002 scikit-llm-0.1.0b1/skllm/openai/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      873 2023-05-13 17:37:39.000000 scikit-llm-0.1.0b1/skllm/openai/chatgpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2186 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b1/skllm/openai/prompts.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.733873 scikit-llm-0.1.0b2/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b2/LICENSE
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5943 2023-05-19 20:03:18.733554 scikit-llm-0.1.0b2/PKG-INFO
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5410 2023-05-19 20:00:45.000000 scikit-llm-0.1.0b2/README.md
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      780 2023-05-19 20:02:19.000000 scikit-llm-0.1.0b2/pyproject.toml
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.729107 scikit-llm-0.1.0b2/scikit_llm.egg-info/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5943 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/PKG-INFO
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      566 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       62 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/requires.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-05-19 20:03:18.000000 scikit-llm-0.1.0b2/scikit_llm.egg-info/top_level.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-05-19 20:03:18.733980 scikit-llm-0.1.0b2/setup.cfg
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.729967 scikit-llm-0.1.0b2/skllm/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       97 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b2/skllm/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-05-13 17:42:03.000000 scikit-llm-0.1.0b2/skllm/config.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.730926 scikit-llm-0.1.0b2/skllm/datasets/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      142 2023-05-13 15:03:57.000000 scikit-llm-0.1.0b2/skllm/datasets/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.1.0b2/skllm/datasets/multi_class.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.1.0b2/skllm/datasets/multi_label.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.731222 scikit-llm-0.1.0b2/skllm/models/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5070 2023-05-19 19:12:30.000000 scikit-llm-0.1.0b2/skllm/models/gpt_zero_shot_clf.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.732631 scikit-llm-0.1.0b2/skllm/openai/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      901 2023-05-19 19:00:05.000000 scikit-llm-0.1.0b2/skllm/openai/chatgpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      111 2023-05-19 18:59:36.000000 scikit-llm-0.1.0b2/skllm/openai/credentials.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      820 2023-05-19 19:02:41.000000 scikit-llm-0.1.0b2/skllm/openai/embeddings.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      730 2023-05-19 19:11:38.000000 scikit-llm-0.1.0b2/skllm/openai/mixin.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     2186 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b2/skllm/openai/prompts.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-19 20:03:18.733205 scikit-llm-0.1.0b2/skllm/preprocessing/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       60 2023-05-19 18:51:50.000000 scikit-llm-0.1.0b2/skllm/preprocessing/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1394 2023-05-19 19:23:03.000000 scikit-llm-0.1.0b2/skllm/preprocessing/gpt_vectorizer.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      244 2023-05-19 18:51:39.000000 scikit-llm-0.1.0b2/skllm/utils.py
```

### Comparing `scikit-llm-0.1.0b1/LICENSE` & `scikit-llm-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b1/PKG-INFO` & `scikit-llm-0.1.0b2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-Metadata-Version: 2.1
-Name: scikit-llm
-Version: 0.1.0b1
-Summary: Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
-Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
-  <img src="https://github.com/iryna-kondr/scikit-llm/blob/main/logo.png?raw=true" height="200"/>
+  <img src="https://github.com/iryna-kondr/scikit-llm/blob/main/logo.png?raw=true" max-height="200"/>
 </p>
 
 # Scikit-LLM: Sklearn Meets Large Language Models
 
 Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks.
 
 ## Installation 💾 
 
 ```bash 
 pip install scikit-llm
 ```
 
+## Support us 🤝
+
+You can support the project in the following ways:
+
+- ⭐ Star Scikit-LLM on GitHub (click the star button in the top right corner)
+- 💡 Provide your feedback or propose ideas in the [issues](https://github.com/iryna-kondr/scikit-llm/issues) section
+- 🔗 Post about Scikit-LLM on LinkedIn or other platforms
+- 🪶 Check out our related project - [Falcon AutoML](https://github.com/OKUA1/falcon)
+
+
 ## Documentation 📚
 
 ### Configuring OpenAI API Key
 At the moment Scikit-LLM is only compatible with some of the OpenAI models. Hence, a user-provided OpenAI API key is required.
 
 ```python
 from skllm.config import SKLLMConfig
@@ -71,14 +68,17 @@
 
 clf = ZeroShotGPTClassifier()
 clf.fit(None, ['positive', 'negative', 'neutral'])
 labels = clf.predict(X)
 
 ```
 
+**Note:** unlike in a typical supervised setting, the performance of a zero-shot classifier greatly depends on how the label itself is structured. It has to be expressed in natural language, be descriptive and self-explanatory. For example, in the previous semantic classification task, it could be beneficial to transform a label from `"<semantics>"` to `"the semantics of the provided text is <semantics>"`. 
+
+
 ### Multi-Label Zero-Shot Text Classification
 
 With a class `MultiLabelZeroShotGPTClassifier` it is possible to perform the classification in multi-label setting, which means that each sample might be assigned to one or several distinct classes.
 
 Example: 
 
 ```python
@@ -90,15 +90,15 @@
 clf = MultiLabelZeroShotGPTClassifier(max_labels=3)
 clf.fit(X, y)
 labels = clf.predict(X)
 ```
 
 Similarly to the `ZeroShotGPTClassifier` it is sufficient if only candidate labels are provided. However, this time the classifier expects `y` of a type `List[List[str]]`.
 
-```
+```python
 from skllm import MultiLabelZeroShotGPTClassifier
 from skllm.datasets import get_multilabel_classification_dataset
 
 X, _ = get_multilabel_classification_dataset()
 candidate_labels = [
     "Quality", 
     "Price", 
@@ -112,18 +112,46 @@
     "Product Information"
 ]
 clf = MultiLabelZeroShotGPTClassifier(max_labels=3)
 clf.fit(None, [candidate_labels])
 labels = clf.predict(X)
 ```
 
+### Text Vectorization
+
+As an alternative to using GPT as a classifier, it can be used solely for data preprocessing. `GPTVectorizer` allows to embed a chunk of text of arbitrary length to a fixed-dimensional vector, that can be used with virtually any classification or regression model.
+
+Example 1: Embedding the text
+```python
+from skllm.preprocessing import GPTVectorizer
+
+model = GPTVectorizer()
+vectors = model.fit_transform(X)
+```
+
+Example 2: Combining the Vectorizer with the XGBoost Classifier in a Sklearn Pipeline
+```python
+from sklearn.pipeline import Pipeline
+from sklearn.preprocessing import LabelEncoder
+from xgboost import XGBClassifier
+
+le = LabelEncoder()
+y_train_encoded = le.fit_transform(y_train)
+y_test_encoded = le.transform(y_test)
+
+steps = [('GPT', GPTVectorizer()), ('Clf', XGBClassifier())]
+clf = Pipeline(steps)
+clf.fit(X_train, y_train_encoded)
+yh = clf.predict(X_test)
+```
+
 ## Roadmap 🧭
 
 - [x] Zero-Shot Classification with OpenAI GPT 3/4
     - [x] Multiclass classification
     - [x] Multi-label classification
     - [x] ChatGPT models
     - [ ] InstructGPT models
 - [ ] Few shot classifier
-- [ ] GPT Vectorizer
+- [x] GPT Vectorizer
 - [ ] GPT Fine-tuning (optional)
-- [ ] Integration of other LLMs
+- [ ] Integration of other LLMs
```

### Comparing `scikit-llm-0.1.0b1/pyproject.toml` & `scikit-llm-0.1.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dependencies = [
 "scikit-learn>=1.1.0",
 "pandas>=1.5.0",
 "openai>=0.27.0",
 "tqdm>=4.60.0",
 ]
 name = "scikit-llm"
-version = "0.1.0b1"
+version = "0.1.0b2"
 authors = [
   { name="Oleg Kostromin", email="kostromin97@gmail.com" },
   { name="Iryna Kondrashchenko", email="iryna230520@gmail.com" },
 ]
 description = "Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks."
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `scikit-llm-0.1.0b1/skllm/config.py` & `scikit-llm-0.1.0b2/skllm/config.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b1/skllm/datasets/multi_class.py` & `scikit-llm-0.1.0b2/skllm/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b1/skllm/datasets/multi_label.py` & `scikit-llm-0.1.0b2/skllm/datasets/multi_label.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b1/skllm/models/gpt_zero_shot_clf.py` & `scikit-llm-0.1.0b2/skllm/models/gpt_zero_shot_clf.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,61 +9,46 @@
 from skllm.openai.prompts import get_zero_shot_prompt_slc, get_zero_shot_prompt_mlc
 from skllm.openai.chatgpt import (
     construct_message,
     get_chat_completion,
     extract_json_key,
 )
 from skllm.config import SKLLMConfig as _Config
+from skllm.utils import to_numpy as _to_numpy
+from skllm.openai.mixin import OpenAIMixin as _OAIMixin
 
-
-class _BaseZeroShotGPTClassifier(ABC, BaseEstimator, ClassifierMixin):
+class _BaseZeroShotGPTClassifier(ABC, BaseEstimator, ClassifierMixin, _OAIMixin):
     def __init__(
         self,
         openai_key: Optional[str] = None,
         openai_org: Optional[str] = None,
         openai_model: str = "gpt-3.5-turbo",
     ):
-        self.openai_key = openai_key
-        self.openai_org = openai_org
+        self._set_keys(openai_key, openai_org)
         self.openai_model = openai_model
 
+    def _to_np(self, X):
+        return _to_numpy(X)
+
     def fit(
         self,
         X: Optional[Union[np.ndarray, pd.Series, List[str]]],
         y: Union[np.ndarray, pd.Series, List[str], List[List[str]]],
     ):
-        if isinstance(X, np.ndarray):
-            X = np.squeeze(X)
+        X = self._to_np(X)        
         self.classes_, self.probabilities_ = self._get_unique_targets(y)
         return self
 
     def predict(self, X: Union[np.ndarray, pd.Series, List[str]]):
-        if isinstance(X, np.ndarray):
-            X = np.squeeze(X)
+        X = self._to_np(X)
         predictions = []
         for i in tqdm(range(len(X))):
             predictions.append(self._predict_single(X[i]))
         return predictions
 
-    def _get_openai_key(self):
-        key = self.openai_key
-        if key is None:
-            key = _Config.get_openai_key()
-        if key is None:
-            raise RuntimeError("OpenAI key was not found")
-        return key
-
-    def _get_openai_org(self):
-        key = self.openai_org
-        if key is None:
-            key = _Config.get_openai_org()
-        if key is None:
-            raise RuntimeError("OpenAI organization was not found")
-        return key
-
     @abstractmethod
     def _extract_labels(self, y: Any) -> List[str]:
         pass
 
     def _get_unique_targets(self, y):
         labels = self._extract_labels(y)
 
@@ -122,16 +107,15 @@
         return label
 
     def fit(
         self,
         X: Optional[Union[np.ndarray, pd.Series, List[str]]],
         y: Union[np.ndarray, pd.Series, List[str]],
     ):
-        if isinstance(y, np.ndarray):
-            y = np.squeeze(y)
+        y = self._to_np(y)
         return super().fit(X, y)
 
 
 class MultiLabelZeroShotGPTClassifier(_BaseZeroShotGPTClassifier):
     def __init__(
         self,
         openai_key: Optional[str] = None,
```

### Comparing `scikit-llm-0.1.0b1/skllm/openai/chatgpt.py` & `scikit-llm-0.1.0b2/skllm/openai/chatgpt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import openai
 import json
+from skllm.openai.credentials import set_credentials
 
 def construct_message(role, content):
     if role not in ("system", "user", "assistant"):
         raise ValueError("Invalid role")
     return {"role": role, "content": content}
 
 def get_chat_completion(messages, key, org, model="gpt-3.5-turbo", max_retries = 3):
-    openai.api_key = key
-    openai.organization = org
+    set_credentials(key, org)
     for _ in range(max_retries):
         try:
             completion = openai.ChatCompletion.create(
                 model=model, temperature=0., messages=messages
             )
             return completion
         except Exception:
```

### Comparing `scikit-llm-0.1.0b1/skllm/openai/prompts.py` & `scikit-llm-0.1.0b2/skllm/openai/prompts.py`

 * *Files identical despite different names*

