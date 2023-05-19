# Comparing `tmp/llp_learn-1.0.4.tar.gz` & `tmp/llp_learn-1.0.5.tar.gz`

## Comparing `llp_learn-1.0.4.tar` & `llp_learn-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 llp_learn-1.0.4/mkdocs.yml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 llp_learn-1.0.4/docs/index.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.0.4/docs/reference.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/__about__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/base.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/alter/__init__.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/alter/_base.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/alter/_classes.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/dllp/__init__.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/dllp/_classes.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/em/__init__.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/em/_classes.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/__init__.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/_base.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/_classes.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/alternating.mean.map.R
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/mean.map.R
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/model_selection/__init__.py
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/model_selection/_search.py
--rw-r--r--   0        0        0    17509 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/model_selection/_split.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/util/__init__.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/util/_util.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 llp_learn-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 llp_learn-1.0.4/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 llp_learn-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 llp_learn-1.0.4/README.md
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 llp_learn-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 llp_learn-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 llp_learn-1.0.5/mkdocs.yml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 llp_learn-1.0.5/docs/index.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.0.5/docs/reference.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/base.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/alter/__init__.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/alter/_base.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/alter/_classes.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/dllp/__init__.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/dllp/_classes.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/em/__init__.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/em/_classes.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/mm/__init__.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/mm/_base.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/mm/_classes.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/mm/almostnolabel/alternating.mean.map.R
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/mm/almostnolabel/mean.map.R
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/model_selection/__init__.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/model_selection/_search.py
+-rw-r--r--   0        0        0    17509 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/model_selection/_split.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/util/__init__.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 llp_learn-1.0.5/src/llp_learn/util/_util.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 llp_learn-1.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 llp_learn-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 llp_learn-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 llp_learn-1.0.5/README.md
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 llp_learn-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 llp_learn-1.0.5/PKG-INFO
```

### Comparing `llp_learn-1.0.4/src/llp_learn/base.py` & `llp_learn-1.0.5/src/llp_learn/base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/alter/_base.py` & `llp_learn-1.0.5/src/llp_learn/alter/_base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/alter/_classes.py` & `llp_learn-1.0.5/src/llp_learn/alter/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/dllp/_classes.py` & `llp_learn-1.0.5/src/llp_learn/dllp/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/em/_classes.py` & `llp_learn-1.0.5/src/llp_learn/em/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/mm/_base.py` & `llp_learn-1.0.5/src/llp_learn/mm/_base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/mm/_classes.py` & `llp_learn-1.0.5/src/llp_learn/mm/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/alternating.mean.map.R` & `llp_learn-1.0.5/src/llp_learn/mm/almostnolabel/alternating.mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R` & `llp_learn-1.0.5/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/mean.map.R` & `llp_learn-1.0.5/src/llp_learn/mm/almostnolabel/mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/model_selection/_search.py` & `llp_learn-1.0.5/src/llp_learn/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/model_selection/_split.py` & `llp_learn-1.0.5/src/llp_learn/model_selection/_split.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/src/llp_learn/util/_util.py` & `llp_learn-1.0.5/src/llp_learn/util/_util.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/.gitignore` & `llp_learn-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/LICENSE.txt` & `llp_learn-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/README.md` & `llp_learn-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.4/pyproject.toml` & `llp_learn-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llp-learn"
 description = "Learning from Label Proportions (LLP) methods in Python"
 readme = "README.md"
-requires-python = ">=3.8, <=3.11"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Gabriel Franco", email = "gvfranco@bu.edu" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `llp_learn-1.0.4/PKG-INFO` & `llp_learn-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llp-learn
-Version: 1.0.4
+Version: 1.0.5
 Summary: Learning from Label Proportions (LLP) methods in Python
 Project-URL: Documentation, https://github.com/gaabrielfranco/llp-learn#readme
 Project-URL: Issues, https://github.com/gaabrielfranco/llp-learn/issues
 Project-URL: Source, https://github.com/gaabrielfranco/llp-learn
 Author-email: Gabriel Franco <gvfranco@bu.edu>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: <=3.11,>=3.8
+Requires-Python: >=3.8
 Requires-Dist: joblib~=1.2.0
 Requires-Dist: matplotlib~=3.7.1
 Requires-Dist: numpy~=1.24.2
 Requires-Dist: pandas~=1.5.3
 Requires-Dist: rpy2~=3.5.10
 Requires-Dist: scikit-learn~=1.2.2
 Requires-Dist: scipy~=1.10.1
```

