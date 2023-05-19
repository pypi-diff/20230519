# Comparing `tmp/dropkick-1.2.6.tar.gz` & `tmp/dropkick-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dropkick-1.2.6.tar", last modified: Fri Jul 23 19:22:03 2021, max compression
+gzip compressed data, was "dropkick-1.2.7.tar", last modified: Fri May 19 15:52:02 2023, max compression
```

## Comparing `dropkick-1.2.6.tar` & `dropkick-1.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2021-07-23 19:22:03.741404 dropkick-1.2.6/
--rw-r--r--   0 cody       (501) staff       (20)     1070 2021-07-23 19:18:42.000000 dropkick-1.2.6/LICENSE
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2021-07-23 19:22:03.736299 dropkick-1.2.6/LICENSES/
--rw-r--r--   0 cody       (501) staff       (20)    18046 2021-07-23 19:18:42.000000 dropkick-1.2.6/LICENSES/GLMNET_LICENSE
--rw-r--r--   0 cody       (501) staff       (20)    18396 2021-07-23 19:18:42.000000 dropkick-1.2.6/LICENSES/PYTHON_GLMNET_LICENSE
--rw-r--r--   0 cody       (501) staff       (20)     1558 2021-07-23 19:18:42.000000 dropkick-1.2.6/LICENSES/SCIKIT_LEARN_LICENSE
--rw-r--r--   0 cody       (501) staff       (20)      163 2021-07-23 19:18:42.000000 dropkick-1.2.6/MANIFEST.in
--rw-r--r--   0 cody       (501) staff       (20)     3127 2021-07-23 19:22:03.741536 dropkick-1.2.6/PKG-INFO
--rw-r--r--   0 cody       (501) staff       (20)     2030 2021-07-23 19:18:42.000000 dropkick-1.2.6/README.rst
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2021-07-23 19:22:03.742345 dropkick-1.2.6/dropkick/
--rw-r--r--   0 cody       (501) staff       (20)      500 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/__init__.py
--rw-r--r--   0 cody       (501) staff       (20)     8351 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/__main__.py
--rw-r--r--   0 cody       (501) staff       (20)     5448 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/_glmnet.pyf
--rw-r--r--   0 cody       (501) staff       (20)      498 2021-07-23 19:22:03.742440 dropkick-1.2.6/dropkick/_version.py
--rw-r--r--   0 cody       (501) staff       (20)    35910 2021-07-23 19:17:34.000000 dropkick-1.2.6/dropkick/api.py
--rw-r--r--   0 cody       (501) staff       (20)     2323 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/errors.py
--rw-r--r--   0 cody       (501) staff       (20)    22911 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/logistic.py
--rw-r--r--   0 cody       (501) staff       (20)     7803 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/qc.py
--rw-r--r--   0 cody       (501) staff       (20)    12679 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/scorer.py
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2021-07-23 19:22:03.734006 dropkick-1.2.6/dropkick/src/
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2021-07-23 19:22:03.740620 dropkick-1.2.6/dropkick/src/glmnet/
--rw-r--r--   0 cody       (501) staff       (20)   561094 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/src/glmnet/glmnet5.f90
--rw-r--r--   0 cody       (501) staff       (20)     8003 2021-07-23 19:18:42.000000 dropkick-1.2.6/dropkick/util.py
-drwxr-xr-x   0 cody       (501) staff       (20)        0 2021-07-23 19:22:03.740320 dropkick-1.2.6/dropkick.egg-info/
--rw-r--r--   0 cody       (501) staff       (20)     3127 2021-07-23 19:22:03.000000 dropkick-1.2.6/dropkick.egg-info/PKG-INFO
--rw-r--r--   0 cody       (501) staff       (20)      582 2021-07-23 19:22:03.000000 dropkick-1.2.6/dropkick.egg-info/SOURCES.txt
--rw-r--r--   0 cody       (501) staff       (20)        1 2021-07-23 19:22:03.000000 dropkick-1.2.6/dropkick.egg-info/dependency_links.txt
--rw-r--r--   0 cody       (501) staff       (20)       53 2021-07-23 19:22:03.000000 dropkick-1.2.6/dropkick.egg-info/entry_points.txt
--rw-r--r--   0 cody       (501) staff       (20)       93 2021-07-23 19:22:03.000000 dropkick-1.2.6/dropkick.egg-info/requires.txt
--rw-r--r--   0 cody       (501) staff       (20)       17 2021-07-23 19:22:03.000000 dropkick-1.2.6/dropkick.egg-info/top_level.txt
--rw-r--r--   0 cody       (501) staff       (20)       93 2021-07-23 19:18:42.000000 dropkick-1.2.6/requirements.txt
--rw-r--r--   0 cody       (501) staff       (20)      205 2021-07-23 19:22:03.741987 dropkick-1.2.6/setup.cfg
--rw-r--r--   0 cody       (501) staff       (20)     2642 2021-07-23 19:18:42.000000 dropkick-1.2.6/setup.py
--rw-r--r--   0 cody       (501) staff       (20)    68611 2021-07-23 19:18:42.000000 dropkick-1.2.6/versioneer.py
+drwxrwxr-x   0 cody      (1002) cody      (1002)        0 2023-05-19 15:52:02.134774 dropkick-1.2.7/
+-rw-rw-r--   0 cody      (1002) cody      (1002)     1070 2023-05-19 15:31:50.000000 dropkick-1.2.7/LICENSE
+drwxrwxr-x   0 cody      (1002) cody      (1002)        0 2023-05-19 15:52:02.134774 dropkick-1.2.7/LICENSES/
+-rw-rw-r--   0 cody      (1002) cody      (1002)    18046 2023-05-19 15:31:50.000000 dropkick-1.2.7/LICENSES/GLMNET_LICENSE
+-rw-rw-r--   0 cody      (1002) cody      (1002)    18396 2023-05-19 15:31:50.000000 dropkick-1.2.7/LICENSES/PYTHON_GLMNET_LICENSE
+-rw-rw-r--   0 cody      (1002) cody      (1002)     1558 2023-05-19 15:31:50.000000 dropkick-1.2.7/LICENSES/SCIKIT_LEARN_LICENSE
+-rw-rw-r--   0 cody      (1002) cody      (1002)      163 2023-05-19 15:31:50.000000 dropkick-1.2.7/MANIFEST.in
+-rw-rw-r--   0 cody      (1002) cody      (1002)     3329 2023-05-19 15:52:02.134774 dropkick-1.2.7/PKG-INFO
+-rw-rw-r--   0 cody      (1002) cody      (1002)     2216 2023-05-19 15:31:50.000000 dropkick-1.2.7/README.rst
+drwxrwxr-x   0 cody      (1002) cody      (1002)        0 2023-05-19 15:52:02.134774 dropkick-1.2.7/dropkick/
+-rw-rw-r--   0 cody      (1002) cody      (1002)      500 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/__init__.py
+-rw-rw-r--   0 cody      (1002) cody      (1002)     8351 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/__main__.py
+-rw-rw-r--   0 cody      (1002) cody      (1002)     5448 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/_glmnet.pyf
+-rw-rw-r--   0 cody      (1002) cody      (1002)      498 2023-05-19 15:52:02.134774 dropkick-1.2.7/dropkick/_version.py
+-rw-rw-r--   0 cody      (1002) cody      (1002)    36076 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/api.py
+-rw-rw-r--   0 cody      (1002) cody      (1002)     2323 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/errors.py
+-rw-rw-r--   0 cody      (1002) cody      (1002)    22911 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/logistic.py
+-rw-rw-r--   0 cody      (1002) cody      (1002)     7803 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/qc.py
+-rw-rw-r--   0 cody      (1002) cody      (1002)    12679 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/scorer.py
+drwxrwxr-x   0 cody      (1002) cody      (1002)        0 2023-05-19 15:52:02.130774 dropkick-1.2.7/dropkick/src/
+drwxrwxr-x   0 cody      (1002) cody      (1002)        0 2023-05-19 15:52:02.134774 dropkick-1.2.7/dropkick/src/glmnet/
+-rw-rw-r--   0 cody      (1002) cody      (1002)   561094 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/src/glmnet/glmnet5.f90
+-rw-rw-r--   0 cody      (1002) cody      (1002)     8003 2023-05-19 15:31:51.000000 dropkick-1.2.7/dropkick/util.py
+drwxrwxr-x   0 cody      (1002) cody      (1002)        0 2023-05-19 15:52:02.134774 dropkick-1.2.7/dropkick.egg-info/
+-rw-rw-r--   0 cody      (1002) cody      (1002)     3329 2023-05-19 15:52:02.000000 dropkick-1.2.7/dropkick.egg-info/PKG-INFO
+-rw-rw-r--   0 cody      (1002) cody      (1002)      582 2023-05-19 15:52:02.000000 dropkick-1.2.7/dropkick.egg-info/SOURCES.txt
+-rw-rw-r--   0 cody      (1002) cody      (1002)        1 2023-05-19 15:52:02.000000 dropkick-1.2.7/dropkick.egg-info/dependency_links.txt
+-rw-rw-r--   0 cody      (1002) cody      (1002)       53 2023-05-19 15:52:02.000000 dropkick-1.2.7/dropkick.egg-info/entry_points.txt
+-rw-rw-r--   0 cody      (1002) cody      (1002)       93 2023-05-19 15:52:02.000000 dropkick-1.2.7/dropkick.egg-info/requires.txt
+-rw-rw-r--   0 cody      (1002) cody      (1002)       17 2023-05-19 15:52:02.000000 dropkick-1.2.7/dropkick.egg-info/top_level.txt
+-rw-rw-r--   0 cody      (1002) cody      (1002)       93 2023-05-19 15:31:51.000000 dropkick-1.2.7/requirements.txt
+-rw-rw-r--   0 cody      (1002) cody      (1002)      205 2023-05-19 15:52:02.134774 dropkick-1.2.7/setup.cfg
+-rw-rw-r--   0 cody      (1002) cody      (1002)     2642 2023-05-19 15:31:51.000000 dropkick-1.2.7/setup.py
+-rw-rw-r--   0 cody      (1002) cody      (1002)    68611 2023-05-19 15:31:51.000000 dropkick-1.2.7/versioneer.py
```

### Comparing `dropkick-1.2.6/LICENSE` & `dropkick-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/LICENSES/GLMNET_LICENSE` & `dropkick-1.2.7/LICENSES/GLMNET_LICENSE`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/LICENSES/PYTHON_GLMNET_LICENSE` & `dropkick-1.2.7/LICENSES/PYTHON_GLMNET_LICENSE`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/LICENSES/SCIKIT_LEARN_LICENSE` & `dropkick-1.2.7/LICENSES/SCIKIT_LEARN_LICENSE`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/PKG-INFO` & `dropkick-1.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 1.2
 Name: dropkick
-Version: 1.2.6
+Version: 1.2.7
 Summary: Automated scRNA-seq filtering
 Home-page: https://github.com/KenLauLab/dropkick
 Author: Cody Heiser
 Author-email: codyheiser49@gmail.com
 License: UNKNOWN
 Description: |Dropkick Logo|
         
+        |Latest Version|
+        
         Automated cell filtering for single-cell RNA sequencing data.
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
-        |Latest Version|
+        See our `Genome Research paper <https://doi.org/10.1101/gr.271908.120>`_ for details on ``dropkick``'s guiding principles and validation.
         
         ----
         
         ``dropkick`` works primarily with |scanpy|_'s ``AnnData`` objects, and accepts input files in ``.h5ad`` or flat (``.csv``, ``.tsv``) format. It also writes outputs to ``.h5ad`` files when called from the terminal.
         
