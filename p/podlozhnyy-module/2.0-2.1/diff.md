# Comparing `tmp/podlozhnyy_module-2.0.tar.gz` & `tmp/podlozhnyy_module-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podlozhnyy_module-2.0.tar", last modified: Fri May 19 18:04:15 2023, max compression
+gzip compressed data, was "dist\podlozhnyy_module-2.1.tar", last modified: Fri May 19 18:41:41 2023, max compression
```

## Comparing `podlozhnyy_module-2.0.tar` & `podlozhnyy_module-2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/
--rw-rw-rw-   0        0        0     2202 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1237 2023-01-08 22:40:36.000000 podlozhnyy_module-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/podlozhnyy_module/
--rw-rw-rw-   0        0        0      743 2023-05-19 12:29:55.000000 podlozhnyy_module-2.0/podlozhnyy_module/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-05-18 20:56:40.000000 podlozhnyy_module-2.0/podlozhnyy_module/bootstrap.py
--rw-rw-rw-   0        0        0     3259 2023-05-18 23:00:11.000000 podlozhnyy_module-2.0/podlozhnyy_module/charts.py
--rw-rw-rw-   0        0        0     5253 2023-05-18 22:28:37.000000 podlozhnyy_module-2.0/podlozhnyy_module/collocation.py
--rw-rw-rw-   0        0        0     2414 2023-05-18 22:12:12.000000 podlozhnyy_module-2.0/podlozhnyy_module/correlation.py
--rw-rw-rw-   0        0        0     4317 2023-05-18 20:59:14.000000 podlozhnyy_module-2.0/podlozhnyy_module/pareto.py
--rw-rw-rw-   0        0        0     4088 2023-05-19 12:24:40.000000 podlozhnyy_module-2.0/podlozhnyy_module/permutation.py
--rw-rw-rw-   0        0        0    31391 2023-05-19 17:35:12.000000 podlozhnyy_module-2.0/podlozhnyy_module/regression.py
--rw-rw-rw-   0        0        0    15610 2023-05-18 23:18:18.000000 podlozhnyy_module-2.0/podlozhnyy_module/timeseries.py
--rw-rw-rw-   0        0        0     4622 2023-05-18 23:49:13.000000 podlozhnyy_module-2.0/podlozhnyy_module/timetest.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/podlozhnyy_module.egg-info/
--rw-rw-rw-   0        0        0     2202 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/podlozhnyy_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/podlozhnyy_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/podlozhnyy_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/podlozhnyy_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/podlozhnyy_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 18:04:15.000000 podlozhnyy_module-2.0/setup.cfg
--rw-rw-rw-   0        0        0     1143 2023-05-19 17:51:18.000000 podlozhnyy_module-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/
+-rw-rw-rw-   0        0        0     2202 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1237 2023-01-08 22:40:36.000000 podlozhnyy_module-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/podlozhnyy_module/
+-rw-rw-rw-   0        0        0      729 2023-05-19 18:40:24.000000 podlozhnyy_module-2.1/podlozhnyy_module/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-05-18 20:56:40.000000 podlozhnyy_module-2.1/podlozhnyy_module/bootstrap.py
+-rw-rw-rw-   0        0        0     2956 2023-05-19 18:39:18.000000 podlozhnyy_module-2.1/podlozhnyy_module/charts.py
+-rw-rw-rw-   0        0        0     5255 2023-05-19 18:39:18.000000 podlozhnyy_module-2.1/podlozhnyy_module/collocation.py
+-rw-rw-rw-   0        0        0     2416 2023-05-19 18:39:18.000000 podlozhnyy_module-2.1/podlozhnyy_module/correlation.py
+-rw-rw-rw-   0        0        0     4315 2023-05-19 18:39:18.000000 podlozhnyy_module-2.1/podlozhnyy_module/pareto.py
+-rw-rw-rw-   0        0        0     4103 2023-05-19 18:39:18.000000 podlozhnyy_module-2.1/podlozhnyy_module/permutation.py
+-rw-rw-rw-   0        0        0    30654 2023-05-19 18:39:18.000000 podlozhnyy_module-2.1/podlozhnyy_module/regression.py
+-rw-rw-rw-   0        0        0    15398 2023-05-19 18:31:11.000000 podlozhnyy_module-2.1/podlozhnyy_module/timeseries.py
+-rw-rw-rw-   0        0        0     5598 2023-05-19 18:31:11.000000 podlozhnyy_module-2.1/podlozhnyy_module/timetest.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/podlozhnyy_module.egg-info/
+-rw-rw-rw-   0        0        0     2202 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/podlozhnyy_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/podlozhnyy_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/podlozhnyy_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/podlozhnyy_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/podlozhnyy_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 18:41:41.000000 podlozhnyy_module-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1143 2023-05-19 18:41:09.000000 podlozhnyy_module-2.1/setup.py
```

### Comparing `podlozhnyy_module-2.0/PKG-INFO` & `podlozhnyy_module-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podlozhnyy_module
-Version: 2.0
+Version: 2.1
 Summary: One place for the most useful methods for work
 Home-page: https://github.com/NPodlozhniy/podlozhnyy-module
 Author: Nikita Podlozhnyy
 Author-email: podlozhnyy.ne@phystech.edu
 License: MIT
 Description: # podlozhnyy-module
```

### Comparing `podlozhnyy_module-2.0/README.md` & `podlozhnyy_module-2.1/README.md`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/__init__.py` & `podlozhnyy_module-2.1/podlozhnyy_module/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import numpy as np
 import pandas as pd
 import seaborn as sns
-
 from matplotlib import pyplot as plt
 
 from podlozhnyy_module import (
     bootstrap,
     charts,
     collocation,
     correlation,
     pareto,
     permutation,
     regression,
     timeseries,
-    timetest
+    timetest,
 )
 
-print('Привет! Ты импортировал модуль созданный https://github.com/NPodlozhniy')
-print('В нем собраны часто востребованные в работе аналитика методы')
-print('Посмотреть полный cписок пакетов можно с помощью команды dir(<название библиотеки>)')
-print('Приятного использования!')
+print("Привет! Ты импортировал модуль созданный https://github.com/NPodlozhniy")
+print("В нем собраны часто востребованные в работе аналитика методы")
+print("Посмотреть полный cписок пакетов можно с помощью dir(<название библиотеки>)")
+print("Приятного использования!")
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/bootstrap.py` & `podlozhnyy_module-2.1/podlozhnyy_module/bootstrap.py`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/charts.py` & `podlozhnyy_module-2.1/podlozhnyy_module/charts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,103 +1,76 @@
-from podlozhnyy_module import np, pd, sns, plt
+from podlozhnyy_module import np, pd, plt, sns
 
-sns.set_style(rc = {'figure.facecolor': 'floralwhite'})
+sns.set_style(rc={"figure.facecolor": "floralwhite"})
 
-def plot_hist(df: pd.core.frame.DataFrame, feature: str, target: str, n: int = 10) -> None:
+
+def plot_hist(
+    df: pd.core.frame.DataFrame, feature: str, target: str, n: int = 10
+) -> None:
     """
     Строит приятную гистограмму распределения признака от целевой переменной
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Признак, распределение которого, требуется посмотреть
     target: Целевая переменная для разбиения признака
     n: Кол-во bin-ов, default=10
     """
-    df2 = pd.melt(df[[feature, target]], id_vars=target,
-                  value_vars=[feature], value_name='target')
-    bins = np.linspace(df2['target'].min(), df2['target'].max(), n + 1)
-  
+    df2 = pd.melt(
+        df[[feature, target]], id_vars=target, value_vars=[feature], value_name="target"
+    )
+    bins = np.linspace(df2["target"].min(), df2["target"].max(), n + 1)
+
     g = sns.FacetGrid(
-        df2,
-        col='variable',
-        hue=target,
-        palette='rainbow',
-        col_wrap=2,
-        height=10)
-    g.map(plt.hist, 'target', alpha=0.5, density=True, bins=bins, ec="k")
+        df2, col="variable", hue=target, palette="rainbow", col_wrap=2, height=10
+    )
+    g.map(plt.hist, "target", alpha=0.5, density=True, bins=bins, ec="k")
     g.axes[-1].legend()
     plt.show()
 
 
 def plot_stacked_hist(df: pd.core.frame.DataFrame, feature: str, target: str) -> None:
     """
     Возвращает столбец распределения признака в рамках каждого из значений целевой переменной
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Признак, распределение которго, требуется посмотреть
     target: Целевая переменная, будет на оси x графика
     """
-    overview = pd.crosstab(
-        df[target],
-        df[feature]).sort_values(
-        target,
-        ascending=True)
+    overview = pd.crosstab(df[target], df[feature]).sort_values(target, ascending=True)
     sum_series = overview.sum(axis=1)
     for col in list(overview.columns):
         overview[col] = overview[col] / sum_series
