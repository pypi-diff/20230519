# Comparing `tmp/estival-0.2.4.tar.gz` & `tmp/estival-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estival-0.2.4.tar", max compression
+gzip compressed data, was "estival-0.2.5.tar", max compression
```

## Comparing `estival-0.2.4.tar` & `estival-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3458 2023-05-10 03:44:23.083361 estival-0.2.4/estival/calibration/__pycache__/pymc.cpython-310.pyc
--rw-r--r--   0        0        0     4772 2023-05-06 03:26:51.437183 estival-0.2.4/estival/calibration/__pycache__/pymc.cpython-311.pyc
--rw-r--r--   0        0        0    14995 2023-05-05 04:48:51.863477 estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc
--rw-r--r--   0        0        0    25353 2023-05-05 05:24:17.406283 estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc
--rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
--rw-r--r--   0        0        0     2324 2023-05-05 04:48:54.568004 estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc
--rw-r--r--   0        0        0     3213 2023-05-05 05:24:18.633294 estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc
--rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
--rw-r--r--   0        0        0     3211 2023-05-05 04:48:54.551505 estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc
--rw-r--r--   0        0        0     5303 2023-05-05 05:24:18.606294 estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc
--rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
--rw-r--r--   0        0        0    23290 2023-05-03 06:12:36.018586 estival-0.2.4/estival/calibration/mcmc/adaptive.py
--rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.4/estival/calibration/mcmc/covariance.py
--rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.4/estival/calibration/mcmc/transformations.py
--rw-r--r--   0        0        0     3080 2023-05-11 03:41:35.661930 estival-0.2.4/estival/calibration/pymc.py
--rw-r--r--   0        0        0     2683 2023-05-11 02:56:54.916427 estival-0.2.4/estival/model.py
--rw-r--r--   0        0        0     2666 2023-05-03 21:37:51.092087 estival-0.2.4/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
--rw-r--r--   0        0        0     4511 2023-05-05 05:24:18.926797 estival-0.2.4/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
--rw-r--r--   0        0        0     2635 2023-05-03 21:00:19.800964 estival-0.2.4/estival/optimization/nevergrad.py
--rw-r--r--   0        0        0     4222 2023-05-10 03:48:52.052508 estival-0.2.4/estival/priors.py
--rw-r--r--   0        0        0    11364 2023-05-11 02:58:25.406441 estival-0.2.4/estival/targets.py
--rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.4/estival/utils.py
--rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.4/LICENSE
--rw-r--r--   0        0        0     1034 2023-05-11 03:44:56.420364 estival-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      522 2023-05-11 03:57:10.793592 estival-0.2.4/README.md
--rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 estival-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3458 2023-05-18 00:47:35.180316 estival-0.2.5/estival/calibration/__pycache__/pymc.cpython-310.pyc
+-rw-r--r--   0        0        0     4772 2023-05-06 03:26:51.437183 estival-0.2.5/estival/calibration/__pycache__/pymc.cpython-311.pyc
+-rw-r--r--   0        0        0    14995 2023-05-05 04:48:51.863477 estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc
+-rw-r--r--   0        0        0    25353 2023-05-05 05:24:17.406283 estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc
+-rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
+-rw-r--r--   0        0        0     2324 2023-05-05 04:48:54.568004 estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc
+-rw-r--r--   0        0        0     3213 2023-05-05 05:24:18.633294 estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc
+-rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
+-rw-r--r--   0        0        0     3211 2023-05-05 04:48:54.551505 estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc
+-rw-r--r--   0        0        0     5303 2023-05-05 05:24:18.606294 estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc
+-rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
+-rw-r--r--   0        0        0    23290 2023-05-03 06:12:36.018586 estival-0.2.5/estival/calibration/mcmc/adaptive.py
+-rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.5/estival/calibration/mcmc/covariance.py
+-rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.5/estival/calibration/mcmc/transformations.py
+-rw-r--r--   0        0        0     3080 2023-05-11 03:41:35.661930 estival-0.2.5/estival/calibration/pymc.py
+-rw-r--r--   0        0        0     2683 2023-05-11 02:56:54.916427 estival-0.2.5/estival/model.py
+-rw-r--r--   0        0        0     2666 2023-05-03 21:37:51.092087 estival-0.2.5/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
+-rw-r--r--   0        0        0     4511 2023-05-05 05:24:18.926797 estival-0.2.5/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
+-rw-r--r--   0        0        0     2635 2023-05-03 21:00:19.800964 estival-0.2.5/estival/optimization/nevergrad.py
+-rw-r--r--   0        0        0     4222 2023-05-10 03:48:52.052508 estival-0.2.5/estival/priors.py
+-rw-r--r--   0        0        0    11486 2023-05-19 02:24:52.265480 estival-0.2.5/estival/targets.py
+-rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.5/estival/utils.py
+-rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1034 2023-05-19 02:26:27.177228 estival-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-05-19 02:26:51.906422 estival-0.2.5/README.md
+-rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 estival-0.2.5/PKG-INFO
```

### Comparing `estival-0.2.4/estival/calibration/__pycache__/pymc.cpython-310.pyc` & `estival-0.2.5/estival/calibration/__pycache__/pymc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 03:44:00 2023 UTC, .py size: 3187 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0013 5b64 730c 0000  o.........[ds...
+00000000: 6f0d 0d0a 0000 0000 ef63 5c64 080c 0000  o........c\d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d05 5a06 0100 6400 6402 6c07  d.l.m.Z...d.d.l.
 00000050: 6d08 5a08 0100 6400 6401 6c09 5a09 6403  m.Z...d.d.l.Z.d.
 00000060: 6508 6602 6404 6405 8404 5a0a 640c 6403  e.f.d.d...Z.d.d.
 00000070: 6508 6407 650b 6604 6408 6409 8405 5a0c  e.d.e.f.d.d...Z.
```

### Comparing `estival-0.2.4/estival/calibration/__pycache__/pymc.cpython-311.pyc` & `estival-0.2.5/estival/calibration/__pycache__/pymc.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc` & `estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/adaptive.py` & `estival-0.2.5/estival/calibration/mcmc/adaptive.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/covariance.py` & `estival-0.2.5/estival/calibration/mcmc/covariance.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/mcmc/transformations.py` & `estival-0.2.5/estival/calibration/mcmc/transformations.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/calibration/pymc.py` & `estival-0.2.5/estival/calibration/pymc.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/model.py` & `estival-0.2.5/estival/model.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/optimization/__pycache__/nevergrad.cpython-310.pyc` & `estival-0.2.5/estival/optimization/__pycache__/nevergrad.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/optimization/__pycache__/nevergrad.cpython-311.pyc` & `estival-0.2.5/estival/optimization/__pycache__/nevergrad.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/optimization/nevergrad.py` & `estival-0.2.5/estival/optimization/nevergrad.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/priors.py` & `estival-0.2.5/estival/priors.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/estival/targets.py` & `estival-0.2.5/estival/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
 
     @abstractmethod
     def get_evaluator(self, model_times: pd.Index, epoch: Epoch) -> TargetEvaluator:
         raise NotImplementedError()
 
 
 class TargetEvaluator(ABC):
-    def __init__(self, target: BaseTarget, model_times: pd.Index, epoch: Epoch=None):
-
+    def __init__(self, target: BaseTarget, model_times: pd.Index, epoch: Epoch = None):
         if not isinstance(target.data.index, pd.DatetimeIndex):
             if epoch is not None:
                 model_times = epoch.dti_to_index(model_times)
         else:
             if epoch is None:
                 raise Exception("Target data expressed as datetime but no ref_date set for model")
 
@@ -142,17 +141,18 @@
         self,
         name: str,
         data: pd.Series,
         sample_sizes: pd.Series,
         weight: float = 1.0,
         time_weights: pd.Series = None,
     ):