-        Installation via ``pip`` or from source requires a Fortran compiler (``brew install gcc`` for Mac users).
+        Installation via ``pip`` or from source requires a Fortran compiler (``brew install gcc`` for Mac users, ``sudo apt install gfortran`` for Linux users).
         
         Install from PyPI:
         ^^^^^^^^^^^^^^^^^^
         .. code:: bash
         
            pip install dropkick
```

### Comparing `dropkick-1.2.6/README.rst` & `dropkick-1.2.7/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 |Dropkick Logo|
 
+|Latest Version|
+
 Automated cell filtering for single-cell RNA sequencing data.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-|Latest Version|
+See our `Genome Research paper <https://doi.org/10.1101/gr.271908.120>`_ for details on ``dropkick``'s guiding principles and validation.
 
 ----
 
 ``dropkick`` works primarily with |scanpy|_'s ``AnnData`` objects, and accepts input files in ``.h5ad`` or flat (``.csv``, ``.tsv``) format. It also writes outputs to ``.h5ad`` files when called from the terminal.
 
-Installation via ``pip`` or from source requires a Fortran compiler (``brew install gcc`` for Mac users).
+Installation via ``pip`` or from source requires a Fortran compiler (``brew install gcc`` for Mac users, ``sudo apt install gfortran`` for Linux users).
 
 Install from PyPI:
 ^^^^^^^^^^^^^^^^^^
 .. code:: bash
 
    pip install dropkick