-    overview.plot(kind='bar', stacked=True)
+    overview.plot(kind="bar", stacked=True)
 
 
-def plot_dual_axis(data: pd.core.frame.DataFrame, col1: str, col2: str, title: str = None):
+def plot_dual_axis(
+    data: pd.core.frame.DataFrame, col1: str, col2: str, title: str = None
+):
     """
     Построение графика с двумя осями ординат
 
     Parameters
     ----------
     data: Объект pandas.DataFrame
     col1: Название основоного признака (левая ось)
     col2: Название дополнительного признака (правая ось)
     title: Заголовок графика
     """
-    fig, ax1 = plt.subplots(
-        figsize=(12, 6)
-    )
+    fig, ax1 = plt.subplots(figsize=(12, 6))
     ax2 = ax1.twinx()
 
-    ax2.bar(
-        data.index,
-        data[col2],
-        alpha=0.15,
-        fill=True,
-        edgecolor='b'
-    )
-    ax1.plot(
-        data.index,
-        data[col1],
-        'go--',
-        linewidth=2
-    )
+    ax2.bar(data.index, data[col2], alpha=0.15, fill=True, edgecolor="b")
+    ax1.plot(data.index, data[col1], "go--", linewidth=2)
 
     def naming(name):
-        return ' '.join(
-            [x[0].upper() + x[1:]
-             for x in name.split('_')
-            ]
-        )
+        return " ".join([x[0].upper() + x[1:] for x in name.split("_")])
 
     if data.index.name:
