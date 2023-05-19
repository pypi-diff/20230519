# Comparing `tmp/GOFevaluation-0.1.1.tar.gz` & `tmp/GOFevaluation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GOFevaluation-0.1.1.tar", last modified: Tue Jun  7 08:26:05 2022, max compression
+gzip compressed data, was "dist/GOFevaluation-0.1.2.tar", last modified: Fri May 19 18:02:48 2023, max compression
```

## Comparing `GOFevaluation-0.1.1.tar` & `GOFevaluation-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 08:26:05.000000 GOFevaluation-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 08:26:05.000000 GOFevaluation-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    14431 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/tests/test_evaluators_nd.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4692 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/tests/test_gof_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6459 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/tests/test_evaluators_1d.py
--rw-r--r--   0 runner    (1001) docker     (121)     5812 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 08:26:05.000000 GOFevaluation-0.1.1/GOFevaluation/
--rw-r--r--   0 runner    (1001) docker     (121)    12641 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/GOFevaluation/evaluator_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/GOFevaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/GOFevaluation/evaluators_1d.py
--rw-r--r--   0 runner    (1001) docker     (121)     5805 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/GOFevaluation/gof_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    13194 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/GOFevaluation/evaluators_nd.py
--rw-r--r--   0 runner    (1001) docker     (121)    18459 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/GOFevaluation/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 08:26:05.000000 GOFevaluation-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/HISTORY.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 08:26:05.000000 GOFevaluation-0.1.1/GOFevaluation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-07 08:26:04.000000 GOFevaluation-0.1.1/GOFevaluation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 08:26:04.000000 GOFevaluation-0.1.1/GOFevaluation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-06-07 08:26:05.000000 GOFevaluation-0.1.1/GOFevaluation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8002 2022-06-07 08:26:04.000000 GOFevaluation-0.1.1/GOFevaluation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-07 08:26:04.000000 GOFevaluation-0.1.1/GOFevaluation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5511 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     8002 2022-06-07 08:26:05.000000 GOFevaluation-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-07 08:25:44.000000 GOFevaluation-0.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/GOFevaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/GOFevaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/GOFevaluation/evaluator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/GOFevaluation/evaluators_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/GOFevaluation/evaluators_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/GOFevaluation/gof_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/GOFevaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/GOFevaluation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/GOFevaluation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/GOFevaluation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/GOFevaluation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/GOFevaluation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/GOFevaluation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:02:48.000000 GOFevaluation-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/tests/test_evaluators_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/tests/test_evaluators_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/tests/test_gof_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-05-19 18:02:42.000000 GOFevaluation-0.1.2/tests/test_utils.py
```

### Comparing `GOFevaluation-0.1.1/tests/test_evaluators_nd.py` & `GOFevaluation-0.1.2/tests/test_evaluators_nd.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,23 @@
 
         for order in [[0, 1], [1, 0]]:
             gofclass_bin_equiprobable = BinnedPoissonChi2GOF.bin_equiprobable(
                 data_sample, reference_sample, nevents_expected=n_expected,
                 n_partitions=n_partitions, order=order)
             gof_bin_equiprobable = gofclass_bin_equiprobable.get_gof()
             self.assertAlmostEqual(gof_bin_equiprobable, gof_from_binned, 10)
+        # Test if equiprobable binning with weights=None
+        # and weights=np.ones give the same result
+        gofclass_bin_equiprobable = BinnedPoissonChi2GOF.bin_equiprobable(
+            data_sample, reference_sample, nevents_expected=n_expected,
+            n_partitions=n_partitions,
+            reference_sample_weights=np.ones(len(reference_sample)))
+        gof_bin_equiprobable_weighted = gofclass_bin_equiprobable.get_gof()
+        self.assertAlmostEqual(
+            gof_bin_equiprobable_weighted, gof_bin_equiprobable, 10)
 
 
 class TestPointToPointGOF(unittest.TestCase):
     def test_distances(self):
         # test if number of distance values is correct
         xs = np.linspace(0, 1, 100)
         xs_ref = np.linspace(0, 1, 200)
@@ -286,14 +295,23 @@
 
         for order in [[0, 1], [1, 0]]:
             gofclass_bin_equiprobable = BinnedChi2GOF.bin_equiprobable(
                 data_sample, reference_sample, nevents_expected=n_expected,
                 n_partitions=n_partitions, order=order)
             gof_bin_equiprobable = gofclass_bin_equiprobable.get_gof()
             self.assertAlmostEqual(gof_bin_equiprobable, gof_from_binned, 10)
+        # Test if equiprobable binning with weights=None
+        # and weights=np.ones give the same result
+        gofclass_bin_equiprobable = BinnedChi2GOF.bin_equiprobable(
+            data_sample, reference_sample, nevents_expected=n_expected,
+            n_partitions=n_partitions,
+            reference_sample_weights=np.ones(len(reference_sample)))
+        gof_bin_equiprobable_weighted = gofclass_bin_equiprobable.get_gof()
+        self.assertAlmostEqual(
+            gof_bin_equiprobable_weighted, gof_bin_equiprobable, 10)
 
 
 class TestPvalue(unittest.TestCase):
     def test_dimension_two_sample(self):
         """Test if p-value for two identical samples is 1
         for higher dimensional samples."""
         d_min = .00001