-        super().__init__(name, data, weight, time_weights)
+        # Enforce floats for data and sample_sizes so TFP doesn't complain later
+        super().__init__(name, data.astype(float), weight, time_weights)
         self._data_attrs = ["sample_sizes"]
-        self.sample_sizes = sample_sizes
+        self.sample_sizes = sample_sizes.astype(float)
 
     def get_evaluator(self, model_times: pd.Index, epoch: Epoch) -> TargetEvaluator:
         return BinomialEvaluator(self, model_times, epoch)
 
 
 class BinomialEvaluator(TargetEvaluator):
     def __init__(self, target: BaseTarget, model_times: pd.Index, epoch: Epoch):
@@ -162,15 +162,15 @@
 
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         from tensorflow_probability.substrates import jax as tfp
 
         # use a binomial (n, p) where n is the sample size observed in the data and p the modelled proportion
         # We then evaluate the binomial density for k, which represents the numerator observed in the data
         n = self.target.sample_sizes
-        p = modelled
+        p = modelled[self.index]
         k = self.target.data * n
 
         bdist = tfp.distributions.Binomial(total_count=n, probs=p)
         ll = bdist.log_prob(k)
 
         if self.time_weights is not None:
             ll = ll * self.time_weights
```

### Comparing `estival-0.2.4/estival/utils.py` & `estival-0.2.5/estival/utils.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/LICENSE` & `estival-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `estival-0.2.4/pyproject.toml` & `estival-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "estival"
-version = "0.2.4"
+version = "0.2.5"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/estival"
 repository = "https://github.com/monash-emu/estival"
 documentation = "https://github.com/monash-emu/estival"
 keywords = [
     "calibration",
```

### Comparing `estival-0.2.4/README.md` & `estival-0.2.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 
 - 0.2.2  
 Add logprior/logposterior to BayesianCompartmentalModel
 - 0.2.3  
 Include tensorflow-probability(jax) for more (and better tested) stats modules
 - 0.2.4
 Bugfix (vector priors were not exported to pymc correctly)
-Add Epoch support to allow DatetimeIndex targets
+Add Epoch support to allow DatetimeIndex targets
+- 0.2.5
+Bugfix for BinomialTarget (wasn't indexing modelled data)
```

### Comparing `estival-0.2.4/PKG-INFO` & `estival-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estival
-Version: 0.2.4
+Version: 0.2.5
 Summary: A set of calibration and probabilistic programming tools for use with summerepi2
 Home-page: https://github.com/monash-emu/estival
 License: BSD-2-Clause
 Keywords: calibration,optimization,bayesian,compartmental modelling,summerepi
 Author: David Shipman
 Author-email: dshipman@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -39,7 +39,9 @@
 - 0.2.2  
 Add logprior/logposterior to BayesianCompartmentalModel
 - 0.2.3  
 Include tensorflow-probability(jax) for more (and better tested) stats modules
 - 0.2.4
 Bugfix (vector priors were not exported to pymc correctly)
 Add Epoch support to allow DatetimeIndex targets
+- 0.2.5
+Bugfix for BinomialTarget (wasn't indexing modelled data)
```