```

### Comparing `dropkick-1.2.6/dropkick/__main__.py` & `dropkick-1.2.7/dropkick/__main__.py`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/dropkick/_glmnet.pyf` & `dropkick-1.2.7/dropkick/_glmnet.pyf`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/dropkick/api.py` & `dropkick-1.2.7/dropkick/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,27 +48,27 @@
     filter : bool, optional (default=True)
         remove cells with less than min_genes detected and genes with zero total counts
     min_genes : int, optional (default=50)
         threshold for minimum genes detected. ignored if `filter`==False.
     calc_metrics : bool, optional (default=True)
         if False, do not calculate metrics in `.obs`/`.var`
     mito_names : str, optional (default="^mt-|^MT-")
-        substring encompassing mitochondrial gene names for calculation of mito 
+        substring encompassing mitochondrial gene names for calculation of mito
         expression. ignored if `calc_metrics`==False.
     n_ambient : int, optional (default=10)
-        number of ambient genes to call (top genes by cells). ignored if 
+        number of ambient genes to call (top genes by cells). ignored if
         `calc_metrics`==False.
     target_sum : int, optional (default=None)
-        total sum of counts for each cell prior to arcsinh or log1p transformations. 
+        total sum of counts for each cell prior to arcsinh or log1p transformations.
         if None, use median counts.
     n_hvgs : int, optional (default=2000)