```

### Comparing `GOFevaluation-0.1.1/tests/test_gof_test.py` & `GOFevaluation-0.1.2/tests/test_gof_test.py`

 * *Files identical despite different names*

### Comparing `GOFevaluation-0.1.1/tests/test_evaluators_1d.py` & `GOFevaluation-0.1.2/tests/test_evaluators_1d.py`

 * *Files identical despite different names*

### Comparing `GOFevaluation-0.1.1/setup.py` & `GOFevaluation-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,31 +10,30 @@
     long_description = fh.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(
     name="GOFevaluation",
-    version="0.1.1",
+    version="0.1.2",
     author="GOFevaluation contributors, the XENON collaboration",
     description="Evaluate the Goodness-of-Fit(GoF) for binned or \
         unbinned data.",
     long_description=long_description + '\n\n' + history,
     long_description_content_type="text/markdown",
     setup_requires=['pytest-runner'],
     install_requires=requires,
     tests_require=requires + [
         'pytest',
         'flake8',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     url="https://github.com/XENONnT/GOFevaluation",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `GOFevaluation-0.1.1/GOFevaluation/evaluator_base.py` & `GOFevaluation-0.1.2/GOFevaluation/evaluator_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,15 +81,16 @@
                    pdf=binned_reference / np.sum(binned_reference),
                    bin_edges=None,
                    nevents_expected=np.sum(binned_reference))
 
     @classmethod
     def bin_equiprobable(cls, data_sample, reference_sample, nevents_expected,
                          n_partitions, order=None, plot=False,
-                         plot_mode='sigma_deviation', **kwargs):
+                         plot_mode='sigma_deviation',
+                         reference_sample_weights=None, **kwargs):
         """Initialize with data and reference sample that are binned
         such that the expectation value is the same in each bin.
         kwargs are passed to `plot_equiprobable_histogram` if plot is True.
         """
         check_sample_sanity(data_sample)
         check_sample_sanity(reference_sample)
         if len(reference_sample) < 50 * len(data_sample):
@@ -99,15 +100,18 @@
                 + f'({len(data_sample)}) to ensure negligible statistical '
                 + 'fluctuations for the equiprobable binning.', stacklevel=2)
 
         pdf, bin_edges = equiprobable_histogram(
             data_sample=reference_sample,
             reference_sample=reference_sample,
             n_partitions=n_partitions,
-            order=order)
+            order=order,
+            data_sample_weights=reference_sample_weights,
+            reference_sample_weights=reference_sample_weights,
+            **kwargs)
         pdf = pdf / np.sum(pdf)
 
         binned_data = apply_irregular_binning(
             data_sample=data_sample,
             bin_edges=bin_edges,
             order=order)
 
@@ -171,36 +175,44 @@
                           f'{min(fake_gofs):.2e}). For a more '
                           f'precise result, increase n_mc!', stacklevel=2)
 
         self.pvalue = pvalue
         return pvalue, fake_gofs
 
     def get_pvalue(self, n_mc=1000):
-        """p-value is calculated
+        """The approximate p-value is calculated.
 
         Computes the p-value by means of generating toyMCs and calculating
         their GoF. The p-value can then be obtained from the distribution of
         these fake-gofs.
 
+        Note that this is only an approximate method, since the model is not
+        refitted to the toy data. Especially with low statistics and many fit
+        parameters, this can introduce a bias towards larger p-values.
+
         :param n_mc: Number of fake-gofs calculated, defaults to 1000
         :type n_mc: int, optional
         :return: p-value
         :rtype: float
         """
         pvalue, _ = self._get_pvalue(n_mc=n_mc)
         return pvalue
 
     def get_pvalue_return_fake_gofs(self, n_mc=1000):
-        """p-value is calculated
+        """The approximate p-value is calculated.
 
         Computes the p-value by means of generating toyMCs and calculating
         their GoF. The p-value can then be obtained from the distribution of
         these fake-gofs. The array of fake-gofs is returned together with
         the p-value.
 
+        Note that this is only an approximate method, since the model is not
+        refitted to the toy data. Especially with low statistics and many fit
+        parameters, this can introduce a bias towards larger p-values.
+
         :param n_mc: Number of fake-gofs calculated, defaults to 1000
         :type n_mc: int, optional
         :return: p-value
         :rtype: float
         """
         pvalue, fake_gofs = self._get_pvalue(n_mc=n_mc)
         return pvalue, fake_gofs
@@ -272,49 +284,57 @@
         percentile = sps.percentileofscore(fake_gofs, self.gof, kind='strict')
         pvalue = 1 - percentile / 100
 
         if pvalue == 0:
             warnings.warn(f'p-value is 0.0. (Observed GoF: '
                           f'{self.gof:.2e}, maximum of simulated GoFs: '
                           f'{max(fake_gofs):.2e}). For a more '
-                          f'precise result, increase n_mc!', stacklevel=2)
+                          f'precise result, increase n_perm!', stacklevel=2)
         elif pvalue == 1:
             warnings.warn(f'p-value is 1.0. (Observed GoF '
                           f'{self.gof:.2e}, minimum of simulated GoFs: '
                           f'{min(fake_gofs):.2e}). For a more '
-                          f'precise result, increase n_mc!', stacklevel=2)
+                          f'precise result, increase n_perm!', stacklevel=2)
         self.pvalue = pvalue
 
         return pvalue, fake_gofs
 
     def get_pvalue(self, n_perm=1000, d_min=None):
-        """p-value is calculated
+        """The approximate p-value is calculated.
 
         Computes the p-value by means of re-sampling data sample
         and reference sample. For each re-sampling, the gof is calculated.
         The p-value can then be obtained from the distribution of these
         fake-gofs.
 
+        Note that this is only an approximate method, since the model is not
+        refitted to the re-sampled data. Especially with low statistics and
+        many fit parameters, this can introduce a bias towards larger p-values.
+
         :param n_perm: Number of fake-gofs calculated, defaults to 1000
         :type n_perm: int, optional
         :return: p-value
         :rtype: float
         """
         pvalue, _ = self._get_pvalue(n_perm=n_perm, d_min=d_min)
         return pvalue
 
     def get_pvalue_return_fake_gofs(self, n_perm=1000, d_min=None):
-        """p-value is calculated
+        """The approximate p-value is calculated.
 
         Computes the p-value by means of re-sampling data sample
         and reference sample. For each re-sampling, the gof is calculated.
         The p-value can then be obtained from the distribution of these
         fake-gofs. The array of fake-gofs is returned together with
         the p-value.
 
+        Note that this is only an approximate method, since the model is not
+        refitted to the re-sampled. Especially with low statistics and many fit
+        parameters, this can introduce a bias towards larger p-values.
+
         :param n_perm: Number of fake-gofs calculated, defaults to 1000
         :type n_perm: int, optional
 
         :return: p-value, fake_gofs
         :rtype: float
         """
         pvalue, fake_gofs = self._get_pvalue(n_perm=n_perm, d_min=d_min)
```

### Comparing `GOFevaluation-0.1.1/GOFevaluation/evaluators_1d.py` & `GOFevaluation-0.1.2/GOFevaluation/evaluators_1d.py`

 * *Files identical despite different names*

### Comparing `GOFevaluation-0.1.1/GOFevaluation/gof_test.py` & `GOFevaluation-0.1.2/GOFevaluation/gof_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import OrderedDict
 from inspect import signature
 import warnings
 
-from GOFevaluation.evaluators_1d import ADTestTwoSampleGOF
-from GOFevaluation.evaluators_1d import KSTestTwoSampleGOF
-from GOFevaluation.evaluators_nd import BinnedPoissonChi2GOF
-from GOFevaluation.evaluators_nd import BinnedChi2GOF
-from GOFevaluation.evaluators_nd import PointToPointGOF
+from GOFevaluation.evaluators_1d import ADTestTwoSampleGOF  # noqa: F401
+from GOFevaluation.evaluators_1d import KSTestTwoSampleGOF  # noqa: F401
+from GOFevaluation.evaluators_nd import BinnedPoissonChi2GOF  # noqa: F401
+from GOFevaluation.evaluators_nd import BinnedChi2GOF  # noqa: F401
+from GOFevaluation.evaluators_nd import PointToPointGOF  # noqa: F401
 
 
 class GOFTest(object):
     """This wrapper class is meant to streamline the creation of commonly used
     function calls of the package
 
     :param gof_list: list of strings referring to the gof measures from
@@ -119,15 +119,15 @@
             gof = func(**specific_kwargs)
             self.gofs[key] = gof
             kwargs_used += specific_kwargs.keys()
         self._check_kwargs_used(kwargs_used, kwargs)
         return self.gofs
 
     def get_pvalues(self, **kwargs):
-        """Calculate p-values for individual GoF measures.
+        """Calculate the approximate p-values for individual GoF measures.
 
         :param kwargs: All parameters from a get_pvalue method are viable kwargs.
             gof_list: A list of gof_measures for which p-value should be
             calculated. If none is given, the p-value is calculated for all
             GoF measures defined at initialisation.
         """
         kwargs_used = []  # check if all kwargs were used
```

### Comparing `GOFevaluation-0.1.1/GOFevaluation/evaluators_nd.py` & `GOFevaluation-0.1.2/GOFevaluation/evaluators_nd.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,16 @@
             :type nevents_expected: float
 
         - **unbinned data, bin with equiprobable binning**
         initialise with .bin_equiprobable(...)
             :param data_sample: sample of unbinned data
             :type data_sample: array_like, n-Dimensional
             :param reference_sample: sample of unbinned reference
-                (should have >50 samples than the data sample so that
-                statistical fluctuations are negligible.)
+                (should have at least 50 times larger than the data sample
+                to ensure that statistical fluctuations are negligible.)
             :type reference_sample: array_like, n-Dimensional
             :param nevents_expected: total number of expected events
             :type nevents_expected: float
             :param n_partitions: Number of partitions in each dimension
             :type n_partitions: list of int
             :param order: Order in which the partitioning is performed, defaults to None
                 [0, 1] : first bin x then bin y for each partition in x
@@ -88,15 +88,15 @@
         return gof
 
     def get_pvalue(self, n_mc=1000):
         return super().get_pvalue(n_mc)
 
 
 class BinnedChi2GOF(EvaluatorBaseBinned):
-    """Compoutes the binned chi2 GoF based on Pearson's chi2.
+    """Computes the binned chi2 GoF based on Pearson's chi2.
 
         - **unbinned data, bin with regular binning**
             :param data_sample: sample of unbinned data
             :type data_sample: array_like, n-Dimensional
             :param pdf: binned pdf to be tested
             :type pdf: array_like, n-Dimensional
             :param bin_edges: binning of the pdf
@@ -105,16 +105,16 @@
             :type nevents_expected: float
 
         - **unbinned data, bin with equiprobable binning**
         initialise with .bin_equiprobable(...)
             :param data_sample: sample of unbinned data
             :type data_sample: array_like, n-Dimensional
             :param reference_sample: sample of unbinned reference
-                (should have >50 samples than the data sample so that
-                statistical fluctuations are negligible.)
+                (should have at least 50 times larger than the data sample
+                to ensure that statistical fluctuations are negligible.)
             :type reference_sample: array_like, n-Dimensional
             :param nevents_expected: total number of expected events
             :type nevents_expected: float
             :param n_partitions: Number of partitions in each dimension
             :type n_partitions: list of int
             :param order: Order in which the partitioning is performed, defaults to None
                 [0, 1] : first bin x then bin y for each partition in x
@@ -301,21 +301,25 @@
 
         gof = self.calculate_gof(
             self.data_sample, self.reference_sample, d_min=d_min)
         self.gof = gof
         return gof
 
     def get_pvalue(self, n_perm=1000, d_min=None):
-        """p-value is calculated
+        """The approximate p-value is calculated.
 
         Computes the p-value by means of re-sampling data sample
         and reference sample. For each re-sampling, the gof is calculated.
         The p-value can then be obtained from the distribution of these
         fake-gofs.
 
+        Note that this is only an approximate method, since the model is not
+        refitted to the re-sampled data. Especially with low statistics and
+        many fit parameters, this can introduce a bias towards larger p-values.
+
         :param n_perm: Number of fake-gofs calculated, defaults to 1000
         :type n_perm: int, optional
         :param d_min: Replaces the distance for distance d < d_min.
             If None, d_min is estimated by :func:`get_dmin`,
             defaults to None
         :type d_min: float, optional
         :return: p-value
```

### Comparing `GOFevaluation-0.1.1/GOFevaluation/utils.py` & `GOFevaluation-0.1.2/GOFevaluation/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import warnings
 from matplotlib.patches import Rectangle
-from sklearn.preprocessing import KBinsDiscretizer
 import numpy as np
 import matplotlib as mpl
+import matplotlib.pyplot as plt
+from copy import deepcopy
 
 
 def equiprobable_histogram(data_sample, reference_sample, n_partitions,
-                           order=None, plot=False, **kwargs):
+                           order=None, plot=False, reference_sample_weights=None,
+                           data_sample_weights=None, **kwargs):
     """Define equiprobable histogram based on the reference sample and
     bin the data sample according to it.
     :param data_sample: Sample of unbinned data.
     :type data_sample: array
     :param reference_sample: sample of unbinned reference
     :type reference_sample: array_like, n-Dimensional
     :param n_partitions: Number of partitions in each dimension
@@ -17,45 +20,52 @@
     :param order: Order in which the partitioning is performed, defaults to None
         [0, 1] : first bin x then bin y for each partition in x
         [1, 0] : first bin y then bin x for each partition in y
         if None, the natural order, i.e. [0, 1] is used. For 1D just put None.
     :type order: list, optional
     :param plot: if True, histogram of data sample is plotted, defaults to False
     :type plot: bool, optional
+    :param reference_sample_weights: weights of reference_sample
+    :type reference_sample_weights: array_like, 1-Dimensional
+    :param data_sample_weights: weights of data_sample
+    :type data_sample_weights: array_like, 1-Dimensional
     :return: n, bin_edges
         n: number of counts of data sample in each bin
         bin_edges: For order [0, 1]([1, 0])
         these are the bin edges in x(y) and y(x) respectively. bin_edges[1]
         is a list of bin edges corresponding to the partitions defined in
         bin_edges[0].
     .. note::
         Reference: F. James, 2008: "Statistical Methods in Experimental
                     Physics", Ch. 11.2.3
     """
-    bin_edges = _get_equiprobable_binning(
+    check_dimensionality_for_eqpb(data_sample, reference_sample,
+                                  n_partitions, order)
+    bin_edges = get_equiprobable_binning(
         reference_sample=reference_sample, n_partitions=n_partitions,
-        order=order)
+        order=order, reference_sample_weights=reference_sample_weights)
     n = apply_irregular_binning(data_sample=data_sample,
                                 bin_edges=bin_edges,
-                                order=order)
+                                order=order,
+                                data_sample_weights=data_sample_weights)
     if plot:
         plot_equiprobable_histogram(data_sample=data_sample,
                                     bin_edges=bin_edges,
                                     order=order,
                                     **kwargs)
     return n, bin_edges
 
 
 def _get_finite_bin_edges(bin_edges, data_sample, order):
     """Replaces infinite values in bin_edges with finite
     values determined such that the bins encompass all
     the counts in data_sample. Necessary for plotting
     and for determining bin area.
     :param bin_edges: list of bin_edges,
-    probably form _get_equiprobable_binning
+    probably form get_equiprobable_binning
     :type bin_edges: array
     :param data_sample: Sample of unbinned data.
     :type data_sample: array
     :param order: Order in which the partitioning is performed,
     defaults to None
         [0, 1] : first bin x then bin y for each partition in x
         [1, 0] : first bin y then bin x for each partition in y
@@ -67,20 +77,20 @@
         respectively. bin_edges[1] is a list of bin edges corresponding to the
         partitions defined in bin_edges[0].
     :rtype: list of arrays
     """
     xlim, ylim = get_plot_limits(data_sample)
     be = []
     if len(data_sample.shape) == 1:
