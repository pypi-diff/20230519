# Comparing `tmp/EmaCalc-0.9.6.tar.gz` & `tmp/EmaCalc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmaCalc-0.9.6.tar", last modified: Mon Apr 17 04:04:46 2023, max compression
+gzip compressed data, was "EmaCalc-1.0.0.tar", last modified: Fri May 19 05:51:02 2023, max compression
```

## Comparing `EmaCalc-0.9.6.tar` & `EmaCalc-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 04:04:46.549601 EmaCalc-0.9.6/
--rw-r--r--   0 arne       (503) staff       (20)     1083 2021-11-24 10:59:26.000000 EmaCalc-0.9.6/LICENSE.txt
--rw-r--r--   0 arne       (503) staff       (20)    10307 2023-04-17 04:04:46.549657 EmaCalc-0.9.6/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)     9590 2023-03-19 07:22:45.000000 EmaCalc-0.9.6/README.md
--rw-r--r--   0 arne       (503) staff       (20)       92 2023-03-19 04:45:17.000000 EmaCalc-0.9.6/pyproject.toml
--rw-r--r--   0 arne       (503) staff       (20)      960 2023-04-17 04:04:46.549936 EmaCalc-0.9.6/setup.cfg
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 04:04:46.542883 EmaCalc-0.9.6/src/
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 04:04:46.548680 EmaCalc-0.9.6/src/EmaCalc/
--rw-r--r--   0 arne       (503) staff       (20)     5369 2023-04-17 00:54:07.000000 EmaCalc-0.9.6/src/EmaCalc/__init__.py
--rw-r--r--   0 arne       (503) staff       (20)    16290 2022-08-23 14:54:59.000000 EmaCalc-0.9.6/src/EmaCalc/dirichlet.py
--rw-r--r--   0 arne       (503) staff       (20)    50462 2023-04-13 14:27:33.000000 EmaCalc-0.9.6/src/EmaCalc/ema_base.py
--rw-r--r--   0 arne       (503) staff       (20)    44608 2023-04-11 04:01:26.000000 EmaCalc-0.9.6/src/EmaCalc/ema_data.py
--rw-r--r--   0 arne       (503) staff       (20)    38185 2023-04-17 04:02:27.000000 EmaCalc-0.9.6/src/EmaCalc/ema_display.py
--rw-r--r--   0 arne       (503) staff       (20)    21804 2023-04-17 03:41:17.000000 EmaCalc-0.9.6/src/EmaCalc/ema_display_format.py
--rw-r--r--   0 arne       (503) staff       (20)     9191 2022-08-21 09:20:55.000000 EmaCalc-0.9.6/src/EmaCalc/ema_file.py
--rw-r--r--   0 arne       (503) staff       (20)    28796 2023-03-08 03:30:42.000000 EmaCalc-0.9.6/src/EmaCalc/ema_group.py
--rw-r--r--   0 arne       (503) staff       (20)     8019 2022-08-20 18:28:46.000000 EmaCalc-0.9.6/src/EmaCalc/ema_latent.py
--rw-r--r--   0 arne       (503) staff       (20)     1272 2022-08-20 11:02:31.000000 EmaCalc-0.9.6/src/EmaCalc/ema_logging.py
--rw-r--r--   0 arne       (503) staff       (20)    14502 2022-11-29 02:42:44.000000 EmaCalc-0.9.6/src/EmaCalc/ema_model.py
--rw-r--r--   0 arne       (503) staff       (20)    14769 2023-04-14 02:40:04.000000 EmaCalc-0.9.6/src/EmaCalc/ema_nap.py
--rw-rw-rw-   0 arne       (503) staff       (20)    18893 2023-03-30 01:50:53.000000 EmaCalc-0.9.6/src/EmaCalc/ema_respondent.py
--rw-r--r--   0 arne       (503) staff       (20)    23228 2022-11-23 02:02:29.000000 EmaCalc-0.9.6/src/EmaCalc/ema_simulation.py
--rw-r--r--   0 arne       (503) staff       (20)    20379 2023-02-27 09:08:48.000000 EmaCalc-0.9.6/src/EmaCalc/ema_thresholds.py
--rw-r--r--   0 arne       (503) staff       (20)    20031 2022-08-18 08:38:01.000000 EmaCalc-0.9.6/src/EmaCalc/gauss_gamma.py
--rw-r--r--   0 arne       (503) staff       (20)    15413 2023-04-17 03:41:17.000000 EmaCalc-0.9.6/src/EmaCalc/run_ema.py
--rw-r--r--   0 arne       (503) staff       (20)    16662 2023-04-17 00:54:07.000000 EmaCalc-0.9.6/src/EmaCalc/run_sim.py
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-04-17 04:04:46.549479 EmaCalc-0.9.6/src/EmaCalc.egg-info/
--rw-r--r--   0 arne       (503) staff       (20)    10307 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)      691 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/SOURCES.txt
--rw-r--r--   0 arne       (503) staff       (20)        1 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/dependency_links.txt
--rw-r--r--   0 arne       (503) staff       (20)       79 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/requires.txt
--rw-r--r--   0 arne       (503) staff       (20)        8 2023-04-17 04:04:46.000000 EmaCalc-0.9.6/src/EmaCalc.egg-info/top_level.txt
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-05-19 05:51:02.262801 EmaCalc-1.0.0/
+-rw-r--r--   0 arne       (503) staff       (20)     1083 2021-11-24 10:59:26.000000 EmaCalc-1.0.0/LICENSE.txt
+-rw-r--r--   0 arne       (503) staff       (20)    10307 2023-05-19 05:51:02.262863 EmaCalc-1.0.0/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)     9590 2023-03-19 07:22:45.000000 EmaCalc-1.0.0/README.md
+-rw-r--r--   0 arne       (503) staff       (20)       92 2023-03-19 04:45:17.000000 EmaCalc-1.0.0/pyproject.toml
+-rw-r--r--   0 arne       (503) staff       (20)      962 2023-05-19 05:51:02.263118 EmaCalc-1.0.0/setup.cfg
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-05-19 05:51:02.259423 EmaCalc-1.0.0/src/
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-05-19 05:51:02.262048 EmaCalc-1.0.0/src/EmaCalc/
+-rw-r--r--   0 arne       (503) staff       (20)     5792 2023-05-18 12:48:17.000000 EmaCalc-1.0.0/src/EmaCalc/__init__.py
+-rw-r--r--   0 arne       (503) staff       (20)    16290 2022-08-23 14:54:59.000000 EmaCalc-1.0.0/src/EmaCalc/dirichlet.py
+-rw-r--r--   0 arne       (503) staff       (20)    51115 2023-05-16 17:01:31.000000 EmaCalc-1.0.0/src/EmaCalc/ema_base.py
+-rw-r--r--   0 arne       (503) staff       (20)    54253 2023-05-16 08:11:57.000000 EmaCalc-1.0.0/src/EmaCalc/ema_data.py
+-rw-r--r--   0 arne       (503) staff       (20)    40426 2023-05-14 05:47:59.000000 EmaCalc-1.0.0/src/EmaCalc/ema_display.py
+-rw-r--r--   0 arne       (503) staff       (20)    21969 2023-05-14 06:13:43.000000 EmaCalc-1.0.0/src/EmaCalc/ema_display_format.py
+-rw-r--r--   0 arne       (503) staff       (20)     9448 2023-05-14 06:13:43.000000 EmaCalc-1.0.0/src/EmaCalc/ema_file.py
+-rw-r--r--   0 arne       (503) staff       (20)    29119 2023-05-18 06:33:06.000000 EmaCalc-1.0.0/src/EmaCalc/ema_group.py
+-rw-r--r--   0 arne       (503) staff       (20)     8001 2023-05-19 05:31:32.000000 EmaCalc-1.0.0/src/EmaCalc/ema_latent.py
+-rw-r--r--   0 arne       (503) staff       (20)     1272 2022-08-20 11:02:31.000000 EmaCalc-1.0.0/src/EmaCalc/ema_logging.py
+-rw-r--r--   0 arne       (503) staff       (20)    15171 2023-05-18 06:33:06.000000 EmaCalc-1.0.0/src/EmaCalc/ema_model.py
+-rw-r--r--   0 arne       (503) staff       (20)    14769 2023-04-14 02:40:04.000000 EmaCalc-1.0.0/src/EmaCalc/ema_nap.py
+-rw-rw-rw-   0 arne       (503) staff       (20)    19789 2023-05-14 06:36:04.000000 EmaCalc-1.0.0/src/EmaCalc/ema_respondent.py
+-rw-r--r--   0 arne       (503) staff       (20)    23310 2023-05-14 06:55:43.000000 EmaCalc-1.0.0/src/EmaCalc/ema_simulation.py
+-rw-r--r--   0 arne       (503) staff       (20)    20265 2023-05-14 06:55:43.000000 EmaCalc-1.0.0/src/EmaCalc/ema_thresholds.py
+-rw-r--r--   0 arne       (503) staff       (20)    21867 2023-05-14 06:55:43.000000 EmaCalc-1.0.0/src/EmaCalc/gauss_gamma.py
+-rw-r--r--   0 arne       (503) staff       (20)    14980 2023-05-19 05:46:43.000000 EmaCalc-1.0.0/src/EmaCalc/run_ema.py
+-rw-r--r--   0 arne       (503) staff       (20)    17024 2023-05-19 05:46:43.000000 EmaCalc-1.0.0/src/EmaCalc/run_sim.py
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-05-19 05:51:02.262664 EmaCalc-1.0.0/src/EmaCalc.egg-info/
+-rw-r--r--   0 arne       (503) staff       (20)    10307 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)      691 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/SOURCES.txt
+-rw-r--r--   0 arne       (503) staff       (20)        1 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/dependency_links.txt
+-rw-r--r--   0 arne       (503) staff       (20)       81 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/requires.txt
+-rw-r--r--   0 arne       (503) staff       (20)        8 2023-05-19 05:51:02.000000 EmaCalc-1.0.0/src/EmaCalc.egg-info/top_level.txt
```

### Comparing `EmaCalc-0.9.6/LICENSE.txt` & `EmaCalc-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.6/PKG-INFO` & `EmaCalc-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmaCalc
-Version: 0.9.6
+Version: 1.0.0
 Summary: Statistical Analysis of Ecological Momentary Assessment (EMA) Data
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: Momentary Assessment,Nominal Categories,Ordinal Ratings,Bayesian
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `EmaCalc-0.9.6/README.md` & `EmaCalc-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.6/setup.cfg` & `EmaCalc-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	numpy >=1.22
 	scipy >=1.7
 	matplotlib >=3.6.2
 	samppy >=1.3
-	pandas >=2.0
+	pandas >=2.0.1
 	openpyxl >=3.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/__init__.py` & `EmaCalc-1.0.0/src/EmaCalc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,31 +28,38 @@
 
 ema_model: defines class EmaModel as a probabilistic model for EMA data
     and a variational learning algorithm for all model parameters.
 
 ema_group: defines class EmaGroupModel defining probabilistic model for
     ONE population and a group of EMA respondents recruited from that population.
 
-ema_respondent: defines class EmaRespondentModel including data and parameters
+ema_respondent: defines class EmaRespondentModel including recorded data and parameters
     for ONE EMA respondent.
 
 ema_display: classes and functions to display analysis results
 
-ema_display_format: functions formatting the plots and tables with results
+ema_display_format: functions formatting plots and tables with analysis results
 
 ema_base: defines help class EmaParamBase defining internal properties and methods
-    for the storage indexing of all model parameters.
+    for accessing all model parameters.
 
 *** Reference:
 A Leijon, Petra von Gablenz, Inga Holube, Jalil Taghia and Karolina Smeds (2023):
 Bayesian Analysis of Ecological Momentary Assessment (EMA) Data Collected in Adults
 Before and After Hearing Rehabilitation.
 Frontiers in Digital Health, 5(1100705). doi: 10.3389/fdgth.2023.1100705
 
 *** Version History:
+*Version 1.0.0:
+2023-05-17, EmaModel.initialize(...) using n_participants_per_comp instead of max_n_comp.
+2023-04-23, Respondent group specifications moved to ema_data.EmaFrame.
+            EmaDataSet.load() signature changed: can find group category(-ies) in file path.
+            EmaDataSet.save() signature changed: can save data in one single file,
+                or in separate files, by group and / or participant
+
 * Version 0.9.6:
 Include range percentile plots and tables by groups, to show group differences
 
 * Version 0.9.5:
 Show observed and model-predicted attribute grade-counts,
     as requested by one reviewer of Frontiers (2023) paper.
 
@@ -114,10 +121,10 @@
             regardless of regression_effect specification. (NO GOOD! Changed in v. 0.6)
 
 * Version 0.5:
 2021-10-12, Crude version, based on CountProfileCalc-2021, and PairedCompCalc (on PyPi),
 2021-11-24, Functional beta version tested with simulated and (some) real data.
 """
 __name__ = 'EmaCalc'
-__version__ = '0.9.6'
+__version__ = '1.0.0'
 
 __all__ = ['__version__', 'run_ema', 'run_sim']
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/dirichlet.py` & `EmaCalc-1.0.0/src/EmaCalc/dirichlet.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_base.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 from EmaCalc.gauss_gamma import GaussianRV
 # from EmaCalc.ema_thresholds import ThresholdsOld  # for backward compatibility
 from EmaCalc.ema_thresholds import ThresholdsFree, ThresholdsMidFixed
 
 # from EmaCalc.ema_display import aggregate_situation_prob  # ********* for TEST
 
 # ------------------------------------------------------
-__version__ = "2023-04-13"
+__version__ = "2023-05-13"
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
 PRIOR_PSEUDO_RESPONDENT = 0.5  # seems to work OK
 # = hyperprior total pseudo-count re ONE real respondent
 # = prior GaussianRV.mean.learned_weight for all GMM components.
@@ -103,17 +103,24 @@
 # = main hyperprior scale of most Gaussian model parameters,
 # defined in Thurstone d-prime (probit) units for attribute parameters,
 # rescaled if the Bradley (logistic) model is used for latent variables.
 # This prior may have effect on the Occam's Razor function:
 # small values may allow several active GMM components with small variance,
 # but experiments suggest the prior value is not critical.
 
+# *** 2023-05-16, tested with PRIOR_PARAM_SCALE = 0.3:
+# *** Too small, -> some GMM population-model comp. with only ONE member.
+
 PRIOR_PREC_A = PRIOR_PSEUDO_RESPONDENT / 2
 # = GaussianRV precision shape for ALL parameters
 
+# PRIOR_PREC_A_THRESHOLDS = 4 * PRIOR_PREC_A
+# *** Allow user to set smaller prior variance for threshold parameters ?
+# *** 2023-05-13 TESTED, does not make clear difference to GMM number of components.
+
 PRIOR_PREC_B = PRIOR_PARAM_SCALE**2 / 2
 # = GaussianRV precision inv_scale for MOST EmaModel parameters
 # -> allows very small precision <=> large inter-individual variance
 # -> mode of prior component-element variance = PRIOR_PREC_B /(PRIOR_PREC_A + 1) approx= PRIOR_PREC_B
 
 ETA_W_EPSILON = np.finfo(float).eps
 # = additive constant to prevent too small mapped_width(eta)
@@ -287,15 +294,17 @@
                                  rv_class)
         # = single GaussianRV instance, prior for ALL GMM components,
         # fixed throughout the VI learning procedure.
         logger.debug(f'PRIOR_PSEUDO_RESPONDENT = {PRIOR_PSEUDO_RESPONDENT:.3f}; ' +
                      f'PRIOR_PARAM_SCALE = {PRIOR_PARAM_SCALE:.3f}; ' +
                      f'PRIOR_PREC_A = {PRIOR_PREC_A:.3f}; ' +
                      f'PRIOR_PREC_B = {PRIOR_PREC_B:.3f}')
-        logger.debug(f'comp_prior.prec.a = {comp_prior.prec.a:.3f}')
+        logger.debug(f'comp_prior.prec.a = '
+                     + np.array_str(comp_prior.prec.a,
+                                    precision=3))
         logger.debug('comp_prior.prec.b = '
                      + np.array_str(comp_prior.prec.b,
                                     precision=5))
         logger.debug('mode{1 / comp_prior.prec}= '
                      + np.array_str(comp_prior.prec.mode_inv(),
                                     precision=5))
         return cls(emf, effects, rv_class,
@@ -370,20 +379,20 @@
                                               names=[sample_head, *self.emf.situation_dtypes.keys()])
         if groupby is None:
             return pd.Series(u.reshape((-1,)), index=df_index)
         else:
             u /= u.shape[1]
             # u[s, k0, k1, k2, ...] = s-th sample of prob-mass P[(k0, k1, k2,...)-th situation]
             df = pd.Series(u.reshape((-1,)), index=df_index)
-            df = df.groupby(level=[0, *groupby], sort=False).sum()
+            df = df.groupby(level=[0, *groupby], sort=False, group_keys=True).sum()
             # **** needed only if len(groupby) > 1
             if len(groupby) > 1:
                 # scale to CONDITIONAL prob for categories in groupby[0], given other dimensions
-                ds_norm_factor = df.groupby(level=[0, *groupby[1:]]).transform(sum)
-                df = df / df.groupby(level=[0, *groupby[1:]]).transform(sum)
+                df = df / df.groupby(level=[0, *groupby[1:]],
+                                     sort=False, group_keys=True).transform(sum)
                 # CHECK: df.groupby(level=[0, *groupby[1:]], sort=False).sum() == 1., in all groups
             return df
 
     def attribute_theta(self, xi, a):
         """Extract location of latent sensory variable, for ONE given attribute
         used only by ema_display
         :param xi: 2D array with parameter sample vectors
@@ -431,20 +440,21 @@
             # u = Series object with same MultiIndex as theta_ds),
             # containing the CONDITIONAL probability for categories in situation_dtypes[1:]
             # given Phase category in situation_dtypes[0]
             u = u / len(u.index.levels[1])
             # u = absolute prob.mass for each sample and situation category
             # w_cond = u / u.groupby(level=[0, *groupby], sort=False).transform(sum)
             # # = CONDITIONAL prob.mass for categories in aggregate_by, GIVEN each category in groupby
-            w_av = u.groupby(level=[0, *aggregate_by], sort=False).transform(sum)
+            w_av = u.groupby(level=[0, *aggregate_by],
+                             sort=False, group_keys=True).transform(sum)
             # = AVERAGE prob.mass for categories in aggregate_levels
             # = same as ema_display.aggregate_situation_theta
             # -> slightly less variability than w_cond
             theta_ds = theta_ds * w_av  # w_cond  # ???
-            return theta_ds.groupby(level=[0, *groupby], sort=False).sum()
+            return theta_ds.groupby(level=[0, *groupby], sort=False, group_keys=True).sum()
 
     def attribute_tau(self, xi, a):
         """Extract response thresholds for ONE given attribute,
         EXCEPT fixed extreme limits at -inf, +inf.
         Used only by ema_display
         :param xi: 2D array with parameter sample vectors
             xi[s, :] = s-th parameter sample vector
@@ -770,18 +780,20 @@
                 rv_class):
     """Create hyperprior for parameter distribution in the total population
     :param n_parameters: total number of parameters
     :param alpha_slices: list with index slice for each situation phase
     :param attribute_slices: list with one AttributeSlice tuple for each attribute
     :return: single GaussianRV instance
     """
-    prec_a = PRIOR_PREC_A  # scalar, same for all elements
+    prec_a = PRIOR_PREC_A  # * np.ones(n_parameters)  # still scalar, same for all elements
     prec_b = PRIOR_PREC_B * np.ones(n_parameters)
     for (b_slice, e_slice) in attribute_slices:
         prec_b[b_slice] *= rv_class.scale**2
+        # prec_a[e_slice] *= 100.  # ****** temp fix just for TEST
+        # ************* TEST reduce prior threshold-parameter variance, no
     loc = np.zeros(n_parameters)
     for a_slice in alpha_slices:
         loc[a_slice] = - np.log(a_slice.stop - a_slice.start)
     return GaussianRV.initialize(loc=loc,
                                  learned_weight=PRIOR_PSEUDO_RESPONDENT,
                                  prec_a=prec_a,
                                  prec_b=prec_b)
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_data.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,137 @@
 """This module defines classes to access and store recorded EMA data,
 and methods and functions to read and write such data.
 
 Each EMA Record includes nominal and ordinal elements, defining
 * a participant ID label,
 * a single SITUATION specified by selected categories in ONE or MORE Situation Dimension(s),
 * ordinal RATING(s) for ZERO, ONE, or MORE perceptual ATTRIBUTE(s) in the current situation.
+* (optionally) group category label(s) for this participant
 
 *** Class Overview:
 
 EmaFrame: defines study layout and category labels of data in each EMA Record.
     EmaFrame properties can also define selection criteria
     for a subset of data to be included for analysis.
 
 EmaDataSet: container of all EMA data to be used as input for statistical analysis.
 
 *** File Formats:
 
 Data may be stored in various table-style file formats allowed by package pandas,
 e.g., xlsx, csv, odt, etc.
-A single data file may include EMA records from ONE or SEVERAL participants.
+Each data file may include EMA records from ONE or SEVERAL participants.
+
 The participant id may be stored in a designated column of the table,
 or the file name may be used as participant id,
 or (in Excel-type files) the participant may be identified by the sheet name.
 
-However, EmaDataSet.save(...) method always creates one table file for each participant.
+Group category(-ies) may be defined in table column(s),
+OR defined by sub-string(s) of the absolute path for each file.
 
+A collected EMA data set can be saved in various file formats, similar to input files.
 
 *** Input Data Files:
 
 All input files from an experiment must be stored in ONE directory tree.
 
-If results are to be analyzed for more than one GROUP of test participants,
-the data for each group must be stored in separate sub-directories
-within the specified top directory.
-
-Groups are identified by a tuple of pairs (group_factor, group_category), where
-group_factor is a grouping dimension, e.g., 'Age', or 'Gender', and
-group_category is a category label within the factor, e.g., 'old', or 'female'.
-
-A sequence of one element from each group-factor pair must define a unique path
-to files containing data for participants in ONE group.
-Group directories must have names like, e.g., 'Age_old' for group = ('Age', 'old')
-
-Participant file names can be arbitrary, although they may be somehow associated with
-the encoded name of the participant, to facilitate data organisation.
+If a group dimension is specified by the file path, the path must include a sub-string
+combining the group dimension and one category,
+for example, 'Age_old', if the group dimension 'Age' has allowed categories 'young' and 'old'.
 
 Each participant in the same group MUST have a unique participant ID.
 
-Different files in the same directory
-may include data for the same participant in the group,
+Different files may include data for the same participant,
 e.g., results obtained in different test phases,
 or simply for additional sets of EMA records from the same participant.
 
 Participants in different groups may have the same participant ID values,
 because the groups are separated anyway,
 but normally the participant IDs should be unique across all groups.
 
 *** Example Directory Tree:
 
 Assume we have data files in the following directory structure:
-~/ema_study / Age_old / Gender_male, containing files Data_EMA_64.xlsx and Response_Data_LAB_64.xlsx
-    with data to be analyzed for group key= (('Age', 'old'), ('Gender', 'male'))
-~/ema_study / Age_old / Gender_female, containing files Subjects_EMA_64.xlsx and Data_EMA_65.xlsx
-~/ema_study / Age_young / Gender_male,  containing files EMA_64.xlsx and EMA_65.xlsx
-~/ema_study / Age_young / Gender_female, containing files EMA_64.xlsx and EMA_65.xlsx
+~/ema_study / Age_old / Gender_male, containing files Test_EMA_64.xlsx and Response_Data_LAB_64.xlsx
+    with data to be analyzed for group key= ('old', 'male') in group dimensions ('Age', 'Gender').
+~/ema_study / Age_old / Gender_female, containing files Test_EMA_64.xlsx and Data_EMA_65.xlsx
+~/ema_study / Age_young / Gender_male,  containing files Test_EMA_64.xlsx and EMA_65.xlsx
+~/ema_study / Age_young / Gender_female, containing files Test_EMA_64.xlsx and EMA_65.xlsx
 
-Four separate groups may then be defined by factors Age and Gender,
+Four separate groups may then be defined by dimensions 'Age' and 'Gender',
 and the analysis may be restricted to only use data in files with names including 'EMA_64'.
 
-
 *** Accessing Input Data for Analysis:
 *1: Create an EmaFrame object defining the experimental layout, e.g., as:
 
 emf = EmaFrame.setup(situations={'CoSS': [f'C{i}' for i in range(1, 8)],
                                  'Important': ('Slightly', 'Medium', 'Very'),
                                  },  # nominal variables
                      attributes={'Speech': ('Very Hard', 'Fairly Hard', 'Fairly Easy','Very Easy')},
+                     groups={'Age': ('young', 'old'),
+                             'Gender': ('female', 'male'),
+                             'Test': ('EMA_64',)},
         )
-NOTE: String CASE is always distinctive, i.e., 'Male' and 'male' are different categories.
+NOTE: String CASE is always distinctive, i.e., 'Male' and 'male' are DIFFERENT categories.
 
 *2: Load all test results into an EmaDataSet object:
 
 ds = EmaDataSet.load(emf, path='~/ema_study',
-                    grouping={'Age': ('young', 'old'),
-                              'Gender': ('female', 'male'),
-                              'Test': ('EMA_64',)}
                     fmt='xlsx',
                     participant='sheet',  # xlsx sheet title is used as participant ID
+                    path_groups=['Age', 'Gender', 'Test']  # group dimensions identified by file path
                     )
+The parameter emf is an EmaFrame object that defines all variables to be analyzed,
+and the other arguments specify where these variables are to be found.
 
+The resulting data set includes exactly FOUR combinations of 'Age' and 'Gender',
+with an extra dimension 'Test' that has only one allowed category.
 The object ds can now be used as input for analysis.
-The parameter emf is an EmaFrame object that defines the variables to be analyzed.
 
 *** Selecting Subsets of Data for Analysis:
-It is possible to define a data set including only a subset of recorded data files.
-For example, assume we want to analyze only two groups, old males, and old females.
+It is possible to define a data set using only a subset of the data files in the given directory tree.
+For example, assume we want to analyze only TWO groups, old males, and old females,
+and only data from group dimension 'Test' with the single category 'EMA_64',
 and only responses for Situation dimension 'CoSS'.
+
 Then we must define a new EmaFrame object, and load only a subset of group data:
 
 emf = EmaFrame.setup(situations={'CoSS': [f'C{i}' for i in range(1, 8)],
                                  },  # nominal variables
                      attributes={'Speech': ('Very Hard', 'Fairly Hard', 'Fairly Easy','Very Easy')},
-                     )
+                     groups={'Age': ('old',),
+                             'Gender': ('female', 'male'),
+                             'Test': ('EMA_64',)}
+                    )
+ds = EmaDataSet.load(emf, path='~/ema_study',
+                    fmt='xlsx',
+                    participant='sheet',
+                    path_groups=['Age', 'Gender', 'Test'])
+
+In case all input data have been collected in a single file in the data directory,
+the file must include columns with header 'Age', 'Gender',
+and one column for the participant ID, with header, e.g., 'Test Subject'.
+Then the data may be accessed as
+
 ds = EmaDataSet.load(emf, path='~/ema_study',
-                    grouping={'Age': ('old',),
-                              'Gender': ('female', 'male'),
-                              'Test': ('EMA_64',)}
                     fmt='xlsx',
-                    participant='sheet',    # xlsx sheet title is participant ID
+                    participant='Test Subject',  # column header
+                    path_groups=['Test']  # read only file paths including 'Test_EMA_64'
                     )
+This data set will include TWO groups named ('old', 'female', EMA_64), and ('old', 'male', EMA_64)
 
 
 *** Version History:
+* Version 1.0.0:
+2023-04-25, Group categories specified in EmaFrame.setup(...)
+            EmaFrame.filter(...) does all data checking.
+            EmaDataSet.load(...) allows group category in file path.
+            EmaDataSet.save(...) can save separate group/participant files, or one big file.
+            EmaDataSet.groups: keys include only group categories, NOT group "dimensions".
+
 * Version 0.9.6:
 2023-04-11, bugfix EmaDataSet.join_df, .attribute_count, .attribute_mean
 
 * Version 0.9.4:
 2022-11-06: Fix to avoid FutureWarning in EmaDataSet.attribute_grade_mean
 
 * Version 0.9.3:
@@ -149,86 +165,89 @@
 * Version 0.5:
 2021-10-15, first functional version
 2021-11-18, groupby moved from EmaFrame -> EmaDataSet.load
 2021-11-20, EmaDataSet.ensure_complete
 2021-11-23, Group dir name MUST include both (g_factor, g_cat), e.g., 'Age_old'
 2021-11-xx, allow empty attribute_grades
 """
-# *** move grouping info -> EmaFrame, allow group categories in table column OR path string
-# *** save EmaDataSet as ONE big DataFrame file, OR separate by participants or groups
-
-# Future ?:
+# *** Future:
 # *** EmaDataSet.initialize + add method ? load = initialize + add
-# *** EmaDataSet store groups / subgroups hierarchically in tree structure ???
 
 import numpy as np
 from pathlib import Path
 import pandas as pd
 
-from itertools import product
+from itertools import product, chain
 import logging
 
 from EmaCalc.ema_file import ema_gen, Table, FileReadError, FileWriteError
 from EmaCalc.ema_nap import nap_pandas
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
 
 # ------------------------------------------------------------------
 class EmaFrame:
     """Defines variable names and categories of all data elements
-    recorded by each respondent in an EMA study.
+    to be analyzed in an EMA study.
     The allowed categories of each EMA variable is stored as a pd.CategoricalDtype instance.
     """
-    def __init__(self, situation_dtypes, phase_key, ordinal_scales, attribute_scales):
+    def __init__(self, situation_dtypes, phase_key, ordinal_scales, attribute_scales, group_dtypes):
         """
         :param situation_dtypes: dict with elements (dimension, dtype), where
             dimension is a string label identifying one situation "dimension",
             dtype is a pd.CategoricalDtype defining NOMINAL categories within this dimension.
         :param phase_key: situation key (dimension name) for the test phase,
             which MUST be the FIRST element of situation_dtypes.
         :param ordinal_scales: dict with elements (scale_id: dtype), where
             dtype is a pd.CategoricalDtype defining ORDINAL categories for the scale.
         :param attribute_scales: dict with elements (attribute_key, scale_id), defining
             the scale used by each attribute.
             Note: Separate attributes may use the SAME ordinal scale,
                 if so specified by the researcher.
+        :param group_dtypes: dict with elements (dimension, dtype), where
+            dimension is a string label identifying one grouping "dimension", e.g., 'Age'
+            dtype is a pd.CategoricalDtype defining NOMINAL categories within this dimension.
         """
-        # ******** include group_dtypes here, like situation_dtypes
         self.situation_dtypes = situation_dtypes
         self.phase_key = phase_key
         self.ordinal_scales = ordinal_scales
         self.attribute_scales = attribute_scales
+        self.group_dtypes = group_dtypes
 
     def __repr__(self):
         return (self.__class__.__name__ + '(\n\t\t' +
                 ',\n\t\t'.join(f'{key}={repr(v)}'
                                for (key, v) in vars(self).items()) +
                 '\n\t\t)')
 
     @classmethod
-    def setup(cls, situations=None, phase_key='Phase', attributes=None):  # include groups = dict here *******
+    def setup(cls, situations=None, phase_key='Phase', attributes=None, groups=None):
         """Create the EmaFrame object defining all EMA variables to be analyzed.
         :param situations: (optional) dict or iterable with elements (dimension, category_list), where
             dimension is a string label identifying one situation "dimension",
             category_list is an iterable of labels for NOMINAL categories within this dimension.
         :param attributes: (optional) dict or iterable with elements (attribute, grades),
             attribute is string id of a rated perceptual attribute,
             grades is an iterable with ORDINAL categories, strings or integer.
         :param phase_key: (optional) situation key for the test phase, with
             situation_dtypes[phase_key] = list of test phases (e.g., before vs after treatment),
                 specified by experimenter, i.e., NOT given as an EMA response
             situation_dtypes[phase_key] is automatically added with a SINGLE value,
             if not already defined in given situation_dtypes.
+        :param groups: (optional) dict or iterable with elements (dimension, category_list), where
+            dimension is a string label identifying one grouping "dimension", e.g., 'Age' or 'Gender',
+            category_list is an iterable of labels for NOMINAL categories within this dimension.
 
-        NOTE: situation_dtypes and attribute_grades may define a subset of
-            data columns in input data files, if not all variants are to be analyzed.
-            MUST be specified EXACTLY as stored in data files,
+        NOTE: situation_dtypes and attribute_grades and groups may define a subset of
+            data in input data files, if not all variants are to be analyzed.
+            Categories MUST be specified EXACTLY as stored in data files,
             case-sensitive, i.e., 'A', and 'a' are different categories.
+
             If needed, the EmaDataSet.load(...) method allows
             argument 'converters' to pandas reader function,
             defining a dict with function(s) to make saved data fields agree with pre-defined categories.
             Column headers in the data files may also be re-named, if needed,
             as specified by argument rename_cols to the EmaDataSet.load(...) method.
         """
         if situations is None:
@@ -251,15 +270,20 @@
         # NOTE: some attributes.values() may be IDENTICAL objects, not only equal.
         ordinal_scales = {id(a_cats): pd.CategoricalDtype(categories=a_cats,
                                                           ordered=True)
                           for (a, a_cats) in attributes.items()}
         # including only UNIQUE scales, each possibly tied to more than one attribute
         attribute_scales = dict((a, id(a_cats))
                                 for (a, a_cats) in attributes.items())
-        return cls(situations, phase_key, ordinal_scales, attribute_scales)
+        if groups is None:
+            groups = dict()  # {'': ['']}  # Empty?, ONE un-named group with all participants
+        groups = dict((g, pd.CategoricalDtype(categories=g_cats,
+                                             ordered=False))
+                     for (g, g_cats) in groups.items())
+        return cls(situations, phase_key, ordinal_scales, attribute_scales, group_dtypes=groups)
 
     @property
     def tied_response_scales(self):
         """Some ordinal scale tied to more than one attribute scale"""
         return len(self.ordinal_scales) < len(self.attribute_scales)
 
     @property
@@ -283,73 +307,58 @@
                 for s_id in self.ordinal_scales.keys()}
 
     @property
     def dtypes(self):
         """
         :return: dict with all defined ema variables and their dtypes
         """
-        return self.situation_dtypes | self.attribute_dtypes
+        return self.situation_dtypes | self.attribute_dtypes | self.group_dtypes
 
     @property
     def situation_shape(self):
         """tuple with number of nominal categories for each situation dimension"""
         return tuple(len(sit_dtype.categories)
                      for sit_dtype in self.situation_dtypes.values())
 
     @property
-    def n_situations(self):  # **** needed ?
-        return np.prod(self.situation_shape, dtype=int)
-
-    def situation_axes(self, sits):
-        """Translate situation keys -> integer axes indices
-        :param sits: sequence of one or more situation keys
-        :return: tuple of corresponding numerical axes
-        """
-        sit_keys = list(self.situation_dtypes.keys())
-        sit_ind = []
-        for sit_i in sits:
-            try:
-                sit_ind.append(sit_keys.index(sit_i))
-            except ValueError:
-                logger.warning(f'{repr(sit_i)} is not a situation key')
-        return tuple(sit_ind)
-
-    @property
     def rating_shape(self):
         """tuple with number of ordinal response levels for each attribute
         """
         return tuple(len(r_cat.categories)
                      for r_cat in self.attribute_dtypes.values())
 
     @property
     def n_phases(self):
         # == situation_shape[0]
         return len(self.situation_dtypes[self.phase_key].categories)
 
-    def required_vars(self):
-        return [*self.situation_dtypes.keys()] + [*self.attribute_dtypes.keys()]
+    def group_head(self):
+        return tuple(self.group_dtypes.keys())
 
-    # def required_types(self):  # *** not needed, use property dtypes ***
-    #     return self.situation_dtypes | self.attribute_dtypes
+    def required_vars(self):
+        return list(chain(self.situation_dtypes.keys(),
+                          self.attribute_dtypes.keys(),
+                          self.group_dtypes.keys()))
 
-    def filter(self, ema):
+    def filter(self, ema, participant):
         """Check and filter EMA data for ONE participant, to ensure that
         it includes the required columns, with required data types.
         :param ema: a pd.DataFrame instance
+        :param participant: a required column name
         :return: a pd.DataFrame instance with complete data
             or an empty DataFrame if no usable EMA records were found
         """
+        # *** check and correct for Phase column here ? ***********
+        required_col = self.required_vars() + [participant]
+        required_dtypes = self.dtypes | {participant: object}  # *** string?
         try:
-            ema = ema[self.required_vars()]
-            ema = ema.astype(self.dtypes, errors='raise')
+            ema = ema[required_col]  # *** do not drop columns, only TEST ? ****
+            ema = ema.astype(required_dtypes, errors='raise')
             # *** this accepts NaN, but sets NaN if cell contents not in defined categories ***
-            # if np.any(ema.isna()):
-            #     logger.warning('Some input data is NaN:\n'
-            #                    + str(ema.head(10)))
-            # # ******* delete rows with NaN not needed? NaNs excluded by DataFrame.value_counts()
+            # *** delete rows with NaN not needed? NaNs excluded anyway by DataFrame.value_counts()
         except KeyError as e:
             raise FileReadError(f'Some missing required data column(s). Error {e}')
         except ValueError as e:
             raise FileReadError(f'Incompatible data type. Error {e}')
         return ema
 
     def count_situations(self, ema):
@@ -361,15 +370,14 @@
             z.shape == self.situation_shape
         """
         # 2022-05-24, Arne Leijon: verified manually with input data
         z = ema.value_counts(subset=list(self.situation_dtypes.keys()), sort=False)
         # = pd.Series including only non-zero counts, indexed by situation or tuple(situation_dtypes)
         ind = pd.MultiIndex.from_product([sit_dtype.categories
                                           for sit_dtype in self.situation_dtypes.values()])
-        # ind as EmaFrame method?
         z = z.reindex(index=ind, fill_value=0)
         # must reindex to include zero counts
         return np.array(z).reshape(self.situation_shape)
 
     def count_grades(self, a, ema):
         """Count grade occurrences for given attribute
         :param a: attribute key
@@ -392,16 +400,16 @@
 class EmaDataSet:
     """Container of all data input for one complete EMA study.
     """
     def __init__(self, emf, groups):
         """
         :param emf: an EmaFrame instance
         :param groups: dict with elements (group_id: group_dict), where
-            group_id = tuple with one or more pairs (g_factor, g_category),
-                identifying a sub-population,
+            group_id = tuple (g_cat_0, g_cat_1,...), identifying a population
+                by one category selected for each group "dimension".
             group_dict = dict with elements (participant_id, ema_df), where
             ema_df = a pd.DataFrame instance with one column for each EMA variable,
             and one row for each EMA record.
             ema_df.shape == (n_records, n SITUATION dimensions + n ATTRIBUTES)
         """
         self.emf = emf
         self.groups = groups
@@ -415,135 +423,215 @@
                 + f'emf= {self.emf},\n\t'
                 + 'groups= {' + '\n\t\t'
                 + '\n\t\t'.join((f'{g}: {len(g_participants)} participants '
                                  + f'with {sum_n_records(g_participants)} EMA records in total,')
                                 for (g, g_participants) in self.groups.items())
                 + '\n\t\t})')
 
-    # *** separate classmethod initialize, method add; load = initialize + add
+    # *** separate classmethod initialize, method add; load = initialize + add ?
+    # *** to allow collecting data from several sources, with different file formats...
 
     @classmethod
-    def load(cls, emf, path,
+    def load(cls, emf, path, fmt=None,
              participant='file',
-             grouping=None,
-             fmt=None,
-             ema_vars=None,
+             path_groups=None,
+             group_join_str='_',
+             ema_vars=None, grouping=None,
              **kwargs):
-        """Create one class instance with selected data from input files.
+        """Create one class instance with selected data from input file(s).
         :param emf: EmaFrame instance
-        :param path: string or Path defining top of directory tree with all data files
+        :param path: string or Path defining top of directory tree containing all data files.
+            Files in all subdirectories are searched, hierarchically.
+        :param fmt: (optional) string with file suffix for data files.
+            If None, all files are tried, so files with mixed formats can be used as input.
         :param participant: string defining where to find participant ID in a file,
-            = column name, 'file', or 'sheet' if fmt == xlsx
-        :param grouping: (optional) dict or iterable with elements (group_dim, category_list),
-            where
-            group_dim is a string label identifying one "dimension" of populations,
-            category_list is a list of labels for allowed categories within group_factor.
-            If None, only ONE (unnamed) group is included.
-        :param fmt: (optional) string with file suffix for accepted data files.
-            If None, all files are tried, so mixed file formats can be used as input.
-        :param ema_vars: (optional) *** only for version warning, no longer used
+            = column name, 'file', or 'sheet' if excel-type file that has 'sheet's
+        :param path_groups: (optional) list with group-dimension labels
+            for group categories to be specified by substrings in file paths,
+            used only IF NOT specified in a column in the data file.
+        :param group_join_str: (optional) string between group dimension and category in file path,
+            e.g., '_' in '... / Age_old / ...'
+        :param ema_vars: *** only for version warning, no longer used
+        :param grouping: *** only for version warning, no longer used
         :param kwargs: (optional) any additional arguments for pandas file_reader
+            e.g., rename_cols={...},  converters={...}.
         :return: a single cls object
 
-        NOTE: Situation categories and Attribute grades in input files must agree EXACTLY
-            with categories defined in emf.
-            Use argument 'converters' to pandas reader function
-            with function(s) to make saved data fields agree with pre-defined categories.
-            Use argument 'rename_cols' to translate file column headers to desired names.
-        """
-        if ema_vars is not None:  # warning for backwards incompatibility
-            logger.warning('EmaCalc v. >= 0.9: ema_vars not used to select EMA variables. '
+        NOTE: Situation categories and Attribute grades and group categories must agree EXACTLY
+            with the categories previously defined in emf.
+            If needed, use keyword argument
+            converters={column_head: convert_fcn, ...} to pandas reader function
+            with converter function(s) to make saved data fields agree with pre-defined categories.
+            Use keyword argument
+            rename_cols={old_head: new_head, ...} to change file column headers to desired names.
+        """
+        def clean_up(s_ema):
+            """Remove unused group and participant columns, re-index EMA records
+            :param s_ema: a pd.DataFrame for ONE participant, incl group and participant id columns
+                with a single RangeIndex for EMA record number
+            :return: copy of s_ema, with redundant info removed
+            """
+            index_cols = list(emf.group_head()) + [participant]
+            drop_cols = [c for c in index_cols if c in s_ema.columns]  # avoid KeyError in drop()
+            s_ema = s_ema.drop(columns=drop_cols)
+            s_ema.index = pd.RangeIndex(range(s_ema.shape[0]))
+            # because the original index was artificially created by concat
+            return s_ema
+
+        # ---------------------------------------------------------------
+        if ema_vars is not None:  # backwards incompatibility
+            logger.warning('EmaCalc v. > 0.9.0: ema_vars not used to select EMA variables. '
                            + 'Using file table header instead. \n'
                            + 'Change column names by "rename_cols" argument, if needed.')
+        if grouping is not None:  # backwards incompatibility
+            logger.warning('EmaCalc v. > 0.9.6: group categories are defined in EmaFrame.setup().'
+                           +'\nDefine only "path_groups" here, for group dim.s specified by path string.')
+        if fmt is not None and fmt[0] != '.':
+            fmt = '.' + fmt
         path = Path(path)
-        if grouping is None:
-            grouping = dict()
-        else:
-            grouping = dict(grouping)
-        groups = {g: dict() for g in _groups(grouping)}
-        # = dict with empty dict for participants in each group
+        if path_groups is None:
+            path_groups = []
         # **** up to here -> classmethod initialize
         # **** following: -> add method, to allow collecting data from different file formats ?
-        for (g, g_path) in _gen_group_file_paths(path, fmt, [*grouping.items()]):
-            logger.info(f'Reading {g_path}')
+
+        # v 1.0.0: collect a list of ema chunks, then concat and separate by group and participant:
+        all_ema = []  # space for all input EMA tables
+        path_groups = {g_key: emf.group_dtypes[g_key].categories
+                       for g_key in emf.group_dtypes if g_key in path_groups}
+        # = dict with (g_key, g_cats) for all g_keys that MAY be derived from file path.
+        for (path_group_id, g_path) in _gen_group_file_paths(path, fmt, path_groups, group_join_str):
+            # path_group_id = dict with element (group_key, group_cat) specified as g_path sub-strings
+            logger.info(f'Path group {path_group_id}: Reading {g_path}')
             try:
                 ema_file = ema_gen(g_path,
                                    participant=participant,
                                    **kwargs)
-                for (s, ema) in ema_file:
-                    # ema is a pd.DataFrame with a COPY of (possibly converted) data from file
+                for ema in ema_file:
+                    # ema is a pd.DataFrame with a COPY of (possibly converted) data from file,
+                    # with one column name == participant.
+                    for (g_key, g_cat) in path_group_id.items():
+                        if g_key not in ema.columns:
+                            ema[g_key] = g_cat  # set group categories derived from path sub-string
                     if emf.n_phases == 1:  # phase-code might be unspecified in file
                         # if file rows have phase as empty string, Pandas reads it as NaN!
-                        # *** Should never happen!
-                        phase_cat = emf.situation_dtypes[emf.phase_key].categories[0]
                         if emf.phase_key not in ema.columns:
-                            ema[emf.phase_key] = phase_cat
-                    ema = emf.filter(ema)  # ensure it conforms to given emf
-                    logger.info(f'participant {repr(s)}: {ema.shape[0]} EMA records. '
+                            ema[emf.phase_key] = emf.situation_dtypes[emf.phase_key].categories[0]
+                    ema = emf.filter(ema, participant)
+                    # = pd.DataFrame with all required columns, and nothing else!
+                    logger.info(f'EMA chunk with {ema.shape[0]} records. '
                                 + ('Some missing data. Valid data count =\n'
                                    + _table_valid(ema) if np.any(ema.isna()) else ''))
-                    # ******* delete rows with NaN not needed!
-                    # NaNs excluded later anyway by pandas.DataFrame.value_counts()
-                    logger.debug(f'Participant {repr(s)}:\n' + ema.to_string())
                     if not ema.empty:
-                        if s not in groups[g]:
-                            groups[g][s] = ema
-                        else:
-                            groups[g][s] = pd.concat(groups[g][s], ema)
+                        all_ema.append(ema)
             except FileReadError as e:
                 logger.warning(e)  # and just try next file
+        if len(all_ema) == 0:
+            raise FileReadError('No EMA data found')
+        else:
+            all_ema = pd.concat(all_ema, axis=0, ignore_index=True)
+        # store all data in structured dict instead: **** or just leave it as a single chunk ? ***
+        if len(emf.group_dtypes) == 0:
+            groups = {(): {s: clean_up(s_ema)
+                           for (s, s_ema) in all_ema.groupby(participant)}
+                      }
+        else:
+            groups = {g: {s: clean_up(s_ema)
+                          for (s, s_ema) in g_ema.groupby(participant)}
+                      for (g, g_ema) in all_ema.groupby(list(emf.group_dtypes.keys()))}
         return cls(emf, groups)
 
     # def add method, to include data from new files with different layout ???
 
-    def save(self, dir, allow_over_write=False, fmt='csv', **kwargs):
-        """Save self.groups in a directory tree with one folder for each group,
-        with one file for each participant.
-        :param dir: Path or string defining the top directory where files are saved
-        :param allow_over_write: boolean switch, over-write files if True
-        :param fmt: string label specifying file format
+    def save(self, path, fmt='.csv', allow_over_write=False,
+             participant='file',
+             join_groups=False,
+             group_join_str='_',
+             **kwargs):
+        """Save all EMA data from self.groups, either
+        as a single file with EMA records for all participants in all groups,
+        OR in a directory tree for groups, with one file for each group,
+        OR with one separate file for each participant.
+        :param path: Path or string defining the top directory where files are saved
+        :param allow_over_write: (optional) boolean switch
+        :param fmt: (optional) file-name extension string specifying file format
+        :param join_groups: (optional) boolean switch: True -> ONE file for all groups
+        :param participant: (optional) string defining where to store participant ID,
+            = column name, -> all participants in a group saved in ONE file
+            or 'file' -> one file for each participant, with participant ID as file name
+        :param group_join_str: (optional) string between group dimension and category in file path
         :param kwargs: (optional) arguments to Table.save() or selected pandas.to_xxx()
         :return: None
         """
-        # *** allow save as ONE concatenated pd.DataFrame instance ? *********
-        dir = Path(dir)
-        for (g, group_data) in self.groups.items():
-            g = _dir_name(g, '/')
-            if len(g) == 0:
-                g_path = dir
+        def drop_empty_phase(df):
+            # if Phase column contains only empty strings, drop it, do NOT save it,
+            # because Pandas might read it as NaN, not as empty string
+            phase_key = self.emf.phase_key
+            if self.emf.n_phases == 1 and all(df[phase_key] == ''):
+                df = df.drop(columns=[phase_key], inplace=False)
+            return df
+
+        # --------------------------------------------------------------
+        if fmt[0] != '.':
+            fmt = '.' + fmt
+        path = Path(path)
+        if participant == 'file':
+            if join_groups:
+                join_groups = False
+                logger.warning('Must have join_groups = False to save participants in separate files')
+        try:
+            if join_groups:  # AND participants
+                groups = self.join_df(participant=participant)
+                groups = drop_empty_phase(groups)
+                f_name = group_join_str.join(emf.group_head())
+                if len(f_name) == 0:
+                    f_name = 'participants'
+                else:
+                    f_name += '_participants'
+                f_path = (path / f_name).with_suffix(fmt)
+                f_path.parent.mkdir(parents=True, exist_ok=True)
+                Table(groups).save(f_path, allow_over_write, **kwargs)
             else:
-                g_path = dir / g
-            g_path.mkdir(parents=True, exist_ok=True)
-            for (s_id, s_df) in group_data.items():
-                # if Phase column contains only empty strings, drop it, do NOT save it,
-                # because Pandas might read it as NaN, not as empty string
-                phase_key = self.emf.phase_key
-                if self.emf.n_phases == 1 and all(s_df[phase_key] == ''):
-                    s_df = s_df.drop(columns=[phase_key], inplace=False)
-                try:
-                    p = (g_path / str(s_id)).with_suffix('.' + fmt)  # one file per participant
-                    Table(s_df).save(p, allow_over_write, **kwargs)
-                except FileWriteError as e:
-                    raise RuntimeError(f'Could not save {self.__class__.__name__} in {repr(fmt)} format. '
-                                       + f'Error: {e}')
+                for (g, group_data) in self.groups.items():
+                    g_dir = group_dir_str(self.emf.group_head(), g, sep=group_join_str)
+                    # = group sub-path string, empty if single un-named group
+                    g_path = path / g_dir
+                    if participant == 'file':
+                        g_path.mkdir(parents=True, exist_ok=True)
+                        for (s_id, s_df) in group_data.items():
+                            s_df = drop_empty_phase(s_df)
+                            p = (g_path / str(s_id)).with_suffix(fmt)  # one file per participant
+                            Table(s_df).save(p, allow_over_write, **kwargs)
+                    else:
+                        g_table = pd.concat(group_data, axis=0,
+                                            ignore_index=False,
+                                            sort=False,
+                                            names=[participant]
+                                            )
+                        g_table = drop_empty_phase(g_table)
+                        f_path = g_path.with_suffix(fmt)  # last dir level becomes the file
+                        g_path.parent.mkdir(parents=True, exist_ok=True)
+                        Table(g_table).save(f_path, allow_over_write, **kwargs)
+        except FileWriteError as e:
+            raise RuntimeError(f'Could not save {self.__class__.__name__} in {repr(fmt)} format. '
+                               + f'Error: {e}')
 
     def ensure_complete(self):
         """Check that we have at least one participant in every sub-population category,
         with at least one ema record for each participant (already checked in load method).
         :return: None
 
         Result:
         self.groups may be reduced:
         participants with no records are deleted,
         groups with no participants are deleted
         logger warnings for missing data.
         """
         for (g, g_participants) in self.groups.items():
             incomplete_participants = set(s for (s, s_ema) in g_participants.items()
-                                      if len(s_ema) == 0)
+                                      if s_ema.empty)
             for s in incomplete_participants:
                 logger.warning(f'No EMA data for participant {repr(s)} in group {repr(g)}. Deleted!')
                 del g_participants[s]
         incomplete_groups = set(g for (g, g_participants) in self.groups.items()
                                 if len(g_participants) == 0)
         for g in incomplete_groups:
             logger.warning(f'No participants in group {repr(g)}. Deleted!')
@@ -551,55 +639,47 @@
         if len(self.groups) == 0:
             raise RuntimeError('No EMA data in any group.')
         for attr in self.emf.attribute_dtypes.keys():
             a_count = self.attribute_grade_count(attr)
             # = pd.DataFrame with all groups, all participants
             _check_ratings(attr, a_count)
 
-    # def join_df(self):
-    #     """Join all EMA data into ONE single pd.DataFrame instance
-    #     for all groups and all participants
-    #     :return: a single pd.DataFrame instance
-    #     """
-    #     df_list = []
-    #     for (g_tuple, g_data) in self.groups.items():
-    #         for (s, s_ema) in g_data.items():
-    #             df = Table(s_ema.copy())
-    #             df['Participant'] = s
-    #             for g in g_tuple:
-    #                 df[g[0]] = g[1]
-    #             df_list.append(df)
-    #     return pd.concat(df_list, ignore_index=True)
-
-    def group_head(self):  # TEMP fix -> EmaFrame *****
-        g_head = list(self.groups.keys())[0]  # they are all equal
-        return tuple(g_k[0] for g_k in g_head)
-
-    @staticmethod
-    def group_id(g_key):
-        """split g_key into actual group-id part
-        :param g_key: tuple of pairs (g_head, g_id)
-        :return: tuple including only g_id parts
-        """
-        return tuple(g_k[1] for g_k in g_key)
-
-    def join_df(self):
+    def join_df(self, participant='Participant'):  # **** default 'Participant' where ?
         """Join all EMA data into ONE single pd.DataFrame instance
         for all groups and all participants
-        :return: a single pd.DataFrame instance
+        :param participant: (optional) name of column with participant ID
+        :return: a single pd.DataFrame instance  **** NOT Table ?
         """
-        g_dict = {self.group_id(g_key): pd.concat({s: s_data
-                                                   for (s, s_data) in g_data.items()},
-                                                  axis=0,
-                                                  sort=False,
-                                                  names=['Participant'])  # *** -> cls property ?
+        g_dict = {g_key: pd.concat({s: s_data
+                                    for (s, s_data) in g_data.items()},
+                                   axis=0,
+                                   sort=False,
+                                   names=[participant])
                   for (g_key, g_data) in self.groups.items()}
-        df = pd.concat(g_dict, axis=0, names=self.group_head(), sort=False)
+        # if len(g_dict) == 1 and len(self.emf.group_head()) == 0:  # only ONE UN-NAMED group
+        #     (g_cat, df) = g_dict.popitem()
+        # else:
+        #     df = pd.concat(g_dict, axis=0, names=self.emf.group_head(), sort=False)
+        df = self._join_group_dict(g_dict)
         return Table(df)
 
+    def _join_group_dict(self, g_dict):
+        """Help method to concat pd.DataFrame or pd.Series instances across groups,
+        with special treatment in case of single un-named group.
+        Needed only internally.
+        :param g_dict: dict with elements (g_key, g_data), where
+            g_data is a DataFrame or pd.Series object
+        :return: a single pd.DataFrame or pd.Series instance
+        """
+        if len(g_dict) == 1 and len(self.emf.group_head()) == 0:  # only ONE UN-NAMED group
+            (g_cat, df) = g_dict.popitem()
+        else:
+            df = pd.concat(g_dict, axis=0, names=self.emf.group_head(), sort=False)
+        return df
+
     def attribute_grade_count(self, a, groupby=None):
         """Collect table of ordinal grades for ONE attribute,
         for each (group, participant), optionally sub-divided by situation
         :param a: ONE selected attribute key
         :param groupby: (optional) single situation dimension or list of such dimensions
             for which separate attribute-counts are calculated.
             Counts are summed across any OTHER situation dimensions.
@@ -622,21 +702,25 @@
         # ------------------------------------------------------------
 
         if groupby is None:
             groupby = []
         elif isinstance(groupby, str):
             groupby = [groupby]
         groupby = [gb for gb in groupby if gb in self.emf.situation_dtypes.keys()]
-        g_dict = {self.group_id(g_key): pd.concat({s: s_count(s_data, a, groupby)
-                                                   for (s, s_data) in g_data.items()},
-                                                  axis=0,
-                                                  sort=False,
-                                                  names=['Participant'])  # *** -> cls property ?
+        g_dict = {g_key: pd.concat({s: s_count(s_data, a, groupby)
+                                    for (s, s_data) in g_data.items()},
+                                   axis=0,
+                                   sort=False,
+                                   names=['Participant'])  # *** -> cls property ?
                   for (g_key, g_data) in self.groups.items()}
-        df = pd.concat(g_dict, axis=0, names=self.group_head(), sort=False)
+        # if len(g_dict) == 1 and len(self.emf.group_head()) == 0:  # only ONE UN-NAMED group
+        #     (g_cat, df) = g_dict.popitem()
+        # else:
+        #     df = pd.concat(g_dict, axis=0, names=self.emf.group_head(), sort=False)
+        df = self._join_group_dict(g_dict)
         return Table(df.unstack(a))
 
     def attribute_grade_mean(self, a=None, groupby=None):
         """Average raw attribute grades, encoded numerically as (1,.., n_grades)
         :param a: (optional) attribute label or sequence of attribute,
             if None, include all attributes
         :param groupby: (optional) single situation dimension or iterable of such keys
@@ -678,21 +762,25 @@
             a = [a]
         a = [a_i for a_i in a if a_i in self.emf.attribute_dtypes.keys()]
         if groupby is None:
             groupby = []
         elif isinstance(groupby, str):
             groupby = [groupby]
         groupby = [gb for gb in groupby if gb in self.emf.situation_dtypes.keys()]
-        g_dict = {self.group_id(g_key): pd.concat({s: s_mean(s_data, a, groupby)
-                                                   for (s, s_data) in g_data.items()},
-                                                  axis=0,
-                                                  sort=False,
-                                                  names=['Participant'])  # *** -> cls property ?
+        g_dict = {g_key: pd.concat({s: s_mean(s_data, a, groupby)
+                                    for (s, s_data) in g_data.items()},
+                                   axis=0,
+                                   sort=False,
+                                   names=['Participant'])  # *** -> cls property ?
                   for (g_key, g_data) in self.groups.items()}
-        df = pd.concat(g_dict, axis=0, names=self.group_head(), sort=False)
+        # if len(g_dict) == 1 and len(self.emf.group_head()) == 0:  # only ONE UN-NAMED group
+        #     (g_cat, df) = g_dict.popitem()
+        # else:
+        #     df = pd.concat(g_dict, axis=0, names=self.emf.group_head(), sort=False)
+        df = self._join_group_dict(g_dict)
         return Table(df)
 
     def nap_table(self, sit, nap_cat=None, a=None, groupby=None, p=0.95):
         """Calculate proportion of Non-overlapping Pairs = NAP result
         in ONE situation dimension with EXACTLY TWO categories, X and Y,
         = estimate of P(attribute grade in X < attribute grade in Y),
         given observed ordinal i.i.d. grade samples for attribute in situation_dtypes X and Y.
@@ -717,124 +805,103 @@
              if a_i in self.emf.attribute_dtypes.keys()]
         if groupby is None:
             groupby = []
         elif isinstance(groupby, str):
             groupby = [groupby]
         groupby = [gb for gb in groupby if gb in self.emf.situation_dtypes.keys()]
         df = self.join_df()
-        g_cols = list(set([g[0] for g_tuple in self.groups.keys() for g in g_tuple]))
+        g_cols = list(self.emf.group_dtypes.keys())
         if len(g_cols) == 1 and len(g_cols[0]) == 0:
             g_cols = []
         groupby = g_cols + ['Participant'] + groupby
         return Table(nap_pandas(df, col=sit, nap_cat=nap_cat,
                                 group_cols=groupby, grade_cols=a, p=p))
 
 
 # -------------------------------------------- module help functions
 
-def _dir_name(g, sep='_'):  # ***
+def group_dir_str(g_head, g, sep='_'):
     """Convert group id to a directory path string
-    :param g: string or tuple of strings
+    :param g_head: tuple of strings with group "dimensions"
+    :param g: tuple of labels with corresponding group categories
+    :param sep: string joining group dimension and category
     :return: string to be used as directory path
     """
-    if type(g) is tuple:  # one or more (g_factor, g_cat) tuples
-        g = sep.join(_dir_name(g_s, sep='_')
-                     for g_s in g)
-    return g
+    s = '/'.join((str(h_i) + sep + str(g_i)
+                     for (h_i, g_i) in zip(g_head, g)))
+    if s == sep:  # only a single group with empty head and category
+        return ''
+    else:
+        return s
 
 
-def _groups(group_factors):
-    """Generate group labels from group_factors tree
-    :param group_factors: dict or iterable with elements (group_factor, category_list),
-    :return: generator of all combinations of (gf, gf_category) pairs from each group factor
-        Generated pairs are sorted as in group_factors
+def _gen_group_file_paths(path, fmt, group_factors, sep='_'):
+    """Generator of group categories and corresponding file Paths, recursively, for all groups
+    :param path: Path instance defining top directory to be searched
+    :param fmt: file suffix of desired files, INCL leading '.'
+    :param group_factors: dict with tuples (g_factor, list of categories)
+    :param sep: (optional) separator string between group dimension and category in file path
+    :return: generator of tuples (group_key, file_path), where
+        group_key is a dict with elements (g_key, g_cat), for all g_key in group_factors,
+        file_path is a Path object to a file that may hold EMA data for the group,
+        Only paths with matching group sub-strings AND desired file format are included.
     """
-    if len(group_factors) == 0:  # NO grouping
-        return [tuple()]  # ONE empty group label
+    if fmt is None:
+        path_gen = path.glob('**/*.*')  # try all files in all subdirectories
     else:
-        return product(*(product([gf], gf_cats)
-                         for (gf, gf_cats) in group_factors.items())
-                       )
+        path_gen = path.glob('**/*' + fmt)  # try only requested file format
+    for p in path_gen:
+        group_key = _match_group_factors(p, group_factors, sep)
+        # = empty dict if group_factors is empty dict -> OK file
+        # = None if group_factors is non-empty, but NOT ALL matched in p
+        if group_key is not None:
+            yield (group_key, p)
 
 
-def _gen_group_file_paths(path, fmt, group_factors, g_tuple=()):
-    """Generator of group keys and corresponding file Paths, recursively, for all groups
-    :param path: Path instance defining top directory to be searched
-    :param fmt: file suffix of desired files
-    :param group_factors: list of tuples (g_factor, labels)
-    :param g_tuple: list of tuples (g_factor, factor_label),
-        defining a combined group label or a beginning of a complete such label
-    :return: generator of tuples (group_key, file_path), where
-        group_key is an element of emf.groups,
-        file_path is a Path object to a file that may hold count data for the group.
+def _match_group_factors(p, group_factors, sep='_'):
     """
-    # exclude files like .xxx and require exact suffix match ************
-    def file_ok(f):
-        """Check if file is acceptable
-        :param f: file path
-        :return: True if acceptable
-        """
-        if fmt is None:
-            return f.stem[0] != '.'
+    :param p: path to be checked
+    :param group_factors: dict with elements (g_key, g_cats),
+        where g_cats is a list of allowed categories fpr group dimension g_key
+    :param sep: (optional) separator string between group dimension and category in file path
+    :return: g_cats = dict with elements (g_key, g_cat), for all g_key in group_factors,
+        IFF all matching patterns, e.g., 'Age_old' for g_key='Age', g_cat = 'old'
+        were found in p.
+        Otherwise, None, if not all group_factors were matched.
+    """
+    def find_in_string(s, k, cats):
+        for c in cats:
+            if 0 <= s.find(str(k) + sep + str(c)):
+                return c
+        return None
+
+    # -------------------------------------------------
+    g_keys = dict()
+    for (g_key, g_cats) in group_factors.items():
+        g_cat = find_in_string(str(p), g_key, g_cats)
+        if g_cat is None:
+            return None
         else:
-            return fmt == f.suffix[1:] and f.stem[0] != '.'
-    # ----------------------------------------------------
-
-    for f in path.iterdir():
-        if len(group_factors) == 0:  # now at lowest grouping level in directory tree
-            if f.is_file():  # include all files here and in sub-directories
-                if file_ok(f):  # fmt in f.suffix:
-                    # print(f'Reading file {f}')
-                    yield g_tuple, f
-            elif f.is_dir():  # just search sub-tree recursively
-                yield from _gen_group_file_paths(f, fmt,
-                                                 group_factors,
-                                                 g_tuple)
-        else:  # len(grouping) >=1
-            g_factor_key = group_factors[0][0]
-            for g_cat in group_factors[0][1]:
-                factor_cat = (g_factor_key, g_cat)
-                # = new tuple to be included in final group label
-                if f.is_dir():
-                    # if f.name.find(g_cat) == 0:
-                    if (f.name.find(g_factor_key) == 0
-                            and f.name.find(g_cat) == len(g_factor_key) + 1):
-                        # iterate recursively in sub-directory
-                        yield from _gen_group_file_paths(f, fmt,
-                                                         group_factors[1:],
-                                                         (*g_tuple, factor_cat))
-                elif f.is_file() and len(group_factors) == 1:
-                    # at final sub-directory level, also accept group category in file name:
-                    if (g_factor_key in f.name) and (g_cat in f.name) and file_ok(f):  # fmt in f.suffix:
-                        # print(f'Reading file {f}')
-                        yield (*g_tuple, factor_cat), f
+            g_keys[g_key] = g_cat
+    return g_keys
 
 
 def _table_valid(ema: pd.DataFrame):
     """Count valid data elements for all columns
     :param ema: Pandas.DataFrame instance with input EMA data
     :return: table string for logger output
     """
     return pd.DataFrame([ema.count()]).to_string(index=False)
 
 
-def _table_missing(ema: pd.DataFrame):  # *** needed ?
-    """make logger warning
-    :param ema: Pandas.DataFrame instance with input EMA data
-    :return: string for logger output
-    """
-    missing = pd.DataFrame({key: [sum(val.isna())]
-                            for key, val in ema.iteritems()})
-    return missing.to_string(index=False)
-
-
 def _check_ratings(a, a_count):
     """Warning about zero rating counts in some categories
     :param a: attribute key
     :param a_count: pd.DataFrame with count distribution for this attribute
+        one row for each (group, participant), summed across Situations
     :return: None
     """
     max_zero = 0.5  # proportion of all participants
     n_rows = a_count.shape[0]
     zero_participants = np.sum(a_count.to_numpy() == 0, axis=0)
     if np.any(zero_participants == n_rows):
         logger.warning(f'Attribute {a}: Some grades unused by ALL participants! '
@@ -880,42 +947,135 @@
                                                 'Hard',
                                                 'Easy',
                                                 'Very Easy',
                                                 'Perfect'],
                                      'Comfort': ['Bad',
                                                  'Not Good',
                                                  'Not Bad',
-                                                 'Good']})
+                                                 'Good']},
+                         groups={'Age': ('young', 'old'),
+                                 # 'Gender': ('M', 'F'),
+                                 }
+                         )
 
     print('emf=\n', emf)
     print(f'emf.n_phases= {emf.n_phases}')
     print(f'emf.situation_shape= {emf.situation_shape}')
     print(f'emf.rating_shape= {emf.rating_shape}')
 
-    # group_factors = {'Age': ['young', 'old'],
-    #                  'Gender': ['male', 'female'],
-    #                  'ORCA': ['AR_64']}
-    grouping = {'Age': ('old',),  # analyze only Age=old
-                }
-    # grouping={'Age': ('young','old')},  # analyze both Age groups separately
-    for (g, g_path) in _gen_group_file_paths(data_path, 'csv', [*grouping.items()]):
-        print('g= ', g, ': g_path= ', g_path)
-
     ds = EmaDataSet.load(emf, data_path, fmt='csv',
-                         grouping=grouping,
                          participant='file',
-                         dtype={'CoSS': 'string'},
-                         # converters={'CoSS': lambda c: str(c)}
-                         )
+                         path_groups=['Age', 'Gender'],
+                         dtype={'CoSS': 'string'})
     print('ds= ', ds)
 
+    test = ds.attribute_grade_count(a='Speech', groupby=('HA', 'CoSS'))
+    test.to_string(work_path / 'test_attribute_count.txt')
+    print('rating_count=\n', test)
+
     test = ds.attribute_grade_mean(groupby=('HA', 'CoSS'))
-    test.to_string(work_path / 'test_attribute_table.txt')
+    test.to_string(work_path / 'test_attribute_mean.txt')
     print('mean_rating=\n', test)
 
     nap = ds.nap_table(sit='HA', groupby=('CoSS',))
     nap.to_string(work_path / 'test_nap_table.txt', float_format='%.3f')
-    # nap.to_latex(work_path / 'test_nap_table.tex', float_format='%.2f')
-    # Styler(nap, precision=3).to_latex(work_path / 'test_nap_table.txt')
     print('NAP(HA B > A)=\n', nap)
 
-    # ***** TEST Empty situation_dtypes or Empty attribute_grades ***********
+    # -------------------- test EmaDataSet.save
+    test_path = work_path / 'test_save'
+    ds.save(test_path, fmt='csv', participant='file', join_groups=False, group_join_str='_')
+    print(f'Data set saved in {test_path}')
+
+    # -------------------------------------TEST zero group dimensions
+    emf = EmaFrame.setup(situations=sim_situations,
+                         phase_key='Phase',
+                         attributes={'Speech': ['Very Hard',
+                                                'Hard',
+                                                'Easy',
+                                                'Very Easy',
+                                                'Perfect'],
+                                     'Comfort': ['Bad',
+                                                 'Not Good',
+                                                 'Not Bad',
+                                                 'Good']},
+                         # groups={'Age': ('young', 'old'),
+                         #         # 'Gender': ('M', 'F'),
+                         #         }
+                         )
+
+    ds = EmaDataSet.load(emf, data_path, fmt='csv',
+                         participant='file',
+                         # path_groups=['Age', 'Gender'],
+                         dtype={'CoSS': 'string'})
+    print('ds= ', ds)
+    test_path = work_path / 'test_save_nogroup'
+    ds.save(test_path, fmt='csv', participant='TP', join_groups=True, group_join_str='_')
+    print(f'Data set saved in {test_path}')
+
+    # -------------------------------------TEST ONE group with ONE category
+    emf = EmaFrame.setup(situations=sim_situations,
+                         phase_key='Phase',
+                         attributes={'Speech': ['Very Hard',
+                                                'Hard',
+                                                'Easy',
+                                                'Very Easy',
+                                                'Perfect'],
+                                     'Comfort': ['Bad',
+                                                 'Not Good',
+                                                 'Not Bad',
+                                                 'Good']},
+                         groups={'Age': ['young'],  # *** ONE group, named
+                                 # 'Gender': ('M', 'F'),
+                                 }
+                         )
+
+    ds = EmaDataSet.load(emf, data_path, fmt='csv',
+                         participant='file',
+                         path_groups=['Age'],
+                         dtype={'CoSS': 'string'})
+    print('ds= ', ds)
+    test_path = work_path / 'test_save_onegroup'
+    ds.save(test_path, fmt='csv', participant='TP', join_groups=True, group_join_str='_')
+    print(f'Data set saved in {test_path}')
+
+    # -------------------------------------TEST ONE group with NO situation keys
+    print('\n*** Test one group with no sitution keys')
+    emf = EmaFrame.setup(#  situations=sim_situations,
+                         #  phase_key='Phase',
+                         attributes={'Speech': ['Very Hard',
+                                                'Hard',
+                                                'Easy',
+                                                'Very Easy',
+                                                'Perfect'],
+                                     'Comfort': ['Bad',
+                                                 'Not Good',
+                                                 'Not Bad',
+                                                 'Good']},
+                         groups={'Age': ['young'],  # *** ONE group, named
+                                 # 'Gender': ('M', 'F'),
+                                 }
+                         )
+
+    ds = EmaDataSet.load(emf, data_path, fmt='csv',
+                         participant='file',
+                         path_groups=['Age'],
+                         dtype={'CoSS': 'string'})
+    print('ds= ', ds)
+    test_path = work_path / 'test_save_no_Sit'
+    ds.save(test_path, fmt='csv', participant='TP', join_groups=True, group_join_str='_')
+    print(f'Data set saved in {test_path}')
+
+    # -------------------------------------- TEST Empty attribute_grades
+    print('\n*** Test one group, empty Attributes')
+    emf = EmaFrame.setup(situations=sim_situations,
+                         phase_key='Phase',
+                         groups={'Age': ['young'],  # *** ONE group, named
+                                 # 'Gender': ('M', 'F'),
+                                 }
+                         )
+    ds = EmaDataSet.load(emf, data_path, fmt='csv',
+                         participant='file',
+                         path_groups=['Age'])
+    print('ds= ', ds)
+    test_path = work_path / 'test_save_no_Attr'
+    ds.save(test_path, fmt='csv', participant='TP', join_groups=True, group_join_str='_')
+    print(f'Data set saved in {test_path}')
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_display.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_display.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,21 @@
 result_path / group / 'random_individual' / attributes / ....
 result_path / group / 'random_individual' / situations / ....
 result_path / group / 'participants' / participant_id / attributes / ....
 result_path / group / 'participants' / participant_id / situations / ....
 result_path / 'group_effects' / 'population_mean' / attributes / ...  (if more than one group)
 
 *** Version History:
+* Version 1.0.0:
+2023-04-29, AttributeProfile, SituationProfile work-around for Pandas groupby sort bug, reported,
+            to be fixed in Pandas v. 2.0.2 or 2.1 ?
+2023-04-22, adapted to simplified group-key representation in ema_data classes
+
 * Version 0.9.6:
-2023-04-13, code cleanup, SituationProfile, AttributeProfile, SituationDiff, AttributeDiff
+2023-04-13, code cleanup: SituationProfile, AttributeProfile, SituationDiff, AttributeDiff
             using Pandas access to model results via new ema_base methods
 2023-03-29, include percentile plots and tables in SituationDiff and AttributeDiff objects
 
 * Version 0.9.5:
 2023-03-07, include observed and model-estimated grade-count profiles,
             as requested by one reviewer for the Frontiers (2023) paper.
 2023-02-27, allow user to set n_samples for population-model display calculations
@@ -91,24 +96,26 @@
 * Version 0.5.1
 2021-11-27, allow NO Attributes in model, check display requests, minor cleanup
 
 * Version 0.5
 2021-11-05, copied from PairedCompCalc, modified for EmaCalc
 2021-11-09, first functional version
 """
+# ***** check if Pandas v >= 2.0.2 solved problem with groupby.quantiles sort bug
 # ***** local superclass for pretty-printed repr() ?
 # ***** allow several Attributes in single plot ?
 
 import numpy as np
 from pathlib import Path
 import logging
 import string
 import pandas as pd
 
 from . import ema_display_format as fmt
+from .ema_data import group_dir_str
 
 from samppy import credibility_pd as cred_pd
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
 # ---------------------------- Default display parameters
@@ -124,14 +131,15 @@
        'participants': False,   # show results for each respondent
        'scale_unit': '',  # scale unit for attribute plot axis
        'sit_probability': 'Situation Probability',  # label in figs and tables
        'credibility': 'Credibility',  # heading in difference table
        'population_mean_dir': 'population_mean',  # directory name
        'random_individual_dir': 'random_individual',  # directory name
        'participants_dir': 'participants',  # directory name
+       'group_join_str': '_',   # between group dimension and category in path string
        'group_effects_dir': 'group_effects',  # directory name
        'n_samples': 1000,  # number of samples for percentile calculations
        }
 
 DEFAULT_FIGURE_FORMAT = 'pdf'
 DEFAULT_TABLE_FORMAT = 'txt'
 
@@ -217,21 +225,23 @@
     of selected predictive situation and attribute results
     from one ema_model.EmaModel instance learned from one ema_data.EmaDataSet instance.
 
     All display elements can be saved as files in a selected directory three.
     The complete instance can also be serialized and dumped to a pickle file,
     then re-loaded, edited, and re-saved, if user needs to modify some display element(s).
     """
-    def __init__(self, groups, group_effects=None):
+    def __init__(self, group_head, groups, group_effects=None):
         """
+        :param group_head: tuple group dimension labels, copied form EmaFrame instance
         :param groups: dict with (group_id, GroupDisplaySet) elements
         :param group_effects: (optional) single GroupEffectSet instance,
             showing jointly credible differences between groups,
             IFF there is more than one group
         """
+        self.group_head = group_head  # copy from EmaModel.emf.group_head()
         self.groups = groups
         self.group_effects = group_effects
 
     def __repr__(self):  # *** general superclass for repr?
         return (self.__class__.__name__ + '(' +
                 '\n\t'.join(f'{k}= {repr(v)},'
                             for (k, v) in self.__dict__.items()) +
@@ -242,15 +252,16 @@
         :param dir_top: Path or string with top directory for all displays
         :param kwargs: (optional) dict with any additional format parameters, e.g.,
             figure_format, table_format, and any Pandas file-writer parameters.
         :return: None
         """
         dir_top = Path(dir_top)
         for (g, g_display) in self.groups.items():
-            g = _dir_name(g, sep='/')
+            # g = _dir_name(self.group_head, g, sep='/')
+            g = group_dir_str(self.group_head, g, sep=FMT['group_join_str'])
             if len(g) == 0 or all(s in string.whitespace for s in g):
                 g_display.save(dir_top, **kwargs)
             else:
                 g_display.save(dir_top / g, **kwargs)
         if self.group_effects is not None:
             self.group_effects.save(dir_top / FMT['group_effects_dir'], **kwargs)
 
@@ -309,24 +320,25 @@
             grade_counts = [(gc,) if isinstance(gc, str) else gc
                             for gc in grade_counts]
         set_format_param(situations=situations,
                          attributes=attributes,
                          grade_counts=grade_counts,
                          **kwargs)
         # display separate results for each group
+        group_head = emm.base.emf.group_head()
         groups = {g: GroupDisplaySet.display(emm_g)
                   for (g, emm_g) in emm.groups.items()}
 
         if len(groups) > 1:
             group_effects = GroupEffectSet.display(emm)
         else:
             group_effects = None
         logger.info(fig_comments())
         logger.info(table_comments())
-        return cls(groups, group_effects)
+        return cls(group_head, groups, group_effects)
 
 
 class GroupDisplaySet:
     """Container for all quality displays related to ONE study group:
     Predictive results for the population from which the participants were recruited,
     and for each individual participant, if requested by user.
     """
@@ -350,15 +362,15 @@
     def __repr__(self):
         return (self.__class__.__name__ + '(' +
                 '\n\t'.join(f'{k}= {repr(v)},'
                             for (k, v) in self.__dict__.items()) +
                 '\n\t)')
 
     def save(self, path, **kwargs):
-        """Save all stored display objects in their corresponding sub-trees
+        """Save all stored display objects in their corresponding subdirectories
         """
         if self.population_mean is not None:
             self.population_mean.save(path / FMT['population_mean_dir'], **kwargs)
         if self.random_individual is not None:
             self.random_individual.save(path / FMT['random_individual_dir'], **kwargs)
         if self.participants is not None:
             for (s, s_disp) in self.participants.items():
@@ -476,15 +488,17 @@
                 # df_obs is a Series object, make it a DataFrame with one row
                 df_obs = df_obs.to_frame().T
                 df_q = df_mod.quantile(q, numeric_only=True)
                 fill_value = df_obs.index.values[0]
                 i = ((fill_value, q) for q in df_q.index.values)
                 df_q = df_q.set_index(keys=i)
             else:
-                df_q = df_mod.groupby(sit_case).quantile(q, numeric_only=True)
+                df_q = df_mod.groupby(sit_case,
+                                      sort=False, group_keys=True).quantile(q,
+                                                                            numeric_only=True)
             return Profile(plot=fmt.fig_category_barplot(df=df_obs, df_q=df_q,
                                                          x_label=a + ': Ordinal Grades',
                                                          y_label='EMA counts',
                                                          file_label=a)
                            )
         # ------------------------------------------
 
@@ -506,21 +520,22 @@
         """Generate a probability-profile display for selected distribution and factor
         :param xi: 2D array of parameter-vector samples drawn from m_xi
         :param m_xi: a population or individual model instance
         :param sit_keys: tuple of one or more key(s) selected from emf.situation_dtypes.keys()
         :return: single cls instance showing CONDITIONAL probabilities
             for sit_keys[0], GIVEN each combination (j1,..., jD) for sit_keys[1], ...
         """
-        quantiles = np.array(FMT['percentiles']) / 100.
         u_ds = m_xi.base.situation_prob_df(xi, groupby=sit_keys)
         # = pd.Series object with MultiIndex axes [sample, *sit_keys]
-        q_ds = u_ds.groupby(level=list(sit_keys),
-                            sort=False).quantile(quantiles,
-                                                 numeric_only=True)
-        # = pd.Series object with MultiIndex axes [*sit_keys, quantiles]
+        # quantiles = np.array(FMT['percentiles']) / 100.
+        # q_ds = u_ds.groupby(level=list(sit_keys),
+        #                     sort=False, group_keys=True).quantile(quantiles,
+        #                                                           numeric_only=True)
+        # # = pd.Series object with MultiIndex axes [*sit_keys, quantiles]
+        q_ds = _series_quantile_fix(u_ds, sit_keys)  # *** TEMP fix for Pandas bug
         tab_perc = fmt.tab_percentiles(q_ds)
         fig_perc = fmt.fig_percentiles(tab_perc, y_label=FMT['sit_probability'], file_label='', y_min=0.)
         # ---------------------------------------- sit_keys differences
         # NOTE: Comparing CONDITIONAL probabilities of categories in FIRST sit_keys dimension,
         # GIVEN categories in other dimensions.
         d_pd = cred_pd.cred_diff(u_ds, diff_axis=sit_keys[0], case_axis=sit_keys[1:], p_lim=FMT['credibility_limit'])
         tab_diff = fmt.tab_credible_diff(d_pd, diff_head=sit_keys[0:1], cred_head=FMT['credibility'],
@@ -553,16 +568,26 @@
             tau = np.median(m_xi.base.attribute_tau(xi, a), axis=0)
             # tau[l] = l-th median rating threshold for attribute a, SAME for all situations
         else:
             tau = None
         # --------------------------------------- percentile table:
         theta_ds =  m_xi.base.attribute_theta_df(xi, a, groupby=sit_keys)
         # = pd.Series with MultiIndex [samples, *sit_keys]
-        quantiles = np.array(FMT['percentiles']) / 100.
-        theta_q = theta_ds.groupby(level=sit_keys, sort=False).quantile(quantiles)
+        # ***** with UN-sorted sit_keys
+        # quantiles = np.array(FMT['percentiles']) / 100.
+        # if len(sit_keys) > 1:
+        #     theta_q = theta_ds.groupby(level=sit_keys,
+        #                                sort=False, group_keys=True).quantile(quantiles)
+        # # *** with SORTED index.levels for sit_key if only one dimension. Pandas v 2.0.0, 2.0.1
+        # # *** UN-sorted index.levels, if sit_keys is more than one level ***
+        # else:  # *** work-around for Pandas bugg ***
+        #     theta_q = pd.concat({s: q.quantile(quantiles)
+        #                          for (s, q) in theta_ds.groupby(level=sit_keys, sort=False)},
+        #                         names=list(sit_keys))
+        theta_q = _series_quantile_fix(theta_ds, sit_keys)  # *** TEMP fix for Pandas bug
         tab_perc = fmt.tab_percentiles(theta_q, file_label=a)
         fig_perc = fmt.fig_percentiles(tab_perc, y_label=a + ' (' + str(FMT['scale_unit']) + ')',
                                        file_label=a,
                                        cat_limits=tau)
         # ---------------------------------------- attr differences
         # NOTE: comparing all situation-categories, in all requested sit_keys dimensions
         d_pd = cred_pd.cred_diff(theta_ds, diff_axis=sit_keys, p_lim=FMT['credibility_limit'])
@@ -666,26 +691,24 @@
         :param xi: list of 2D arrays of parameter-vector samples
             len(xi) == len(emm.groups)
         :param emm: ema_model.EmaModel object
         :param sit_keys: tuple of one or more key(s) selected from emf.situation_dtypes.keys()
         :return: single cls instance
         """
         # --------------------------------- situation prob. vs (sit_keys, groups):
-        group_head = [tuple(gk[0] for gk in g_key)
-                      for g_key in emm.groups][0] # [0] all same
-        group_cat = [tuple(gk[1] for gk in g_key)
-                     for g_key in emm.groups]
+        group_head = emm.base.emf.group_head()  # ********************
+        group_cat = list(emm.groups.keys())
         u_groups = {g: emm.base.situation_prob_df(xi_g, groupby=sit_keys)
                     for (g, xi_g) in zip(group_cat, xi)}
         # = dict of pd.Series objects, each with MultiIndex [sample, *sit_keys]
         u_ds = pd.concat(u_groups, axis=0, names=list(group_head))
         quantiles = np.array(FMT['percentiles']) / 100.
         u_q = u_ds.groupby(level=list(sit_keys) + list(group_head),
-                           sort=False).quantile(quantiles,
-                                                numeric_only=True)
+                           sort=False, group_keys=True).quantile(quantiles,
+                                                                 numeric_only=True)
         # = pd.Series with MultiIndex [*sit_keys, quantiles]
         tab_perc = fmt.tab_percentiles(u_q)
         fig_perc = fmt.fig_percentiles(tab_perc, y_label=FMT['sit_probability'], file_label='', y_min=0.)
         # ---------------------------------------- group differences by sit_keys
         # NOTE: Comparing CONDITIONAL probabilities of categories in FIRST sit_keys dimension,
         # GIVEN categories in other dimensions.
         d_pd = cred_pd.cred_group_diff(u_groups, group_axis=group_head,
@@ -717,25 +740,23 @@
             tau = tau.reshape((-1, tau.shape[-1]))
             # tau[gs, :] = gs-th sample across all groups
             tau = np.median(tau, axis=0)
             # tau[l] = l-th median rating threshold for attribute a
         else:
             tau = None
         # --------------------------------------- percentile table
-        group_head = [tuple(gk[0] for gk in g_key)
-                      for g_key in emm.groups][0]  # [0] all same
-        group_cat = [tuple(gk[1] for gk in g_key)
-                     for g_key in emm.groups]
+        group_head = emm.base.emf.group_head()
+        group_cat = list(emm.groups.keys())
         theta_groups = {g: emm.base.attribute_theta_df(xi_g, a, groupby=sit_keys)
                         for (g, xi_g) in zip(group_cat, xi)}
         theta_ds = pd.concat(theta_groups, axis=0, names=list(group_head))
         quantiles = np.array(FMT['percentiles']) / 100.
         theta_q = theta_ds.groupby(level=list(sit_keys) + list(group_head),
-                                    sort=False).quantile(quantiles,
-                                                         numeric_only=True)
+                                   sort=False, group_keys=True).quantile(quantiles,
+                                                                         numeric_only=True)
         tab_perc = fmt.tab_percentiles(theta_q, file_label=a)
         fig_perc = fmt.fig_percentiles(tab_perc, y_label=a + ' (' + str(FMT['scale_unit']) + ')', file_label=a,
                                        cat_limits=tau)
         # ---------------------------------------- attribute differences between groups
         # NOTE: comparing all situation-categories, in all requested sc dimensions
         d_pd = cred_pd.cred_group_diff(theta_groups,
                                        group_axis=group_head,
@@ -745,23 +766,32 @@
                                          cred_head=FMT['credibility'],
                                          case_head=sit_keys,
                                          y_label=a, file_label=a)
         return cls(plot=fig_perc, tab=tab_perc, diff=tab_diff)
 
 
 # ---------------------------------- Help functions:
-def _dir_name(g, sep='_'):
-    """make sure group name is a possible directory name
-    :param g: string or tuple of strings
-    :return: string to be used as directory
-    """
-    if type(g) is tuple:  # several strings
-        g = sep.join(_dir_name(g_s, sep='_')
-                     for g_s in g)
-    return g
+
+def _series_quantile_fix(ds, sit_keys):  # *** Not needed after bug fix in Pandas >= 2.0.2 ?
+    """Work-around for possible Pandas bug in groupby with sort=False
+    :param ds: pandas.Series instance with Multi-index [_sample, *sit_keys]
+    :param sit_keys: tuple with one or more index levels in ds
+    :return: series with Multi-Index levels [*sit_keys, quantiles]
+    """
+    quantiles = np.array(FMT['percentiles']) / 100.
+    if len(sit_keys) > 1:
+        q = ds.groupby(level=sit_keys,
+                                   sort=False, group_keys=True).quantile(quantiles)
+    # *** -> SORTED index.levels for sit_key if only one dimension. Pandas v 2.0.0, 2.0.1
+    # *** -> OK UN-sorted index.levels, if sit_keys is more than one level ***
+    else:  # *** work-around for Pandas bugg ***
+        q = pd.concat({s: q.quantile(quantiles)
+                       for (s, q) in ds.groupby(level=sit_keys, sort=False)},
+                      names=list(sit_keys))
+    return q
 
 
 def fig_comments():
     """Generate figure explanations.
     :return: comment string
     """
     p_min = np.amin(FMT['percentiles'])
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_display_format.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_display_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 1: specifying matplotlib style sheet(s) by keyword argument mpl_style
 2: setting specific matplotlib parameters at runtime by keyword argument mpl_params
 3: setting specific parameters in FMT, e.g., 'colors' and 'markers'
 
 *** Version History:
 * Version 0.9.6:
 2023-04-16, some plot parameters -> FMT for user control
-2023-04-12, new simplified tab_percentle_pd, tab_credible_difference_pd
+2023-04-12, new simplified tab_percentles, tab_credible_diff
 2023-03-31, new help function make_product_name *** NO LONGER NEEDED
 
 * Version 0.9.5:
 2023-03-07, fig_category_barplot allow both observed and model-predicted quantile data
 
 * Version 0.9.4:
 2023-01-22, Bug fix in output file name creation, to avoid problem under Windows.
@@ -59,16 +59,18 @@
 
 
 FMT = {'colors': 'rbgk',    # to distinguish results in plots, cyclic use
        'markers': 'oxs*_',  # corresponding markers, cyclic use
        'x_space': 0.3,      # clean space between x_tick categories
        'interaction_sep': '\u00D7',  # mult.sign. separating situation labels in result file names
        'condition_sep': '_',    # separating attribute and its conditioning situation(s) in file names
-       'max_plot_cases': 30,    # max cases in percentile plots
-       'max_case_heads': 2,     # limit in plot legends
+       'max_plot_cases': 50,    # max cases in percentile plots
+       'max_case_heads': 1,     # limit in plot legends
+       'and_head': ('', ''),    # two-level heading for diff-table first column
+       'and_label': 'and',      # logical and in diff-table first column
        }
 
 # NOTE: FMT['colors'] and FMT['markers'] override matplotlib.rcParams.axes.prop_cycle,
 #   because prop_cycle allows only equal lengths of 'colors' and 'markers'.
 #   The FMT['colors'] and FMT['markers'] are used cyclically,
 #   so the default sequences with unequal lengths will combine
 #   into a sequence with many combinations, before repeating itself.
@@ -204,15 +206,14 @@
     :param y_max: (optional) enforced upper limit of vertical axis
     :param kwargs: (optional) dict with any additional keyword arguments for plot commands.
     :return: ResultPlot instance with plot axis with all results
     NOTE: plot will use df.index.level[0] categories as x-axis labels,
     and index.level[1:] as plot labels in the legend
     """
     # ----------------------------------- set up plot design:
-    # x_space = FMT['x_space']
     if df is None:
         return None
     if df.index.nlevels == 1:
         x_label = df.index.name
         x_tick_labels = list(df.index.values)
         case_head = ()
         case_list = [()]
@@ -329,16 +330,16 @@
 
 
 def fig_category_barplot(df,
                          x_label,
                          y_label,
                          df_q=None,
                          file_label='',
-                         y_min=None,
-                         y_max=None,
+                         y_min=None,  # *** not needed, always = 0
+                         y_max=None,  # *** not needed, adaptive
                          mpl_params=None,  # *** not needed? called only from ema_display ***
                          **kwargs
                          ):
     """Bar plot of DataFrame values,
     to be displayed with one sequence of vertical bars along x-axis for each row,
     with one bar for each column,
     suitable, e.g., for plotting attribute_grade_counts
@@ -423,21 +424,21 @@
 
 def tab_credible_diff(diff,
                       diff_head,
                       cred_head,
                       case_head=(),
                       y_label='',
                       file_label='',
-                      and_label='and',  # label in And column  -> FMT ***
-                      and_head=('', '')  # -> FMT ***
+                      and_label=FMT['and_label'],
+                      and_head=FMT['and_head']   # ('', '')  # -> FMT ***
                       ):
     """Create table with credible differences among results -- pandas version
     :param diff: list of tuples (((i,j), c0,...), p),
         defining jointly credible differences, indicating that
-        prob{ quality of diff catgory i > quality of category j, given case category c
+        prob{ quality of diff category i > quality of category j, given case category c
         AND all previous pairs } == p
         i, j are either a string label or a tuple of such labels
         c0,... is one or more case labels
     :param diff_head: tuple of keys for heading of diff_labels column in table
         len(diff_head) == len(i) == len(j) if tuple, or len(diff_head) == 1
     :param cred_head: string for header of Credibility column
     :param case_head: (optional) tuple of case keys, one for each case-dimension table column
@@ -508,11 +509,11 @@
     """Select xtick properties to avoid tick-label clutter
     :param labels: list of tick label strings
     :return: dict with keyword arguments for set_xticklabels
     """
     maxL = max(len(l) for l in labels)
     rotate_x_label = maxL * len(labels) > 75  # ad hoc criterion
     if rotate_x_label:
-         style = dict(rotation=15, horizontalalignment='right')
+        style = dict(rotation=15, horizontalalignment='right')
     else:
         style = dict(rotation='horizontal', horizontalalignment='center')
     return style
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_file.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """This module defines functions that read / write EMA data and analysis result tables,
-from/to a table file of any kind that package pandas can handle.
+from/to a table file of any kind that package Pandas can handle.
 
-A single data file for READING may include EMA records from ONE or SEVERAL respondents.
+A single data file for READING may include EMA records from ONE or SEVERAL respondents,
+in ONE or SEVERAL respondent groups.
 The participant id may be stored in a designated column of the table,
 otherwise the file name can be used as participant id,
 or (in Excel-type file) the participant may be identified by the sheet name.
+The table may include grouping categories, and other data not used for EMA analysis.
 
 Regardless of the file storage format, even if an input file represents only ONE participant,
 the EMA data is always delivered by a generator function
-ema_gen, which is an iterable over tuples (participant_id, df), where
-participant_id is a string or any other object that can be used as dict key,
-df is a pandas.DataFrame instance.
+ema_gen, which is an iterable over pandas DataFrame instances.
 
 Some pandas file readers can also do some
 data conversions and/or type checking.
 Column names may be modified before the data are delivered to caller.
 
 For writing EMA data or any other table to a file,
 cast the DataFrame instance to subclass Table,
 and use Table(df).save(...) method.
-This always creates a separate file for each table.
 
 
 *** Version History:
+* Version 1.0.0:
+2023-04-20, simplified ema_gen(..): yield whole table as a single pd.DataFrame,
+            All data checking, and separation by group(s) and participant, is done externally.
+
 * Version 0.9.3:
 2022-07-22, changed 'subject' -> 'participant'
 2022-07-15, minor bugfix in ema_gen.separate
 
 * Version 0.9:
 2022-03-21, use pd.DataFrame as interface to all file formats
 
 * Version 0.8.3 and earlier: Handled only xlsx files.
 """
-import warnings
-
 import pandas as pd
 import logging
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
 
@@ -71,26 +72,28 @@
             write function for the specific file format.
         :return: None
         """
         if not allow_over_write:
             file_path = safe_file_path(file_path)
         suffix = file_path.suffix
         try:
+            # ******** file_path.parent.mkdir here? NO, done by container class
             if write_fcn is None:
                 if suffix in ['.xlsx', '.xls', '.odf', '.ods', '.odt']:
                     self.to_excel(file_path, sheet_name=file_path.stem, **file_kwargs)
                 elif suffix in ['.csv']:
                     self.to_csv(file_path, **file_kwargs)
                 elif suffix in ['.txt']:
                     self.to_string(file_path, **file_kwargs)
                 elif suffix in ['.tex']:
-                    with warnings.catch_warnings():
-                        # suppress Pandas FutureWarning about to_latex method
-                        warnings.simplefilter('ignore')
-                        self.to_latex(file_path, **file_kwargs)
+                    # with warnings.catch_warnings():
+                    #     # suppress Pandas FutureWarning about to_latex method
+                    #     warnings.simplefilter('ignore')
+                    #     self.to_latex(file_path, **file_kwargs)
+                    self.to_latex(file_path, **file_kwargs)
                 else:
                     raise FileWriteError(f'No DataFrame write method for file type {suffix}')
             else:
                 write_fcn(self, file_path, **file_kwargs)
         except Exception as e:
             raise FileWriteError(f'Could not write to {file_path}. Error: {e}')
 
@@ -98,74 +101,71 @@
 # ----------------------------------------- General File Reader:
 def ema_gen(file_path,
             participant=None,
             rename_cols=None,
             read_fcn=None,
             **file_kwargs
             ):
-    """Reader of data stored in a table-style file that can be read by Pandas.
+    """Reader of data stored in a table-style file that can be read by Pandas.read_xxx()
+    or user-supplied function with similar signature.
     Each file row is assumed to include fields for one EMA record, but may also include other data fields.
     :param file_path: Path to existing file for reading
     :param participant: (optional) 'sheet' or 'file' or column header for participant identification label
         None -> 'sheet', if Excel-type file, otherwise -> 'file'
-    :param rename_cols: (optional) dict with elements (old_name: new_name)
+    :param rename_cols: (optional) dict with elements (old_name: new_name) for table column(s)
     :param read_fcn: (optional) basic read function, e.g., pd.read_excel,
         or any user-supplied function with similar signature.
         If None, a default pandas function is determined by file_path.suffix.
     :param file_kwargs: any additional arguments for the
         read function for the specific file format
-    :return: generator object yielding tuples (participant_id, df), where
-        participant_id is a string or other object to be used as participant key,
-        df is a pd.DataFrame instance, with one row for each EMA record,
-    """
-    def separate(df, index_col):
-        """Generator of tuples (participant_id, data_frame)
-        using participant ids stored in a column
-        :param df: a pd.DataFrame instance
-        :param index_col: column index for separation
-        :return: generator of tuples (participant, self)
-        """
-        participant_set = set(df[index_col])
-        for s in participant_set:
-            yield s, df[(df[index_col] == s)].copy()  # COPY of df slice
-        # --------------------------------------------------------
-
+    :return: generator object yielding pd.DataFrame instance(s),
+        with one row for each EMA record,
+        and one column specifies participant id,
+        possibly copied from file name or sheet name if requested.
+    """
     if read_fcn is None:
         read_fcn = _default_reader(file_path)
     logger.debug(f'Reading from {file_path} with {read_fcn}')
     if participant == 'sheet':
         if read_fcn is pd.read_excel:
             if 'sheet_name' not in file_kwargs.keys():
                 file_kwargs['sheet_name'] = None
-                # because read_excel uses sheet_name=0 by default
+                # because pd.read_excel uses sheet_name=0 by default
         else:
             logger.warning(f'File type {file_path.suffix} has no "sheet"s. Using participant="file".')
             participant = 'file'
     try:
         df = read_fcn(file_path,
                       **file_kwargs)
     except Exception as e:
         raise FileReadError(f'{read_fcn.__name__}({file_path}) error: {e}')
     if type(df) is pd.DataFrame:
         if rename_cols is not None:
             df.rename(columns=rename_cols, inplace=True)
         if participant is None or participant == 'file':
-            yield file_path.stem, df
+            df['file'] = file_path.stem
+            yield df
+        elif participant in df.columns:
+            yield df
         else:
-            yield from separate(df, participant)
+            logger.debug(f'No column participant={participant} in this file')
     else:  # we have a dict of sheet DataFrames
-        for (sh, df_s) in df.items():
+        for (sheet_name, df_s) in df.items():
             if rename_cols is not None:
                 df_s.rename(columns=rename_cols, inplace=True)
             if participant is None or participant == 'sheet':
-                yield sh, df_s
+                df_s['sheet'] = sheet_name
+                yield df_s
             elif participant == 'file':
-                yield file_path.stem, df_s
+                df_s[participant] = file_path.stem
+                yield df_s
+            elif participant in df_s.columns:
+                yield df_s
             else:
-                yield from separate(df_s, participant)
+                logger.debug(f'Missing column participant={participant} in sheet {sheet_name} of this file')
 
 
 # ------------------------------------------ help functions:
 def safe_file_path(p):
     """Ensure previously non-existing file path, to avoid over-writing,
     by adding a sequence number to the path stem
     :param p: file path
@@ -201,23 +201,24 @@
 # ----------------------------------------- TEST:
 if __name__ == '__main__':
     from pathlib import Path
     import ema_logging
 
     work_path = Path.home() / 'Documents' / 'EMA_sim'  # or whatever...
     data_path = work_path / 'data_xlsx' / 'Age_old'  # to use simulation data generated by run_sim.py
+    # data_path = work_path / 'data' / 'Age_old'  # to use simulation data generated by run_sim.py
 
     ema_logging.setup()  # to save the log file
 
     ema_file = ema_gen(data_path / 'Pop0_S1.xlsx',
                        participant='sheet',
-                       dtype={'CoSS': pd.StringDtype()}
+                       dtype={'CoSS': pd.StringDtype()}  # ******** needed ?
                        )
-    for (s, ema) in ema_file:
-        print(f'participant {repr(s)}:')
+    # for (s, ema) in ema_file:
+    for ema in ema_file:
         print(ema.head(100))
         print('dtypes=\n', ema.dtypes)
         count = ema.value_counts(subset=['HA', 'CoSS'], sort=False)
         # ind = pd.MultiIndex.from_frame(ema[['HA', 'CoSS']])
         # c1 = count.reindex(index=ind, fill_value=0)
         print(count)
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_group.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module defines classes for a Bayesian probabilistic model of EMA data,
 for ONE group of respondents representing ONE population.
 
 *** Class Overview:
 
 EmaGroupModel: Container for individual response-probability models,
-    as implemented by an ema_respondent.EmaRespondentModel instance for each participant
+    implemented by an ema_respondent.EmaRespondentModel instance for each participant
     in ONE group of test participants, assumed recruited from ONE population.
     Also contains a PopulationModel instance representing the population
     from which the participants were recruited.
 
 PopulationModel: Defines a Gaussian Mixture Model (GMM)
     for the parameter distribution in ONE population,
     from which participants in ONE group were recruited.
@@ -16,14 +16,18 @@
 
 PredictivePopulationModel: marginal distribution of parameters
     in ONE population represented by ONE EmaGroupModel.
     Specifies a mixture of Student-t distributions,
     used for result displays.
 
 *** Version History:
+* Version 1.0.0:
+2023-05-17, EmaGroupModel.initialize(...,n_participants_per_comp,...) to set initial number of GMM components
+2023-05-15, logger.info participant GMM weights after pruning
+
 * Version 0.9.3:
 2022-07-27, changed 'subject' -> 'participant' or 'respondent'
 
 * Version 0.8.3:
 2022-03-07, changed class name GroupModel -> EmaGroupModel
 2022-03-07, changed class name ProfileMixtureModel -> PredictivePopulationModel
 2022-03-07, separate class for GMM: EmaGroupModel.pop_gmm = a PopulationModel instance
@@ -33,35 +37,35 @@
 2022-03-02, test prepare to allow multiprocesing Pool.imap
             allow multi-processing Pool in EmaGroupModel.adapt, parallel across subjects
 
 * Version 0.8.1
 2022-02-26, complete separate GMM for each group, GMM components -> EmaGroupModel property comp
 """
 # *** test multiprocessing start method fork? Does not work in windows ! *********
-# *** try using shared_memory or Ray to reduce multiprocessing overhead?
+# *** Future: try using shared_memory or Ray to reduce multiprocessing overhead?
 import copy
 import logging
 import os
 from multiprocessing.pool import Pool
 
 import numpy as np
 from scipy.special import logsumexp, softmax
-import pandas as pd
+# import pandas as pd
 
 from EmaCalc.dirichlet import DirichletVector
 from EmaCalc.dirichlet import JEFFREYS_CONC
 from EmaCalc.ema_respondent import EmaRespondentModel
 
 MixtureWeight = DirichletVector
 
 # -------------------------------------------------------------------
 __ModelVersion__ = "2022-03-08"
 
 PRIOR_MIXTURE_CONC = JEFFREYS_CONC
-# = prior conc for sub-population mixture weights.
+# = prior conc for population mixture weights.
 
 N_SAMPLES = 1000
 # = default number of parameter samples in PredictivePopulationModel.rvs() calculation
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
@@ -97,36 +101,37 @@
     def __repr__(self):
         return (self.__class__.__name__ + '(' +
                 f'\n\tparticipants= {len(self.participants)} individuals,' +
                 f'\n\tpop_gmm={repr(self.pop_gmm)})'
                 )
 
     @classmethod
-    def initialize(cls, max_n_comp, base, group_data, seed_seq, rng):
+    def initialize(cls, n_participants_per_comp, base, group_data, seed_seq, rng):
         """Crude initial group model given group EMA data
-        :param max_n_comp: integer number of GMM components
+        :param n_participants_per_comp: scalar integer = desired number of participants per GMM component
         :param base: single common EmaParamBase object, used by all model parts
         :param group_data: a dict with elements (s_id, s_ema), where
             s_id = a participant key,
             s_ema = a Pandas.DataFrame with EMA records from an ema_data.EmaDataSet object.
         :param seed_seq: SeedSequence object to spawn children for participants of this group
         :param rng: random Generator for this group, used by self.pop_gmm
         :return: a cls instance crudely initialized
         """
         participant_rng_list = [np.random.default_rng(s)
                                 for s in seed_seq.spawn(len(group_data))]
         s_models = {s_id: EmaRespondentModel.initialize(base, s_ema, s_rng, id=s_id)
                     for ((s_id, s_ema), s_rng) in zip(group_data.items(),
                                                       participant_rng_list)}
         n_participants = len(s_models)
-        if max_n_comp is None:
-            max_n_comp = n_participants // 2
-        else:
-            max_n_comp = min(n_participants // 2, max_n_comp)
-        pop_gmm = PopulationModel.initialize(max_n_comp, s_models, base, rng)
+        # if max_n_comp is None:
+        #     max_n_comp = n_participants // 2
+        # else:
+        #     max_n_comp = min(n_participants // 2, max_n_comp)
+        n_comp = max(1, n_participants // n_participants_per_comp)
+        pop_gmm = PopulationModel.initialize(n_comp, s_models, base, rng)
         return cls(base, s_models, pop_gmm)
 
     def adapt(self, g_name):
         """One VI adaptation step for all model parameters
         :param g_name: group id label for logger output
         :return: ll = scalar VI lower bound to data log-likelihood,
             incl. negative contributions for parameter KLdiv re priors
@@ -175,28 +180,36 @@
         """
         w_sum = np.sum([np.mean(self.pop_gmm.mean_conditional_zeta(s.xi), axis=-1)
                         for s in self.participants.values()],
                        axis=0, keepdims=False)
         # = sum of mean individual mixture weights, given xi
         logger.debug(f'{repr(g_name)}: Before pruning: w_sum = '
                      + np.array2string(w_sum, precision=2, suppress_small=True))
-        if np.any(np.logical_and(min_weight < w_sum, w_sum <= 1.5)):
-            logger.warning(f'{repr(g_name)}: *** Some component(s) with only ONE member.')
+        if np.any(np.logical_and(min_weight < w_sum, w_sum <= 2.5)):
+            logger.warning(f'Group {repr(g_name)}: *** Some GMM component(s) has TWO or LESS participants. '
+                           'Variance estimates may be unreliable. ***')
         keep = min_weight < w_sum
+        n_keep = np.sum(keep)
+        n_total = len(keep)
         self.pop_gmm.prune(keep)
-        logger.info(f'{repr(g_name)}: Model pruned to {np.sum(keep)} active mixture component(s) '
-                    + f'out of initially {len(keep)}')
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f'{repr(g_name)}.pop_gmm.mean_zeta=\n\t'
-                         + '\n\t'.join((s_name + ': '
-                                        + np.array_str(np.mean(self.pop_gmm.mean_conditional_zeta(s_model.xi),
-                                                               axis=-1),
-                                                       precision=2,
-                                                       suppress_small=True)
-                                        for (s_name, s_model) in self.participants.items())))
+        # --- make logger message:
+        msg = f'Group {repr(g_name)}:\t'
+        if n_keep < n_total:
+            msg += f'Model pruned to {n_keep} active mixture component(s) out of initially {n_total}'
+        else:
+            msg += f'All initial {n_total} mixture component(s) still active.'
+        if len(self.pop_gmm.comp) > 1:
+            msg += (f'\nParticipant GMM weights =\n\t'
+                    + '\n\t'.join((str(s_name) + ':\t'
+                                   + np.array_str(np.mean(self.pop_gmm.mean_conditional_zeta(s_model.xi),
+                                                          axis=-1),
+                                                  precision=2,
+                                                  suppress_small=True)
+                                   for (s_name, s_model) in self.participants.items())))
+        logger.info(msg)
 
     # ---------------------------- make final results for display:
     def predictive_population_ind(self):
         """Predictive probability-distribution for a Random Individual
         in the population represented by self
         :return: a PredictivePopulationModel object
         """
@@ -219,20 +232,14 @@
             Counts are summed across any OTHER situation dimensions.
         :return: a pd.DataFrame object with all grade counts,
             with one row for each (*groupby) combination
             and one column for each grade category
         """
         return sum((s_model.attribute_grade_count(a, groupby=groupby)
                     for s_model in self.participants.values()))
-        # df_list = []
-        # for (s_id, s_model) in self.participants.items():
-        #     df = s_model.attribute_grade_count(a, groupby=groupby)
-        #     df['Participant'] = s_id
-        #     df_list.append(df)
-        # return pd.concat(df_list)
 
     def rvs_grade_count(self, a, groupby=None):
         """Collect table of predicted grade counts for ONE attribute,
         summed across all participants, optionally subdivided by situation.
         :param a: selected attribute key
         :param groupby: (optional) single situation dimension or sequence of such keys
             for which separate attribute-counts are calculated.
@@ -272,28 +279,28 @@
     def __repr__(self):
         return (self.__class__.__name__ + '(' +
                 f'\n\tmix_weight={repr(self.mix_weight)},'
                 f'\n\tcomp= {len(self.comp)} mixture components)'
                 )
 
     @classmethod
-    def initialize(cls, max_n_comp, participants, base, rng):
+    def initialize(cls, n_comp, participants, base, rng):
         """Crude initial group model given group EMA data
-        :param max_n_comp: integer number of GMM components
+        :param n_comp: integer number of GMM components
         :param participants: list with EmaRespondentModel instances for group participants,
             only crudely initialized
         :param base: single common EmaParamBase object, used by all model parts
         :param rng: random Generator for this group
         :return: a cls instance crudely initialized
         """
-        mix_weight = MixtureWeight(alpha=np.ones(max_n_comp) * PRIOR_MIXTURE_CONC,
+        mix_weight = MixtureWeight(alpha=np.ones(n_comp) * PRIOR_MIXTURE_CONC,
                                    rng=rng)
         # -> equal mean weights for all mixture components
         comp = [copy.deepcopy(base.comp_prior)
-                for _ in range(max_n_comp)]
+                for _ in range(n_comp)]
         self = cls(base, mix_weight, comp, rng)
         self._init_comp(participants)
         # Mixture weights will be adapted later in the general VI procedure.
         return self
 
     def _init_comp(self, participants):
         """Initialize Gaussian mixture components to make them distinctly separated,
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_latent.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_latent.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         :return: log_p = array with log probabilities, element-wise
             log_p.shape == a.shape == b.shape
         """
         # **** Fix numerical divide by zero in log, asymmetric numerical sensitivity!
         # ***** problem when b = inf and a > 36.7  -> d == 0.
         # ***** No problem with b = -100. and a = -inf
         d = expit(b) - expit(a)
-        # *** this may be inaccurately == 0. for about 36.7. < a < b in double prec.
+        # *** this may be inaccurately == 0. if 36.7. < a < b in double prec.
         non_positive = d <= 0.
         if np.any(non_positive):
             d[non_positive] = expit(-a[non_positive]) - expit(-b[non_positive])  # using expit symmetry
         non_positive = np.logical_or(d <= 0., np.isnan(d))
         if np.any(non_positive):  # some other error
             logger.warning(f'Bradley.log_cdf_diff: {np.sum(non_positive)} non-positive probability values. '
                            + 'Should never happen!')
@@ -86,15 +86,15 @@
     def __repr__(self):
         return f'<class {self.__class__.__name__}>'
 
 
 class Thurstone:
     """Distribution of decision variable in the Thurstone Case V model.
     with distribution function
-    cdf(x) = Phi(x / sqrt(pi))
+    cdf(x) = Phi(x)
     NOTE: Thurstone.scale is now included in all calculations.
     This is different from corresponding MatLab code.
     """
     unit_label = 'd-prime unit'
 
     sqrt_2pi = np.sqrt(2. * np.pi)
     scale = 1.
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_logging.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_logging.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_model.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     and contains all individual response-probability models,
     implemented by an ema_respondent.EmaRespondentModel instance for each participant,
     in ONE group of test participants, assumed recruited from the SAME population.
 
 ema_respondent.EmaRespondentModel: Distribution of individual parameter vector
     assumed to determine the observed EMA data for ONE participant.
     Each EMA record specifies
-    (1) a nominal (possibly multi-dimensional) Situation category, and
+    (1) a nominal (possibly multidimensional) Situation category, and
     (2) ordinal Ratings for zero, one, or more subjective Attributes.
     The parameter distribution is represented by an array xi with many samples.
 
 ema_base.EmaParamBase: common properties defining
     indexing into array of parameter vectors, and
     a prior GaussianRV instance for all GMM components in all groups.
 
@@ -46,19 +46,23 @@
 the model of the PairedCompCalc package, partly described in
 A. Leijon, M. Dahlquist, and K. Smeds (2019):
 Bayesian analysis of paired-comparison sound quality ratings. JASA 146(5):3174–3183.
 
 EXCEPT for the present use of a mixture model for the population(s).
 
 Detailed math documentation is presented in
-A Leijon et al. (2022):
-Bayesian Analysis of Ecological Momentary Assessment (EMA) Data in python
-Journal manuscript 2022-08-xx
+A. Leijon, P. von Gablenz, I. Holube, J. Taghia, and K. Smeds.
+Bayesian analysis of ecological momentary assessment (EMA) data
+collected in adults before and after hearing rehabilitation.
+Frontiers in Digital Health, 5(1100705), 2023.
 
 *** Version History:
+* Version 1.0.0:
+2023-05-17, EmaModel.initialize(...) using n_participants_per_comp instead of max_n_comp.
+
 * Version 0.9.3:
 2022-08-20, ensure restrict_attributes=False, in case tied response scales
 2022-06-xx, adapted to use pandas.DataFrame storage in ema_data.
 
 * Version 0.8.3:
 2022-03-08, minor cleanup
 
@@ -107,15 +111,15 @@
 
 from EmaCalc.ema_base import EmaParamBase
 from EmaCalc.ema_group import EmaGroupModel
 from EmaCalc.ema_latent import Bradley
 
 
 # -------------------------------------------------------------------
-__ModelVersion__ = "2022-08-20"
+__ModelVersion__ = "2023-05-17"
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
 
 # ------------------------------------------------------------------
 class EmaModel:
@@ -161,35 +165,40 @@
         self.rng = rng
 
     def __repr__(self):
         return self.__class__.__name__ + '(groups=groups)'
 
     @classmethod
     def initialize(cls, ds, effects,
-                   max_n_comp=None,
+                   max_n_comp=None,  # *** no longer used
+                   n_participants_per_comp=5,
                    rv_class=Bradley,
                    restrict_attribute=False,
                    restrict_threshold=True,
                    seed=None):
         """Create a crude initial model from all available count-profile data.
         :param ds: a single ema_data.EmaDataSet instance with all EMA data for analysis
         :param effects: iterable with desired estimated effects of situatio on attribute attribute_grades.
             Each effect element = a key in ds.emf.situation_dtypes, or a tuple of such keys.
-        :param max_n_comp: (optional) max number of profile clusters in learned model
-            = max number of mixture components in the population model
+        :param max_n_comp: Not used, only for compatibility warning
+        :param n_participants_per_comp: (optional) expected number participants per mixture component
+            -> initial n_comp = n_participants // n_participants_per_comp
             The number of actually used components may be reduced during VI learning.
         :param rv_class: (optional) class of latent sensory random variable
         :param restrict_attribute: (optional) boolean switch
             to force restriction on attribute sensory-variable locations
         :param restrict_threshold: (optional) boolean switch
             to force restriction on response-threshold locations
         :param seed: (optional) integer to get reproducible random sequences
         :return: a cls instance
         """
         ds.ensure_complete()
+        if max_n_comp is not None:
+            logger.warning(f'Version >= 1.0: max_n_comp no longer used. Set n_participants_per_comp instead.')
+        n_participants_per_comp = max(2, n_participants_per_comp)
         if restrict_attribute and ds.emf.tied_response_scales:
             restrict_attribute = False
             logger.warning('*** Cannot use restrict_attribute=True with tied response scales')
         if restrict_attribute and restrict_threshold:
             restrict_attribute = False  # ONLY ONE restriction allowed
             logger.warning(f'Only ONE restriction allowed: using restrict_threshold={restrict_threshold}')
         if not (restrict_attribute or restrict_threshold):
@@ -200,20 +209,21 @@
                                        restrict_threshold=restrict_threshold)
         # = all base variables, to be used by all model objects
         seed_seq = np.random.SeedSequence(seed)
         rng = np.random.default_rng(seed_seq)
         # = main Generator for all random numbers, EXCEPT EmaRespondentModel instances
         # Same rng for all EmaGroupModel instances, but separate for EmaRespondentModel-s
         group_seeds = seed_seq.spawn(len(ds.groups))
-        groups = {g: EmaGroupModel.initialize(max_n_comp, base, g_data, g_seed, rng)
+        groups = {g: EmaGroupModel.initialize(n_participants_per_comp, base, g_data, g_seed, rng)
                   for ((g, g_data), g_seed) in zip(ds.groups.items(),
                                                    group_seeds)}
         logger.info('EmaModel initialized with ' +
                     f'{len(groups)} group(s); ' +
                     f'{base.n_parameters} model parameters;\n\t' +
+                    f'n_participants_per_comp={n_participants_per_comp}; '
                     f'restrict_attribute = {restrict_attribute}; '
                     f'restrict_threshold = {restrict_threshold};')
         if seed is None:
             logger.debug(f'*** Using seed={seed}')
         else:
             logger.warning(f'*** Using seed={seed} -> reproducible results.')
         return cls(base, groups, rng)
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_nap.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_nap.py`

 * *Files identical despite different names*

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_respondent.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_respondent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """This module defines a class for individual participant parameter model
 to be part of an ema_group.EmaGroupModel instance,
 which is part the main Bayesian probabilistic model of EMA data.
 
 Individual parameter distributions are approximated by sampling.
 The population mixture model is common prior for all individuals in
-the group recruited from the same population.
+the participant group recruited from the same population.
 
 *** Class Defined here:
 
 EmaRespondentModel: Distribution of individual parameter vector
     assumed to determine the observed EMA data from ONE respondent,
     including, in each EMA record,
     (1) a nominal (possibly multidimensional) Situation category, and
     (2) ordinal Ratings for zero, one, or more perceptual Attributes.
     The parameter distribution is represented by an array xi with many samples.
-    The sample distribution is independent across EmaRespondentModel instances,
+    The sample distributions are independent across EmaRespondentModel instances,
     so instances may be adapt-ed in parallel processes.
 
 *** Version History:
+* Version 1.0.0:
+2023-05-01, EmaRespondentModel.rvs_grade_count() reverted to old method from Frontiers paper.
+            Alternative method from v.0.9.5 sometimes incorrect.
+2023-04-26, corrected bug in EmaRespondentModel.rvs_grade_count(), in case multiple Phase-s
+            Private property EmaRespondentModel._rng, using sampler rng, for reproducibility.
+
 * Version 0.9.5:
 2023-03-11, rvs_grade_count() uses model-PREDICTED situation count profiles,
             -> greater variability, compared to earlier OBSERVED counts for each situation
 2023-03-03, new methods EmaRespondentModel.attribute_grade_count() and .rvs_grade_count()
 
 * Version 0.9.3:
 2022-07-27, changed module name ema_subject -> ema_respondent
@@ -37,42 +43,41 @@
 2022-06-15, new _initialize_rating_eta(y); changed _initialize_rating_theta(y, eta)
             tested initial response thresholds crudely based on response counts
 
 2022-05-21, EmaSubjectModel.cdf_arg: check for too small response interval,
             that might cause numerical underflow in case of many missing data
 
 * Version 0.8.3:
-2022-03-08, minor cleanup logging to work in multi-processing
+2022-03-08, minor cleanup logging to work in multiprocessing
 
 * Version 0.8.2: prepared for multi-processing subject adapt() in parallel processes
 2022-03-03, EmaSubjectModel methods mean_zeta, mean_zeta_mom no longer needed
 
 * Version 0.8.1: minor cleanup of comments and logger output
 
 * Version 0.8
 2022-02-12, Changed VI factorization for better approximation,
     with individual indicators conditional on parameter samples,
     defining variational q(zeta_n, xi_n) = q(zeta_n | xi_n) q(xi_n)
 """