-        ax1.set_xlabel(
-            naming(data.index.name)
-        )
-    ax1.set_ylabel(
-        naming(col1),
-        color='g'
-    )
-    ax2.set_ylabel(
-        naming(col2),
-        color='b'
-    )
+        ax1.set_xlabel(naming(data.index.name))
+    ax1.set_ylabel(naming(col1), color="g")
+    ax2.set_ylabel(naming(col2), color="b")
     plt.title(title)
     plt.show()
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/collocation.py` & `podlozhnyy_module-2.1/podlozhnyy_module/collocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from itertools import combinations
+
 from nltk.corpus import stopwords
 
 from podlozhnyy_module import pd
 
 
 def prepare_frequency_dictionary(
     documents: dict, length: int, analysed_documents: set
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/correlation.py` & `podlozhnyy_module-2.1/podlozhnyy_module/correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from scipy.stats import t as student
 
-from podlozhnyy_module import pd, sns, plt
+from podlozhnyy_module import pd, plt, sns
+
 
 def plot_corr_matrix(
     df: pd.core.frame.DataFrame,
     features: list = None,
     method: str = "pearson",
 ) -> None:
     """
@@ -15,17 +16,17 @@
     df: Объект pandas.DataFrame
     features: Список признаков, взаимную корреляцию которых требуется посчитать, default=None
     method : Метод расчета корреляции {'pearson', 'kendall', 'spearman'}, default='pearson'
     """
     if features is None:
         features = df.columns[df.dtypes != "object"]
     corr = df[features].corr(method=method)
-    plt.figure(figsize=(10, 10), facecolor='floralwhite')
-    sns.heatmap(corr, vmax=1, square=True, annot=True, cmap='cubehelix')
-    plt.title('Correlation between different features')
+    plt.figure(figsize=(10, 10), facecolor="floralwhite")
+    sns.heatmap(corr, vmax=1, square=True, annot=True, cmap="cubehelix")
+    plt.title("Correlation between different features")
     bottom, top = plt.ylim()
     plt.ylim([bottom + 0.05, top - 0.05])
     plt.show()
 
 
 def correlation_significance(
     df: pd.core.frame.DataFrame,
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/pareto.py` & `podlozhnyy_module-2.1/podlozhnyy_module/pareto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from scipy.optimize import minimize
-from scipy.stats import pareto, bernoulli
+from scipy.stats import bernoulli, pareto
 
 from podlozhnyy_module import np
 
 
 def ParetoApprox(
     data: np.ndarray,
     default_value: float = 1,
@@ -47,15 +47,14 @@
         )
 
     bounds = ((0.01, np.inf), (-np.inf, np.inf), (-np.inf, np.inf))
     result = minimize(func, x0=[1, 0, 1], bounds=bounds)
     return {"alpha": result.x[0], "loc": result.x[1], "scale": result.x[2]}
 
 
-
 class ParetoExtended:
     """
     Распределение Парето дополненное значением слева принимаемым с заданной вероятностью.
     Прекрасно подходит для описания выборок с большим количеством нулей и тяжелым хвостом
 
     Parameters
     ----------
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/permutation.py` & `podlozhnyy_module-2.1/podlozhnyy_module/permutation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from itertools import product, combinations
+from itertools import combinations, product
 
 from podlozhnyy_module import np
 
 
 def permutation_t_stat(sample1, sample2):
     return np.mean(sample1) - np.mean(sample2)
 
-    
+
 def get_random_permutations(n, max_permutations):
-    return set([tuple(x) for x in 2 * np.random.randint(2, size = (max_permutations, n)) - 1])
+    return set(
+        [tuple(x) for x in 2 * np.random.randint(2, size=(max_permutations, n)) - 1]
+    )
 
 
 def permutation_zero_dist_one_samp(sample, mean, max_permutations):
     centered_sample = np.array(sample) - mean
     if max_permutations:
         signs_array = get_random_permutations(len(sample), max_permutations)
     else:
-        signs_array = product([-1, 1], repeat = len(sample))
+        signs_array = product([-1, 1], repeat=len(sample))
     return [np.mean(centered_sample * signs) for signs in signs_array]
 
 
 def get_random_combinations(n1, n2, max_combinations):
     index = list(range(n1 + n2))
     indices = set([tuple(index)])
     for i in range(max_combinations - 1):
@@ -32,20 +34,31 @@
 def permutation_zero_dist_ind(sample1, sample2, max_combinations):
     joined_sample = np.hstack((sample1, sample2))
     n1, n2 = len(sample1), len(sample2)
     n = len(joined_sample)
     if max_combinations:
         indices = get_random_combinations(n1, n2, max_combinations)
     else:
-        indices = [(list(index), filter(lambda i: i not in index, range(n)))
-                   for index in combinations(range(n), n1)]
-    return [joined_sample[list(i[0])].mean() - joined_sample[list(i[1])].mean() for i in indices]
-
-
-def permutation_test(test, control, kind: str = 'independent', max_permutations: int = None, alternative: str = 'two-sided'):
+        indices = [
+            (list(index), filter(lambda i: i not in index, range(n)))
+            for index in combinations(range(n), n1)
+        ]
+    return [
+        joined_sample[list(i[0])].mean() - joined_sample[list(i[1])].mean()
+        for i in indices
+    ]
+
+
+def permutation_test(
+    test,
+    control,
+    kind: str = "independent",
+    max_permutations: int = None,
+    alternative: str = "two-sided",
+):
     """
     Проводит одно- или двух- выборочный статистический тест, используя семейство перестановочных критериев
     Возвращает значение p-value для заданного типа альтернативы
 
     Parameters
     ----------
     test: list
@@ -55,41 +68,38 @@
     kind: str
         Связаны ли выборки в двухстороннем тесте {'related', 'independent'}, default='independent'
     max_permutations: int
         Максимальное количество перестановок, исключительно полезно в случае больших выборок, default=None
     alternative: str
         Тип альтернативы: {'two-sided', 'less', 'greater'}, default='two-sided'
     """
-    if alternative not in ('two-sided', 'less', 'greater'):
-        raise ValueError("alternative not recognized, should be 'two-sided', 'less' or 'greater'")
-    
-    if kind not in ('independent', 'related'):
+    if alternative not in ("two-sided", "less", "greater"):
+        raise ValueError(
+            "alternative not recognized, should be 'two-sided', 'less' or 'greater'"
+        )
+
+    if kind not in ("independent", "related"):
         raise ValueError("kind not recognized, should be 'related' or 'independent'")
-    
+
     if isinstance(control, int) or isinstance(control, float):
-        zero_distr = permutation_zero_dist_one_samp(
-            test, control, max_permutations
-        )
-    elif kind == 'related':
+        zero_distr = permutation_zero_dist_one_samp(test, control, max_permutations)
+    elif kind == "related":
         if len(test) != len(control):
             raise ValueError("related samples must have the same size")
         zero_distr = permutation_zero_dist_one_samp(
             np.array(test) - np.array(control), 0.0, max_permutations
         )
     else:
-        zero_distr = permutation_zero_dist_ind(
-            test, control, max_permutations
-        )
+        zero_distr = permutation_zero_dist_ind(test, control, max_permutations)
 
     t_stat = permutation_t_stat(test, control)
 
-    if alternative == 'two-sided':
-        return sum([1. if abs(x) >= abs(t_stat)
-                   else 0. for x in zero_distr]) / len(zero_distr)
-
-    if alternative == 'less':
-        return sum([1. if x <= t_stat else 0. for x in zero_distr]
-                   ) / len(zero_distr)
-
-    if alternative == 'greater':
-        return sum([1. if x >= t_stat else 0. for x in zero_distr]
-                   ) / len(zero_distr)
+    if alternative == "two-sided":
+        return sum([1.0 if abs(x) >= abs(t_stat) else 0.0 for x in zero_distr]) / len(
+            zero_distr
+        )
+
+    if alternative == "less":
+        return sum([1.0 if x <= t_stat else 0.0 for x in zero_distr]) / len(zero_distr)
+
+    if alternative == "greater":
+        return sum([1.0 if x >= t_stat else 0.0 for x in zero_distr]) / len(zero_distr)
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/regression.py` & `podlozhnyy_module-2.1/podlozhnyy_module/regression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,129 @@
-import holoviews as hv
-
+from functools import wraps
 from itertools import product
+from math import log
 
-from sklearn.metrics import r2_score
+import holoviews as hv
+from scipy.stats import f as fisher
 from sklearn.linear_model import LinearRegression
+from sklearn.metrics import r2_score
 from sklearn.model_selection import train_test_split
 from statsmodels.stats.proportion import proportion_confint
 
-from math import log
-from functools import wraps
-from scipy.stats import f as fisher
-
 from podlozhnyy_module import np, pd, plt
 
 
 def _set_options(func):
     """Обертка для применения визуальных настроек"""
+
     @wraps(func)
     def wrapper(*args, **kwargs):
         diagramm = func(*args, **kwargs)
-        for bnd, opts in [('matplotlib', matplotlib_opts),
-                          ('bokeh', bokeh_opts)]:
-            if (bnd in hv.Store._options and bnd == hv.Store.current_backend):
+        for bnd, opts in [("matplotlib", matplotlib_opts), ("bokeh", bokeh_opts)]:
+            if bnd in hv.Store._options and bnd == hv.Store.current_backend:
                 return diagramm.opts(opts)
         return diagramm
+
     return wrapper
 
 
-colors = hv.Cycle(['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd',
-                   '#8c564b', '#e377c2', '#7f7f7f', '#bcbd22', '#17becf'])
+colors = hv.Cycle(
+    [
+        "#1f77b4",
+        "#ff7f0e",
+        "#2ca02c",
+        "#d62728",
+        "#9467bd",
+        "#8c564b",
+        "#e377c2",
+        "#7f7f7f",
+        "#bcbd22",
+        "#17becf",
+    ]
+)
 
 matplotlib_opts = {
-    'Scatter.Weight_of_Evidence': {
-        'plot': dict(show_grid=True, legend_position='right', width=450),
-        'style': dict(color='r', size=5),
-    },
-    'NdOverlay.Objects_rate': {
-        'plot': dict(xrotation=45, legend_cols=1, legend_position='right'),
-    },
-    'Spread.Objects_rate': {
-        'plot': dict(show_legend=True, show_grid=True),
-        'style': dict(facecolor=colors),
-    },
-    'Overlay.Woe_Stab': {
-        'plot': dict(legend_position='right'),
-    },
-    'Curve.Weight_of_Evidence': {
-        'style': dict(color=colors),
-    },
-    'Spread.Confident_Intervals': {
-        'plot': dict(show_grid=True, xrotation=45),
-        'style': dict(facecolor=colors, alpha=0.3),
+    "Scatter.Weight_of_Evidence": {
+        "plot": dict(show_grid=True, legend_position="right", width=450),
+        "style": dict(color="r", size=5),
+    },
+    "NdOverlay.Objects_rate": {
+        "plot": dict(xrotation=45, legend_cols=1, legend_position="right"),
+    },
+    "Spread.Objects_rate": {
+        "plot": dict(show_legend=True, show_grid=True),
+        "style": dict(facecolor=colors),
+    },
+    "Overlay.Woe_Stab": {
+        "plot": dict(legend_position="right"),
+    },
+    "Curve.Weight_of_Evidence": {
+        "style": dict(color=colors),
+    },
+    "Spread.Confident_Intervals": {
+        "plot": dict(show_grid=True, xrotation=45),
+        "style": dict(facecolor=colors, alpha=0.3),
     },
 }
 
 bokeh_opts = {
-    'Scatter.Weight_of_Evidence': {
-        'plot': dict(show_grid=True, tools=['hover'], legend_position='right', width=450),
-        'style': dict(color='r', size=5),
-    },
-    'NdOverlay.Objects_rate': {
-        'plot': dict(xrotation=45, legend_position='right', width=450),
-    },
-    'Spread.Objects_rate': {
-        'plot': dict(show_legend=True, show_grid=True, tools=['hover']),
-        'style': dict(color=colors),
-    },
-    'Overlay.Woe_Stab': {
-        'plot': dict(legend_position='right', width=450),
-    },
-    'Curve.Weight_of_Evidence': {
-        'plot': dict(tools=['hover']),
-        'style': dict(color=colors),
-    },
-    'Spread.Confident_Intervals': {
-        'plot': dict(show_grid=True, xrotation=45),
-        'style': dict(color=colors, alpha=0.3),
+    "Scatter.Weight_of_Evidence": {
+        "plot": dict(
+            show_grid=True, tools=["hover"], legend_position="right", width=450
+        ),
+        "style": dict(color="r", size=5),
+    },
+    "NdOverlay.Objects_rate": {
+        "plot": dict(xrotation=45, legend_position="right", width=450),
+    },
+    "Spread.Objects_rate": {
+        "plot": dict(show_legend=True, show_grid=True, tools=["hover"]),
+        "style": dict(color=colors),
+    },
+    "Overlay.Woe_Stab": {
+        "plot": dict(legend_position="right", width=450),
+    },
+    "Curve.Weight_of_Evidence": {
+        "plot": dict(tools=["hover"]),
+        "style": dict(color=colors),
+    },
+    "Spread.Confident_Intervals": {
+        "plot": dict(show_grid=True, xrotation=45),
+        "style": dict(color=colors, alpha=0.3),
     },
 }
 
 
 def make_bucket(df, feature, num_buck=10):
     """
     Производит разбиение на бакеты
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Название признака числового или категориального
     num_buck: Количество бакетов для группирровки
     """
-    bucket = np.ceil(
-        df[feature].rank(
-            pct=True) *
-        num_buck).fillna(
-            num_buck +
-        1)
-    agg = df[feature].groupby(bucket).agg(['min', 'max'])
+    bucket = np.ceil(df[feature].rank(pct=True) * num_buck).fillna(num_buck + 1)
+    agg = df[feature].groupby(bucket).agg(["min", "max"])
 
     def _format_buck(row):
-        if row['bucket'] == num_buck + 1:
-            return 'missing'
-        elif row['min'] == row['max']:
-            return _format_(row['min'])
+        if row["bucket"] == num_buck + 1:
+            return "missing"
+        elif row["min"] == row["max"]:
+            return _format_(row["min"])
         else:
-            return _format_(row['min']) + ' - ' + _format_(row['max'])
+            return _format_(row["min"]) + " - " + _format_(row["max"])
 
-    bucket = df[[feature]].assign(bucket=bucket)\
-        .join(agg, on='bucket')\
+    bucket = (
+        df[[feature]]
+        .assign(bucket=bucket)
+        .join(agg, on="bucket")
         .apply(_format_buck, axis=1)
+    )
 
     return df.assign(bucket=bucket)
 
 
 def _format_(x, decimal=3):
     """
     Форматируем названия бакетов
@@ -122,33 +133,31 @@
     x: Вход - строка или число
     decimal: Желаемое кол-во знаков после запятой
     """
     if not isinstance(x, str):
         div, mod = x // 1, x % 1
         if mod == 0:
             if div == 0:
-                return '%d' % x
+                return "%d" % x
             elif int(np.floor(np.log10(abs(div)))) < 3:
-                return '%d' % x
+                return "%d" % x
         if div == 0:
             power = int(np.floor(np.log10(abs(mod))))
             digits = decimal - power - 1
-            return '%s' % np.around(x, digits)
+            return "%s" % np.around(x, digits)
         else:
             power = int(np.floor(np.log10(abs(div))))
             digits = decimal
             if power < 3:
-                return '%s' % np.around(x, digits)
+                return "%s" % np.around(x, digits)
             elif power < 10:
-                return '%se+0%s' % (np.around(x /
-                                    np.power(10, power), digits), power)
+                return "%se+0%s" % (np.around(x / np.power(10, power), digits), power)
             else:
-                return '%se+%s' % (np.around(x /
-                                   np.power(10, power), digits), power)
-    return '%s' % x
+                return "%se+%s" % (np.around(x / np.power(10, power), digits), power)
+    return "%s" % x
 
 
 @_set_options
 def check_linearity(df, feature, target, num_buck=10):
     """
     Позволяет оценивать линейность зависимости целевой переменной от признака.
     Строит график зависимости и лучшую регрессионную прямую (с наименьшим r_2)
@@ -156,45 +165,54 @@
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Название признака (числового!)
     target: Название целевой переменной
     num_buck: Количество бакетов, если признак числовой
     """
-    return df.pipe(make_bucket, feature, num_buck) \
-             .groupby('bucket').mean() \
-             .pipe(lambda x: hv.Scatter(zip(np.array(x[feature]), np.array(x[target])),
-                                        kdims=f'{feature}', vdims=f'{target}',
-                                        label=f"Проверка линейности зависимости {target} от {feature}")
-                   * simple_reg(np.array(x[feature]),
-                                np.array(x[target])))
+    return (
+        df.pipe(make_bucket, feature, num_buck)
+        .groupby("bucket")
+        .mean()
+        .pipe(
+            lambda x: hv.Scatter(
+                zip(np.array(x[feature]), np.array(x[target])),
+                kdims=f"{feature}",
+                vdims=f"{target}",
+                label=f"Проверка линейности зависимости {target} от {feature}",
+            )
+            * simple_reg(np.array(x[feature]), np.array(x[target]))
+        )
+    )
 
 
 @_set_options
 def check_homoscedacity(df, feature, target):
     """
     Позволяет оценивать гомоскедастичность зависимости целевой переменной от признака.
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Название признака (числового!)
     target: Название целевой переменной
     """
     simple_model = LinearRegression()
-    simple_model.fit(
-        np.array(df[feature]).reshape(-1, 1), np.array(df[target]))
+    simple_model.fit(np.array(df[feature]).reshape(-1, 1), np.array(df[target]))
     predicts = simple_model.predict(np.array(df[feature]).reshape(-1, 1))
 
     def get_residuals(y, pred):
         return np.array(y) - np.array(pred)
 
-    return hv.Scatter(zip(predicts, get_residuals(df[target], predicts)),
-                      kdims=['Estimated target'], vdims=['Residual'],
-                      label=f"Проверка гомоскедастичности признака {feature}")
+    return hv.Scatter(
+        zip(predicts, get_residuals(df[target], predicts)),
+        kdims=["Estimated target"],
+        vdims=["Residual"],
+        label=f"Проверка гомоскедастичности признака {feature}",
+    )
 
 
 def _logit(p):
     """
     Возвращает логит от вероятности
 
     Parameters
@@ -223,15 +241,15 @@
 
     Parameters
     ----------
     n: кол-во просрочек в бакете
     cnt: кол-во элементов в бакете
     q: вероятность просрочки на всем корпусе
     """
-    p_low, p_high = proportion_confint(n, cnt, method='normal')
+    p_low, p_high = proportion_confint(n, cnt, method="normal")
     return _woe(p_low, q), _woe(p_high, q)
 
 
 def bad_rate(df, feature, target, num_buck=10):
     """
     Считает bad_rate для каждого бакета признака в модели классификации.
     Возвращает датафрейм с аггрегациями (сумма таргета в бакете, среднее значение предсказания,
@@ -241,28 +259,32 @@
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Название признака (числового или категориального)
     target: Название целевой переменной
     num_buck: Количество бакетов, если признак числовой
     """
-    if df[feature].dtype == 'O':
-        return df.pipe(make_bucket, feature, num_buck)\
-            .assign(obj_cnt=1)\
-            .groupby('bucket')\
-            .agg({target: 'sum', 'obj_cnt': 'sum'})\
-            .rename(columns={target: 'target_sum'})\
+    if df[feature].dtype == "O":
+        return (
+            df.pipe(make_bucket, feature, num_buck)
+            .assign(obj_cnt=1)
+            .groupby("bucket")
+            .agg({target: "sum", "obj_cnt": "sum"})
+            .rename(columns={target: "target_sum"})
             .assign(bad_rate=lambda x: x.target_sum / x.obj_cnt)
+        )
     else:
-        return df.pipe(make_bucket, feature, num_buck)\
-            .assign(obj_cnt=1)\
-            .groupby('bucket')\
-            .agg({target: 'sum', 'obj_cnt': 'sum', feature: 'mean'})\
-            .rename(columns={target: 'target_sum', feature: 'feature_avg'})\
+        return (
+            df.pipe(make_bucket, feature, num_buck)
+            .assign(obj_cnt=1)
+            .groupby("bucket")
+            .agg({target: "sum", "obj_cnt": "sum", feature: "mean"})
+            .rename(columns={target: "target_sum", feature: "feature_avg"})
             .assign(bad_rate=lambda x: x.target_sum / x.obj_cnt)
+        )
 
 
 def woe(df, feature, target, num_buck=10):
     """
     Считает WOE для признака в модели классификации.
     Доля объектов каждого класса ограничивается 0.001 - снизу и 0.999 - сверху.
 
@@ -271,116 +293,141 @@
     df: Объект pandas.DataFrame
     feature: Название признака (числового или категориального)
     target: Название целевой переменной
     num_buck: Количество бакетов, если признак числовой
     """
     agg = bad_rate(df, feature, target, num_buck).reset_index()
     agg = agg[agg.target_sum != 0]
-    return agg.assign(nums=agg['obj_cnt'].sum(), bad_nums=agg['target_sum'].sum())\
-              .assign(woe=lambda x: _woe(x.bad_rate, x.bad_nums / x.nums))\
-              .drop(['bad_nums', 'nums'], axis=1)\
-              .sort_values(by='woe', ascending=False)\
-              .set_index('bucket')
+    return (
+        agg.assign(nums=agg["obj_cnt"].sum(), bad_nums=agg["target_sum"].sum())
+        .assign(woe=lambda x: _woe(x.bad_rate, x.bad_nums / x.nums))
+        .drop(["bad_nums", "nums"], axis=1)
+        .sort_values(by="woe", ascending=False)
+        .set_index("bucket")
+    )
 
 
 def IV(df, feature, target, num_buck=10):
     """
     Считает Information Value для признака в модели бинарной классификации.
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Название признака (числового или категориального)
     target: Название целевой переменной
     num_buck: Количество бакетов, если признак числовой
     """
-    return woe(df, feature, target, num_buck)\
-        .assign(iv=lambda x: (x.target_sum / x.target_sum.sum() -
-                              (x.obj_cnt - x.target_sum) / (x.obj_cnt.sum() - x.target_sum.sum())) * x.woe)\
+    return (
+        woe(df, feature, target, num_buck)
+        .assign(
+            iv=lambda x: (
+                x.target_sum / x.target_sum.sum()
+                - (x.obj_cnt - x.target_sum) / (x.obj_cnt.sum() - x.target_sum.sum())
+            )
+            * x.woe
+        )
         .iv.sum()
+    )
 
 
 def iv_report(df, features, target, num_buck=10):
     """
     Считает IV для указанных признаков в модели классификации.
     Возвращает в порядке убывания кортежи из трех элементов:(признак, IV, интерпретация)
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     features: Список названий признаков (числовых или категориальных)
     target: Название целевой переменной
     num_buck: Количество бакетов для разбиения
     """
+
     def desc(x):
         if x > 0.5:
-            power = 'Suspicious'
+            power = "Suspicious"
         elif x > 0.3:
-            power = 'Strong'
+            power = "Strong"
         elif x > 0.1:
-            power = 'Medium'
+            power = "Medium"
         elif x > 0.02:
-            power = 'Weak'
+            power = "Weak"
         else:
-            power = 'Useless'
+            power = "Useless"
         return (x, power)
 
     ivs = {}
     for column in list(features):
         ivs[column] = desc(IV(df, column, target, num_buck))
 
     ivs = list(ivs.items())
     ivs.sort(key=lambda i: i[1], reverse=True)
-    print('         Name         ||  Value  || Interpretation')
-    print('--------------------------------------------------')
+    print("         Name         ||  Value  || Interpretation")
+    print("--------------------------------------------------")
     for feature in ivs:
-        print(f'{feature[0]:21} ||  {feature[1][0]:.3f}  || {feature[1][1]}')
+        print(f"{feature[0]:21} ||  {feature[1][0]:.3f}  || {feature[1][1]}")
 
 
 def iv_agg(df, features, target, num_bucks=[10, 10]):
     """
     Считает совокупный IV для указанных признаков в модели бинарной классификации.
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     features: Список названий признаков (числовых или категориальных)
     target: Название целевой переменной
     num_bucks: Список количества бакетов для каждой из переменных
     """
-    index = make_bucket(df[[features[-1]]], features[-1],
-                        num_buck=num_bucks[-1])['bucket'].values
+    index = make_bucket(df[[features[-1]]], features[-1], num_buck=num_bucks[-1])[
+        "bucket"
+    ].values
     columns = []
 
     for i, feature in enumerate(features[:-1]):
-        columns.append(make_bucket(
-            df[[feature]], feature, num_buck=num_bucks[i])['bucket'].values)
-
-    obj_cnt = (pd.crosstab(index=index,
-                           columns=columns,
-                           margins=True))
-    target_sum = (pd.crosstab(index=index,
-                              columns=columns,
-                              values=df[target].values,
-                              aggfunc=np.sum,
-                              margins=True))
-    bad_rate = (pd.crosstab(index=index,
-                            columns=columns,
-                            values=df[target].values,
-                            aggfunc=np.mean,
-                            margins=True))
-    agg = pd.DataFrame({'obj_cnt': obj_cnt.iloc[:-1, :-1].unstack().values,
-                        'target_sum': target_sum.iloc[:-1, :-1].unstack().values,
-                        'bad_rate': bad_rate.iloc[:-1, :-1].unstack().values})
+        columns.append(
+            make_bucket(df[[feature]], feature, num_buck=num_bucks[i])["bucket"].values
+        )
+
+    obj_cnt = pd.crosstab(index=index, columns=columns, margins=True)
+    target_sum = pd.crosstab(
+        index=index,
+        columns=columns,
+        values=df[target].values,
+        aggfunc=np.sum,
+        margins=True,
+    )
+    bad_rate = pd.crosstab(
+        index=index,
+        columns=columns,
+        values=df[target].values,
+        aggfunc=np.mean,
+        margins=True,
+    )
+    agg = pd.DataFrame(
+        {
+            "obj_cnt": obj_cnt.iloc[:-1, :-1].unstack().values,
+            "target_sum": target_sum.iloc[:-1, :-1].unstack().values,
+            "bad_rate": bad_rate.iloc[:-1, :-1].unstack().values,
+        }
+    )
     agg = agg[agg.target_sum != 0]
-    return agg.assign(nums=agg['obj_cnt'].sum(), bad_nums=agg['target_sum'].sum())\
-              .assign(woe=lambda x: _woe(x.bad_rate, x.bad_nums / x.nums))\
-              .assign(iv=lambda x: (x.target_sum / x.target_sum.sum() -
-                                    (x.obj_cnt - x.target_sum) / (x.obj_cnt.sum() - x.target_sum.sum())) * x.woe)\
-              .iv.sum()
+    return (
+        agg.assign(nums=agg["obj_cnt"].sum(), bad_nums=agg["target_sum"].sum())
+        .assign(woe=lambda x: _woe(x.bad_rate, x.bad_nums / x.nums))
+        .assign(
+            iv=lambda x: (
+                x.target_sum / x.target_sum.sum()
+                - (x.obj_cnt - x.target_sum) / (x.obj_cnt.sum() - x.target_sum.sum())
+            )
+            * x.woe
+        )
+        .iv.sum()
+    )
 
 
 @_set_options
 def simple_reg(predictor, target):
     """
     Строит простую линейную регрессию
     Использует для отрисовки прямой и подсчета r^2
@@ -388,16 +435,21 @@
     Parameters
     ----------
     predictor: Массив значений признака
     target: Массив значений целевой переменной
     """
     check = LinearRegression()
     check.fit(predictor.reshape(-1, 1), target)
-    return hv.Curve((np.array([min(predictor) - 1, max(predictor) + 1]),
-                     check.coef_ * np.array([min(predictor) - 1, max(predictor) + 1]) + check.intercept_))
+    return hv.Curve(
+        (
+            np.array([min(predictor) - 1, max(predictor) + 1]),
+            check.coef_ * np.array([min(predictor) - 1, max(predictor) + 1])
+            + check.intercept_,
+        )
+    )
 
 
 def r_2check(df, feature, target, num_buck=10):
     """
     Для заданного признака строт простую линейную регрессию для бакетов получаемых из функции woe
     Возвращает r2_score полученного результата
 
@@ -430,161 +482,185 @@
     feature: Название признака (числового!)
     target: Название целевой переменной
     num_buck: Количество бакетов, если признак числовой
     """
 
     agg = bad_rate(df, feature, target, num_buck).reset_index()
     agg = agg[(agg.target_sum != 0) & (agg.feature_avg.notnull())]
-    agg = agg.assign(nums=agg['obj_cnt'].sum(), bad_nums=agg['target_sum'].sum())\
-        .assign(woe=lambda x: _woe(x.bad_rate, x.bad_nums / x.nums),
-                woe_low=lambda x: _woe_confint(x.target_sum,
-                                               x.obj_cnt,
-                                               x.bad_nums / x.nums)[0],
-                woe_high=lambda x: _woe_confint(x.target_sum,
-                                                x.obj_cnt,
-                                                x.bad_nums / x.nums)[1])\
-        .assign(woe_u=lambda x: x.woe_high - x.woe,
-                woe_b=lambda x: x.woe - x.woe_low)
+    agg = (
+        agg.assign(nums=agg["obj_cnt"].sum(), bad_nums=agg["target_sum"].sum())
+        .assign(
+            woe=lambda x: _woe(x.bad_rate, x.bad_nums / x.nums),
+            woe_low=lambda x: _woe_confint(
+                x.target_sum, x.obj_cnt, x.bad_nums / x.nums
+            )[0],
+            woe_high=lambda x: _woe_confint(
+                x.target_sum, x.obj_cnt, x.bad_nums / x.nums
+            )[1],
+        )
+        .assign(woe_u=lambda x: x.woe_high - x.woe, woe_b=lambda x: x.woe - x.woe_low)
+    )
 
     r2_woe = r_2check(df, feature, target, num_buck)
-    scatter = hv.Scatter(data=agg,
-                         kdims=['feature_avg'],
-                         vdims=['woe'],
-                         group='Weight of Evidence',
-                         label=f'r2_score = {r2_woe}')
-    errors = hv.ErrorBars(data=agg,
-                          kdims=['feature_avg'],
-                          vdims=['woe', 'woe_u', 'woe_b'],
-                          group='Confident Intervals')
+    scatter = hv.Scatter(
+        data=agg,
+        kdims=["feature_avg"],
+        vdims=["woe"],
+        group="Weight of Evidence",
+        label=f"r2_score = {r2_woe}",
+    )
+    errors = hv.ErrorBars(
+        data=agg,
+        kdims=["feature_avg"],
+        vdims=["woe", "woe_u", "woe_b"],
+        group="Confident Intervals",
+    )
     reg = simple_reg(np.array(agg.feature_avg), np.array(agg.woe))
-    return hv.Overlay(items=[scatter, errors, reg],
-                      group='Woe Curve',
-                      label=feature).redim.range(feature_avg=(agg.feature_avg.min() * 1.15,
-                                                              agg.feature_avg.max() * 1.15),
-                                                 woe=(agg.woe.min() * 1.15,
-                                                      agg.woe.max() * 1.15))
+    return hv.Overlay(
+        items=[scatter, errors, reg], group="Woe Curve", label=feature
+    ).redim.range(
+        feature_avg=(agg.feature_avg.min() * 1.15, agg.feature_avg.max() * 1.15),
+        woe=(agg.woe.min() * 1.15, agg.woe.max() * 1.15),
+    )
+
 
 # Динамика переменных и WoE
 
 
 @_set_options
-def distribution(df, feature, date, num_buck=10, date_freq='Q'):
+def distribution(df, feature, date, num_buck=10, date_freq="Q"):
     """
     Строит график распределения признака во времени
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Название признака числового или категориального
     date: Наименование временной переменной
     num_buck: Количество бакетов, если признак числовой
     date_freq: Частота агрегации времени
     """
-    agg = df.pipe(make_bucket, feature, num_buck)\
-            .assign(obj_cnt=1)\
-            .groupby([pd.Grouper(key=date, freq=date_freq), 'bucket'])\
-            .agg({'obj_cnt': sum})\
-            .reset_index()\
-            .assign(obj_total=lambda x: (x.groupby([pd.Grouper(key=date,
-                                                               freq=date_freq)])['obj_cnt'].transform('sum')))\
-            .assign(obj_rate=lambda x: x.obj_cnt / x.obj_total)\
-            .reset_index()\
-            .assign(objects_rate=lambda x:
-                    x.groupby(date).apply(
-                        lambda y: y.obj_rate.cumsum().to_frame())
-                    .reset_index(drop=True))\
-        .assign(obj_rate_u=0, obj_rate_b=lambda x: x['obj_rate'])
+    agg = (
+        df.pipe(make_bucket, feature, num_buck)
+        .assign(obj_cnt=1)
+        .groupby([pd.Grouper(key=date, freq=date_freq), "bucket"])
+        .agg({"obj_cnt": sum})
+        .reset_index()
+        .assign(
+            obj_total=lambda x: (
+                x.groupby([pd.Grouper(key=date, freq=date_freq)])["obj_cnt"].transform(
+                    "sum"
+                )
+            )
+        )
+        .assign(obj_rate=lambda x: x.obj_cnt / x.obj_total)
+        .reset_index()
+        .assign(
+            objects_rate=lambda x: x.groupby(date)
+            .apply(lambda y: y.obj_rate.cumsum().to_frame())
+            .reset_index(drop=True)
+        )
+        .assign(obj_rate_u=0, obj_rate_b=lambda x: x["obj_rate"])
+    )
 
     data = hv.Dataset(
-        agg, kdims=[
-            'bucket', date], vdims=[
-            'objects_rate', 'obj_rate_b', 'obj_rate_u'])
-
-    return data.to.spread(kdims=[date],
-                          vdims=['objects_rate', 'obj_rate_b', 'obj_rate_u'],
-                          group='Objects rate',
-                          label=feature).overlay('bucket')
+        agg, kdims=["bucket", date], vdims=["objects_rate", "obj_rate_b", "obj_rate_u"]
+    )
+
+    return data.to.spread(
+        kdims=[date],
+        vdims=["objects_rate", "obj_rate_b", "obj_rate_u"],
+        group="Objects rate",
+        label=feature,
+    ).overlay("bucket")
 
 
 @_set_options
-def woe_stab(df, feature, target, date, num_buck=3, date_freq='Q'):
+def woe_stab(df, feature, target, date, num_buck=3, date_freq="Q"):
     """
     Строит WoE признака во времени, позволяет оценить его устойчивость
 
     Parameters
     ----------
     df: Объект pandas.DataFrame
     feature: Название признака числового или категориального
     target: Название целевой переменной
     date: Наименование временной переменной
     num_buck: Количество бакетов, если признак числовой
     date_freq: Частота агрегации времени
     """
-    agg = df.pipe(make_bucket, feature, num_buck)\
-            .assign(obj_cnt=1)\
-            .groupby([pd.Grouper(key=date, freq=date_freq), 'bucket'])\
-            .agg({target: 'sum', 'obj_cnt': sum})\
-            .rename(columns={target: 'target_sum'})\
-            .assign(bad_rate=lambda x: x.target_sum / x.obj_cnt)
+    agg = (
+        df.pipe(make_bucket, feature, num_buck)
+        .assign(obj_cnt=1)
+        .groupby([pd.Grouper(key=date, freq=date_freq), "bucket"])
+        .agg({target: "sum", "obj_cnt": sum})
+        .rename(columns={target: "target_sum"})
+        .assign(bad_rate=lambda x: x.target_sum / x.obj_cnt)
+    )
 
-    agg = agg.assign(nums=agg.groupby([date])['obj_cnt'].transform('sum'),
-                     bad_nums=agg.groupby([date])['target_sum'].transform('sum'))\
-        .assign(woe=lambda x: _woe(x.bad_rate, x.bad_nums / x.nums),
-                woe_low=lambda x: _woe_confint(x.target_sum,
-                                               x.obj_cnt,
-                                               x.bad_nums / x.nums)[0],
-                woe_high=lambda x: _woe_confint(x.target_sum,
-                                                x.obj_cnt,
-                                                x.bad_nums / x.nums)[1])\
-        .assign(woe_u=lambda x: x.woe_high - x.woe,
-                woe_b=lambda x: x.woe - x.woe_low)\
+    agg = (
+        agg.assign(
+            nums=agg.groupby([date])["obj_cnt"].transform("sum"),
+            bad_nums=agg.groupby([date])["target_sum"].transform("sum"),
+        )
+        .assign(
+            woe=lambda x: _woe(x.bad_rate, x.bad_nums / x.nums),
+            woe_low=lambda x: _woe_confint(
+                x.target_sum, x.obj_cnt, x.bad_nums / x.nums
+            )[0],
+            woe_high=lambda x: _woe_confint(
+                x.target_sum, x.obj_cnt, x.bad_nums / x.nums
+            )[1],
+        )
+        .assign(woe_u=lambda x: x.woe_high - x.woe, woe_b=lambda x: x.woe - x.woe_low)
         .reset_index()
+    )
 
     agg = agg[agg.target_sum != 0]
 
-    data = hv.Dataset(
-        agg, kdims=[
-            'bucket', date], vdims=[
-            'woe', 'woe_b', 'woe_u'])
-
-    confident_intervals = (data.to.spread(kdims=[date],
-                                          vdims=['woe', 'woe_b', 'woe_u'],
-                                          group='Confident Intervals')
-                           .overlay('bucket'))
-    woe_curves = (data.to.curve(kdims=[date],
-                                vdims=['woe'],
-                                group='Weight of Evidence')
-                  .overlay('bucket'))
-    return hv.Overlay(items=[confident_intervals * woe_curves],
-                      group='Woe Stab',
-                      label=f'{feature}')
+    data = hv.Dataset(agg, kdims=["bucket", date], vdims=["woe", "woe_b", "woe_u"])
+
+    confident_intervals = data.to.spread(
+        kdims=[date], vdims=["woe", "woe_b", "woe_u"], group="Confident Intervals"
+    ).overlay("bucket")
+    woe_curves = data.to.curve(
+        kdims=[date], vdims=["woe"], group="Weight of Evidence"
+    ).overlay("bucket")
+    return hv.Overlay(
+        items=[confident_intervals * woe_curves], group="Woe Stab", label=f"{feature}"
+    )
 
 
 def HL(target, predict, num_buck=10):
     """
     Считает статистику Хосмера-Лемешева
 
     Parameters
     ----------
     target - истинные значения целевой переменной
     predict - предсказания вероятности
     num_buck - количество бакетов
     """
-    data = pd.DataFrame({'target': target, 'predict': predict})
+    data = pd.DataFrame({"target": target, "predict": predict})
 
     data = (
-        data.pipe(make_bucket, 'predict', num_buck)
-            .assign(obj_cnt=1)
-            .groupby('bucket')
-            .agg({'target': 'sum', 'predict': 'mean', 'obj_cnt': 'sum'})
-            .assign(bad_rate=lambda x: x.target / x.obj_cnt)
-            .reset_index()
+        data.pipe(make_bucket, "predict", num_buck)
+        .assign(obj_cnt=1)
+        .groupby("bucket")
+        .agg({"target": "sum", "predict": "mean", "obj_cnt": "sum"})
+        .assign(bad_rate=lambda x: x.target / x.obj_cnt)
+        .reset_index()
+    )
+    return int(
+        sum(
+            (data.predict - data.bad_rate) ** 2
+            / (data.predict * (1 - data.predict))
+            * data.obj_cnt
+        )
     )
-    return int(sum((data.predict - data.bad_rate) ** 2 /
-               (data.predict * (1 - data.predict)) * data.obj_cnt))
 
 
 @_set_options
 def plot_gain_chart(target, predict, num_buck=10):
     """
     Строит gain_chart по истиным и предсказанным меткам
     На первом шаге бьет наблюдения на бакеты, затем считает средний bad_rate.
@@ -592,33 +668,39 @@
 
     Parameters
     ----------
     target - истинные значения целевой переменной
     predict - предсказания вероятности
     num_buck - количество бакетов
     """
-    data = pd.DataFrame({'target': target, 'predict': predict})
+    data = pd.DataFrame({"target": target, "predict": predict})
     H = HL(target, predict, num_buck)
     data = (
-        data.assign(bucket=np.ceil(data['predict'].rank(pct=True) * num_buck))
-            .assign(obj_cnt=1)
-            .groupby('bucket')
-            .agg({'target': 'sum', 'predict': 'mean', 'obj_cnt': 'sum'})
-            .assign(bad_rate=lambda x: x.target / x.obj_cnt)
-            .reset_index()
+        data.assign(bucket=np.ceil(data["predict"].rank(pct=True) * num_buck))
+        .assign(obj_cnt=1)
+        .groupby("bucket")
+        .agg({"target": "sum", "predict": "mean", "obj_cnt": "sum"})
+        .assign(bad_rate=lambda x: x.target / x.obj_cnt)
+        .reset_index()
     )
 
-    bars_gain = hv.Bars(data, kdims=['bucket'], vdims=['bad_rate'], label='observed') \
-                  .opts(plot={'xrotation': 90, 'show_legend': True}, style={'color': 'yellow'})
-
-    curve_gain = hv.Curve(data, kdims=['bucket'], vdims=['predict'], label='predicted') \
-        .opts(plot={'xrotation': 90, 'show_legend': True}, style={'color': 'black'})
-
-    return hv.Overlay([bars_gain, curve_gain]).redim.label(**{'target': 'Bad Rate'})\
-             .relabel(f'HL_score = {H}').opts(plot={'legend_position': 'top_left'})
+    bars_gain = hv.Bars(
+        data, kdims=["bucket"], vdims=["bad_rate"], label="observed"
+    ).opts(plot={"xrotation": 90, "show_legend": True}, style={"color": "yellow"})
+
+    curve_gain = hv.Curve(
+        data, kdims=["bucket"], vdims=["predict"], label="predicted"
+    ).opts(plot={"xrotation": 90, "show_legend": True}, style={"color": "black"})
+
+    return (
+        hv.Overlay([bars_gain, curve_gain])
+        .redim.label(**{"target": "Bad Rate"})
+        .relabel(f"HL_score = {H}")
+        .opts(plot={"legend_position": "top_left"})
+    )
 
 
 def feature_importance(names, values, verbose=False, thr=0.05):
     """
     Возвращает словарь и печатает в порядке убывания коэффициенты для признаков
 
     Parameters
@@ -633,69 +715,71 @@
     for name, value in zip(names, values):
         val_dict[name] = round(value, 3)
     if verbose:
         coef_list = list(val_dict.items())
         coef_list.sort(key=lambda i: i[1], reverse=True)
         for i in coef_list:
             if i[1] >= thr:
-                print(i[0], ':', round(i[1], 5))
+                print(i[0], ":", round(i[1], 5))
     return val_dict
 
 
 @_set_options
 def plot_confusion_matrix(
-    cm,
-    classes,
-    normalize=False,
-    title='Confusion matrix',
-    cmap=plt.cm.Blues
+    cm, classes, normalize=False, title="Confusion matrix", cmap=plt.cm.Blues
 ) -> None:
     """
     Печатает и отрисовывает матрицу ошибок для задачи классификации
     Для нормализации небходимо передать аргумент normalize=True
 
     Parameters
     ----------
     cm: Матрица ошибок вида metrics.confusion_matrix(.., ..)
     classes: Наименование для значений целевой переменной
     normalize: Булева переменная, для нормализации матрицы
     title: Название для графика
     cmap: Цветовая палитра, по умолчанию: plt.cm.Blues
     """
-    plt.imshow(cm, interpolation='nearest', cmap=cmap)
+    plt.imshow(cm, interpolation="nearest", cmap=cmap)
     plt.title(title)
     plt.colorbar()
     tick_marks = np.arange(len(classes))
     bottom, top = plt.ylim()
     plt.xticks(tick_marks, classes, rotation=45)
     plt.yticks(tick_marks, classes, rotation=45)
     plt.ylim([bottom, top])
 
     if normalize:
-        cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
+        cm = cm.astype("float") / cm.sum(axis=1)[:, np.newaxis]
         print("Normalized confusion matrix")
     else:
-        print('Confusion matrix, without normalization')
+        print("Confusion matrix, without normalization")
 
     print(cm)
 
-    thresh = cm.max() / 2.
+    thresh = cm.max() / 2.0
     for i, j in product(range(cm.shape[0]), range(cm.shape[1])):
-        plt.text(j, i, cm[i, j],
-                 horizontalalignment="center",
-                 verticalalignment="center",
-                 color="white" if cm[i, j] > thresh else "black")
+        plt.text(
+            j,
+            i,
+            cm[i, j],
+            horizontalalignment="center",
+            verticalalignment="center",
+            color="white" if cm[i, j] > thresh else "black",
+        )
 
     plt.tight_layout()
-    plt.ylabel('Истинный класс')
-    plt.xlabel('Предсказанный класс')
+    plt.ylabel("Истинный класс")
+    plt.xlabel("Предсказанный класс")
     plt.show()
 
 
-def regression_report(X: pd.core.frame.DataFrame, y: np.ndarray, model: object, **kwargs) -> dict:
+def regression_report(
+    X: pd.core.frame.DataFrame, y: np.ndarray, model: object, **kwargs
+) -> dict:
     """
     Обучает заданную модель регрессии на предоставленных данных.
     В стандартный поток вывода публикуются метрики качества построенной модели и важность признаков.
     Возвращает словарь весов признаков для линейной модели или словарь важности для деревьев и ансамблей.
 
     Parameters
     ----------
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module/timeseries.py` & `podlozhnyy_module-2.1/podlozhnyy_module/timeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,18 +44,18 @@
                 continue
             if i >= len(self.series):  # прогнозируем
                 m = i - len(self.series) + 1
                 self.result.append(level + m * trend)
             else:
                 self.result.append(level + trend)
                 val = self.series[i]
-                prev_level, level = level, self.alpha * \
-                    val + (1 - self.alpha) * (level + trend)
-                trend = self.beta * (level - prev_level) + \
-                    (1 - self.beta) * trend
+                prev_level, level = level, self.alpha * val + (1 - self.alpha) * (
+                    level + trend
+                )
+                trend = self.beta * (level - prev_level) + (1 - self.beta) * trend
 
             self.Level.append(level)
             self.Trend.append(trend)
 
 
 class HoltWinters:
 
@@ -81,45 +81,46 @@
     Season: массив сезонных компонент в модели сглаживаня
     Trend: массив значений тренда в модели сглаживаня
     UpperBond: массив верхних границ дов.интервалов Брутлага
     LowerBond: массив нижних значений дов.интерваллов Брутлага
 
     """
 
-    def __init__(self, series, slen, alpha, beta,
-                 gamma, n_preds, scaling_factor=1.96):
+    def __init__(self, series, slen, alpha, beta, gamma, n_preds, scaling_factor=1.96):
         self.series = series
         self.slen = slen
         self.alpha = alpha
         self.beta = beta
         self.gamma = gamma
         self.n_preds = n_preds
         self.scaling_factor = scaling_factor
 
     def initial_trend(self):
         sum = 0.0
         for i in range(self.slen):
-            sum += float(self.series[i + self.slen] -
-                         self.series[i]) / self.slen
+            sum += float(self.series[i + self.slen] - self.series[i]) / self.slen
         return sum / self.slen
 
     def initial_seasonal_components(self):
         seasonals = {}
         season_averages = []
         n_seasons = int(len(self.series) / self.slen)
         # вычисляем сезонные средние
         for j in range(n_seasons):
             season_averages.append(
-                sum(self.series[self.slen * j: self.slen * j + self.slen]) / float(self.slen))
+                sum(self.series[self.slen * j : self.slen * j + self.slen])
+                / float(self.slen)
+            )
         # вычисляем начальные значения
         for i in range(self.slen):
             sum_of_vals_over_avg = 0.0
             for j in range(n_seasons):
-                sum_of_vals_over_avg += self.series[self.slen *
-                                                    j + i] - season_averages[j]
+                sum_of_vals_over_avg += (
+                    self.series[self.slen * j + i] - season_averages[j]
+                )
             seasonals[i] = sum_of_vals_over_avg / n_seasons
         return seasonals
 
     def triple_exponential_smoothing(self):
         self.result = []
         self.Smooth = []
         self.Season = []
@@ -138,64 +139,65 @@
                 self.Smooth.append(smooth)
                 self.Trend.append(trend)
 
                 self.Season.append(seasonals[i % self.slen])
 
                 self.PredictedDeviation.append(deviations[i % self.slen])
 
-                self.UpperBond.append(self.result[0] +
-                                      self.scaling_factor *
-                                      self.PredictedDeviation[0])
-
-                self.LowerBond.append(self.result[0] -
-                                      self.scaling_factor *
-                                      self.PredictedDeviation[0])
+                self.UpperBond.append(
+                    self.result[0] + self.scaling_factor * self.PredictedDeviation[0]
+                )
+
+                self.LowerBond.append(
+                    self.result[0] - self.scaling_factor * self.PredictedDeviation[0]
+                )
                 continue
             if i >= len(self.series):  # прогнозируем
                 m = i - len(self.series) + 1
-                self.result.append(smooth + m * trend +
-                                   seasonals[i % self.slen])
+                self.result.append(smooth + m * trend + seasonals[i % self.slen])
 
                 # во время прогноза с каждым шагом увеличиваем неопределенность
                 prev_deviation = deviations[i % self.slen]
                 deviations[i % self.slen] = deviations[i % self.slen] * 1.01
 
             else:
                 self.result.append(smooth + trend + seasonals[i % self.slen])
                 val = self.series[i]
-                prev_smooth, smooth = smooth, self.alpha * \
-                    (val - seasonals[i % self.slen]) + \
-                    (1 - self.alpha) * (smooth + trend)
-                trend = self.beta * (smooth - prev_smooth) + \
-                    (1 - self.beta) * trend
-                seasonals[i % self.slen] = self.gamma * \
-                    (val - smooth) + (1 - self.gamma) * \
-                    seasonals[i % self.slen]
+                prev_smooth, smooth = smooth, self.alpha * (
+                    val - seasonals[i % self.slen]
+                ) + (1 - self.alpha) * (smooth + trend)
+                trend = self.beta * (smooth - prev_smooth) + (1 - self.beta) * trend
+                seasonals[i % self.slen] = (
+                    self.gamma * (val - smooth)
+                    + (1 - self.gamma) * seasonals[i % self.slen]
+                )
 
                 # Отклонение рассчитывается в соответствии с алгоритмом
                 # Брутлага
                 prev_deviation = deviations[i % self.slen]
-                deviations[i % self.slen] = self.gamma * np.abs(
-                    self.series[i] - self.result[i]) + (1 - self.gamma) * prev_deviation
-
-            self.UpperBond.append(self.result[-1] +
-                                  self.scaling_factor *
-                                  prev_deviation)
-
-            self.LowerBond.append(self.result[-1] -
-                                  self.scaling_factor *
-                                  prev_deviation)
+                deviations[i % self.slen] = (
+                    self.gamma * np.abs(self.series[i] - self.result[i])
+                    + (1 - self.gamma) * prev_deviation
+                )
+
+            self.UpperBond.append(
+                self.result[-1] + self.scaling_factor * prev_deviation
+            )
+
+            self.LowerBond.append(
+                self.result[-1] - self.scaling_factor * prev_deviation
+            )
 
             self.Smooth.append(smooth)
             self.Trend.append(trend)
             self.Season.append(seasonals[i % self.slen])
             self.PredictedDeviation.append(deviations[i % self.slen])
 
 
-def timeseriesCVscore(x, data, r=0, method='HoltWinters', slen=7):
+def timeseriesCVscore(x, data, r=0, method="HoltWinters", slen=7):
     """
     Производит кросс-валидацию на временных рядах для модели линейного тренда Хольта или модели Хольта-Винтерса
     Максимальное значение n_splits, таково, что (n_splits + 1) * 2 * slen <= len(data) (для линейной модели Хольта slen=1)
     Возвращает функцию, которую надо передать на вход оптимизатору, например:
     opt = scipy.optimize.minimize(timeseriesCVscore, x0=[0, 0, 0], args=(data, ), method="TNC", bounds = ((0, 1), (0, 1), (0, 1)))
     Из оптимизатора можно взять  оптимальные значение параметров:
     alpha, beta, gamma = opt.x
@@ -209,52 +211,52 @@
     method: Какую модель требуется валидировать двойного ('Holt') или тройного ('HoltWinters') экспоненциального сглаживания
     slen: Длина сезона для method = 'HoltWinters'
     """
     # Метрика
     def weighted_mse(actual, predictions, r):
         weights = [1 / np.power(1 + r, i) for i in range(len(actual), 0, -1)]
         return np.mean(
-            ((np.array(actual) - np.array(predictions)) ** 2) * np.array(weights))
+            ((np.array(actual) - np.array(predictions)) ** 2) * np.array(weights)
+        )
 
     # Вектор ошибок
     errors = []
 
     # Данные в numpy массив
     values = data.values
 
     # Задаём число фолдов для кросс-валидации
     tscv = TimeSeriesSplit(n_splits=3)
 
     # Идем по фолдам, на каждом обучаем модель, строим прогноз на отложенной
     # выборке и считаем ошибку
     for train, test in tscv.split(values):
 
-        if method == 'HoltWinters':
+        if method == "HoltWinters":
             model = HoltWinters(
                 series=values[train],
                 slen=slen,
                 alpha=x[0],
                 beta=x[1],
                 gamma=x[2],
-                n_preds=len(test))
+                n_preds=len(test),
+            )
             model.triple_exponential_smoothing()
 