-        bin_edges[0] = xlim[0]
-        bin_edges[-1] = xlim[1]
-        be = [bin_edges.copy(), None]
+        be = [deepcopy(bin_edges), None]
+        be[0][0] = xlim[0]
+        be[0][-1] = xlim[1]
     else:
-        be_first = bin_edges[0].copy()
-        be_second = bin_edges[1].copy()
+        be_first = deepcopy(bin_edges[0])
+        be_second = deepcopy(bin_edges[1])
 
         if order == [0, 1]:
             be_first[be_first == -np.inf] = xlim[0]
             be_first[be_first == np.inf] = xlim[1]
             be_second[be_second == -np.inf] = ylim[0]
             be_second[be_second == np.inf] = ylim[1]
         elif order == [1, 0]:
@@ -130,111 +140,207 @@
                 ns[i][j] = ns[i][j] / ((high_f - low_f) * (high_s - low_s))
                 j += 1
             i += 1
 
     return ns
 
 
-def _get_equiprobable_binning(reference_sample, n_partitions, order=None):
+def _equi(n_bins, reference_sample):
+    """Perform a 1D equiprobable binning for reference_sample.
+    :param n_bins: number of partitions in this dimension
+    :type n_bins: int
+    :param reference_sample: sample of unbinned reference
+    :type reference_sample: array_like, 1-Dimensional
+    :return: Returns bin_edges.
+    :rtype: array_like, 1-Dimensional
+    """
+    bin_edges = np.quantile(reference_sample, np.linspace(0, 1, n_bins + 1)[1:-1])
+    bin_edges = np.hstack([-np.inf, bin_edges, np.inf])
+    return bin_edges
+
+
+def _weighted_equi(n_bins, reference_sample, reference_sample_weights):
+    """Perform a 1D equiprobable binning for reference_sample with weights.
+    :param n_bins: number of partitions in this dimension
+    :type n_bins: int
+    :param reference_sample: sample of unbinned reference
+    :type reference_sample: array_like, 1-Dimensional
+    :param reference_sample_weights: weights of reference_sample
+    :type reference_sample_weights: array_like, 1-Dimensional
+    :return: Returns bin_edges.
+    :rtype: array_like, 1-Dimensional
+    """
+    argsort = reference_sample.argsort()
+    reference_sample_weights = reference_sample_weights[argsort]
+    reference_sample = reference_sample[argsort]
+    cumsum = np.cumsum(reference_sample_weights)
+    cumsum -= cumsum[0]
+    bin_edges = np.interp(
+        np.linspace(0, 1, n_bins + 1)[1:-1],
+        cumsum / cumsum[-1],
+        reference_sample)
+    bin_edges = np.hstack([-np.inf, bin_edges, np.inf])
+    return bin_edges
+
+
+def get_equiprobable_binning(reference_sample, n_partitions,
+                             order=None, reference_sample_weights=None):
     """Define an equiprobable binning for the reference sample. The binning
     is defined such that the number of counts in each bin are (almost) equal.
     Bins are defined based on the ECDF of the reference sample.
     The number of partitions in x and y direction as well as the order of
     partitioning influence the result.
     :param reference_sample: sample of unbinned reference
     :type reference_sample: array_like, n-Dimensional
     :param n_partitions: Number of partitions in each dimension
     :type n_partitions: list of int
     :param order: Order in which the partitioning is performed, defaults to None
         [0, 1] : first bin x then bin y for each partition in x
         [1, 0] : first bin y then bin x for each partition in y
         if None, the natural order, i.e. [0, 1] is used. For 1D just put None.
     :type order: list, optional
+    :param reference_sample_weights: weights of reference_sample
+    :type reference_sample_weights: array_like, 1-Dimensional
     :return: Returns bin_edges.
         1D: list of bin edges
         2D: For order [0, 1]([1, 0]) these are the bin edges in x(y) and y(x)
         respectively. bin_edges[1] is a list of bin edges corresponding to the
         partitions defined in bin_edges[0].
     :rtype: list of arrays
     :raises ValueError: when an unknown order is passed.
     .. note::
         Reference: F. James, 2008: "Statistical Methods in Experimental
                     Physics", Ch. 11.2.3
     """
