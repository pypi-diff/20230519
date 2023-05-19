# Comparing `tmp/docs-ranking-metrics-0.0.4.dev1.tar.gz` & `tmp/docs-ranking-metrics-0.0.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs-ranking-metrics-0.0.4.dev1.tar", last modified: Fri May 19 14:30:11 2023, max compression
+gzip compressed data, was "docs-ranking-metrics-0.0.4.dev2.tar", last modified: Fri May 19 16:10:03 2023, max compression
```

## Comparing `docs-ranking-metrics-0.0.4.dev1.tar` & `docs-ranking-metrics-0.0.4.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 14:30:11.408939 docs-ranking-metrics-0.0.4.dev1/
--rw-rw-rw-   0        0        0     2332 2023-05-19 14:30:11.407945 docs-ranking-metrics-0.0.4.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     2694 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev1/README.md
--rw-rw-rw-   0        0        0       97 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 14:30:11.408939 docs-ranking-metrics-0.0.4.dev1/setup.cfg
--rw-rw-rw-   0        0        0     8957 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 14:30:11.392982 docs-ranking-metrics-0.0.4.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 14:30:11.394976 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics/
--rw-rw-rw-   0        0        0      147 2023-05-19 14:30:07.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics/__init__.py
--rw-rw-rw-   0        0        0     9860 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics/evaluation_metrics.py
--rw-rw-rw-   0        0        0     1029 2023-05-19 14:29:43.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics/models.py
--rw-rw-rw-   0        0        0     9684 2023-05-19 14:29:43.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics/ranking_metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-19 14:30:11.407945 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics.egg-info/
--rw-rw-rw-   0        0        0     2332 2023-05-19 14:30:11.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-05-19 14:30:11.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 14:30:11.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-05-19 14:30:11.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-19 14:30:11.000000 docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 16:10:03.852362 docs-ranking-metrics-0.0.4.dev2/
+-rw-rw-rw-   0        0        0     2332 2023-05-19 16:10:03.852362 docs-ranking-metrics-0.0.4.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     2694 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev2/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 16:10:03.852362 docs-ranking-metrics-0.0.4.dev2/setup.cfg
+-rw-rw-rw-   0        0        0     8957 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:10:03.843389 docs-ranking-metrics-0.0.4.dev2/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 16:10:03.845383 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/
+-rw-rw-rw-   0        0        0      147 2023-05-19 16:10:00.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/__init__.py
+-rw-rw-rw-   0        0        0     9860 2023-05-19 13:43:59.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     1535 2023-05-19 14:39:57.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/models.py
+-rw-rw-rw-   0        0        0     9668 2023-05-19 16:10:00.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:10:03.852362 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/
+-rw-rw-rw-   0        0        0     2332 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-19 16:10:03.000000 docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/top_level.txt
```

### Comparing `docs-ranking-metrics-0.0.4.dev1/PKG-INFO` & `docs-ranking-metrics-0.0.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.4.dev1
+Version: 0.0.4.dev2
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 Keywords: test
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `docs-ranking-metrics-0.0.4.dev1/README.md` & `docs-ranking-metrics-0.0.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.4.dev1/setup.py` & `docs-ranking-metrics-0.0.4.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics/evaluation_metrics.py` & `docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics/ranking_metrics.py` & `docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics/ranking_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,27 +132,27 @@
             Массив меток
 
         Returns
         ------------
         `List[Tuple[float, int]]`
             Отсортированный список ранжируемых элементов по релевантности
         """
-        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0])
+        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
 
 class USE:
     """Класс метрики ранжирования USE"""
     def __init__(self):
         self.model = ModelUSE()
 
     def name(self) -> str:
         return "USE"
 
     def ranking(self, query: str, sentences: List[str], labels: List[int]) -> List[Tuple[float, int]]:
         """
-        Функция ранжирования LaBSE
+        Функция ранжирования USE
 
         Parameters
         ------------
         query: `str`
             Строка запроса
         sentences: `List[str]`
             Список строк текстов
@@ -160,15 +160,15 @@
             Список меток текстов
 
         Returns
         ------------
         `List[Tuple[float, int]]`
             Список оценок релевантности текстов
         """
-        # query = self.model.encode(query)
+
         sentences.append(query)
         embeddings = [x.numpy() for x in self.model.encode(sentences)]
         embeddings = torch.Tensor(embeddings)
         scores = util.pytorch_cos_sim(embeddings[-1], embeddings[:-1]).numpy()[0]
         scores = self._sorted(scores, labels)
         return scores
 
@@ -184,15 +184,15 @@
             Массив меток
 
         Returns
         ------------
         `List[Tuple[float, int]]`
             Отсортированный список ранжируемых элементов по релевантности
         """
-        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0])
+        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
 
 class RankingMetrics:
     """Класс аккумулирующий все метрики"""
     FAKE_DOC_LABEL: int = -1
 
     def __init__(self, metrics) -> None:
         # Среднее место фейковых документов в финальной выдаче
```

### Comparing `docs-ranking-metrics-0.0.4.dev1/src/docs_ranking_metrics.egg-info/PKG-INFO` & `docs-ranking-metrics-0.0.4.dev2/src/docs_ranking_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.4.dev1
+Version: 0.0.4.dev2
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 Keywords: test
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