-        if method == 'Holt':
+        if method == "Holt":
             model = HoltLinearTrend(
-                series=values[train],
-                alpha=x[0],
-                beta=x[1],
-                n_preds=len(test))
+                series=values[train], alpha=x[0], beta=x[1], n_preds=len(test)
+            )
             model.double_exponential_smoothing()
 
-        predictions = model.result[-len(test):]
+        predictions = model.result[-len(test) :]
         actual = values[test]
 
-    # Можно считать обыычный MSE или взвесить и дать больший вес свежим
-    # значением
+        # Можно считать обыычный MSE или взвесить и дать больший вес свежим
+        # значением
         error = weighted_mse(actual, predictions, r=r)
         errors.append(error)
 
     # Возвращаем средний квадрат ошибки по вектору ошибок
     return np.mean(np.array(errors))
 
 
@@ -267,28 +269,28 @@
     model: обучення модель Хольта
     dataset: Объект pandas.DataFrame
     target: Пригнозирумая переменная
     predict_interval: Временной интервал для прогнозирования
     xlim: Сколько последних точек надо отобразить на графике, по умолчанию - все
     """
     if len(model.result) > len(dataset):
-        dataset = pd.concat([dataset, pd.DataFrame(
-            np.array([np.NaN] * predict_interval), columns=[target])])
+        dataset = pd.concat(
+            [
+                dataset,
+                pd.DataFrame(np.array([np.NaN] * predict_interval), columns=[target]),
+            ]
+        )
     plt.figure(figsize=(25, 10))
     plt.plot(model.result, "b", label="Model")
     plt.plot(dataset[target].values, "g", label="Actual")
     plt.axvspan(
-        len(dataset) -
-        predict_interval -
-        1,
-        len(dataset),
-        alpha=0.5,
-        color='lightgrey')
+        len(dataset) - predict_interval - 1, len(dataset), alpha=0.5, color="lightgrey"
+    )
     plt.grid(True)
-    plt.axis('tight')
+    plt.axis("tight")
     plt.legend(loc="best", fontsize=13)
     if xlim:
         plt.xlim(len(dataset) - xlim, len(dataset))
     plt.show()
 
 
 def plotHoltWinters(model, dataset, target, predict_interval, xlim=None):
@@ -301,39 +303,42 @@
     model: обучення модель Хольта-Винтреса
     dataset: Объект pandas.DataFrame
     target: Пригнозирумая переменная
     predict_interval: Временной интервал для прогнозирования
     xlim: Сколько последних точек надо отобразить на графике, по умолчанию - все
     """
     if len(model.result) > len(dataset):