-# **** predicted_count and observed count here ***********
 import multiprocessing
 import logging
 
 import numpy as np
 from scipy.optimize import minimize
 import pandas as pd
 
 from samppy import hamiltonian_sampler as ham
 from samppy.sample_entropy import entropy_nn_approx as entropy
 
 from EmaCalc.ema_base import PRIOR_PARAM_SCALE
 
 
 # -------------------------------------------------------------------
-__ModelVersion__ = "2022-07-27"
+__ModelVersion__ = "2023-05-01"
 
 DITHER_PARAM_SCALE = 0.1 * PRIOR_PARAM_SCALE
 # -> initial dithering of point-estimated individual parameters
 
 N_SAMPLES = 1000
 # = number of parameter vector samples in each EmaRespondentModel instance
 
@@ -132,14 +137,18 @@
                                                max_accept_rate=0.95,    # = default
                                                rng=rng
                                                )
         # keeping sampler properties across learning iterations
         self.prior = prior
         self.ll = None  # space for log-likelihood result from self.adapt()
 
+    @property
+    def _rng(self):
+        return self._sampler._rng
+
     def __repr__(self):
         return (self.__class__.__name__ + '('
                 + '\n\tsituation_count=' + f'{self.situation_count},'
                 + '\n\trating_count=' + f'{self.rating_count},'
                 + f'\n\txi= parameter array with shape {self.xi.shape}; id={id(self.xi)},'
                 + f'\n\tid(prior)= {id(self.prior)},'
                 + f'\n\tll= {self.ll})')