+    check_for_ties(reference_sample)
     if len(reference_sample.shape) == 1:
-        enc = KBinsDiscretizer(n_bins=n_partitions, encode='ordinal',
-                               strategy='quantile')
-        enc.fit(np.vstack(reference_sample.T))
-        bin_edges = enc.bin_edges_[0]
-        bin_edges[0] = -np.inf
-        bin_edges[-1] = np.inf
+        dim = 1
+    elif len(reference_sample.shape) == 2:
+        dim = 2
     else:
+        raise TypeError(f"reference_sample has unsupported shape {reference_sample.shape}.")
+
+    if reference_sample_weights is None:
+        weights_flag = 0
+    else:
+        _check_weight_sanity(reference_sample, reference_sample_weights)
+        weights_flag = 1
+    if dim == 1:
+        if weights_flag:
+            bin_edges = _weighted_equi(
+                n_partitions,
+                reference_sample,
+                reference_sample_weights)
+        else:
+            bin_edges = _equi(n_partitions, reference_sample)
+    elif dim == 2:
         if order is None:
             order = [0, 1]
-        # Define data that is binned first and second based on the order argument
-        first = np.vstack(reference_sample.T[order[0]])
-        second = np.vstack(reference_sample.T[order[1]])
-
-        # Get binning in first dimension:
-        enc = KBinsDiscretizer(n_bins=n_partitions[order[0]], encode='ordinal',
-                               strategy='quantile')
-        enc.fit(first)
-        bin_edges_first = enc.bin_edges_[0]
-        bin_edges_first[0] = -np.inf
-        bin_edges_first[-1] = np.inf
+        first = reference_sample.T[order[0]]
+        second = reference_sample.T[order[1]]
+        if weights_flag:
+            bin_edges_first = _weighted_equi(
+                n_partitions[order[0]],
+                first,
+                reference_sample_weights)
+        else:
+            bin_edges_first = _equi(n_partitions[order[0]], first)
 
         # Get binning in second dimension (for each bin in first dimension):