-        number of HVGs to calculate using Seurat method. if None, do not calculate 
+        number of HVGs to calculate using Seurat method. if None, do not calculate
         HVGs.
     X_final : str, optional (default="raw_counts")
-        which normalization layer should be left in `.X` slot? ("raw_counts", 
+        which normalization layer should be left in `.X` slot? ("raw_counts",
         "arcsinh_norm", "log1p_norm")
     verbose : bool, optional (default=True)
         print updates to the console
 
     Returns
     -------
 
@@ -191,26 +191,26 @@
     Parameters
     ----------
 
     adata : anndata.AnnData
         object containing unfiltered scRNA-seq data
     obs_cols : list of str, optional (default="arcsinh_n_genes_by_counts")
         name of column(s) to threshold from `adata.obs`
-    methods : list of str {"otsu","multiotsu","li","mean"}, optional 
+    methods : list of str {"otsu","multiotsu","li","mean"}, optional
     (default="multiotsu")
         automated thresholding method(s) corresponding to each element in `obs_cols`
     directions : list of str {"above","below"}, optional (default="above")
-        which direction to keep during training (dropkick label = 1) corresponding 
+        which direction to keep during training (dropkick label = 1) corresponding
         to each element in `obs_cols`
 
     Returns
     -------
 
     thresholds : dict
-        keys are `obs_cols` and values are dictionaries with "thresh" : threshold 
+        keys are `obs_cols` and values are dictionaries with "thresh" : threshold
         results & "direction" : direction to keep for training
     """
     # convert to lists before looping
     if isinstance(obs_cols, str):
         obs_cols = [obs_cols]
     if isinstance(methods, str):
         methods = [methods]
@@ -238,38 +238,38 @@
         thresholds[obs_cols[i]]["direction"] = directions[i]
 
     return thresholds
 
 
 def plot_thresh_obs(adata, thresholds, bins=40, axes=None, save_to=None, verbose=True):
     """
-    Plots automated thresholding on metrics in `adata.obs` as output by 
+    Plots automated thresholding on metrics in `adata.obs` as output by
     `auto_thresh_obs()`
 
     Parameters
     ----------
 
     adata : anndata.AnnData
         object containing unfiltered scRNA-seq data
     thresholds : dict
         output of `auto_thresh_obs()` function
     bins : int, optional (default=40)
         number of bins for histogram
     axes : matplotlib.axes.Axes, optional (default=None)
-        single ax or list of axes objects corresponding to number of thresholds to 
+        single ax or list of axes objects corresponding to number of thresholds to
         plot. ignored if `save_to` is not None.
     save_to : str, optional (default=None)
         path to `.png` file for saving figure; returns figure by default
     verbose : bool, optional (default=True)
         print updates to console
 
     Returns
     -------
 
-    plot of distributions of `obs_cols` in thresholds dictionary with corresponding 
+    plot of distributions of `obs_cols` in thresholds dictionary with corresponding
     thresholds
     """
     if save_to or not axes:
         fig, axes = plt.subplots(
             ncols=len(thresholds),
             nrows=1,
             figsize=(len(thresholds) * 4, 4),
@@ -314,15 +314,15 @@
     thresholds,
     obs_cols=["arcsinh_n_genes_by_counts"],
     inclusive=True,
     name="thresh_filter",
     verbose=True,
 ):
     """
-    Filters cells by thresholding on metrics in `adata.obs` as output by 
+    Filters cells by thresholding on metrics in `adata.obs` as output by
     `auto_thresh_obs()`
 
     Parameters
     ----------
 
     adata : anndata.AnnData
         object containing unfiltered scRNA-seq data
@@ -480,31 +480,31 @@
 
     Parameters
     ----------
 
     adata : anndata.AnnData
         object containing unfiltered, raw scRNA-seq counts in `.X` layer
     min_genes : int, optional (default=50)
-        threshold for minimum genes detected. ignores all cells with less than 
+        threshold for minimum genes detected. ignores all cells with less than
         min_genes (dropkick label = 0).
     mito_names : str, optional (default="^mt-|^MT-")
-        substring encompassing mitochondrial gene names for calculation of mito 
+        substring encompassing mitochondrial gene names for calculation of mito
         expression
     n_ambient : int, optional (default=10)
         number of ambient genes to call. top genes by cells.
     n_hvgs : int or None, optional (default=2000)
-        number of HVGs to calculate using Seurat method. if None, do not calculate 
+        number of HVGs to calculate using Seurat method. if None, do not calculate
         HVGs
     metrics : list of str, optional (default="arcsinh_n_genes_by_counts")
         name of column(s) to threshold from `adata.obs`
-    thresh_methods : list of str {"otsu","multiotsu","li","mean"}, optional 
+    thresh_methods : list of str {"otsu","multiotsu","li","mean"}, optional
     (default="multiotsu")
         automated thresholding method(s) corresponding to each element in `metrics`
     directions : list of str {"above","below"}, optional (default="above")
-        which direction to keep during training (dropkick label = 1) corresponding 
+        which direction to keep during training (dropkick label = 1) corresponding
         to each element in `metrics`
     alphas : list of float, optional (default=0.1)
         alpha value(s) to test using glmnet with n-fold cross validation
     max_iter : int, optional (default=2000)
         number of iterations for glmnet optimization
     n_jobs : int, optional (default=2)
         number of threads for cross validation by glmnet
@@ -515,15 +515,15 @@
 
     Returns
     -------
 
     rc : LogisticRegression
         trained logistic regression classifier
 
-    updates `adata` inplace to include "train", "dropkick_score", and 
+    updates `adata` inplace to include "train", "dropkick_score", and
     "dropkick_label" columns in `.obs`
     """
     # 0) preprocess counts and calculate required QC metrics
     a = adata.copy()  # make copy of anndata before manipulating
     a = recipe_dropkick(
         a,
         filter=True,
@@ -615,29 +615,37 @@
         print("Chosen lambda value:\n\t{}".format(rc_.lambda_best_))
         lambda_, alpha_ = rc_.lambda_best_, alphas[0]
 
     # 4) use model to assign scores and labels to original adata
     print("Assigning scores and labels")
     if "dropkick_score" in adata.obs.columns:
         print("Warning: Overwriting existing dropkick scores in .obs")
-        adata.obs.drop(columns=["dropkick_score"], inplace=True)
+
+    adata.obs["dropkick_score"] = np.nan  # initialize dropkick_score as NaNs
     adata.obs.loc[a.obs_names, "dropkick_score"] = rc_.predict_proba(X)[:, 1]
     adata.obs.dropkick_score.fillna(0, inplace=True)  # fill ignored cells with zeros
+
     if "dropkick_label" in adata.obs.columns:
         print("Warning: Overwriting existing dropkick labels in .obs")
-        adata.obs.drop(columns=["dropkick_label"], inplace=True)
+
+    adata.obs["dropkick_label"] = np.nan  # initialize dropkick_label as NaNs
     adata.obs.loc[a.obs_names, "dropkick_label"] = rc_.predict(X)
     adata.obs.dropkick_label.fillna(0, inplace=True)  # fill ignored cells with zeros
     adata.obs.dropkick_label = (
         adata.obs.dropkick_label.astype(bool).astype(str).astype("category")
     )  # convert to categorical strings
+
+    # add heuristics to .obs
     for metric in metrics:
+        adata.obs[metric] = np.nan  # initialize as NaNs
         adata.obs.loc[a.obs_names, metric] = a.obs[metric]
         adata.obs[metric].fillna(0, inplace=True)  # fill ignored cells with zeros
+
     # add dropkick coefficients to genes used in model (hvgs from `a`)
+    adata.var["dropkick_coef"] = np.nan  # initialize gene coefs as NaNs
     adata.var.loc[
         a.var_names[a.var.highly_variable], "dropkick_coef"
     ] = rc_.coef_.squeeze()
 
     # 5) save model hyperparameters in .uns
     adata.uns["dropkick_thresholds"] = adata_thresh
     adata.uns["dropkick_args"] = {
@@ -658,15 +666,15 @@
 
     print("Done!\n")
     return rc_
 
 
 def coef_inventory(adata, n=10):
     """
-    Returns highest and lowest coefficient values from logistic regression model, 
+    Returns highest and lowest coefficient values from logistic regression model,
     along with sparsity
 
     Parameters
     ----------
 
     adata : anndata.AnnData
         object generated from `dropkick`
@@ -690,15 +698,15 @@
             n_zero, sparsity
         )
     )
 
 
 def coef_plot(adata, save_to=None, verbose=True):
     """
-    Plots dropkick coefficient values and cross validation (CV) scores for tested 
+    Plots dropkick coefficient values and cross validation (CV) scores for tested
     values of lambda (`lambda_path`)
 
     Parameters
     ----------
 
     adata : anndata.AnnData
         object generated from `dropkick`
@@ -832,36 +840,36 @@
 def score_plot(
     adata,
     metrics=["arcsinh_n_genes_by_counts", "pct_counts_ambient"],
     save_to=None,
     verbose=True,
 ):
     """