@@ -219,15 +228,15 @@
                      + f'n_steps= {self._sampler.n_steps}')
         self.xi = self._sampler.x
         self.base.restrict(self.xi)
         # adjust for modified xi:
         self._sampler.U = self._sampler.potential(self._sampler.x)
         self._sampler.args = ()  # just in case a pickled prior copy was there
         # Calc log-likelihood contribution with final xi samples:
-        lp_xi = - np.mean(self._sampler.U)  # after restrict_xi
+        lp_xi = - np.mean(self._sampler.U)  # after base.restrict
         # lp_xi = E_xi{ ln p(data | xi) + self.prior.logpdf(xi) }
         h_xi = entropy(self.xi)
         # approx = - E{ ln q(xi) }
         kl_zeta = self._kl_div_zeta(self.prior)
         self.ll = lp_xi + h_xi - kl_zeta
         logger.debug(f'{self.id}: adapt: ll={self.ll:.3f}; '
                      + f'(lp_xi={lp_xi:.3f}; '
@@ -310,29 +319,29 @@
         a_grades = emf.ordinal_scales[emf.attribute_scales[a]].categories
         df = pd.DataFrame(self.rating_count[a_ind].T,
                           index=sit_index, columns=a_grades)
         df.columns.set_names(a, inplace=True)
         if groupby is None:
             return df.sum()
         else:
-            return df.groupby(level=groupby).sum()
+            return df.groupby(level=groupby, sort=False, group_keys=True).sum()
 
     def rvs_grade_count(self, a, groupby=None, sample_head='_Sample'):
         """Calculate sampled model-predicted distribution of response counts
         for comparison with observed count histograms.
         :param a: key for selected attribute
         :param groupby: (optional) single situation key (dimension) or list of such keys
             for which separate attribute-counts are calculated.
             Counts are summed across any OTHER situation dimensions.
         :param sample_head: (optional) header name for sample index
         :return: a pd.DataFrame object with all grade counts,
             with one row for each (sample, *groupby) multi-index combination
             and one column for each grade category.
         """
-        # *** use only total observed count to estimate situation-count distribution ! *********
+        # *** use total observed count to estimate situation-count distribution !
         emf = self.base.emf
         a_index = list(emf.attribute_dtypes.keys()).index(a)
         if groupby is None:
             groupby = []
         elif isinstance(groupby, str):
             groupby = [groupby]
         theta = self.base.attribute_theta(self.xi, a)
@@ -347,29 +356,33 @@
         # tau[s, l] = s-th sample of l-th median rating threshold for attribute a
         arg_low = tau[..., :-1, None] - theta[..., None, :]
         # a[s, l, k] = lower interval limits for l-th category in k-th situation
         arg_high = tau[..., 1:, None] - theta[..., None, :]  # upper interval limits
         lp = self.base.rv_class.log_cdf_diff(arg_low, arg_high)
         p_response = np.exp(lp).transpose((0, 2, 1))
         # p[s, k, l] = s-th sample of prob of l-th response in k-th situation
-        p_sit = self.base.situation_prob(self.xi)
-        # p_sit[s, k0, k1,...] = s-th sample of prob for k-th <-> (k0, k1,...)-th situation
-        p_sit = p_sit.reshape((len(p_sit), -1))
-        # p_sit[s, k] = s-th sample of prob for k-th situation
-        c_tot = np.sum(self.rating_count[a_index])
-        # c_tot = total count across all situations
-        rng = np.random.default_rng()  # ******************
-        c_sit = rng.multinomial(c_tot, p_sit)
-        # c_sit[s, k] = s-th sample of PREDICTED count in k-th situation
-        # c_sit = np.sum(self.rating_count[a_index], axis=0)
-        # c_sit[k] = total OBSERVED count of responses in k-th situation
-        n_count = rng.multinomial(c_sit, pvals=p_response)
+        # p_sit = self.base.situation_prob(self.xi)
+        # # p_sit[s, k0, k1, ...] = s-th sample of CONDITIONAL prob for (k1,...)-th situation, given k0 (Phase)
+        # p_sit /= p_sit.shape[1]  # equal weight for all Phase-s
+        # # p_sit[s, k0, k1,...] = s-th sample of prob for k-th <-> (k0, k1,...)-th situation
+        # p_sit = p_sit.reshape((len(p_sit), -1))
+        # # p_sit[s, k] = s-th sample of prob for k-th situation, across ALL attributes
+        # c_tot = np.sum(self.rating_count[a_index])
+        # # c_tot = total count across all situations
+        # c_sit_all = self._rng.multinomial(c_tot, p_sit)
+        # c_sit_all[s, k] = s-th sample of PREDICTED count in k-th situation across ALL attributes
+        # *** This gives WRONG result in case the attribute is relevant only in some situation,
+        # *** E.g., in the IHAB study, attribute Involvement has responses only in CoSS=C2.
+        c_sit = np.sum(self.rating_count[a_index], axis=0)
+        # c_sit[k] = total OBSERVED count of responses in k-th situation for THIS attribute!
+        # *** This is the method used in the Frontiers paper!
+        n_count = self._rng.multinomial(c_sit, pvals=p_response)
         # n_count[s, k, l] = s-th sample of counts in l-th grade category in k-th situation
         df_index = pd.MultiIndex.from_product([range(len(n_count)),
                                                *[sit_dtype.categories
                                                  for sit_dtype in emf.situation_dtypes.values()]],
                                               names=[sample_head, *emf.situation_dtypes.keys()])
         a_grades = emf.ordinal_scales[emf.attribute_scales[a]].categories
         df = pd.DataFrame(n_count.reshape((-1, n_count.shape[-1])),
                           index=df_index, columns=a_grades)
         df.columns.set_names(a, inplace=True)
-        return df.groupby(level=[0, *groupby]).sum()
+        return df.groupby(level=[0, *groupby], sort=False, group_keys=True).sum()
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_simulation.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 EmaSimPopulation.gen_group(...)
     draws a group of simulated participants at random from the simulated Population.
 
 EmaSimExperiment.gen_dataset(...)
     generates am ema_data.EmaDataSet instance with simulated EMA records
     for one or more groups of simulated participants.
-    All records can be saved to files using the EmaDataSet.save(...) method.
+    All records can be saved to file(s) using the EmaDataSet.save(...) method.
 
 *** Usage example: See script run_sim.py
 
 *** Version History:
 * Version 0.9.4:
 2022-11-22, allow EmaSimPopulation settings restrict_attribute, restrict_threshold
             with same effects as in ema_model.EmaModel
@@ -76,15 +76,15 @@
 # **** plus variance for independent variations across situation_dtypes???
 
 import numpy as np
 import pandas as pd
 import logging
 
 from .ema_data import EmaDataSet
-from .ema_thresholds import ThresholdsOld
+# from .ema_thresholds import ThresholdsOld
 from .ema_thresholds import ThresholdsFree, ThresholdsMidFixed
 from . import ema_latent
 
 
 RNG = np.random.default_rng()
 # = default module-global random generator
 # may be modified via function set_sim_seed
@@ -103,31 +103,23 @@
     """
     global RNG
     RNG = np.random.default_rng(seed)
     if seed is not None:
         logger.warning(f'*** Using seed={seed} -> reproducible results.')
 
 
-# def response_thresholds(eta):
-#     return ThresholdsOld.tau(eta)
-#
-#
-# def tau_inv(tau):
-#     return ThresholdsOld.tau_inv(tau)
-
-
 # --------------------------------------- subject response models
 class EmaSimSubject:
     """Simulate one individual participant in an EMA data-collection experiment.
     Superclass for either SubjectBradley or SubjectThurstone
     """
     def __init__(self, sc_prob, a_theta, a_tau):  # lapse_prob=0.):
         """
         :param sc_prob: mD array with (non-normalized) conditional Situation probability
-            sc_prob[k0, k1, k2,...] propto Prob (k1, k2, ...)-th situation, GIVEN k0-th Stage
+            sc_prob[k0, k1, k2,...] propto Prob (k1, k2, ...)-th situation, GIVEN k0-th Phase
             sc_prob.shape == emf.situation_shape
         :param a_theta: dict with (a_key, a_theta) elements, where
             a_key = a string identifying ONE Attribute among emf.attribute_grades.keys()
             a_theta[k0, k1, ...] = mD array with mean of latent sensory variable for Attribute a_key,
         :param a_tau: dict with (a_key, thr) elements, where
             tnr[l] = UPPER interval limit for l-th ordinal response,
             NOT INCLUDING extreme -inf, +inf limits
@@ -142,16 +134,16 @@
                              for (key, v) in vars(self).items()) +
                 '\n\t)')
 
     def gen_ema_records(self, emf, min_ema, max_ema):
         """Generate a sequence of EMA records at random
         using response properties of self.
         :param emf: ema_data.EmaFrame instance
-        :param min_ema: min random number of EMA records per Stage
-        :param max_ema: max random number of EMA records per Stage
+        :param min_ema: min random number of EMA records per Phase
+        :param max_ema: max random number of EMA records per Phase
         :return: ema_df = a pd.DataFrame instance containing simulated EMA results,
             stored according to given emf.
             One column for each Situation dimension and each Attribute.
             One row for each simulated EMA record.
             Number of records randomly drawn with
             min_ema <= ema_df.shape[0] < max_ema
         """