-        enc = KBinsDiscretizer(n_bins=n_partitions[order[1]], encode='ordinal',
-                               strategy='quantile')
         bin_edges_second = []
         for low, high in zip(bin_edges_first[:-1], bin_edges_first[1:]):
             mask = (first > low) & (first <= high)
-            enc.fit(np.vstack(second[mask]))
-            bin_edges = enc.bin_edges_[0]
-            bin_edges[0] = -np.inf
-            bin_edges[-1] = np.inf
+            if weights_flag:
+                bin_edges = _weighted_equi(
+                    n_partitions[order[1]],
+                    second[mask],
+                    reference_sample_weights[mask])
+            else:
+                bin_edges = _equi(
+                    n_partitions[order[1]],
+                    second[mask])
             bin_edges_second.append(bin_edges)
         bin_edges_second = np.array(bin_edges_second)
         bin_edges = [bin_edges_first, bin_edges_second]
-
     return bin_edges
 
 
-def apply_irregular_binning(data_sample, bin_edges, order=None):
+def _check_weight_sanity(reference_sample, reference_sample_weights):
+    """Check if the weights are larger than 0,
+    and if reference has the same shape to the weights"""
+    mesg = 'data and their weights should be in the same length'
+    assert len(reference_sample) == len(reference_sample_weights), mesg
+
+    mesg = 'weights should be 1D array'
+    assert len(reference_sample_weights.shape) == 1, mesg
+
+    mesg = 'all weights should be non-negative'
+    assert np.all(reference_sample_weights >= 0), mesg
+
+
+def apply_irregular_binning(data_sample, bin_edges,
+                            order=None, data_sample_weights=None):
     """Apply irregular binning to data sample.
     :param data_sample: Sample of unbinned data.
     :type data_sample: array
     :param bin_edges: Array of bin edges
     :type bin_edges_first: array
     :param order: Order in which the partitioning is performed, defaults to None
         [0, 1] : first bin x then bin y for each partition in x
         [1, 0] : first bin y then bin x for each partition in y
         if None, the natural order, i.e. [0, 1] is used. For 1D just put None.
     :type order: list, optional
+    :param data_sample_weights: weights of data_sample
+    :type data_sample_weights: array_like, 1-Dimensional
     :return: binned data. Number of counts in each bin.
     :rtype: array
     """
+    if data_sample_weights is None:
+        weights_flag = 0
+    else:
+        _check_weight_sanity(data_sample, data_sample_weights)
+        weights_flag = 1
     if len(data_sample.shape) == 1:
-        ns, _ = np.histogram(data_sample, bins=bin_edges)
+        ns, _ = np.histogram(
+            data_sample,
+            bins=bin_edges,
+            weights=data_sample_weights)
     else:
         if order is None:
             order = [0, 1]
         first = np.vstack(data_sample.T[order[0]])
         second = np.vstack(data_sample.T[order[1]])
 
         ns = []
         i = 0
         for low, high in zip(bin_edges[0][:-1], bin_edges[0][1:]):
             mask = (first > low) & (first <= high)
-            n, _ = np.histogram(second[mask], bins=bin_edges[1][i])
+            if weights_flag:
+                n, _ = np.histogram(
+                    second[mask],
+                    bins=bin_edges[1][i],
+                    weights=data_sample_weights[mask.flatten()])
+            else:
+                n, _ = np.histogram(
+                    second[mask],
+                    bins=bin_edges[1][i])
             ns.append(n)
             i += 1
-    assert len(data_sample) == np.sum(ns), (f'Sum of binned data {np.sum(ns)}'
-                                            + ' unequal to size of data sample'
-                                            + f' {len(data_sample)}')
+    if weights_flag:
+        mesg = (f'Sum of binned data {np.sum(ns)}'
+                + ' unequal to sum of data weights'
+                + f' {np.sum(data_sample_weights)}')
+        assert np.isclose(
+            np.sum(data_sample_weights),
+            np.sum(ns), rtol=1e-3), mesg
+    else:
+        mesg = (f'Sum of binned data {np.sum(ns)}'
+                + ' unequal to size of data sample'
+                + f' {len(data_sample)}')
+        assert len(data_sample) == np.sum(ns), mesg
     return np.array(ns, dtype=float)
 
 
 def plot_irregular_binning(ax, bin_edges, order=None, c='k', **kwargs):
     """Plot the bin edges as a grid.
     :param ax: axis to plot to
     :type ax: matplotlib axis
@@ -282,17 +388,18 @@
                 plot_funcs[0](low, zorder=4, c=c, **kwargs)
             plot_funcs[1](be_second[i][1:-1], low, high, zorder=4, color=c,
                           **kwargs)
             i += 1
 
 
 def plot_equiprobable_histogram(data_sample, bin_edges, order=None,
-                                ax=None, nevents_expected=None, plot_xlim=None,
-                                plot_ylim=None, plot_mode='sigma_deviation',
-                                **kwargs):
+                                ax=None, nevents_expected=None,
+                                plot_xlim=None, plot_ylim=None,
+                                plot_mode='sigma_deviation',
+                                draw_colorbar=True, **kwargs):
     """Plot 1d/2d histogram of data sample binned according to the passed
     irregular binning.
     :param data_sample: Sample of unbinned data.
     :type data_sample: array
     :param bin_edges: Array of bin edges
     :type bin_edges: array
     :param order: Order in which the partitioning is performed
