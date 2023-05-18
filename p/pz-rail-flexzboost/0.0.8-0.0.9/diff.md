# Comparing `tmp/pz-rail-flexzboost-0.0.8.tar.gz` & `tmp/pz-rail-flexzboost-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-flexzboost-0.0.8.tar", last modified: Tue Apr  4 18:21:30 2023, max compression
+gzip compressed data, was "pz-rail-flexzboost-0.0.9.tar", last modified: Thu May  4 05:17:19 2023, max compression
```

## Comparing `pz-rail-flexzboost-0.0.8.tar` & `pz-rail-flexzboost-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.408945 pz-rail-flexzboost-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.400945 pz-rail-flexzboost-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.404945 pz-rail-flexzboost-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-04 18:21:30.408945 pz-rail-flexzboost-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.404945 pz-rail-flexzboost-0.0.8/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/archive/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/archive/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/archive/x_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/archive/x_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 18:21:30.408945 pz-rail-flexzboost-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.400945 pz-rail-flexzboost-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.408945 pz-rail-flexzboost-0.0.8/src/pz_rail_flexzboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-04 18:21:30.000000 pz-rail-flexzboost-0.0.8/src/pz_rail_flexzboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-04 18:21:30.000000 pz-rail-flexzboost-0.0.8/src/pz_rail_flexzboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:21:30.000000 pz-rail-flexzboost-0.0.8/src/pz_rail_flexzboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-04 18:21:30.000000 pz-rail-flexzboost-0.0.8/src/pz_rail_flexzboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-04 18:21:30.000000 pz-rail-flexzboost-0.0.8/src/pz_rail_flexzboost.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.400945 pz-rail-flexzboost-0.0.8/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.400945 pz-rail-flexzboost-0.0.8/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.408945 pz-rail-flexzboost-0.0.8/src/rail/estimation/algos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.408945 pz-rail-flexzboost-0.0.8/src/rail/estimation/algos/flexz_version/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/src/rail/estimation/algos/flexz_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 18:21:30.000000 pz-rail-flexzboost-0.0.8/src/rail/estimation/algos/flexz_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/src/rail/estimation/algos/flexzboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:21:30.408945 pz-rail-flexzboost-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-04 18:21:16.000000 pz-rail-flexzboost-0.0.8/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/archive/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/archive/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/archive/x_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/archive/x_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/docs/notebooks/fzboost_pdf_representation_comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/src/rail/estimation/algos/flexzboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/src/rail/flexzboost/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/src/rail/flexzboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/rail/flexzboost/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/tests/test_algos.py
```

### Comparing `pz-rail-flexzboost-0.0.8/.github/workflows/main.yml` & `pz-rail-flexzboost-0.0.9/.github/workflows/main.yml`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        pip install wheel numpy # For somoclu
         pip install .
         pip install flake8 pytest pytest-cov mockmpi pytest-timeout
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Test with pytest
       run: |
         python -m pytest --cov=rail.estimation.algos.flexzboost --cov-report=xml
     - name: Upload coverage to Codecov
```