@@ -178,15 +170,16 @@
         sit_prob_phase = self.sc_prob.reshape((self.sc_prob.shape[0], -1))
         for (i, p) in enumerate(sit_prob_phase):
             n_rec = RNG.integers(min_ema, max_ema)
             for _ in range(n_rec):
                 sit_index = (i, *situation_index(p, sit_shape_phase))
                 a_grades = self.gen_attr_grades(emf, sit_index)
                 ema_list.append(situation_dict(sit_index) | a_grades)
-        return pd.DataFrame.from_records(ema_list).astype(emf.dtypes)
+        cat_dtypes = emf.situation_dtypes | emf.attribute_dtypes  # ****** needed ?
+        return pd.DataFrame.from_records(ema_list).astype(cat_dtypes)
 
     def gen_attr_grades(self, emf, sit_index):
         """Generate random ordinal Attribute grades in given Situation
         :param emf: external ema_data.EmaFrame object defining experimental layout
         :param sit_index: index tuple defining ONE situation for this record,
             including index in ALL situation dimensions
         :return: a_grades = dict with elements (a, grade)
@@ -477,14 +470,16 @@
     The experimental procedure is defined by
     emf = an ema_data.EmaFrame instance
     """
     def __init__(self, emf, groups):
         """
         :param emf: EmaFrame instance, defining experimental parameters
         :param groups: dict with elements (g_id, g_sim),
+            g_id is a tuple with one or several group-category labels,
+                one for each element in emf.group_head()
             g_sim = an EmaSimGroup instance
         :param restrict_attribute: (optional) boolean switch
             to force restriction on attribute sensory-variable locations
         :param restrict_threshold: (optional) boolean switch
             to force restriction on response-threshold locations
         """
         self.emf = emf