-    Plots scatter of barcodes across two metrics, with points colored by 
-    `dropkick_score`. Shows automated thresholding on metrics in `adata.obs` as output 
+    Plots scatter of barcodes across two metrics, with points colored by
+    `dropkick_score`. Shows automated thresholding on metrics in `adata.obs` as output
     by `auto_thresh_obs()`
 
     Parameters
     ----------
 
     adata : anndata.AnnData
         object generated from `dropkick`
-    metrics : list of str, optional 
+    metrics : list of str, optional
     (default=["arcsinh_n_genes_by_counts","pct_counts_ambient"])
         names of metrics to plot scatter and histograms for
     save_to : str, optional (default=None)
         path to `.png` file for saving figure; returns figure if None
     verbose : bool, optional (default=True)
         print updates to console
 
     Returns
     -------
 
     g : seaborn.jointgrid
-        joint plot of metric distributions colored by `dropkick_score` and containing 
+        joint plot of metric distributions colored by `dropkick_score` and containing
         corresponding training thresholds
 
     if `save_to` is not None, write to file instead of returning `g` object.
     """
     # initialize joint plot object
     g = sns.jointplot(
         x=adata.obs[metrics[0]],
```

### Comparing `dropkick-1.2.6/dropkick/errors.py` & `dropkick-1.2.7/dropkick/errors.py`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/dropkick/logistic.py` & `dropkick-1.2.7/dropkick/logistic.py`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/dropkick/qc.py` & `dropkick-1.2.7/dropkick/qc.py`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/dropkick/scorer.py` & `dropkick-1.2.7/dropkick/scorer.py`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/dropkick/src/glmnet/glmnet5.f90` & `dropkick-1.2.7/dropkick/src/glmnet/glmnet5.f90`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/dropkick/util.py` & `dropkick-1.2.7/dropkick/util.py`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/dropkick.egg-info/PKG-INFO` & `dropkick-1.2.7/dropkick.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 1.2
 Name: dropkick
-Version: 1.2.6
+Version: 1.2.7
 Summary: Automated scRNA-seq filtering
 Home-page: https://github.com/KenLauLab/dropkick
 Author: Cody Heiser
 Author-email: codyheiser49@gmail.com
 License: UNKNOWN
 Description: |Dropkick Logo|
         
+        |Latest Version|
+        
         Automated cell filtering for single-cell RNA sequencing data.
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
-        |Latest Version|
+        See our `Genome Research paper <https://doi.org/10.1101/gr.271908.120>`_ for details on ``dropkick``'s guiding principles and validation.
         
         ----
         
         ``dropkick`` works primarily with |scanpy|_'s ``AnnData`` objects, and accepts input files in ``.h5ad`` or flat (``.csv``, ``.tsv``) format. It also writes outputs to ``.h5ad`` files when called from the terminal.
         
-        Installation via ``pip`` or from source requires a Fortran compiler (``brew install gcc`` for Mac users).
+        Installation via ``pip`` or from source requires a Fortran compiler (``brew install gcc`` for Mac users, ``sudo apt install gfortran`` for Linux users).
         
         Install from PyPI:
         ^^^^^^^^^^^^^^^^^^
         .. code:: bash
         
            pip install dropkick
```

### Comparing `dropkick-1.2.6/dropkick.egg-info/SOURCES.txt` & `dropkick-1.2.7/dropkick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/setup.py` & `dropkick-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `dropkick-1.2.6/versioneer.py` & `dropkick-1.2.7/versioneer.py`

 * *Files identical despite different names*

