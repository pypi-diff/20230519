# Comparing `tmp/treeordination-1.2.1.tar.gz` & `tmp/treeordination-1.2.2.tar.gz`

## Comparing `treeordination-1.2.1.tar` & `treeordination-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.2.1/environment.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    13307 2020-02-02 00:00:00.000000 treeordination-1.2.1/TreeOrdination/TreeOrdination.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 treeordination-1.2.1/TreeOrdination/__init__.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.2.1/TreeOrdination/feature_importance_treeord.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 treeordination-1.2.1/TreeOrdination/transformers_treeord.py
--rw-r--r--   0        0        0    10961 2020-02-02 00:00:00.000000 treeordination-1.2.1/docs/API.md
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.2.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.2.1/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 treeordination-1.2.1/tests/test_treeord.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.2.1/.gitignore
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.2.1/LICENSE
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 treeordination-1.2.1/README.md
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 treeordination-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 treeordination-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.2.2/environment.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.2.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 treeordination-1.2.2/TreeOrdination/TreeOrdination.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 treeordination-1.2.2/TreeOrdination/__init__.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.2.2/TreeOrdination/feature_importance_treeord.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 treeordination-1.2.2/TreeOrdination/transformers_treeord.py
+-rw-r--r--   0        0        0    10961 2020-02-02 00:00:00.000000 treeordination-1.2.2/docs/API.md
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.2.2/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.2.2/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 treeordination-1.2.2/tests/test_treeord.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 treeordination-1.2.2/README.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 treeordination-1.2.2/PKG-INFO
```

### Comparing `treeordination-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `treeordination-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `treeordination-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/.github/workflows/ci.yml` & `treeordination-1.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/.github/workflows/python-publish.yml` & `treeordination-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/TreeOrdination/TreeOrdination.py` & `treeordination-1.2.2/TreeOrdination/TreeOrdination.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
             self.features_unscaled.append(unscaled_features)
             self.transformers.append(fit_transformer)
 
             # Train model
             model = LANDMarkClassifier(
                 self.unsup_n_estim,
                 use_nnet=False,
-                max_samples_tree=self.max_samples_tree,
+                resampler = None,
                 n_jobs=self.n_jobs,
             ).fit(X_rnd, y_rnd)
             self.Rs.append(model)
 
             # Get proximity
             if self.exclude_col[0]:
                 excl_range = np.asarray(self.exclude_col[1])
```

### Comparing `treeordination-1.2.1/TreeOrdination/feature_importance_treeord.py` & `treeordination-1.2.2/TreeOrdination/feature_importance_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/TreeOrdination/transformers_treeord.py` & `treeordination-1.2.2/TreeOrdination/transformers_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/docs/API.md` & `treeordination-1.2.2/docs/API.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/docs/CONTRIBUTING.md` & `treeordination-1.2.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/tests/test_treeord.py` & `treeordination-1.2.2/tests/test_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/.gitignore` & `treeordination-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/LICENSE` & `treeordination-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treeordination-1.2.1/README.md` & `treeordination-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 ### Install
 From PyPI:
 
 ```
 pip install TreeOrdination
 ```
-This will become available after LANDMark has been updated for distribution on PyPI.
 
 From source:
 
 ```bash
 git clone https://github.com/jrudar/TreeOrdination.git
 cd TreeOrdination
 pip install .
```

### Comparing `treeordination-1.2.1/PKG-INFO` & `treeordination-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TreeOrdination
-Version: 1.2.1
+Version: 1.2.2
 Summary: Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP
 Project-URL: Homepage, https://github.com/jrudar/TreeOrdination
 Project-URL: Repository, https://github.com/jrudar/TreeOrdination.git
 Project-URL: Bug Tracker, https://github.com/jrudar/TreeOrdination/issues
 Author: G. Brian Golding, Stefan C. Kremer
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
@@ -38,15 +38,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: landmarkclassifier>=2.0.0
+Requires-Dist: landmarkclassifier>=2.0.2
 Requires-Dist: numpy==1.23.5
 Requires-Dist: scikit-bio>=0.5.8
 Requires-Dist: scikit-learn>=1.1.2
 Requires-Dist: seaborn
 Requires-Dist: shap>=0.40.0
 Requires-Dist: umap-learn>=0.5.3
 Provides-Extra: dev
@@ -69,15 +69,14 @@
 
 ### Install
 From PyPI:
 
 ```
 pip install TreeOrdination
 ```
-This will become available after LANDMark has been updated for distribution on PyPI.
 
 From source:
 
 ```bash
 git clone https://github.com/jrudar/TreeOrdination.git
 cd TreeOrdination
 pip install .
```