@@ -495,15 +490,15 @@
                 ',\n\t'.join(f'{key}={repr(v)}'
                              for (key, v) in vars(self).items()) +
                 '\n\t)')
 
     def gen_dataset(self, min_ema=3, max_ema=50):
         """Generate a complete EmaDataSet instance for this experiment,
         with one or more groups of participants.
-        :param min_ema: min random number of EMA records in each Stage
-        :param max_ema: max random number of EMA records in each Stage
+        :param min_ema: min random number of EMA records in each Phase
+        :param max_ema: max random number of EMA records in each Phase
         :return: a single EmaDataSet instance
         """
         emd = {g: {s_id: s.gen_ema_records(self.emf, min_ema, max_ema)
                    for (s_id, s) in g_sim.participants.items()}
                for (g, g_sim) in self.groups.items()}
         return EmaDataSet(self.emf, emd)
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/ema_thresholds.py` & `EmaCalc-1.0.0/src/EmaCalc/ema_thresholds.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from given model parameters.
 
 *** Classes:
 Thresholds: OLD model version allowing all response thresholds freely adaptable.
 ThresholdsFree: allowing all response thresholds freely adaptable, new version.
 ThresholdsMidFixed: forcing one mid-range threshold -> zero, other thresholds free
 
-*** CHANGE to set midpoint of middle interval -> zero, if odd number of intervals, like previous versiond ******
-
 *** Version history:
 * Version 0.9.5: NEW module, with functions moved from ema_base
 """
 import numpy as np
 from scipy.special import logit, expit
 # ***** logit, expit are NOT symmetric around mid-point for extreme arguments
 # logit(expit(37.)) = 37.; logit(expit(38.)) = +inf; logit(expit(-38.)) = -38.
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/gauss_gamma.py` & `EmaCalc-1.0.0/src/EmaCalc/gauss_gamma.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 GaussianGivenPrecisionRV: class for the random mean vector of a GaussianRV object
 PrecisionRV: class for the random precision vector of a GaussianRV object
 
 StudentRV: a multivariate Student-t distribution for a vector with independent elements,
     used for predictive distributions derived from a GaussianRV instance.
 
 *** Version History:
+* Version 1.0.0:
+2023-05-02, allow PrecisionRV.a as 1D array, for potential future extension,
+            to allow users to set smaller prior inter-individual threshold variance
 
 * Version 0.7.1:
 2022-01-19, StudentRV has own property rng, to allow external seed control,
             GaussianRV.predictive, and GaussianGivenPrecision.predictive ordinary methods
             GaussianRV.predictive, and GaussianGivenPrecision.predictive take input rng
 
 * Version 0.7:
@@ -30,14 +33,16 @@
 * EmaCalc version 0.5:
 2021-10-22, copied PairedCompCalc -> EmaCalc, unchanged
 2021-10-22, modified for use in EmaCalc
 
 * Older applications:
 2018-08-10, used in general Bayesian mixture models, and package PairedCompCalc
 """