@@ -308,90 +415,116 @@
         cmap scale ranges from min to max. Defaults to None.
     :type nevents_expected: float, optional
     :param plot_mode: sets the plotting schedule. Defaults to sigma_deviation
         which shows the deviation of the counts in each bin from expected.
         Can be set to 'num_counts' to plot the total number of counts in each
         bin or 'count_density' to show the counts scaled by the inverse of the
         area of the bin, throws error if set to other value
-    :type plot_mode: string
+    :type plot_mode: string, optional
+    :param draw_colorbar: whether draw the colorbar
+    :type draw_colorbar: bool, optional
     :param plot_xlim: xlim to use for the plot. If None is passed, take min and
         max values of the data sample. Defaults to None.
     :type plot_xlim: tuple, optional
     :param plot_ylim: ylim to use for the plot. If None is passed, take min and
         max values of the data sample. Defaults to None.
     :type plot_ylim: tuple, optional
     :raises ValueError: when an unknown order is passed.
     """
     if order is None:
         order = [0, 1]
     if ax is None:
-        _, ax = mpl.pyplot.subplots(1, figsize=(4, 4))
+        _, ax = plt.subplots(1, figsize=(4, 4))
     if (plot_xlim is None) or (plot_ylim is None):
         xlim, ylim = get_plot_limits(data_sample)
+    if plot_mode == 'count_density':
+        if (plot_xlim is not None) or (plot_ylim is not None):
+            raise RuntimeError('Manually set x or y limit in'
+                               'count_density mode is misleading')
     if plot_xlim is not None:
         xlim = plot_xlim
     if plot_ylim is not None:
         ylim = plot_ylim
-    ax.set_xlim(xlim)
-    ax.set_ylim(ylim)
 
     ns = apply_irregular_binning(data_sample, bin_edges, order=order)
 
     be = _get_finite_bin_edges(bin_edges, data_sample, order)
     be_first = be[0]
     be_second = be[1]
 
-    if(plot_mode == 'sigma_deviation'):
+    alpha = kwargs.pop('alpha', 1)
+
+    if plot_mode == 'sigma_deviation':
         cmap_str = kwargs.pop('cmap', 'RdBu_r')
-        cmap = mpl.cm.get_cmap(cmap_str)
+        cmap = _get_cmap(cmap_str, alpha=alpha)
         if nevents_expected is None:
-            raise ValueError('nevents_expected cannot ' +
+            raise ValueError('nevents_expected cannot '
                              'be None while plot_mode=\'sigma_deviation\'')
-
         n_bins = get_n_bins(bin_edges)
         midpoint = nevents_expected / n_bins
         delta = max(midpoint - ns.min(), ns.max() - midpoint)
         sigma_deviation = delta / np.sqrt(midpoint)
         ns = (ns - midpoint) / np.sqrt(midpoint)
-        norm = mpl.colors.Normalize(vmin=-sigma_deviation,
-                                    vmax=sigma_deviation)
+        vmin = -sigma_deviation
+        vmax = sigma_deviation
+        if abs(kwargs.get('vmin', vmin)) != abs(kwargs.get('vmax', vmax)):
+            warnings.warn('You are specifying different `vmin` and `vmax`!',
+                          stacklevel=2)
         label = (r'$\sigma$-deviation from $\mu_\mathrm{{bin}}$ ='
                  + f'{midpoint:.1f} counts')
-    elif(plot_mode == 'count_density'):
+    elif plot_mode == 'count_density':
         label = r'Counts per area in each bin'
         ns = _get_count_density(ns, be_first, be_second, data_sample)
         cmap_str = kwargs.pop('cmap', 'viridis')
-        cmap = mpl.cm.get_cmap(cmap_str)
-        norm = mpl.colors.Normalize(vmin=np.min(ns),
-                                    vmax=np.max(ns))
-    elif(plot_mode == 'num_counts'):
+        cmap = _get_cmap(cmap_str, alpha=alpha)
+        vmin = np.min(ns)
+        vmax = np.max(ns)
+    elif plot_mode == 'num_counts':
         label = r'Number of counts in eace bin'
         cmap_str = kwargs.pop('cmap', 'viridis')
-        cmap = mpl.cm.get_cmap(cmap_str)
-        norm = mpl.colors.Normalize(vmin=np.min(ns),
-                                    vmax=np.max(ns))
+        cmap = _get_cmap(cmap_str, alpha=alpha)
+        vmin = np.min(ns)
+        vmax = np.max(ns)
     else:
         raise ValueError(f'plot_mode {plot_mode} is not defined.')
 
+    norm = mpl.colors.Normalize(vmin=kwargs.pop('vmin', vmin),
+                                vmax=kwargs.pop('vmax', vmax),
+                                clip=False)
+
+    edgecolor = kwargs.pop('edgecolor', 'k')
     if len(data_sample.shape) == 1:
         i = 0
-        bin_edges[0] = xlim[0]
-        bin_edges[-1] = xlim[1]
-        for low, high in zip(bin_edges[:-1], bin_edges[1:]):
-            rec = Rectangle((low, 0), high - low, 1,
-                            facecolor=cmap(norm(ns[i])),
-                            **kwargs)
-            ax.add_patch(rec)
+        be_first[0] = xlim[0]
+        be_first[-1] = xlim[1]
+        for low, high in zip(be_first[:-1], be_first[1:]):
+            ax.axvspan(low,
+                       high,
+                       facecolor=cmap(norm(ns[i])),
+                       edgecolor=edgecolor,
+                       **kwargs,
+                       )
             i += 1
     else:
         # plot rectangle for each bin
         i = 0
-        edgecolor = kwargs.get('edgecolor', 'k')
+        if order == [0, 1]:
+            be_first[0] = xlim[0]
+            be_first[-1] = xlim[1]
+        elif order == [1, 0]:
+            be_first[0] = ylim[0]
+            be_first[-1] = ylim[1]
         for low_f, high_f in zip(be_first[:-1], be_first[1:]):
             j = 0
+            if order == [0, 1]:
+                be_second[i][0] = ylim[0]
+                be_second[i][-1] = ylim[1]
+            elif order == [1, 0]:
+                be_second[i][0] = xlim[0]
+                be_second[i][-1] = xlim[1]
             for low_s, high_s in zip(be_second[i][:-1], be_second[i][1:]):
                 if order == [0, 1]:
                     rec = Rectangle((low_f, low_s),
                                     high_f - low_f,
                                     high_s - low_s,
                                     facecolor=cmap(norm(ns[i][j])),
                                     edgecolor=edgecolor,
@@ -403,18 +536,34 @@
                                     facecolor=cmap(norm(ns[i][j])),
                                     edgecolor=edgecolor,
                                     **kwargs)
                 ax.add_patch(rec)
                 j += 1
             i += 1
 
-    fig = mpl.pyplot.gcf()
+    ax.set_xlim(xlim)
+    ax.set_ylim(ylim)
+
+    if draw_colorbar:
+        fig = plt.gcf()
 
-    fig.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap), ax=ax,
-                 label=label)
+        extend = 'neither'
+        if norm.vmin > np.min(ns) and norm.vmax < np.max(ns):
+            extend = 'both'
+        elif norm.vmin > np.min(ns):
+            extend = 'min'
+        elif norm.vmax < np.max(ns):
+            extend = 'max'
+
+        fig.colorbar(
+            mpl.cm.ScalarMappable(norm=norm, cmap=cmap),
+            ax=ax,
+            label=label,
+            extend=extend,
+        )
     return
 
 
 def get_n_bins(eqpb_bin_edges):
     if isinstance(eqpb_bin_edges[0], float):
         n_bins = len(eqpb_bin_edges) - 1
     else:
@@ -433,7 +582,48 @@
 
     return xlim, ylim
 
 
 def check_sample_sanity(sample):
     assert ~np.isnan(sample).any(), 'Sample contains NaN entries!'
     assert ~np.isinf(sample).any(), 'Sample contains inf values!'
+
+
+def check_for_ties(sample):
+    any_ties = len(np.unique(sample, axis=0)) != len(sample)
+    if any_ties:
+        warnings.warn("reference_sample contains ties, this might "
+                      "cause problems!", stacklevel=2)
+
+
+def check_dimensionality_for_eqpb(data_sample, reference_sample,
+                                  n_partitions, order):
+    if len(reference_sample.shape) == 1:
+        assert len(data_sample.shape) == 1, "Shape of data_sample is"\
+            " incompatible with shape of reference_sample"
+        assert isinstance(n_partitions, int), "n_partitions must be an"\
+            " integer for 1-dim. data."
+        assert order is None, "providing a not-None value for order is"\
+            " ambiguous for 1-dim. data."
+    elif len(reference_sample.shape) == 2:
+        assert len(data_sample.shape) == 2, "Shape of data_sample is"\
+            " incompatible with shape of reference_sample."
+        # Check dimensionality is two
+        assert (data_sample.shape[1]
+                == reference_sample.shape[1]
+                == len(n_partitions)), \
+            "Shape of data_sample is incompatible with shape of"\
+            " reference_sample and/or dimensionality of n_partitions."
+        if data_sample.shape[1] > 2:
+            raise NotImplementedError("Equiprobable binning is not (yet) "
+                                      f"implemented for {data_sample.shape[1]}"
+                                      "-dimensional data.")
+    else:
+        raise TypeError("reference_sample has unsupported shape "
+                        f"{reference_sample.shape}.")
+
+
+def _get_cmap(cmap_str, alpha=1):
+    _cmap = mpl.cm.get_cmap(cmap_str)
+    cmap = _cmap(np.arange(_cmap.N))
+    cmap[:, -1] = alpha
+    return mpl.colors.LinearSegmentedColormap.from_list("dummy", cmap)
```

### Comparing `GOFevaluation-0.1.1/HISTORY.md` & `GOFevaluation-0.1.2/HISTORY.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+v0.1.2
+==================
+* Add colorbar switch, set 2D histogram x&y limit by @dachengx in #39
+* Some plotting bug fixes by @hoetzsch in #41
+* Homemade equiprobable_binning, still based on ECDF by @dachengx in #43
+* a few patches by @hammannr in #38
+* Exercise notebook by @hammannr in #44
+
 v0.1.1
 ===================
 * Add an example notebook that can be used as a guide when using the package for the first time (#29)
 * Improve and extend plotting of equiprobable binnings. This adds the option of plotting the binwise count density (#35)
 
 v0.1.0
 ===================
```

### Comparing `GOFevaluation-0.1.1/GOFevaluation.egg-info/SOURCES.txt` & `GOFevaluation-0.1.2/GOFevaluation.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 GOFevaluation.egg-info/dependency_links.txt
 GOFevaluation.egg-info/requires.txt
 GOFevaluation.egg-info/top_level.txt
 tests/__init__.py
 tests/test_evaluators_1d.py
 tests/test_evaluators_nd.py
 tests/test_gof_test.py
+tests/test_plots.py
 tests/test_utils.py
```

### Comparing `GOFevaluation-0.1.1/GOFevaluation.egg-info/PKG-INFO` & `GOFevaluation-0.1.2/GOFevaluation.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: GOFevaluation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Evaluate the Goodness-of-Fit(GoF) for binned or         unbinned data.
 Home-page: https://github.com/XENONnT/GOFevaluation
 Author: GOFevaluation contributors, the XENON collaboration
 License: UNKNOWN
 Description: # GOFevaluation
         Evaluate the Goodness-of-Fit (GoF) for binned or unbinned data.  
         ![Test package](https://github.com/XENONnT/GOFevaluation/actions/workflows/python-package.yml/badge.svg)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/XENONnT/GOFevaluation/HEAD)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/GOFevaluation.svg)](https://pypi.python.org/pypi/GOFevaluation/)
         [![CodeFactor](https://www.codefactor.io/repository/github/xenonnt/gofevaluation/badge)](https://www.codefactor.io/repository/github/xenonnt/gofevaluation)
         [![Coverage Status](https://coveralls.io/repos/github/XENONnT/GOFevaluation/badge.svg?branch=master)](https://coveralls.io/github/XENONnT/GOFevaluation?branch=master) 
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5626909.svg)](https://doi.org/10.5281/zenodo.5626909)
         
-        This GoF suite comprises the possibility to calculate different 1D / nD, binned / two-sample (unbinned) GoF measures and the corresponding p-value. A list of implemented measures is given below. 
+        This GoF suite comprises the possibility to calculate different 1D / nD, binned / two-sample (unbinned) GoF measures and the corresponding approximate p-value. A list of implemented measures is given below. 
         
          
         ## Implemented GoF measures
         | GoF measure                   | Class                     |    data input   | reference input | dim |
         |-------------------------------|---------------------------|:---------------:|:---------------:|:---:|
         | Kolmogorov-Smirnov            | `KSTestGOF`               |      sample     |      binned     |  1D |
         | Two-Sample Kolmogorov-Smirnov | `KSTestTwoSampleGOF`      |      sample     |      sample     |  1D |
@@ -141,29 +141,36 @@
         
         ## Contributing
         Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
         
         Please make sure to update tests as appropriate.
         
         
+        v0.1.2
+        ==================
+        * Add colorbar switch, set 2D histogram x&y limit by @dachengx in #39
+        * Some plotting bug fixes by @hoetzsch in #41
+        * Homemade equiprobable_binning, still based on ECDF by @dachengx in #43
+        * a few patches by @hammannr in #38
+        * Exercise notebook by @hammannr in #44
+        
         v0.1.1
         ===================
         * Add an example notebook that can be used as a guide when using the package for the first time (#29)
         * Improve and extend plotting of equiprobable binnings. This adds the option of plotting the binwise count density (#35)
         
         v0.1.0
         ===================
         * Multiple GOF tests (binned and unbinned) can be performed (#1, #5, #10, #12, #13)
         * The p-value is calculated based on toy sampling from the reference or a permutation test (#2, #14)
         * A wrapper class makes it convenient to perform multiple GOF tests in parallel (#19)
         * An equiprobable binning algorithm is implemented. The binning can be applied upon initialisation of the GOF object and a few visualization tools are provided. (#25, #26)
         * CI workflow implemented (#7)
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `GOFevaluation-0.1.1/README.md` & `GOFevaluation-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![Test package](https://github.com/XENONnT/GOFevaluation/actions/workflows/python-package.yml/badge.svg)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/XENONnT/GOFevaluation/HEAD)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/GOFevaluation.svg)](https://pypi.python.org/pypi/GOFevaluation/)
 [![CodeFactor](https://www.codefactor.io/repository/github/xenonnt/gofevaluation/badge)](https://www.codefactor.io/repository/github/xenonnt/gofevaluation)
 [![Coverage Status](https://coveralls.io/repos/github/XENONnT/GOFevaluation/badge.svg?branch=master)](https://coveralls.io/github/XENONnT/GOFevaluation?branch=master) 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5626909.svg)](https://doi.org/10.5281/zenodo.5626909)
 
-This GoF suite comprises the possibility to calculate different 1D / nD, binned / two-sample (unbinned) GoF measures and the corresponding p-value. A list of implemented measures is given below. 
+This GoF suite comprises the possibility to calculate different 1D / nD, binned / two-sample (unbinned) GoF measures and the corresponding approximate p-value. A list of implemented measures is given below. 
 
  
 ## Implemented GoF measures
 | GoF measure                   | Class                     |    data input   | reference input | dim |
 |-------------------------------|---------------------------|:---------------:|:---------------:|:---:|
 | Kolmogorov-Smirnov            | `KSTestGOF`               |      sample     |      binned     |  1D |
 | Two-Sample Kolmogorov-Smirnov | `KSTestTwoSampleGOF`      |      sample     |      sample     |  1D |
```

### Comparing `GOFevaluation-0.1.1/PKG-INFO` & `GOFevaluation-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: GOFevaluation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Evaluate the Goodness-of-Fit(GoF) for binned or         unbinned data.
 Home-page: https://github.com/XENONnT/GOFevaluation
 Author: GOFevaluation contributors, the XENON collaboration
 License: UNKNOWN
 Description: # GOFevaluation
         Evaluate the Goodness-of-Fit (GoF) for binned or unbinned data.  
         ![Test package](https://github.com/XENONnT/GOFevaluation/actions/workflows/python-package.yml/badge.svg)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/XENONnT/GOFevaluation/HEAD)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/GOFevaluation.svg)](https://pypi.python.org/pypi/GOFevaluation/)
         [![CodeFactor](https://www.codefactor.io/repository/github/xenonnt/gofevaluation/badge)](https://www.codefactor.io/repository/github/xenonnt/gofevaluation)
         [![Coverage Status](https://coveralls.io/repos/github/XENONnT/GOFevaluation/badge.svg?branch=master)](https://coveralls.io/github/XENONnT/GOFevaluation?branch=master) 
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5626909.svg)](https://doi.org/10.5281/zenodo.5626909)
         
-        This GoF suite comprises the possibility to calculate different 1D / nD, binned / two-sample (unbinned) GoF measures and the corresponding p-value. A list of implemented measures is given below. 
+        This GoF suite comprises the possibility to calculate different 1D / nD, binned / two-sample (unbinned) GoF measures and the corresponding approximate p-value. A list of implemented measures is given below. 
         
          
         ## Implemented GoF measures
         | GoF measure                   | Class                     |    data input   | reference input | dim |
         |-------------------------------|---------------------------|:---------------:|:---------------:|:---:|
         | Kolmogorov-Smirnov            | `KSTestGOF`               |      sample     |      binned     |  1D |
         | Two-Sample Kolmogorov-Smirnov | `KSTestTwoSampleGOF`      |      sample     |      sample     |  1D |
@@ -141,29 +141,36 @@
         
         ## Contributing
         Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
         
         Please make sure to update tests as appropriate.
         
         
+        v0.1.2
+        ==================
+        * Add colorbar switch, set 2D histogram x&y limit by @dachengx in #39
+        * Some plotting bug fixes by @hoetzsch in #41
+        * Homemade equiprobable_binning, still based on ECDF by @dachengx in #43
+        * a few patches by @hammannr in #38
+        * Exercise notebook by @hammannr in #44
+        
         v0.1.1
         ===================
         * Add an example notebook that can be used as a guide when using the package for the first time (#29)
         * Improve and extend plotting of equiprobable binnings. This adds the option of plotting the binwise count density (#35)
         
         v0.1.0
         ===================
         * Multiple GOF tests (binned and unbinned) can be performed (#1, #5, #10, #12, #13)
         * The p-value is calculated based on toy sampling from the reference or a permutation test (#2, #14)
         * A wrapper class makes it convenient to perform multiple GOF tests in parallel (#19)
         * An equiprobable binning algorithm is implemented. The binning can be applied upon initialisation of the GOF object and a few visualization tools are provided. (#25, #26)
         * CI workflow implemented (#7)
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