-        dataset = pd.concat([dataset, pd.DataFrame(
-            np.array([np.NaN] * predict_interval), columns=[target])])
+        dataset = pd.concat(
+            [
+                dataset,
+                pd.DataFrame(np.array([np.NaN] * predict_interval), columns=[target]),
+            ]
+        )
     Anomalies = np.array([np.NaN] * len(dataset[target]))
-    Anomalies[dataset[target].values <
-              model.LowerBond] = dataset[target].values[dataset[target].values < model.LowerBond]
-    Anomalies[dataset[target].values >
-              model.UpperBond] = dataset[target].values[dataset[target].values > model.UpperBond]
+    Anomalies[dataset[target].values < model.LowerBond] = dataset[target].values[
+        dataset[target].values < model.LowerBond
+    ]
+    Anomalies[dataset[target].values > model.UpperBond] = dataset[target].values[
+        dataset[target].values > model.UpperBond
+    ]
     plt.figure(figsize=(25, 10))
     plt.plot(model.result, "b", label="Model")
     plt.plot(model.UpperBond, "k--", alpha=0.5, label="Up/Low confidence")
     plt.plot(model.LowerBond, "k--", alpha=0.5)
-    plt.fill_between(x=range(0,
-                             len(model.result)),
-                     y1=model.UpperBond,
-                     y2=model.LowerBond,
-                     alpha=0.5,
-                     color="grey")
+    plt.fill_between(
+        x=range(0, len(model.result)),
+        y1=model.UpperBond,
+        y2=model.LowerBond,
+        alpha=0.5,
+        color="grey",
+    )
     plt.plot(dataset[target].values, "g", label="Actual")
     plt.plot(Anomalies, "ro", markersize=7, label="Anomalies")
     plt.axvspan(
-        len(dataset) -
-        predict_interval -
-        1,
-        len(dataset),
-        alpha=0.5,
-        color='lightgrey')
+        len(dataset) - predict_interval - 1, len(dataset), alpha=0.5, color="lightgrey"
+    )
     plt.grid(True)