+# **** allow array as PrecisionRV.a parameter ? *******
+
 import numpy as np
 import logging
 from scipy.special import gammaln, psi
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)  # *** TEST
 
@@ -70,17 +75,17 @@
 
     @classmethod
     def initialize(cls,
                    loc,
                    prec_a, prec_b,
                    learned_weight=0.001):
         """Create cls instance with default structure
-        :param loc: location vector = mean of mean attribute
-        :param prec_a: scalar precision gamma shape parameter *** ONLY scalar for EMA
-        :param prec_b: 1D precision gamma inverse-scale parameter
+        :param loc: 1D array-like location vector = mean of mean attribute
+        :param prec_a: scalar or 1D array-like precision gamma shape parameter
+        :param prec_b: 1D array-like precision gamma inverse-scale parameter
             len(prec_b) == len(loc)
         :param learned_weight: (optional) scalar effective number of observations
             learned_weight = 0. gives a non-informative improper prior density
         """
         prec = PrecisionRV(a=prec_a, b=prec_b)
         mean = GaussianGivenPrecisionRV(loc, learned_weight, prec)
         return cls(mean, prec)
@@ -171,34 +176,33 @@
         self.prec.adapt(x_2, w, prior=prior.prec,
                         new_mean_2=(self.mean.learned_weight * self.mean.loc**2 -
                                     prior.mean.learned_weight * prior.mean.loc**2))
         ll = - self.relative_entropy(prior)
         if self.mean.learned_weight > 0.5:
             logger.debug(f'comp -KLdiv= {ll:.3f}')
             logger.debug(f'comp.mean.learned_weight = {self.mean.learned_weight:.2f}')
