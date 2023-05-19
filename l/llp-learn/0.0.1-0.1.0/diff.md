# Comparing `tmp/llp_learn-0.0.1.tar.gz` & `tmp/llp_learn-0.1.0.tar.gz`

## Comparing `llp_learn-0.0.1.tar` & `llp_learn-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 llp_learn-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 llp_learn-0.0.1/test.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 llp_learn-0.0.1/docs/index.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-0.0.1/docs/reference.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/__about__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/base.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/alter/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/alter/_base.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/alter/_classes.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/dllp/__init__.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/dllp/_classes.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/em/__init__.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/em/_classes.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/mm/__init__.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/mm/_base.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/mm/_classes.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/mm/almostnolabel/alternating.mean.map.R
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/mm/almostnolabel/laplacian.mean.map.R
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/mm/almostnolabel/mean.map.R
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/model_selection/__init__.py
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/model_selection/_search.py
--rw-r--r--   0        0        0    17503 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/model_selection/_split.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/util/__init__.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 llp_learn-0.0.1/src/llp-learn/util/_util.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 llp_learn-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 llp_learn-0.0.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 llp_learn-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 llp_learn-0.0.1/README.md
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 llp_learn-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 llp_learn-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 llp_learn-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 llp_learn-0.1.0/test.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 llp_learn-0.1.0/docs/index.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-0.1.0/docs/reference.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/base.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/alter/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/alter/_base.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/alter/_classes.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/dllp/__init__.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/dllp/_classes.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/em/__init__.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/em/_classes.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/mm/__init__.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/mm/_base.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/mm/_classes.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/mm/almostnolabel/alternating.mean.map.R
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/mm/almostnolabel/mean.map.R
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/model_selection/__init__.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/model_selection/_search.py
+-rw-r--r--   0        0        0    17503 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/model_selection/_split.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/util/__init__.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 llp_learn-0.1.0/src/llp_learn/util/_util.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 llp_learn-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 llp_learn-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 llp_learn-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 llp_learn-0.1.0/README.md
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 llp_learn-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 llp_learn-0.1.0/PKG-INFO
```

### Comparing `llp_learn-0.0.1/test.py` & `llp_learn-0.1.0/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import sys
 import numpy as np
 import pandas as pd
 
 from sklearn.datasets import make_classification
 from sklearn.metrics import classification_report
 from sklearn.datasets import make_blobs, make_circles, make_moons
-sys.path.append('src')
 
-from llp.mm import MM, LMM, AMM
-from llp.dllp import DLLP
-from llp.model_selection import gridSearchCV, SplitBagShuffleSplit, SplitBagBootstrapSplit
+from llp_learn.mm import MM, LMM, AMM
+from llp_learn.dllp import DLLP
+from llp_learn.model_selection import gridSearchCV, SplitBagShuffleSplit, SplitBagBootstrapSplit
 
 random = np.random.RandomState(42)
 
 # Creating a syntetic dataset using sklearn
 X, y = make_classification(n_features=2, n_redundant=0, n_informative=2, n_clusters_per_class=1, n_samples=1000, random_state=42)
 bags = random.randint(0, 5, size=X.shape[0])
```

### Comparing `llp_learn-0.0.1/src/llp-learn/base.py` & `llp_learn-0.1.0/src/llp_learn/base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/alter/_base.py` & `llp_learn-0.1.0/src/llp_learn/alter/_base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/alter/_classes.py` & `llp_learn-0.1.0/src/llp_learn/alter/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/dllp/_classes.py` & `llp_learn-0.1.0/src/llp_learn/dllp/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/em/_classes.py` & `llp_learn-0.1.0/src/llp_learn/em/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/mm/_base.py` & `llp_learn-0.1.0/src/llp_learn/mm/_base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/mm/_classes.py` & `llp_learn-0.1.0/src/llp_learn/mm/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/mm/almostnolabel/alternating.mean.map.R` & `llp_learn-0.1.0/src/llp_learn/mm/almostnolabel/alternating.mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/mm/almostnolabel/laplacian.mean.map.R` & `llp_learn-0.1.0/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/mm/almostnolabel/mean.map.R` & `llp_learn-0.1.0/src/llp_learn/mm/almostnolabel/mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/model_selection/_search.py` & `llp_learn-0.1.0/src/llp_learn/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/model_selection/_split.py` & `llp_learn-0.1.0/src/llp_learn/model_selection/_split.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/src/llp-learn/util/_util.py` & `llp_learn-0.1.0/src/llp_learn/util/_util.py`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/.gitignore` & `llp_learn-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/LICENSE.txt` & `llp_learn-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llp_learn-0.0.1/pyproject.toml` & `llp_learn-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 [project.urls]
 Documentation = "https://github.com/unknown/llp-learn#readme"
 Issues = "https://github.com/unknown/llp-learn/issues"
 Source = "https://github.com/unknown/llp-learn"
 
 [tool.hatch.version]
-path = "src/llp-learn/__about__.py"
+path = "src/llp_learn/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
 ]
 [tool.hatch.envs.default.scripts]
```

### Comparing `llp_learn-0.0.1/PKG-INFO` & `llp_learn-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llp-learn
-Version: 0.0.1
+Version: 0.1.0
 Summary: Learning from Label Proportions (LLP) methods in Python
 Project-URL: Documentation, https://github.com/unknown/llp-learn#readme
 Project-URL: Issues, https://github.com/unknown/llp-learn/issues
 Project-URL: Source, https://github.com/unknown/llp-learn
 Author-email: Gabriel Franco <gvfranco@bu.edu>
 License-Expression: MIT
 License-File: LICENSE.txt
```

