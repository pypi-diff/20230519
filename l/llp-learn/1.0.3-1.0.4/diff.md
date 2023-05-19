# Comparing `tmp/llp_learn-1.0.3.tar.gz` & `tmp/llp_learn-1.0.4.tar.gz`

## Comparing `llp_learn-1.0.3.tar` & `llp_learn-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 llp_learn-1.0.3/mkdocs.yml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 llp_learn-1.0.3/docs/index.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.0.3/docs/reference.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/__about__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/base.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/alter/__init__.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/alter/_base.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/alter/_classes.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/dllp/__init__.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/dllp/_classes.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/em/__init__.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/em/_classes.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/mm/__init__.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/mm/_base.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/mm/_classes.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/mm/almostnolabel/alternating.mean.map.R
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/mm/almostnolabel/mean.map.R
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/model_selection/__init__.py
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/model_selection/_search.py
--rw-r--r--   0        0        0    17509 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/model_selection/_split.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/util/__init__.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 llp_learn-1.0.3/src/llp_learn/util/_util.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 llp_learn-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 llp_learn-1.0.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 llp_learn-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 llp_learn-1.0.3/README.md
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 llp_learn-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 llp_learn-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 llp_learn-1.0.4/mkdocs.yml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 llp_learn-1.0.4/docs/index.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 llp_learn-1.0.4/docs/reference.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/base.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/alter/__init__.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/alter/_base.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/alter/_classes.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/dllp/__init__.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/dllp/_classes.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/em/__init__.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/em/_classes.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/__init__.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/_base.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/_classes.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/alternating.mean.map.R
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/mean.map.R
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/model_selection/__init__.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/model_selection/_search.py
+-rw-r--r--   0        0        0    17509 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/model_selection/_split.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/util/__init__.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 llp_learn-1.0.4/src/llp_learn/util/_util.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 llp_learn-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 llp_learn-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 llp_learn-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 llp_learn-1.0.4/README.md
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 llp_learn-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 llp_learn-1.0.4/PKG-INFO
```

### Comparing `llp_learn-1.0.3/src/llp_learn/base.py` & `llp_learn-1.0.4/src/llp_learn/base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/alter/_base.py` & `llp_learn-1.0.4/src/llp_learn/alter/_base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/alter/_classes.py` & `llp_learn-1.0.4/src/llp_learn/alter/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/dllp/_classes.py` & `llp_learn-1.0.4/src/llp_learn/dllp/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/em/_classes.py` & `llp_learn-1.0.4/src/llp_learn/em/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/mm/_base.py` & `llp_learn-1.0.4/src/llp_learn/mm/_base.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/mm/_classes.py` & `llp_learn-1.0.4/src/llp_learn/mm/_classes.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/mm/almostnolabel/alternating.mean.map.R` & `llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/alternating.mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R` & `llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/laplacian.mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/mm/almostnolabel/mean.map.R` & `llp_learn-1.0.4/src/llp_learn/mm/almostnolabel/mean.map.R`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/model_selection/_search.py` & `llp_learn-1.0.4/src/llp_learn/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/model_selection/_split.py` & `llp_learn-1.0.4/src/llp_learn/model_selection/_split.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/src/llp_learn/util/_util.py` & `llp_learn-1.0.4/src/llp_learn/util/_util.py`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/.gitignore` & `llp_learn-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/LICENSE.txt` & `llp_learn-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/README.md` & `llp_learn-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `llp_learn-1.0.3/pyproject.toml` & `llp_learn-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
   "pytest-cov",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=llp_learn --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
+python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "llp_learn/__about__.py",
 ]
```

### Comparing `llp_learn-1.0.3/PKG-INFO` & `llp_learn-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llp-learn
-Version: 1.0.3
+Version: 1.0.4
 Summary: Learning from Label Proportions (LLP) methods in Python
 Project-URL: Documentation, https://github.com/gaabrielfranco/llp-learn#readme
 Project-URL: Issues, https://github.com/gaabrielfranco/llp-learn/issues
 Project-URL: Source, https://github.com/gaabrielfranco/llp-learn
 Author-email: Gabriel Franco <gvfranco@bu.edu>
 License-Expression: MIT
 License-File: LICENSE.txt
```