-            logger.debug(f'comp.prec.a = {self.prec.a:.2f}')
-            if self.prec.a > 1:
-                logger.debug('comp.std = ' + np.array_str(np.sqrt(self.prec.mean_inv()),
-                                                          precision=2))
-            else:
-                logger.debug('comp.prec.b = ' + np.array_str(self.prec.b,
-                                                             precision=2))
+            logger.debug('comp.prec.a = ' + np.array_str(np.asarray(self.prec.a),
+                                                         precision=2))
+            logger.debug('comp.prec.b = ' + np.array_str(self.prec.b,
+                                                         precision=2))
+            logger.debug('comp.std = ' + np.array_str(np.sqrt(self.prec.mean_inv()),
+                                                      precision=2))
         return ll
 
 
 # ----------------------------------------------------------------------
 class GaussianGivenPrecisionRV:
     """Conditional Gaussian distribution of the mean of a Gaussian random vector,
     given the precision array.
     The probability density function is
     p(mu | Lambda) propto prod_d (beta Lambda_d)^0.5 exp(- 0.5 (mu_d - m_d)^2 beta Lambda_d
     where
     mu is a row vector, sample of random vector self
     m is the location of self,
-    beta is the learned_weight property
+    beta is the scalar learned_weight property
     Lambda is the precision vector.
     """
     def __init__(self, loc, learned_weight, prec):
         """
         Conditional Gaussian vector, given precision matrix
         :param loc: location vector
         :param learned_weight: scalar effective number of learning data
@@ -264,31 +268,36 @@
                          rng=rng)
 
 
 # ---------------------------------------------------------------------------
 class PrecisionRV:
     """Distribution of the precision vector Lambda of a Gaussian vector
     The probability density function is
-    p(Lambda) = prod_d C_d Lambda_d^(a - 1) exp(- b_d Lambda_d), i.e., a gamma density,
+    p(Lambda) = prod_d C_d Lambda_d^(a_d - 1) exp(- b_d Lambda_d), i.e., a gamma density,
         where
-        a = scalar shape parameters ***allow ONLY scalar here, same for all elements
+        a = scalar (or 1D array) shape parameters
         b = 1D array of inverse-scale parameters
         Lambda.shape == b.shape
         a and b must have broadcast-compatible shapes
         C_d = b_d^a / Gamma(a) is the normalization factor
     """
     def __init__(self, a=0., b=1.):
         """
-        :param a: scalar shape parameter
-        :param b: 1D array or array-like list with inverse scale parameters
+        :param a: scalar or 1D array-like shape parameter(s)
+        :param b: 1D array-like with inverse scale parameter(s)
         """
-        assert np.isscalar(a), 'shape parameter should be scalar for EMA usage'
-        # same precision shape parameter for all elements
+        # assert np.isscalar(a), 'shape parameter should be scalar for EMA usage'
+        try:
+            a = np.array(a)
+            b = np.array(b)
+            test = a / b
+        except ValueError as e:
+            raise RuntimeError('a and b parameters must be broadcast-compatible and > 0. ' + str(e))
         self.a = a
-        self.b = np.array(b)
+        self.b = b
 
     def __repr__(self):
         return self.__class__.__name__ + f'(a= {repr(self.a)}, b= {repr(self.b)})'
 
     @property
     def size(self):
         return self.mean.size
@@ -306,18 +315,22 @@
         """E{self}"""
         return self.a / self.b
 
     def mean_inv(self):  # *** not needed for EMA ?
         """E{ inv(self) }, where
         inv(self) has an inverse-gamma distribution
         """
-        if self.a > 1:
-            return self.b / (self.a - 1)
-        else:
+        if self.a.ndim > 0:
+            m = self.b / np.maximum(self.a - 1, np.finfo(float).eps)
+            m[self.a <= 1.] = np.nan
+            return m
+        elif self.a <= 1.:
             return np.full_like(self.b, np.nan)
+        else:
+            return self.b / (self.a - 1)
 
     def mode_inv(self):
         """mode{ inv(self) }, where
         inv(self) has an inverse-gamma distribution
         """
         return self.b / (self.a + 1.)
 
@@ -371,24 +384,24 @@
                       )
 
 
 class StudentRV:
     """Frozen Student distribution of 1D random vector with INDEPENDENT elements
     generalizing scipy.stats.t for vector-valued random variable
     """
-    def __init__(self, df, loc=np.array(0.), scale=1.,
+    def __init__(self, df, loc=np.array(0.), scale=np.array(1.),
                  rng=None):
         """Create a StudentRV instance
-        :param df: scalar degrees of freedom, SAME for all vector elements
+        :param df: scalar or 1D array-like, degrees of freedom
         :param loc: 1D array or array-like list of location elements
         :param scale: scalar or 1D array or array-like list of scale parameter(s)
-            loc and scale must have broadcast-compatible shapes
+            df, loc, and scale must have broadcast-compatible shapes
         :param rng: (optional) random.Generator object
         """
-        self.df = df
+        self.df = np.asarray(df)
         self.loc = np.asarray(loc)
         self.scale = np.asarray(scale)
         if rng is None:
             self.rng = np.random.default_rng()
         else:
             self.rng = rng
 
@@ -396,36 +409,49 @@
         return (self.__class__.__name__
                 + f'(df= {repr(self.df)}, '
                 + f'loc= {repr(self.loc)}, '
                 + f'scale= {repr(self.scale)})')
 
     @property
     def size(self):
-        return len(self.loc)
+        return self.loc.size  # len(self.loc)
 
     @property
     def mean(self):
-        if self.df > 1:
+        if self.df.ndim > 0:
+            m = self.loc + 0.  # copy
+            m[self.df <= 1.] = np.nan
+            return m
+        elif self.df > 1.:
             return self.loc
         else:
+        # if self.df > 1:
+        #     return self.loc
+        # else:
             return np.full_like(self.loc, np.nan)
 
     @property
     def var(self):
         """Variance array"""
-        if self.df > 2:
-            return self.scale**2 * self.df / (self.df - 2)
+        if self.df.ndim > 0:
+            v = self.scale ** 2 * self.df / np.maximum(self.df - 2., np.finfo(float).eps)
+            v[self.df <= 2.] = np.inf
+            v[self.df <= 1.] = np.nan
+            return v
+        elif self.df > 2:  # scalar df
+            return self.scale ** 2 * self.df / (self.df - 2.)
         elif self.df > 1:
             return np.full_like(self.loc, np.inf)
         else:
             return np.full_like(self.loc, np.nan)
 
     def logpdf(self, x):
         """ln pdf(x | self)
         :param x: array or array-like list of sample vectors