### Comparing `pz-rail-flexzboost-0.0.8/.github/workflows/publish-to-pypi.yml` & `pz-rail-flexzboost-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.8/.gitignore` & `pz-rail-flexzboost-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.8/LICENSE` & `pz-rail-flexzboost-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.8/PKG-INFO` & `pz-rail-flexzboost-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.0.8
+Version: 0.0.9
 Summary: RAIL Flexzboost Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-flexzboost-0.0.8/archive/README.md` & `pz-rail-flexzboost-0.0.9/archive/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.8/archive/pypi.yaml` & `pz-rail-flexzboost-0.0.9/archive/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.8/pyproject.toml` & `pz-rail-flexzboost-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,26 +26,29 @@
     "scikit-learn",
     "xgboost"
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage",
+    "ipykernel",
+    "matplotlib",
+    "numpy",
     "pylint",
     "pytest",
     "pytest-cov",
     "yamllint",
 ]
 
 [build-system]
 requires = ["setuptools>=61", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
-write_to = "src/rail/estimation/algos/flexz_version/_version.py"
+write_to = "src/rail/flexzboost/_version.py"
 
 [tool.coverage.run]
 source = ["src/rail"]
 branch = true
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `pz-rail-flexzboost-0.0.8/src/pz_rail_flexzboost.egg-info/PKG-INFO` & `pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.0.8
+Version: 0.0.9
 Summary: RAIL Flexzboost Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-flexzboost-0.0.8/src/pz_rail_flexzboost.egg-info/SOURCES.txt` & `pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 pyproject.toml
 .github/workflows/main.yml
 .github/workflows/publish-to-pypi.yml
 archive/README.md
 archive/pypi.yaml
 archive/x_requirements.txt
 archive/x_setup.py
+docs/notebooks/fzboost_pdf_representation_comparison.ipynb
 src/pz_rail_flexzboost.egg-info/PKG-INFO
 src/pz_rail_flexzboost.egg-info/SOURCES.txt
 src/pz_rail_flexzboost.egg-info/dependency_links.txt
 src/pz_rail_flexzboost.egg-info/requires.txt
 src/pz_rail_flexzboost.egg-info/top_level.txt
 src/rail/estimation/algos/flexzboost.py
-src/rail/estimation/algos/flexz_version/__init__.py
-src/rail/estimation/algos/flexz_version/_version.py
+src/rail/flexzboost/__init__.py
+src/rail/flexzboost/_version.py
 tests/test_algos.py
```

### Comparing `pz-rail-flexzboost-0.0.8/src/rail/estimation/algos/flexzboost.py` & `pz-rail-flexzboost-0.0.9/src/rail/estimation/algos/flexzboost.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,24 +8,15 @@
 
 import numpy as np
 import qp
 import qp_flexzboost
 from ceci.config import StageParameter as Param
 from flexcode.helpers import make_grid
 from rail.estimation.estimator import CatEstimator, CatInformer
-
-def_filt = ['u', 'g', 'r', 'i', 'z', 'y']
-def_bands = [f"mag_{band}_lsst" for band in def_filt]
-def_err_bands = [f"mag_err_{band}_lsst" for band in def_filt]
-def_maglims = dict(mag_u_lsst=27.79,
-                   mag_g_lsst=29.04,
-                   mag_r_lsst=29.06,
-                   mag_i_lsst=28.62,
-                   mag_z_lsst=27.98,
-                   mag_y_lsst=27.05)
+from rail.core.common_params import SHARED_PARAMS
 
 
 def make_color_data(data_dict, bands, err_bands, ref_band, nondetect_val, maglimdict):
     """
     make a dataset consisting of the i-band mag and the five colors.
 
     Parameters
@@ -77,39 +68,40 @@
 
 
 class Inform_FZBoost(CatInformer):
     """ Train a FZBoost CatEstimator
     """
     name = 'Inform_FZBoost'
     config_options = CatInformer.config_options.copy()
-    config_options.update(zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
-                          zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
-                          nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
-                          nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
+    config_options.update(zmin=SHARED_PARAMS,
+                          zmax=SHARED_PARAMS,
+                          nzbins=SHARED_PARAMS,
+                          nondetect_val=SHARED_PARAMS,
+                          mag_limits=SHARED_PARAMS,
+                          bands=SHARED_PARAMS,
+                          err_bands=SHARED_PARAMS,
+                          ref_band=SHARED_PARAMS,
+                          redshift_col=SHARED_PARAMS,    
                           trainfrac=Param(float, 0.75,
                                           msg="fraction of training "
                                           "data to use for training (rest used for bump thresh "
                                           "and sharpening determination)"),
                           bumpmin=Param(float, 0.02,
                                         msg="minimum value in grid of "
                                         "thresholds checked to optimize removal of spurious "
                                         "small bumps"),
                           bumpmax=Param(float, 0.35,
                                         msg="max value in grid checked "
-                                        "for removal of small bumps"),
+                                            "for removal of small bumps"),
                           nbump=Param(int, 20, msg="number of grid points in bumpthresh grid search"),
                           sharpmin=Param(float, 0.7, msg="min value in grid checked in optimal sharpening parameter fit"),
                           sharpmax=Param(float, 2.1, msg="max value in grid checked in optimal sharpening parameter fit"),
                           nsharp=Param(int, 15, msg="number of search points in sharpening fit"),
                           max_basis=Param(int, 35, msg="maximum number of basis funcitons to use in density estimate"),
                           basis_system=Param(str, 'cosine', msg="type of basis sytem to use with flexcode"),
-                          bands=Param(list, def_bands, msg="bands to use in estimation"),
-                          err_bands=Param(list, def_err_bands, msg="error column names to use in estimation"),
-                          ref_band=Param(str, "mag_i_lsst", msg="band to use in addition to colors"),
-                          mag_limits=Param(dict, def_maglims, msg="1 sigma mag limits"),
                           regression_params=Param(dict, {'max_depth': 8, 'objective': 'reg:squarederror'},
                                                   msg="dictionary of options passed to flexcode, includes "
                                                   "max_depth (int), and objective, which should be set "
                                                   " to reg:squarederror"))
 
 
     def __init__(self, args, comm=None):
@@ -144,15 +136,15 @@
         from flexcode.regression_models import XGBoost
         from flexcode.loss_functions import cde_loss
 
         if self.config.hdf5_groupname:
             training_data = self.get_data('input')[self.config.hdf5_groupname]
         else:  #pragma: no cover
             training_data = self.get_data('input')
-        speczs = training_data['redshift']
+        speczs = training_data[self.config['redshift_col']]
         print("stacking some data...")
         color_data = make_color_data(training_data, self.config.bands, self.config.err_bands,
                                      self.config.ref_band, self.config.nondetect_val,
                                      self.config.mag_limits)
         train_dat, val_dat, train_sz, val_sz = self.split_data(color_data,
                                                                speczs,
                                                                self.config.trainfrac)
@@ -192,20 +184,20 @@
 
 
 class FZBoost(CatEstimator):
     """FZBoost-based CatEstimator
     """
     name = 'FZBoost'
     config_options = CatEstimator.config_options.copy()
-    config_options.update(nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
-                          nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
-                          bands=Param(list, def_bands, msg="bands to use in estimation"),
-                          err_bands=Param(list, def_err_bands, msg="error column names to use in estimation"),
-                          ref_band=Param(str, "mag_i_lsst", msg="band to use in addition to colors"),
-                          mag_limits=Param(dict, def_maglims, msg="1 sigma mag limits"),
+    config_options.update(nzbins=SHARED_PARAMS,
+                          nondetect_val=SHARED_PARAMS,
+                          mag_limits=SHARED_PARAMS,
+                          bands=SHARED_PARAMS,
+                          err_bands=SHARED_PARAMS,
+                          ref_band=SHARED_PARAMS,
                           qp_representation=Param(str, "interp", msg="qp generator to use. [interp|flexzboost]")
                           )
 
     def __init__(self, args, comm=None):
         """ Constructor:
         Do CatEstimator specific initialization """
         CatEstimator.__init__(self, args, comm=comm)
```

### Comparing `pz-rail-flexzboost-0.0.8/tests/test_algos.py` & `pz-rail-flexzboost-0.0.9/tests/test_algos.py`

 * *Files identical despite different names*

