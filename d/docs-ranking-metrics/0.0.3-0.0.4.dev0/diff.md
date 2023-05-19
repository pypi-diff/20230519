# Comparing `tmp/docs-ranking-metrics-0.0.3.tar.gz` & `tmp/docs-ranking-metrics-0.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\docs-ranking-metrics-0.0.3.tar", last modified: Mon May 15 05:22:44 2023, max compression
+gzip compressed data, was "docs-ranking-metrics-0.0.4.dev0.tar", last modified: Fri May 19 14:19:41 2023, max compression
```

## Comparing `docs-ranking-metrics-0.0.3.tar` & `docs-ranking-metrics-0.0.4.dev0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 05:22:44.268306 docs-ranking-metrics-0.0.3/
--rw-rw-rw-   0        0        0     2368 2023-05-15 05:22:44.267341 docs-ranking-metrics-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2694 2023-05-05 09:18:40.000000 docs-ranking-metrics-0.0.3/README.md
--rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 05:22:44.268306 docs-ranking-metrics-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     8957 2023-05-05 08:23:25.000000 docs-ranking-metrics-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:22:44.174147 docs-ranking-metrics-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 05:22:44.236935 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/
--rw-rw-rw-   0        0        0      130 2023-05-15 05:21:37.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/__init__.py
--rw-rw-rw-   0        0        0     9860 2023-05-05 08:41:07.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/evaluation_metrics.py
--rw-rw-rw-   0        0        0     7720 2023-05-15 05:18:39.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/ranking_metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:22:44.266322 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/
--rw-rw-rw-   0        0        0     2368 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 14:19:41.870765 docs-ranking-metrics-0.0.4.dev0/
+-rw-rw-rw-   0        0        0     2332 2023-05-19 14:19:41.870765 docs-ranking-metrics-0.0.4.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     2694 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev0/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 14:19:41.870765 docs-ranking-metrics-0.0.4.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     8957 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 14:19:41.852814 docs-ranking-metrics-0.0.4.dev0/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 14:19:41.855805 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics/
+-rw-rw-rw-   0        0        0      147 2023-05-19 14:18:36.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics/__init__.py
+-rw-rw-rw-   0        0        0     9860 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics/evaluation_metrics.py
+-rw-rw-rw-   0        0        0      593 2023-05-19 14:18:36.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics/models.py
+-rw-rw-rw-   0        0        0     9718 2023-05-19 14:12:35.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-19 14:19:41.869768 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics.egg-info/
+-rw-rw-rw-   0        0        0     2332 2023-05-19 14:19:41.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-05-19 14:19:41.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 14:19:41.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-05-19 14:19:41.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-19 14:19:41.000000 docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics.egg-info/top_level.txt
```

### Comparing `docs-ranking-metrics-0.0.3/PKG-INFO` & `docs-ranking-metrics-0.0.4.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.3
+Version: 0.0.4.dev0
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
-License: UNKNOWN
 Keywords: test
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
@@ -69,9 +67,7 @@
     'Bm25_Top@1': 0.91891, 
     'Bm25_Top@3': 1.0, 
     'Bm25_Top@5': 1.0, 
     'LaBSE_FDARO': 0.6216, 
     'Bm25_FDARO': 1.0
 }
 ```
-
-
```

### Comparing `docs-ranking-metrics-0.0.3/README.md` & `docs-ranking-metrics-0.0.4.dev0/README.md`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.3/setup.py` & `docs-ranking-metrics-0.0.4.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/evaluation_metrics.py` & `docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/ranking_metrics.py` & `docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics/ranking_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from rank_bm25 import BM25Okapi
 from typing import List, Dict, Tuple, Union
 from sentence_transformers import SentenceTransformer, util
+from transformers.adapters.utils import pull_from_hub
 from .evaluation_metrics import (
     TopK, AverageLoc, FDARO
 )
-
+from .models import ModelUSE
+from tensorflow import convert_to_tensor
+import torch
 
 class Bm25:
     """Класс метрики ранжирования bm25"""
 
     def __init__(self):
         pass
 
@@ -129,16 +132,67 @@
             Массив меток
 
         Returns
         ------------
         `List[Tuple[float, int]]`
             Отсортированный список ранжируемых элементов по релевантности
         """
-        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
+        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0])
+
+class USE:
+    """Класс метрики ранжирования USE"""
+    def __init__(self):
+        self.model = ModelUSE()
+
+    def name(self) -> str:
+            return "USE"
+
+    def ranking(self, query: str, sentences: List[str], labels: List[int]) -> List[Tuple[float, int]]:
+        """
+        Функция ранжирования LaBSE
+
+        Parameters
+        ------------
+        query: `str`
+            Строка запроса
+        sentences: `List[str]`
+            Список строк текстов
+        labels: `List[int]`
+            Список меток текстов
 
+        Returns
+        ------------
+        `List[Tuple[float, int]]`
+            Список оценок релевантности текстов
+        """
+        # query = self.model.encode(query)
+        sentences.append(query)
+        embeddings = [x.numpy() for x in self.model.encode(sentences)]
+        embeddings = torch.Tensor(embeddings)
+        scores = util.pytorch_cos_sim(embeddings[-1], embeddings[:-1]).numpy()[0]
+        scores = self._sorted(scores, labels)
+        return scores
+
+    def _sorted(self, scores: List[float], labels: List[int]) -> List[Tuple[float, int]]:
+        """
+        Функция сортировки оценки и лейблов
+
+        Parameters
+        ------------
+        scores: `List[float]`
+            Массив оценок ранка присвоенных ранкером
+        labels: `List[int]`
+            Массив меток
+
+        Returns
+        ------------
+        `List[Tuple[float, int]]`
+            Отсортированный список ранжируемых элементов по релевантности
+        """
+        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0])
 
 class RankingMetrics:
     """Класс аккумулирующий все метрики"""
     FAKE_DOC_LABEL: int = -1
 
     def __init__(self, metrics) -> None:
         # Среднее место фейковых документов в финальной выдаче
```

### Comparing `docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/PKG-INFO` & `docs-ranking-metrics-0.0.4.dev0/src/docs_ranking_metrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.3
+Version: 0.0.4.dev0
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
-License: UNKNOWN
 Keywords: test
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
@@ -69,9 +67,7 @@
     'Bm25_Top@1': 0.91891, 
     'Bm25_Top@3': 1.0, 
     'Bm25_Top@5': 1.0, 
     'LaBSE_FDARO': 0.6216, 
     'Bm25_FDARO': 1.0
 }
 ```
-
-
```