+            must be broadcast-compatible with self.loc
         :return: lp = scalar or array of logpdf values
             lp[...] = ln pdf[x[..., :] | self)
             lp.shape == x.shape[:-1]
         Arne Leijon, 2018-07-08, **** checked by comparison to scipy.stats.t
         """
         d = (x - self.loc) / self.scale
         return np.sum(- np.log1p(d**2 / self.df) * (self.df + 1) / 2
@@ -456,50 +482,62 @@
 if __name__ == '__main__':
     from scipy.stats import norm
     from scipy.stats import gamma
     from scipy.stats import t as scipy_t  # ******** skip ?
     import copy
 
     # --------------------------- Test PrecisionRV
-    a = 10.
-    b = [1., 2., 3.]
-    nx = 10
-
-    g = PrecisionRV(a=a, b=b)
-    print(f'\n*** Testing {g}:')
-    x = np.array([gamma(a=a, scale=1/b_i).rvs(size=nx)
-                  for b_i in b]).T
-    print(f'gamma samples x= {x}')
-    print(f'mean(x)= {np.mean(x, axis=0)}')
-    print(f'PrecisionRV.logpdf(x)= {g.logpdf(x)}')
-    g_ll = np.array([np.sum([gamma(a=a, scale=1/b_i).logpdf(x_si)
-                             for (b_i, x_si) in zip(b, x_s)])
-                     for x_s in x])
-    print(f'scipy gamma.logpdf(x)= {g_ll}')
+    b = np.array([1., 2., 3.])
+    nx = 50
+
+    for a in [0.5, 10., [3., 2., 1.]]:
+        g = PrecisionRV(a=a, b=b)
+        print(f'\n*** Testing {g}:')
+        # x = np.array([gamma(a=a, scale=1/b_i).rvs(size=nx)
+        #               for b_i in b]).T
+        x = gamma(a=a, scale=1/b).rvs(size=(nx, len(b)))
+        print(f'mean= {g.mean}')
+        print(f'mean_inv= {g.mean_inv()}')
+        print(f'mode_inv= {g.mode_inv()}')
+        print(f'gamma samples x[:10]= {x[:10]}')
+        print(f'mean(x)= {np.mean(x, axis=0)}')
+        print(f'PrecisionRV.logpdf(x)= {g.logpdf(x)}')
+        # g_ll = np.array([np.sum([gamma(a=a, scale=1/b_i).logpdf(x_si)
+        #                          for (b_i, x_si) in zip(b, x_s)])
+        #                  for x_s in x])
+        g_ll = np.sum(gamma(a=a, scale=1/b).logpdf(x),
+                      axis=-1)
+        print(f'scipy gamma.logpdf(x)= {g_ll}')
 
     # --------------------------- Test StudentRV
     df = 10.
     m = [1., 2., 3.]
     s = [3., 2., 1.]
-    st = StudentRV(df=df, loc=m, scale=s)
-    print(f'\n*** Testing {st}')
-    scipy_x = np.array([scipy_t.rvs(df=df, loc=m_i, scale=s_i, size=nx)
-                        for (m_i, s_i) in zip(m, s)]).T
-    print(f'scipy_t samples x= {scipy_x}')
-    print(f'mean(x)= {np.mean(scipy_x, axis=0)}')
-
-    print(f'StudentRV.rvs() = {st.rvs()}')
-    x = st.rvs(size=[nx])
-    print(f'StudentRV.rvs(size=[nx]) = x = {x}')
-    print(f'mean(x)= {np.mean(x, axis=0)}')
-    print(f'StudentRV.logpdf(x)= {st.logpdf(x)}')
-    st_ll = np.array([np.sum([scipy_t(df=df, loc=m_i, scale=s_i).logpdf(x_si)
-                             for (m_i, s_i, x_si) in zip(m, s, x_s)])
-                     for x_s in x])
-    print(f'scipy_t.logpdf(x)= {st_ll}')
+    for df in [0.5, 1.5, 10., [2., 3., 4.]]:
+        st = StudentRV(df=df, loc=m, scale=s)
+        print(f'\n*** Testing {st}')
+        print(f'mean= {st.mean}')
+        print(f'var= {st.var}')
+        # scipy_x = np.array([scipy_t.rvs(df=df, loc=m_i, scale=s_i, size=nx)
+        #                     for (m_i, s_i) in zip(m, s)]).T
+        scipy_x = scipy_t.rvs(df=df, loc=m, scale=s, size=(nx, len(m)))
+        print(f'scipy_t samples x[:10]= {scipy_x[:10]}')
+        print(f'mean(x)= {np.mean(scipy_x, axis=0)}')
+
+        print(f'StudentRV.rvs() = {st.rvs()}')
+        x = st.rvs(size=[nx])
+        print(f'StudentRV.rvs(size=[nx]) = x[:10] = {x[:10]}')
+        print(f'mean(x)= {np.mean(x, axis=0)}')
+        print(f'StudentRV.logpdf(x)= {st.logpdf(x)}')
+        # st_ll = np.array([np.sum([scipy_t(df=df, loc=m_i, scale=s_i).logpdf(x_si)
+        #                          for (m_i, s_i, x_si) in zip(m, s, x_s)])
+        #                  for x_s in x])
+        st_ll = np.sum(scipy_t(df=df, loc=m, scale=s).logpdf(x),
+                       axis=-1)
+        print(f'scipy_t.logpdf(x)= {st_ll}')
 
     # --------------------------- Test GaussianRV
     scale = np.array([1., 2., 3.])
     prec_a = 1.1
     prec_b = prec_a * scale**2
     g = GaussianRV.initialize(loc=[0., 1., 2.],
                               prec_a=prec_a, prec_b=prec_b,
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/run_ema.py` & `EmaCalc-1.0.0/src/EmaCalc/run_ema.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,26 @@
 *** Usage: four main steps, see also explicit template example below
 
 *1: Set up an EmaFrame instance to define experiment and to select input data.
 *2: Load a set of collected EMA data into an EmaDataSet instance
 *3: Initialize and train an EmaModel instance for observed data.
 *4: Display results and save figures and tables to a directory tree.
 
+**  Recommended to run a couple of times with the same data set,
+    to see random variability in estimated results.
+
 
 *** Version history:
+* Version 1.0.0:
+2023-05-17, EmaModel.initialize(..., n_participants_per_comp, ...) defines initial number of GMM components.
+            Parameter max_n_comp no longer used.
+2023-04-22, adapted to simplified group-key representation in module ema_data.py:
+            Group categories specified in EmaFrame.setup(...)
+            NOTE: changed signatures EmaFrame.setup(), EmaDataSet.load(), EmaDataSet.save().
+
 * Version 0.9.5:
 2023-03-07, ema_display.EmaDisplaySet include observed and model-predicted grade-count histograms
 2023-03-01, timestamp_result if needed to avoid over-writing result files
 
 * Version 0.9.3:
 2022-08-14, Each ordinal rating scale may be unique or shared by more than one Attribute
 2022-07-30, minor cleanup adapting to minor changes in package modules.
@@ -48,44 +58,44 @@
     from EmaCalc.ema_data import EmaFrame, EmaDataSet
     from EmaCalc.ema_model import EmaModel
     from EmaCalc.ema_display import EmaDisplaySet
     from EmaCalc import ema_logging, __version__
     from EmaCalc.ema_display_format import harmonize_ylim
 
     # ------------------------ Set up working directory and result logging:
-    # timestamp_result = True  # Prevent over-writing result files
-    timestamp_result = False  # Repeated runs will save results in same directory
+    timestamp_result = True  # New result folder for each run, to prevent over-writing
+    # timestamp_result = False  # Repeated runs will over-write existing results
 
     work_path = Path.home() / 'Documents' / 'EMA_sim'  # or whatever...
     data_path = work_path / 'data'  # to use simulation data generated by run_sim.py
     result_path = work_path / 'result'  # or whatever
     model_file = 'test_ema_model.pkl'  # name of saved model file (if saved)
 
     if timestamp_result:
         t = dt.datetime.now()
         result_path = result_path.with_name(result_path.name +
-                                            f'-{t.year}-{t.month:02}-{t.day:02}-{t.hour:02}{t.minute}')
+                                            f'-{t.year}-{t.month:02}-{t.day:02}-{t.hour:02}{t.minute:02}')
 
     ema_logging.setup(save_path=result_path,
                       log_file='run_ema_log.txt')  # to save the log file
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.INFO)
 
     logger.info(f'*** Running EmaCalc version {__version__} ***')
 
-    # ------ 1: Define Experimental Framework: Situations, Attributes, and Grades
+    # ------ 1: Define Experimental Framework: Situations, Attributes, and Groups
 
     # NOTE: This example uses data generated by template script run_sim.py
     # Edit as needed for any other EMA data source
 
-    situations = {'Phase': ('',),  # only ONE Test phase with empty label
+    situations = {'Phase': ('',),  # only One Test phase with empty label
                   'HA': ('A', 'B'),  # Two Hearing-aid programs
                   'CoSS': [f'C{i}' for i in range(1, 8)],  # Seven CoSS categories
                   }  # Categorical variables
-    # NOTE: First situation dimension is always phase, even if only ONE phase category.
+    # NOTE: One situation dimension is always phase, even if only ONE phase category.
     # User may set arbitrary phase_key label.
     # Dimension 'Phase' may be omitted, if only one phase category.
     # Category labels may be strings or integers, which can be used as part of file names.
     # If string labels are intended, avoid strings that can be interpreted as numbers,
     # because Pandas will read them as numbers by default.
 
     emf = EmaFrame.setup(situations=situations,
@@ -94,66 +104,59 @@
                                                 'Hard',
                                                 'Easy',
                                                 'Very Easy',
                                                 'Perfect'],
                                      'Comfort': ['Bad',
                                                  'Not Good',
                                                  'Not Bad',
-                                                 'Good']}
+                                                 'Good']},
+                         groups={'Age': ['young', 'old'],
+                                 # 'Gender': ('M', 'F'),
+                                 }
                          )
-    # NOTE: situations and attributes keys will be parts of result file names,
+    # NOTE: situations, attributes, and groups keys will be parts of result file names,
     # so they can include only characters allowed in file names.
 
-    # NOTE: situations and attributes always analyzed as Categorical variables,
+    # NOTE: situations, attributes, and groups are always analyzed as Categorical variables,
     # even if the categories / grades are defined by numeric labels.
-    # The rank order of attribute grades is defined by the order as listed here,
+    # The rank order of attribute grades is defined by the order given in EmaFrame.setup(...),
     # NOT by, e.g., alphabetical or numerical order of the grade labels.
 
-    # NOTE: if EQUAL grades are used for more than one attribute,
+    # NOTE: if EQUAL grade labels are used for more than one attribute,
     # the model still assumes separate rating scales for each attribute.
     # However, if grade sequences are IDENTICAL objects for more than one attribute,
     # the model uses the SAME rating scale for those attributes.
     #
     # Example:
     # common_ordinal_scale = ['Very Hard',
     #                         'Hard',
     #                         'Easy',
     #                         'Very Easy',
     #                         'Perfect']
     # emf = EmaFrame.setup(situations=situations,
     #                      phase_key='Phase',
-    #                      attributes={'Speech': common_ordinal_scale,
-    #                                  'Comfort': common_ordinal_scale}  # SAME scale for both attributes
+    #                      attributes={'Speech': common_ordinal_scale,  # IDENTICAL scale object for both
+    #                                  'Comfort': common_ordinal_scale}
     #                      )
 
     # In either case, response thresholds are always estimated separately for each participant.
 
     # ------ 2: Load data from previously saved file(s):
 
-    # NOTE: if 'grouping' is defined, group directory names must match given labels,
-    # as exemplified in module ema_data doc-string.
-    # With template example: data_path / 'Age_old' is top of directory tree with data files.
-    # If several 'grouping' factors are defined, the directory tree structure must match the factors.
-    # If no grouping is defined: data_path is top of directory tree with all data files
-
-    ds = EmaDataSet.load(emf, data_path,
-                         # fmt='csv',  # None: try any file format
-                         # grouping=None,  # default: include all participants as ONE unnamed group
-                         # grouping={'Age': ('old',),  # analyze only group Age=old
-                         #           },
-                         grouping={'Age': ('young','old')},  # analyze both Age groups separately
-                         # participant='file',  # default
-                         # participant='sheet',   # participant ID defined in xlsx sheet title, OR
-                         # participant='SubjectID',  # participant IDs defined in column 'SubjectID'
-                         # rename_cols={'Hearing Aid: 'HA'},  # dict with (file, new) column names
-                         # header=0,  # first table row shows column headers
-                         # converters={'Comfort': _recode_comfort, ...},  # user-defined mapping(s)
-                         # ... any additional arguments to Pandas read_xxx function, if needed
+    ds = EmaDataSet.load(emf, data_path, fmt='csv', participant='file',
+                         path_groups=['Age',  # find 'Age_old' or 'Age_young' in path string
+                                      ],
+                         # group_join_str='_'  # default in path-string
                          )
-    logger.info(f'Using data ds=\n{ds}')
+    # NOTE: if 'path_groups' elements are specified, group names in path string must match EXACTLY
+    # the labels specified in EmaFrame.setup(...,groups={...}), joined by group_join_str,
+    # e.g. with directory data_path / 'Age_old'
+    # containing data file(s) for group dimension = 'Age', category = 'old'
+
+    logger.info(f'Using data set ds=\n{ds}')
 
     # ----------------- (Optional) show rating counts for all participants
     for attr in emf.attribute_dtypes.keys():
         a_count = ds.attribute_grade_count(attr, groupby='HA')
         logger.info(str(attr) + '_grade_count:\n' + a_count.to_string())
         logger.info(str(attr) + ': sum grade_count= ' + f'{np.sum(a_count.to_numpy())}')
         # a_count.save(result_path / (str(attr) + '_grades.csv'))
@@ -162,16 +165,16 @@
     mean_grades = ds.attribute_grade_mean(groupby=('HA', 'CoSS'))
     mean_grades.save(result_path / 'Attribute_mean_grades.txt', float_format='%.2f')
     # mean_grades.save(result_path / 'Attribute_mean_grades.csv',
     #                  float_format='%.4f')  # if needed for other analysis
     logger.info(f'Attribute mean grades saved in {result_path}'
                 + '\nCAUTION: Mean values presume METRIC data, but attribute grades are only ORDINAL!')
 
-    # nap = ds.nap_table('HA', nap_cat=['A', 'B'], groupby=('CoSS',), p=0.95)  # grouped results
     nap = ds.nap_table('HA', nap_cat=['A', 'B'], p=0.95)  # aggregated across other situation dimensions
+    # nap = ds.nap_table('HA', nap_cat=['A', 'B'], groupby=('CoSS',), p=0.95)  # grouped results
     nap.save(result_path / 'NAP.txt', float_format='%.2f')  # pretty-formatted by Pandas
     # nap.save(result_path / 'NAP.tex', float_format='%.2f')  # for import to LaTeX doc.
     # nap.save(result_path / 'NAP.csv', sep='\t')  # tab-delimited text, for input to other program
     logger.info(f'NAP results saved in {result_path}')
 
     # ------ 3: Learn Analysis Model from loaded data set:
 
@@ -184,39 +187,38 @@
 
     regression_effects = [('HA', 'CoSS')  # joint effects, main AND interaction
                           # 'Phase',  # if there are several phase categories
                           ]
 
     # NOTE: A regression_effects element may include any combination of situation dimensions, BUT
     # including ALL interactions -> many model parameters,
-    # possibly -> less precise estimation for each parameter.
+    # possibly -> less reliable estimation for each parameter.
 
     # In this example: ['HA', 'CoSS'] -> 2 + (7 - 1) = 8 regression-effect parameters
     #                ['CoSS', 'HA'] -> 7 + (2 - 1) = 8 regression-effect parameters
     #                [('HA', 'CoSS')] -> 2 * 7 = 14 regression-effect parameters
 
     emm = EmaModel.initialize(ds,
                               effects=regression_effects,
-                              max_n_comp=10,
-                              restrict_attribute=False,  # default
-                              restrict_threshold=True,  # default
+                              # n_participants_per_comp=5,  # default
+                              # restrict_attribute=False,  # default
+                              # restrict_threshold=True,  # default
                               # seed=12345  # ONLY if reproducible results are required
                               )
-    # max_n_comp = max number of mixture components in population model
+    # n_participants_per_comp = initial number of participants per mixture component in population model
     # restrict_attribute=True -> force attribute mean location at zero
-    # restrict_threshold=True -> force mid-scale response threshold at zero
-    # for each respondent and each sample of each attribute
+    # restrict_threshold=True -> force one mid-scale response threshold at zero
+    # for each respondent and each sample of each attribute.
 
     ll = emm.learn(max_hours=1., max_minutes=0.)
-    logger.info('ll= ' + np.array2string(np.array(ll),
-                                         precision=5))
+    logger.info(f'*** Data log-likelihood = {ll[-1]:.1f}, indicating model fit to data. ***')
+    # *** Recommended to re-run model learning with same data set a couple of times,
+    # and then use best-fitting model result.
+
     emm.prune()  # keep only active mixture components.
-    # NOTE: If the number of components is not reduced,
-    # it might be a good idea to re-run with larger initial max_n_comp,
-    # but max_n_comp always <= half number of participants
 
     # -------- Save learned EmaModel (optional):
     with (work_path / model_file).open('wb') as f:
         pickle.dump(emm, f)
         logger.info('Model pickle-dumped as ' + f.name)
 
     # ------ 4: Generate result displays:
@@ -226,28 +228,27 @@
     #     emm = pickle.load(f)
     # -------------------------------------------------
     emd = EmaDisplaySet.show(emm,
                              situations=['CoSS',  # CoSS probabilities, aggregated across HA
                                          ('CoSS', 'HA'),  # CoSS probabilities, conditional on HA
                                          ('HA', 'CoSS'),  # HA probabilities, conditional on CoSS
                                          ],
-                             attributes=[('Speech', 'CoSS'),  # Speech, main effect of CoSS
-                                         ('Speech', 'HA'),    # Speech, main effect of HA
-                                         ('Speech', ('CoSS', 'HA')),  # joint effect of both
+                             attributes=[('Speech', 'CoSS'),    # Speech, main effect of CoSS
+                                         ('Speech', 'HA'),      # Speech, main effect of HA
+                                         ('Speech', ('CoSS', 'HA')),    # joint effect of both
                                          ('Comfort', ('CoSS', 'HA'))],  # joint effect of both
-                             grade_counts=['Speech',
-                                           ('Speech', 'HA'),
-                                           ('Comfort', 'HA')],  # *** version 0.9.5 ***
-                             random_individual=True,  # random individual in population
-                             population_mean=True,  # population mean
-                             participants=False,  # individual results: True -> MANY plots and tables
-                             grade_thresholds=True,  # response thresholds in attribute plots
-                             percentiles=[2.5, 25, 50, 75, 97.5],  # in profile plots and tables
-                             credibility_limit=0.7,  # minimum credibility in difference tables
-                             # n_samples=10000,  # default=1000, for percentile calculations
+                             grade_counts=['Speech',  # total 'Speech' grade-counts, sum across HA and CoSS
+                                           ('Speech', 'HA'),    # 'Speech' grade-counts, separated by HA
+                                           ('Comfort', 'HA')],
+                             random_individual=True,    # random individual in population
+                             population_mean=True,      # population mean
+                             participants=False,        # individual results: True -> MANY plots and tables
+                             grade_thresholds=True,     # True -> median response thresholds in attribute plots
+                             percentiles=[2.5, 25, 50, 75, 97.5],   # in profile plots and tables
+                             credibility_limit=0.7,     # minimum credibility in difference tables
                              mpl_params={'figure.max_open_warning': 0,
                                          'axes.labelsize': 'x-large'},  # -> matplotlib.rcParam
                              # mpl_style='my_style_sheet',
                              # ... any other ema_display.FMT or ema_display_format.FMT settings
                              )
     # NOTE: joint (=interaction) effects are correct only if included in model regression_effects
 
@@ -257,24 +258,18 @@
                         g_disp.random_individual.attributes[('Speech', ('CoSS', 'HA'))].plot.ax,
                         g_disp.population_mean.attributes[('Comfort', ('CoSS', 'HA'))].plot.ax,
                         g_disp.random_individual.attributes[('Comfort', ('CoSS', 'HA'))].plot.ax
                         ])
         harmonize_ylim([g_disp.population_mean.situations[('CoSS', 'HA')].plot.ax,
                         g_disp.random_individual.situations[('CoSS', 'HA')].plot.ax,
                         ])
-
     # -> matching y-axis limits: nice for plots to be shown side by side
 
     # ------------------------------- save all result displays
-    emd.save(result_path,
-             figure_format='pdf',   # or any other format allowed by Matplotlib
-             table_format='txt',    # or csv, tex, xlsx, or other allowed by ema_file and Pandas
-                                    # NOTE: tex requires jinja2 to be installed manually
-             float_format='%.2f',   # any other parameters for Pandas table-writer function
-             )
+    emd.save(result_path, figure_format='pdf', table_format='txt', float_format='%.2f')
     # (optionally) save in other format(s), too:
     # emd.save(result_path,
     #          table_format='csv',  # for input to other package
     #          float_format='%.4f',  # any other parameters for Pandas table-writer function
     #          # sep='\t'  # -> tab-delimited
     #          )
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc/run_sim.py` & `EmaCalc-1.0.0/src/EmaCalc/run_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 Given some anticipated true effect-sizes in the patterns of population characteristics,
 the simulation will indicate whether these effects can be reliably demonstrated
 in a planned study, given the limited number of participants,
 and the limited number of EMA recordings by each participant.
 
 
 *** Version history:
+* Version 1.0.0:
+2023-05-17, EmaModel.initialize(..., n_participants_per_comp, ...) defines initial number of GMM components.
+            Parameter max_n_comp no longer used.
+2023-04-23, Adapted to simplified group-key representation in ema_data.EmaFrame.
+            NOTE: changed signatures EmaFrame.setup(), EmaDataSet.load(), and .save().
+
 * Version 0.9.3:
 2022-08-17, minor cleanup adapting to minor changes in some package modules.
 
 * Version 0.9.1:
 2022-04-04, all result tables generated and saved as Pandas DataFrame instances
 2022-03-27, NAP and mean-grades results directly from raw data in ema_data.EmaDataSet
 2022-03-21, using Pandas DataFrame format in EmaDataSet, allowing many input file formats
@@ -56,15 +62,15 @@
 
     from EmaCalc.ema_data import EmaFrame, EmaDataSet
     from EmaCalc.ema_model import EmaModel
     from EmaCalc.ema_display import EmaDisplaySet
     from EmaCalc import ema_logging, __version__
     from EmaCalc.ema_display_format import harmonize_ylim
 
-    # ------------ (optional) Set simulator random seed for reproducible results
+    # ------------ (optional) Set simulator random seed for reproducible data generation
     # from EmaCalc.ema_simulation import set_sim_seed
     # set_sim_seed(12345)  # for reproducible results. ONLY FOR TEST OR DEMO
 
     # ------------------------ Set up working directory and result logging:
     work_path = Path.home() / 'Documents' / 'EMA_sim'  # or whatever...
     data_path = work_path / 'data'  # or whatever
     result_path = work_path / 'result'  # or whatever
@@ -76,32 +82,35 @@
                       log_file='run_sim_log.txt')  # to save the log file
 
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.INFO)
 
     logger.info(f'*** Running EmaCalc version {__version__} ***')
 
-    # --------------- Define Experimental Framework: Situations, Attributes, and Grades
+    # ------ 1: Define Experimental Framework: Situations, Attributes, and Groups
 
     emf = EmaFrame.setup(situations={'Phase': ('',),  # Test phase(s), only one unlabelled
                                      'HA': ('A', 'B'),  # two Hearing-aid programs
                                      'CoSS': [f'C{i}' for i in range(1, 8)],  # Seven CoSS categories
                                      },
                          phase_key='Phase',
                          attributes={'Speech': ['Very Hard',
                                                 'Hard',
                                                 'Easy',
                                                 'Very Easy',
                                                 'Perfect'],
                                      'Comfort': ['Bad',
                                                  'Not Good',
                                                  'Not Bad',
-                                                 'Good']}
+                                                 'Good']},
+                         groups = {'Age': ['young', 'old'],
+                                   'Gender': ['X'], # single category, just as example
+                                   }    # -> only TWO distinct groups
                          )
-    # NOTE: situations and attributes keys will be parts of result file names,
+    # NOTE: situations and attributes and group keys will be parts of result file names,
     # so they can include only characters allowed in file names.
 
     # NOTE: situations and attributes always analyzed as Categorical variables,
     # even if the categories / grades are defined by numeric values.
     # The rank order of attribute grades is defined by the order as listed here,
     # not by, e.g., alphabetical or numerical order of the grade labels.
 
@@ -157,20 +166,20 @@
                              # subject_class=SubjectBradley,  # default
                              id='Pop1'
                              )
     # with SAME EmaFrame, but different situation_prob and/or mean Attribute values
 
     # ------------------ Generate Experiment with one Group of participants sampled from each Population:
     ema_exp = EmaSimExperiment(emf,
-                               groups={(('Age', 'old'),): pop_0.gen_group(n_participants=20),
-                                       (('Age', 'young'),): pop_1.gen_group(n_participants=15)
+                               groups={('old', 'X'): pop_0.gen_group(n_participants=20),
+                                       ('young', 'X'): pop_1.gen_group(n_participants=15)
                                        })
-    # NOTE: group keys MUST be a tuple of one or more PAIRS (g_factor, g_category)
-    # because groups may be defined hierarchically
-    #
+    # NOTE: group keys MUST be a tuple of one group category from each group dimension,
+    #   as defined in EmaFrame.setup()
+
     logger.info(f'ema_exp= {ema_exp}')
     # ema_exp defines true parameter values for Population(s) and all participants in each Group
 
     # -------- (Optional) Save EmaSimExperiment instance with true parameter values
     data_path.mkdir(parents=True, exist_ok=True)
     with (data_path / experiment_file).open('wb') as f:
         pickle.dump(ema_exp, f)
@@ -180,18 +189,15 @@
 
     ds = ema_exp.gen_dataset(min_ema=30,    # min n of EMA records per participant
                              max_ema=70)    # max n of EMA records per participant
     # = a complete EmaDataSet instance with simulated EMA records for all participants
 
     # Optionally, save all data in a set of data files, one for each participant
     file_format = 'csv'  # 'xlsx', or other format that Pandas can handle
-    ds.save(data_path, allow_over_write=True, fmt=file_format,
-            # participant='file',  # default for all file formats
-            # participant='sheet',  # participant ID stored in xlsx sheet title
-            )
+    ds.save(data_path, fmt=file_format, allow_over_write=True)
     logging.info('Simulated EMA data saved in ' + str(data_path) + f' as {file_format} files')
 
     # ----------------- (Optional) show mean grades and NAP results for all participants
 
     mean_grades = ds.attribute_grade_mean(groupby=('HA', 'CoSS'))
     mean_grades.save(result_path / 'Attribute_mean_grades.txt', float_format='%.2f')
     # mean_grades.save(result_path / 'Attribute_mean_grades.csv')  # for input to other analysis
@@ -204,82 +210,82 @@
     # nap.save(result_path / 'NAP.csv')  # for input to other analysis
     logger.info(f'NAP results saved in {result_path}')
 
     # ------------------------------- Learn Analysis Model from simulated data set:
 
     # -------- Test re-loading simulated data from saved files (optional):
     logging.info('Simulated EMA data re-loaded from ' + str(data_path) + f' as {file_format} files')
-    ds = EmaDataSet.load(emf, data_path,
-                         fmt=file_format,
-                         # grouping=None,  # default: include all participants as ONE unnamed group
-                         # grouping={'Age': ('old',),  # analyze only Age=old
-                         #           },
-                         grouping={'Age': ('young','old')},  # analyze both Age groups separately
-                         participant='file',  # 'sheet' only for Excel-style file formats
-                         )
+    ds = EmaDataSet.load(emf, data_path, fmt=file_format,
+                         participant='file',
+                         path_groups=['Age', 'Gender'])
 
     logger.info(f'Using data ds=\n{ds}')
 
     # Model ordinal-regression effects of situations on each Attribute:
     # regression_effects = ['HA',     # main linear regression effect only
     #                       'CoSS',   # main linear regression effect only
     #                       # 'Phase',  # if there are several phase categories
     #                       ]
     regression_effects = [('HA', 'CoSS')  # joint effects, main AND interaction
                           # 'Phase',  # if there are several phase categories
                           ]
-    # NOTE: regression effects may include any combination of situation dimensions, but
-    # including ALL interactions -> MANY model parameters,
-    # possibly -> less precise estimation for each parameter.
+    # NOTE: A regression_effects element may include any combination of situation dimensions, BUT
+    # including ALL interactions -> many model parameters,
+    # possibly -> less reliable estimation for each parameter.
 
     # In this example: ['HA', 'CoSS'] -> 2 + (7 - 1) = 8 regression-effect parameters
     #                ['CoSS', 'HA'] -> 7 + (2 - 1) = 8 regression-effect parameters
     #                [('HA', 'CoSS')] -> 2 * 7 = 14 regression-effect parameters
 
     emm = EmaModel.initialize(ds,
                               effects=regression_effects,
-                              max_n_comp=10,
+                              # n_participants_per_comp=5,  # default
                               restrict_attribute=False,  # default
                               restrict_threshold=True,   # default
                               # seed=12345  # ONLY if reproducible results are required
                               )
     # max_n_comp = max number of mixture components in population model
     # restrict_attribute=True -> force attribute mean location at zero
-    # restrict_threshold=True -> force mid-scale response threshold at zero
+    # restrict_threshold=True -> force one mid-scale response threshold at zero
     # for each respondent and each sample of each attribute
 
     ll = emm.learn(max_hours=2., max_minutes=0.)
-    logger.info('ll= ' + np.array2string(np.array(ll), precision=5))
+    logger.info(f'*** Data log-likelihood = {ll[-1]:.1f}, indicating model fit to data. ***')
+    # *** Recommend re-run model learning with same data set a couple of times, use best-fitting model result.
+
     emm.prune()  # keep only active mixture components
 
     # -------- Save learned EmaModel instance (optional):
     with (work_path / model_file).open('wb') as f:
         pickle.dump(emm, f)
 
     # ------------------------------- generate all result displays:
 
     emd = EmaDisplaySet.show(emm,
-                             situations=['CoSS',  # CoSS profile, aggregated across HA
-                                         ('CoSS', 'HA'),  # CoSS profiles, conditional on HA
-                                         ('HA', 'CoSS'),  # HA profiles, conditional on CoSS
+                             situations=['CoSS',  # CoSS probabilities, aggregated across HA
+                                         ('CoSS', 'HA'),  # CoSS probabilities, conditional on HA
+                                         ('HA', 'CoSS'),  # HA probabilities, conditional on CoSS
                                          ],
-                             attributes=[('Speech', 'CoSS'),     # Speech, main effect of CoSS
-                                         ('Speech', 'HA'),       # Speech, main effect of HA
+                             attributes=[('Speech', 'CoSS'),    # Speech, main effect of CoSS
+                                         ('Speech', 'HA'),      # Speech, main effect of HA
                                          ('Speech', ('CoSS', 'HA')),    # joint effect of both
                                          ('Comfort', ('CoSS', 'HA'))],  # joint effect of both
-                             random_individual=True,  # random individual in the population
-                             population_mean=True,  # population mean
-                             participants=True,  # individual results: True -> MANY plots and tables
-                             grade_thresholds=True,  # response thresholds in attribute plots
-                             percentiles=[2.5, 25, 50, 75, 97.5],  # in profile plots and tables
-                             credibility_limit=0.7,  # minimum credibility in difference tables
+                             grade_counts=['Speech',  # total 'Speech' grade-counts, sum across HA and CoSS
+                                           ('Speech', 'HA'),    # 'Speech' grade-counts, separated by HA
+                                           ('Comfort', 'HA')],
+                             random_individual=True,    # random individual in population
+                             population_mean=True,      # population mean
+                             participants=False,        # individual results: True -> MANY plots and tables
+                             grade_thresholds=True,     # True -> median response thresholds in attribute plots
+                             percentiles=[2.5, 25, 50, 75, 97.5],   # in profile plots and tables
+                             credibility_limit=0.7,     # minimum credibility in difference tables
                              mpl_params={'figure.max_open_warning': 0,
                                          'axes.labelsize': 'x-large'},  # -> matplotlib.rcParam
                              # mpl_style='my_style_sheet',
-                             # ... any other ema_display.FMT settings
+                             # ... any other ema_display.FMT or ema_display_format.FMT settings
                              )
     # NOTE: joint (=interaction) effects are correct only if included in EmaModel regression effects
 
     # ------------------------------- (optionally) edit display elements, if desired
     for g_disp in emd.groups.values():
         harmonize_ylim([g_disp.population_mean.attributes[('Speech', ('CoSS', 'HA'))].plot.ax,
                         g_disp.random_individual.attributes[('Speech', ('CoSS', 'HA'))].plot.ax,
@@ -287,19 +293,15 @@
                         g_disp.random_individual.attributes[('Comfort', ('CoSS', 'HA'))].plot.ax
                         ])
         harmonize_ylim([g_disp.population_mean.situations[('CoSS', 'HA')].plot.ax,
                         g_disp.random_individual.situations[('CoSS', 'HA')].plot.ax,
                         ])
 
     # ------------------------------- save all result displays
-    emd.save(result_path,
-             figure_format='pdf',  # or any other format allowed by Matplotlib
-             table_format='txt',  # or any other format allowed by Pandas
-             float_format='%.2f',  # any other parameters for Pandas table-writer function
-             )
+    emd.save(result_path, figure_format='pdf', table_format='txt', float_format='%.2f')
     # (optionally) save in other format(s), too:
     # emd.save(result_path,
     #          table_format='csv',  # for input to other package
     #          float_format='%.4f',  # any other parameters for Pandas table-writer function
     #          # sep='\t'  # -> tab-delimited
     #          )
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc.egg-info/PKG-INFO` & `EmaCalc-1.0.0/src/EmaCalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmaCalc
-Version: 0.9.6
+Version: 1.0.0
 Summary: Statistical Analysis of Ecological Momentary Assessment (EMA) Data
 Author: Arne Leijon
 Author-email: leijon@kth.se
 License: MIT License
 Keywords: Momentary Assessment,Nominal Categories,Ordinal Ratings,Bayesian
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `EmaCalc-0.9.6/src/EmaCalc.egg-info/SOURCES.txt` & `EmaCalc-1.0.0/src/EmaCalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