-    plt.axis('tight')
+    plt.axis("tight")
     plt.legend(loc="best", fontsize=13)
     if xlim:
         plt.xlim(len(dataset) - xlim, len(dataset))
     plt.show()
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module.egg-info/PKG-INFO` & `podlozhnyy_module-2.1/podlozhnyy_module.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podlozhnyy-module
-Version: 2.0
+Version: 2.1
 Summary: One place for the most useful methods for work
 Home-page: https://github.com/NPodlozhniy/podlozhnyy-module
 Author: Nikita Podlozhnyy
 Author-email: podlozhnyy.ne@phystech.edu
 License: MIT
 Description: # podlozhnyy-module
```

### Comparing `podlozhnyy_module-2.0/podlozhnyy_module.egg-info/SOURCES.txt` & `podlozhnyy_module-2.1/podlozhnyy_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podlozhnyy_module-2.0/setup.py` & `podlozhnyy_module-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 with open("requirements.txt", "r") as req_file:
     requirements = req_file.read().split("\n")
 
 setup(
     name="podlozhnyy_module",
-    version="2.0",
+    version="2.1",
     description="One place for the most useful methods for work",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Nikita Podlozhnyy",
     author_email="podlozhnyy.ne@phystech.edu",
     python_requires=">=3.7.0",
     url="https://github.com/NPodlozhniy/podlozhnyy-module",
```

