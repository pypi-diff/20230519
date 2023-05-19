# Comparing `tmp/hydropandas-0.7.3.tar.gz` & `tmp/hydropandas-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydropandas-0.7.3.tar", last modified: Fri Mar 31 11:45:02 2023, max compression
+gzip compressed data, was "hydropandas-0.8.0.tar", last modified: Fri May 19 09:53:09 2023, max compression
```

## Comparing `hydropandas-0.7.3.tar` & `hydropandas-0.8.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:45:02.164052 hydropandas-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-31 11:44:49.000000 hydropandas-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-03-31 11:45:02.164052 hydropandas-0.7.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:45:02.156052 hydropandas-0.7.3/hydropandas/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:45:02.160052 hydropandas-0.7.3/hydropandas/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/data/knmi_meteostation.json
--rw-r--r--   0 runner    (1001) docker     (123)    42249 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/data/knmi_neerslagstation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:45:02.160052 hydropandas-0.7.3/hydropandas/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/extensions/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/extensions/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/extensions/gwobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27552 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/extensions/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/extensions/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:45:02.164052 hydropandas-0.7.3/hydropandas/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/bro.py
--rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/dino.py
--rw-r--r--   0 runner    (1001) docker     (123)    22086 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/fews.py
--rw-r--r--   0 runner    (1001) docker     (123)    65731 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/knmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/menyanthes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/modflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/pastas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/waterinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/io/wiski.py
--rw-r--r--   0 runner    (1001) docker     (123)    69633 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/obs_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    67632 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 11:44:49.000000 hydropandas-0.7.3/hydropandas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:45:02.160052 hydropandas-0.7.3/hydropandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-03-31 11:45:02.000000 hydropandas-0.7.3/hydropandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-31 11:45:02.000000 hydropandas-0.7.3/hydropandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:45:02.000000 hydropandas-0.7.3/hydropandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-31 11:45:02.000000 hydropandas-0.7.3/hydropandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-31 11:45:02.000000 hydropandas-0.7.3/hydropandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-03-31 11:44:49.000000 hydropandas-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-03-31 11:44:49.000000 hydropandas-0.7.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 11:45:02.164052 hydropandas-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:45:02.164052 hydropandas-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_000_run_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_001_to_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_002_obs_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_003_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_004_gwobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_005_dino.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_006_knmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_007_wiski.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_008_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_009_fews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-31 11:44:49.000000 hydropandas-0.7.3/tests/test_011_bro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:53:09.326221 hydropandas-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-19 09:52:58.000000 hydropandas-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-19 09:53:09.326221 hydropandas-0.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:53:09.318221 hydropandas-0.8.0/hydropandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:53:09.322221 hydropandas-0.8.0/hydropandas/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/data/fews_parameterid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/data/knmi_meteostation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42249 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/data/knmi_neerslagstation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:53:09.322221 hydropandas-0.8.0/hydropandas/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/extensions/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/extensions/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/extensions/gwobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27552 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/extensions/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/extensions/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:53:09.322221 hydropandas-0.8.0/hydropandas/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/bro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24215 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23725 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/fews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65731 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/knmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/menyanthes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/modflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/pastas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/waterinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/io/wiski.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73504 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/obs_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67358 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 09:52:58.000000 hydropandas-0.8.0/hydropandas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:53:09.322221 hydropandas-0.8.0/hydropandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-19 09:53:09.000000 hydropandas-0.8.0/hydropandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-19 09:53:09.000000 hydropandas-0.8.0/hydropandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:53:09.000000 hydropandas-0.8.0/hydropandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-19 09:53:09.000000 hydropandas-0.8.0/hydropandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 09:53:09.000000 hydropandas-0.8.0/hydropandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-19 09:52:58.000000 hydropandas-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-19 09:52:58.000000 hydropandas-0.8.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:53:09.326221 hydropandas-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:53:09.326221 hydropandas-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_000_run_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_001_to_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_002_obs_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_003_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_004_gwobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_005_dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_006_knmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_007_wiski.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_008_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_009_fews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-19 09:52:58.000000 hydropandas-0.8.0/tests/test_011_bro.py
```

### Comparing `hydropandas-0.7.3/LICENSE` & `hydropandas-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/PKG-INFO` & `hydropandas-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hydropandas
-Version: 0.7.3
+Version: 0.8.0
 Summary: Module by Artesia for loading observation data into custom DataFrames.
 Author-email: Onno Ebbens <o.ebbens@artesia-water.nl>
-Maintainer-email: "O. Ebbens" <o.ebbens@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
+Maintainer-email: "O.N. Ebbens" <o.ebbens@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 O.E. Ebbens, D.A. Brakenhoff, R. Calje
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -35,118 +35,121 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: rtd
 Provides-Extra: linting
 Provides-Extra: formatting
 Provides-Extra: pytesting
 Provides-Extra: coveraging
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="/docs/_static/Artesia_logo.jpg" alt="Artesia" width="200" align="right">
 
 [![PyPi](https://img.shields.io/pypi/v/hydropandas.svg)](https://pypi.python.org/pypi/hydropandas)
-[![PyPi Supported Python Versions](https://img.shields.io/pypi/pyversions/hydropandas)](https://pypi.org/project/spei/)
+[![PyPi Supported Python Versions](https://img.shields.io/pypi/pyversions/hydropandas)](https://pypi.python.org/pypi/hydropandas)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArtesiaWater/hydropandas/master)
 
 [![hydropandas](https://github.com/ArtesiaWater/hydropandas/workflows/hydropandas/badge.svg)](https://github.com/ArtesiaWater/hydropandas/actions?query=workflow%3Ahydropandas)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/c1b99f474bdc49b0a47e00e4e9f66c2f)](https://www.codacy.com/gh/ArtesiaWater/hydropandas/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ArtesiaWater/hydropandas&utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/c1b99f474bdc49b0a47e00e4e9f66c2f)](https://www.codacy.com/gh/ArtesiaWater/hydropandas/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ArtesiaWater/hydropandas&utm_campaign=Badge_Coverage)
 [![Documentation Status](https://readthedocs.org/projects/hydropandas/badge/?version=latest)](https://hydropandas.readthedocs.io/en/latest/?badge=latest)
 
 [![Format: isort](https://img.shields.io/badge/imports-isort-ef8336)](https://pycqa.github.io/isort/index.html)
 [![Format: Black](https://img.shields.io/badge/code_style-black-black)](https://github.com/psf/black)
 [![Linter: flake8](https://img.shields.io/badge/linter-flake8-yellowgreen)](https://flake8.pycqa.org/)
 [![Linter: ruff](https://img.shields.io/badge/linter-ruff-red)](https://github.com/charliermarsh/ruff)
 
-# hydropandas
+# HydroPandas
 
-The HydroPandas package allows users to store observation data at multiple locations in a single object (ObsCollection).
+Python tools for hydrological measurement data.
+
+## Introduction
+
+The HydroPandas package allows users to store observation data at multiple locations in a single object: ObsCollection.
+An ObsCollection makes it easier to analyse, visualise and export the observation data.
 An ObsCollection is a pandas DataFrame extended with custom methods and attributes related to hydrological timeseries.
+
 The HydroPandas package also provides convenient read functions for Dutch hydrological data from:
--   [BRO](https://www.broloket.nl)
--   [DINO](https://www.dinoloket.nl)
--   FEWS PI-XML
--   [KNMI](https://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script)
--   MODFLOW groundwater models
--   IMOD groundwater models
--   [Pastastore](https://github.com/pastas/pastastore)
--   [waterinfo](https://waterinfo.rws.nl/)
--   WISKI csv files
 
+- [BRO](https://www.broloket.nl)
+- [DINO](https://www.dinoloket.nl)
+- FEWS PI-XML
+- [KNMI](https://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script)
+- MODFLOW groundwater models
+- IMOD groundwater models
+- [Pastastore](https://github.com/pastas/pastastore)
+- [waterinfo](https://waterinfo.rws.nl/)
+- WISKI csv files
 
-## Installation
+## Install
 
 Install the module with pip:
 
 `pip install hydropandas`
 
-Hydropandas requires `numpy`, `scipy`, `matplotlib`, `pandas`, `requests` and `zeep`.
+HydroPandas requires `pandas`, `scipy`, `matplotlib`, `tqdm`, `requests` and `colorama`.
 
 For some functionality additional packages are required:
 
--   `geopandas`: for dealing with shapefiles
--   `pastastore`: for reading or storing data from PastaStore
--   `bokeh`, `branca`, `folium`: for interactive maps
--   `flopy`: for reading data from MODFLOW models
--   `xarray`: for loading data from REGIS
+- `geopandas`: for dealing with shapefiles
+- `pastastore`: for reading or storing data from PastaStore
+- `bokeh`, `branca`, `folium`: for interactive maps
+- `flopy`: for reading data from MODFLOW models
+- `xarray`: for loading data from REGIS
 
 For installing in development mode, clone the repository and install by
 typing `pip install -e .` from the module root directory.
-For installing all the optional packages use `pip install -e .[full]`
+For installing all the optional packages use `pip install -e .[full]`.
+
+## Get in touch
 
-If you have trouble installing HydroPandas, refer to the
-[Dependencies section](#dependencies) below.
+- Questions on HydroPandas ("How can I?") can be asked and answered on [Github Discussions](https://github.com/ArtesiaWater/hydropandas/discussions).
+- Bugs, feature requests and other improvements can be posted as [Github Issues](https://github.com/ArtesiaWater/hydropandas/issues).
+- Find out how to contribute to HydroPandas at our [Contribution page](https://hydropandas.readthedocs.io/en/stable/contribute.html).
 
-## Example usage
+## Examples
 
-Importing a single DINO csv file:
+Importing a groundwater time series from the BRO using the BRO-id and the tube number:
 
 ```python
 import hydropandas as hpd
-fname = './tests/data/2019-Dino-test/Grondwaterstanden_Put/B33F0080001_1.csv'
-gw = hpd.GroundwaterObs.from_dino(fname=fname)
+gw_bro = hpd.GroundwaterObs.from_bro("GMW000000041261", 1)
 ```
 
-Or for a zipfile:
+Or import all groundwater time series from the BRO within a certain extent:
 
 ```python
-import hydropandas as hpd
-dinozip = './tests/data/2019-Dino-test/dino.zip'
-dino_gw = hpd.read_dino(dirname=dinozip,
-			subdir='Grondwaterstanden_Put',
-                        suffix='1.csv',
-                        ObsClass=hpd.GroundwaterObs,
-                        keep_all_obs=False)
+oc = hpd.read_bro(extent=(117850, 118180, 439550, 439900))
 ```
 
 ## The Obs class
 
 The Obs class holds the measurements and metadata for one timeseries. There are
 currently 5 specific Obs classes for different types of measurements:
 
--   GroundwaterObs: for groundwater measurements
--   GroundwaterQualityObs: for groundwater quality measurements
--   WaterlvlObs: for surface water level measurements
--   ModelObs: for "observations" from a MODFLOW model
--   MeteoObs: for meteorological observations
--   PrecipitationObs: for precipitation observations, subclass of MeteoObs
--   EvaporationObs: for evaporation observations, subclass of MeteoObs
+- GroundwaterObs: for groundwater measurements
+- WaterQualityObs: for groundwater quality measurements
+- WaterlvlObs: for surface water level measurements
+- ModelObs: for "observations" from a MODFLOW model
+- MeteoObs: for meteorological observations
+- PrecipitationObs: for precipitation observations, subclass of MeteoObs
+- EvaporationObs: for evaporation observations, subclass of MeteoObs
 
 Each of these Obs classes is essentially a pandas DataFrame with additional
 methods and attributes related to the type of measurement that it holds.
-The classes also contain specific methods to read data from specific sources.
+Each Obs object also contain specific methods to read data from specific sources.
 
 ## The ObsCollection class
 
 The ObsCollection class, as the name implies, represents a collection of Obs
 classes, e.g. 10 timeseries of the groundwater level in a certain area. The
 ObsCollection is also a pandas DataFrame in which each timeseries is stored
 in a different row. Each row contains metadata (e.g. latitude and longitude
@@ -155,48 +158,13 @@
 type, e.g. to create an ObsCollection for 10 GroundwaterObs, and a separate
 ObsCollection for 5 PrecipitationObs.
 
 Like the Obs class, the ObsCollection class contains a bunch of methods for
 reading data from different sources. See the next section for supported data
 sources.
 
-## Dependencies
-
-Hydropandas (indirectly) uses some packages that cannot be installed
-automatically with `pip` on Windows. These packages are:
-
--   GDAL
--   Fiona
--   Shapely
-
-If you do not have these packages already it is recommended to first try
-installing them with `conda install <pkg>`. Otherwise, read the instructions
-below how to install them manually.
-
-Download the packages from [Christoph Gohlke's website](https://www.lfd.uci.edu/~gohlke/pythonlibs).
-Use CTRL+F to find the download link on the page. Be sure to download the
-correct version of the package. The Python version should match your Python
-version. Also the architecture should match (i.e. 64bits vs 32bits).
-For example:
-
--   GDAL-3.1.4-cp38-cp38-win_amd64.whl
-
-This is the GDAL version for Python 3.8 (as can be seen from the cp38 in the
-name), for 64-bits Python (as derived from the amd64 in the name).
-
-Once you have downloaded the correct files, navigate to the directory in which
-you saved your downloads. Now type the following commands (the order is
-important):
-
-1.  `pip install GDAL-3.1.4-cp38-cp38-win_amd64.whl`
-2.  `pip install Fiona-1.8.17-cp38-cp38-win_amd64.whl`
-3.  `pip install Shapely-1.7.1-cp38-cp38-win_amd64.whl`
-
-After you've done this you can install hydropandas using
-`pip install hydropandas`.
-
 ## Authors
 
--   Onno Ebbens, Artesia
--   Ruben Caljé, Artesia
--   Davíd Brakenhoff, Artesia
--   Martin Vonk, Artesia
+- Onno Ebbens, Artesia
+- Ruben Caljé, Artesia
+- Davíd Brakenhoff, Artesia
+- Martin Vonk, Artesia
```

### Comparing `hydropandas-0.7.3/hydropandas/__init__.py` & `hydropandas-0.8.0/hydropandas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # flake8: noqa
 import logging
 
 from .extensions import geo as _geo
 from .extensions import gwobs as _gwobs
 from .extensions import plots as _plots
 from .extensions import stats as _stats
+from .io.fews import get_fews_pid
 from .obs_collection import (
     ObsCollection,
     read_bro,
     read_dino,
+    read_excel,
     read_fews,
     read_imod,
     read_knmi,
     read_menyanthes,
     read_modflow,
+    read_pickle,
     read_waterinfo,
     read_wiski,
 )
 from .observation import (
     EvaporationObs,
     GroundwaterObs,
-    GroundwaterQualityObs,
     MeteoObs,
     ModelObs,
     Obs,
     PrecipitationObs,
     WaterlvlObs,
+    WaterQualityObs,
 )
 from .version import __version__
 
 logging.getLogger("hydropandas").addHandler(logging.NullHandler())
```

### Comparing `hydropandas-0.7.3/hydropandas/data/knmi_meteostation.json` & `hydropandas-0.8.0/hydropandas/data/knmi_meteostation.json`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/data/knmi_neerslagstation.json` & `hydropandas-0.8.0/hydropandas/data/knmi_neerslagstation.json`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/extensions/accessor.py` & `hydropandas-0.8.0/hydropandas/extensions/accessor.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/extensions/geo.py` & `hydropandas-0.8.0/hydropandas/extensions/geo.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/extensions/gwobs.py` & `hydropandas-0.8.0/hydropandas/extensions/gwobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,18 @@
     >>> get_modellayer_from_screen_depth(None, -7, zvec)
     0
 
     >>> get_modellayer_from_screen_depth(None, None, zvec)
     nan
 
     """
+    if isinstance(zvec, np.ndarray):
+        if np.isnan(zvec).all():
+            logger.warning("vertical datum invalid returning nan")
+            return np.nan
 
     zvec = np.sort(zvec)[::-1]
     ftop_invalid = check_if_var_is_invalid(ftop)
     fbot_invalid = check_if_var_is_invalid(fbot)
     if ftop_invalid and fbot_invalid:
         logger.error("- values for ftop and fbot are invalid!")
         return np.nan
@@ -152,15 +156,15 @@
         return lay_ftop
     elif ftop_invalid:
         lay_fbot = get_model_layer_z(fbot, zvec, left=left, right=right)
         logger.error(f"- ftop invalid. selected based on fbot: {lay_fbot}")
         return lay_fbot
 
     if ftop < fbot:
-        logger.warning("- tube screen top below tube screen bot, switch top and bot")
+        logger.warning("- tube screen top below tube screen bot, switching top and bot")
         fbot, ftop = ftop, fbot
 
     lay_ftop = get_model_layer_z(ftop, zvec, left=left, right=right)
     lay_fbot = get_model_layer_z(fbot, zvec, left=left, right=right)
 
     # Piezometer in layer in which majority of screen is located
     if lay_fbot == lay_ftop:
@@ -209,16 +213,14 @@
 
         # choose layer with biggest length
         rel_layer = np.argmax(length_layers)
         lay_out = lay_ftop + rel_layer
         logger.debug(f"  - selected layer: {lay_out}")
         return lay_out
 
-    return np.nan
-
 
 def get_zvec(x, y, gwf=None, ds=None):
     """get a list with the vertical layer boundaries at a point in the model.
 
     Parameters
     ----------
     x : int or float
```

### Comparing `hydropandas-0.7.3/hydropandas/extensions/plots.py` & `hydropandas-0.8.0/hydropandas/extensions/plots.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/extensions/stats.py` & `hydropandas-0.8.0/hydropandas/extensions/stats.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/io/bro.py` & `hydropandas-0.8.0/hydropandas/io/bro.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,15 @@
 
     ns = {"xmlns": "http://www.broservices.nl/xsd/dsgmn/1.0"}
 
     tree = xml.etree.ElementTree.fromstring(req.text)
     gmn = tree.find(".//xmlns:GMN_PO", ns)
     gmws = gmn.findall("xmlns:measuringPoint", ns)
 
-    logger.info(
-        f"{len(gmws)} groundwater monitoring wells within groundwater meetnet")
+    logger.info(f"{len(gmws)} groundwater monitoring wells within groundwater meetnet")
 
     obs_list = []
     for gmw in tqdm(gmws):
         tags = ["MeasuringPoint", "monitoringTube", "GroundwaterMonitoringTube"]
         tube = gmw.find(f".//xmlns:{'//xmlns:'.join(tags)}", ns)
         gmw_id = tube.find("xmlns:broId", ns).text
         tube_nr = int(tube.find("xmlns:tubeNumber", ns).text)
@@ -127,16 +126,15 @@
     if bro_id.startswith("GLD"):
         if only_metadata:
             raise ValueError("cannot get metadata from gld id")
         return measurements_from_gld(bro_id, **kwargs)
 
     elif bro_id.startswith("GMW"):
         if tube_nr is None:
-            raise ValueError(
-                "if bro_id is GMW a filternumber should be specified")
+            raise ValueError("if bro_id is GMW a filternumber should be specified")
 
         meta = get_metadata_from_gmw(bro_id, tube_nr)
         gld_ids = get_gld_ids_from_gmw(bro_id, tube_nr)
 
         if gld_ids is None:
             meta["name"] = f"{bro_id}_{tube_nr}"
             only_metadata = True  # cannot get time series without gld id
@@ -279,16 +277,15 @@
 
     glds = tree.findall(".//ns11:GLD_O", ns)
     if len(glds) != 1:
         raise (Exception("Only one gld supported"))
     gld = glds[0]
 
     meta = {"source": "BRO"}
-    meta["monitoring_well"] = gld.find(
-        "ns11:monitoringPoint//gldcommon:broId", ns).text
+    meta["monitoring_well"] = gld.find("ns11:monitoringPoint//gldcommon:broId", ns).text
     meta["tube_nr"] = int(
         gld.find("ns11:monitoringPoint//gldcommon:tubeNumber", ns).text
     )
     meta["name"] = f"{meta['monitoring_well']}_{meta['tube_nr']}"
     gmn = gld.find("ns11:groundwaterMonitoringNet//gldcommon:broId", ns)
     if gmn is None:
         meta["monitoringsnet"] = None
@@ -298,16 +295,15 @@
     # get observations
     msts = "ns11:observation//om:result//waterml:MeasurementTimeseries"
     times = [time.text for time in gld.findall(f"{msts}//waterml:time", ns)]
     values = [
         np.nan if value.text is None else float(value.text)
         for value in gld.findall(f"{msts}//waterml:value", ns)
     ]
-    qualifiers = [q.text for q in gld.findall(
-        f"{msts}//swe:Category//swe:value", ns)]
+    qualifiers = [q.text for q in gld.findall(f"{msts}//swe:Category//swe:value", ns)]
 
     # to dataframe
     df = pd.DataFrame(
         index=pd.to_datetime(times),
         data={"values": values, "qualifier": qualifiers},
     )
```

### Comparing `hydropandas-0.7.3/hydropandas/io/dino.py` & `hydropandas-0.8.0/hydropandas/io/dino.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 import os
 import re
 import tempfile
+from io import FileIO, TextIOWrapper
+from pathlib import Path
+from typing import Union
+from zipfile import ZipFile
 
 import numpy as np
 import pandas as pd
 
-from ..util import unzip_file
-
 logger = logging.getLogger(__name__)
 
 
 def _read_dino_groundwater_header(f):
     line = f.readline()
     header = dict()
     while line not in ["\n", "", "\r\n"]:
@@ -165,68 +167,77 @@
             measurements = None
     else:
         measurements = None
 
     return line, measurements
 
 
-def read_dino_groundwater_quality_txt(fname):
+def read_dino_groundwater_quality_txt(f: Union[str, Path, FileIO]):
     """Read dino groundwater quality (grondwatersamenstelling) from a dinoloket
     txt file.
 
     Notes
     -----
     this function has not been tested thoroughly
 
     Parameters
     ----------
-    fname : str
+    filepath_or_buffer : str
         path to txt file
 
     Returns
     -------
     measurements : pd.DataFrame
     meta : dict
         dictionary with metadata
     """
-    logger.info("reading -> {}".format(os.path.split(fname)[-1]))
-    with open(fname, "r") as f:
-        # LOCATIE gegevens
-        line = f.readline().rstrip("\n")
-        assert line == "LOCATIE gegevens"
-
-        strt_locatie = f.tell()
-        # determine the number of rows
-        nrows = -1  # the header does not count
+
+    fname = ""
+    if isinstance(f, (str, Path)):
+        if isinstance(f, str):
+            f = Path(f)
+        fname = f.stem
+        f = f.open("r")
+
+    logger.info("reading -> {}".format(fname))
+
+    # LOCATIE gegevens
+    line = f.readline().rstrip("\n")
+    assert line == "LOCATIE gegevens"
+
+    strt_locatie = f.tell()
+    # determine the number of rows
+    nrows = -1  # the header does not count
+    line = f.readline()
+    while line not in ["\n", ""]:
+        nrows += 1
         line = f.readline()
-        while line not in ["\n", ""]:
-            nrows += 1
-            line = f.readline()
-        eind_locatie = f.tell()
-        # go back to where we were before
-        f.seek(strt_locatie)
-        # read the location-information
-        locatie = pd.read_csv(f, sep="\t", nrows=nrows)
-        # there is always only one location (change if this is not the case)
-        assert nrows == 1
-
-        locatie = locatie.squeeze()
-
-        # KWALITEIT gegevens VLOEIBAAR
-        f.seek(eind_locatie)
-        line = f.readline().rstrip("\n")
-        assert line == "KWALITEIT gegevens VLOEIBAAR"
-
-        measurements = pd.read_csv(
-            f,
-            sep="\t",
-            parse_dates=["Monster datum", "Analyse datum"],
-            dayfirst=True,
-            index_col="Monster datum",
-        )
+    eind_locatie = f.tell()
+    # go back to where we were before
+    f.seek(strt_locatie)
+    # read the location-information
+    locatie = pd.read_csv(f, sep="\t", nrows=nrows)
+    # there is always only one location (change if this is not the case)
+    assert nrows == 1
+
+    locatie = locatie.squeeze()
+
+    # KWALITEIT gegevens VLOEIBAAR
+    f.seek(eind_locatie)
+    line = f.readline().rstrip("\n")
+    assert line == "KWALITEIT gegevens VLOEIBAAR"
+
+    measurements = pd.read_csv(
+        f,
+        sep="\t",
+        parse_dates=["Monster datum", "Analyse datum"],
+        dayfirst=True,
+        index_col="Monster datum",
+    )
+    f.close()
 
     meta = {
         "filename": fname,
         "source": "dino",
         "monitoring_well": locatie["NITG-nr"],
         "name": locatie["NITG-nr"],
         "x": locatie["X-coord"],
@@ -237,21 +248,25 @@
     except KeyError:
         meta["ground_level"] = np.nan
 
     return measurements, meta
 
 
 def read_dino_groundwater_csv(
-    fname, to_mnap=True, read_series=True, remove_duplicates=False, keep_dup="last"
+    f: Union[str, Path, FileIO],
+    to_mnap: bool = True,
+    read_series: bool = True,
+    remove_duplicates: bool = False,
+    keep_dup: str = "last",
 ):
     """Read dino groundwater quantity data from a dinoloket csv file.
 
     Parameters
     ----------
-    fname : str
+    f : Union[str, Path, TextIOWrapper]
         path to csv file
     to_mnap : boolean, optional
         if True a column with 'stand_m_tov_nap' is added to the dataframe
     read_series : boolean, optional
         if False only metadata is read, default is True
     remove_duplicates : boolean, optional
         if True duplicate indices are removed. Default is False.
@@ -261,66 +276,76 @@
 
     Returns
     -------
     measurements : pd.DataFrame
     meta : dict
         dictionary with metadata
     """
-    logger.info(f"reading -> {os.path.split(fname)[-1]}")
 
-    with open(fname, "r") as f:
-        # read header
-        line, header = _read_dino_groundwater_header(f)
-        line = _read_empty(f, line)
-        if not header:
-            logger.warning(f"could not read header -> {fname}")
+    if isinstance(f, (str, Path)):
+        if isinstance(f, str):
+            f = Path(f)
+        fname = f.stem
+        f = f.open("r")
+    elif isinstance(f, TextIOWrapper):
+        fname = f.name
+    else:
+        raise TypeError("f should be of type str, Path or TextIOWrapper")
 
-        # read reference level
-        line, ref = _read_dino_groundwater_referencelvl(f, line)
-        line = _read_empty(f, line)
-        if not ref:
-            logger.warning(f"could not read reference level -> {fname}")
+    logger.info("reading -> {}".format(fname))
 
-        # read metadata
-        line, meta, meta_ts = _read_dino_groundwater_metadata(f, line)
-        line = _read_empty(f, line)
-        if not meta["metadata_available"]:
-            logger.warning(f"could not read metadata -> {fname}")
-        meta["filename"] = fname
-        meta["source"] = "dino"
+    # read header
+    line, header = _read_dino_groundwater_header(f)
+    line = _read_empty(f, line)
+    if not header:
+        logger.warning(f"could not read header -> {fname}")
+
+    # read reference level
+    line, ref = _read_dino_groundwater_referencelvl(f, line)
+    line = _read_empty(f, line)
+    if not ref:
+        logger.warning(f"could not read reference level -> {fname}")
+
+    # read metadata
+    line, meta, meta_ts = _read_dino_groundwater_metadata(f, line)
+    line = _read_empty(f, line)
+    if not meta["metadata_available"]:
+        logger.warning(f"could not read metadata -> {fname}")
+    meta["filename"] = fname
+    meta["source"] = "dino"
+
+    # read measurements
+    if read_series:
+        line, measurements = _read_dino_groundwater_measurements(f, line)
+        if measurements is None:
+            logger.warning(f"could not read measurements -> {fname}")
+        elif measurements[~measurements.stand_cm_tov_nap.isna()].empty:
+            logger.warning(f"no NAP measurements available -> {fname}")
+        if to_mnap and measurements is not None:
+            measurements.insert(
+                0, "stand_m_tov_nap", measurements["stand_cm_tov_nap"] / 100.0
+            )
+            meta["unit"] = "m NAP"
+        elif not to_mnap:
+            meta["unit"] = "cm NAP"
+        if remove_duplicates:
+            measurements = measurements[~measurements.index.duplicated(keep=keep_dup)]
 
-        # read measurements
-        if read_series:
-            line, measurements = _read_dino_groundwater_measurements(f, line)
+        # add time variant metadata to measurements
+        for s in meta_ts.values():
             if measurements is None:
-                logger.warning(f"could not read measurements -> {fname}")
-            elif measurements[~measurements.stand_cm_tov_nap.isna()].empty:
-                logger.warning(f"no NAP measurements available -> {fname}")
-            if to_mnap and measurements is not None:
-                measurements.insert(
-                    0, "stand_m_tov_nap", measurements["stand_cm_tov_nap"] / 100.0
-                )
-                meta["unit"] = "m NAP"
-            elif not to_mnap:
-                meta["unit"] = "cm NAP"
-            if remove_duplicates:
-                measurements = measurements[
-                    ~measurements.index.duplicated(keep=keep_dup)
-                ]
-
-            # add time variant metadata to measurements
-            for s in meta_ts.values():
-                if measurements is None:
-                    measurements = pd.DataFrame(data=s.copy(), columns=[s.name])
-                else:
-                    measurements = measurements.join(s, how="outer")
-                measurements.loc[:, s.name] = measurements.loc[:, s.name].ffill()
+                measurements = pd.DataFrame(data=s.copy(), columns=[s.name])
+            else:
+                measurements = measurements.join(s, how="outer")
+            measurements.loc[:, s.name] = measurements.loc[:, s.name].ffill()
 
-        else:
-            measurements = None
+    else:
+        measurements = None
+
+    f.close()
 
     return measurements, meta
 
 
 def _read_artdino_groundwater_metadata(f, line):
     metalist = list()
     line = line.strip()
@@ -467,28 +492,27 @@
     return measurements, meta
 
 
 def read_artdino_dir(
     dirname,
     ObsClass=None,
     subdir="csv",
-    suffix=".csv",
+    suffix="1.csv",
     unpackdir=None,
     force_unpack=False,
     preserve_datetime=False,
     keep_all_obs=True,
     **kwargs,
 ):
     """Read Dino directory with point observations.
 
     TODO:
     - Evt. nog verbeteren door meteen Dataframe te vullen op het moment dat een
     observatie wordt ingelezen. Nu wordt eerst alles ingelezen in een lijst en
     daar een dataframe van gemaakt.
-    - aparte unzip functie maken en toch de juiste tijdelijke directory krijgen.
 
     Parameters
     ----------
     dirname : str
         directory name, can be a .zip file or the parent directory of subdir
     ObsClass : type
         class of the observations, e.g. GroundwaterObs or WaterlvlObs
@@ -502,22 +526,24 @@
         force unpack if dst already exists
     preserve_datetime : boolean, optional
         use date of the zipfile for the destination file
     keep_all_obs : boolean, optional
         add all observation points to the collection, even without data or
         metadata
     **kwargs: dict, optional
-        Extra arguments are passed to ObsClass.from_dino_file()
+        Extra arguments are passed to ObsClass.from_artdino_file()
 
     Returns
     -------
     obs_df : pd.DataFrame
         collection of multiple point observations
     """
 
+    from ..util import unzip_file
+
     # unzip dir
     if dirname.endswith(".zip"):
         zipf = dirname
         if unpackdir is None:
             dirname = tempfile.TemporaryDirectory().name
         else:
             dirname = unpackdir
@@ -621,136 +647,154 @@
     # measurements['Stand (m t.o.v. NAP)'] = measurements['Stand (cm t.o.v. NAP)'] /100.
 
     # measurements.set_index('Peildatum', inplace=True)
 
     return measurements
 
 
-def read_dino_waterlvl_csv(fname, to_mnap=True, read_series=True):
+def read_dino_waterlvl_csv(
+    f: Union[str, Path, FileIO], to_mnap: bool = True, read_series: bool = True
+):
     """Read dino waterlevel data from a dinoloket csv file.
 
     Parameters
     ----------
     fname : str
     to_mnap : boolean, optional
         if True a column with 'stand_m_tov_nap' is added to the dataframe
     read_series : boolean, optional
         if False only metadata is read, default is True
     """
-    logging.info(f"reading -> {os.path.split(fname)[-1]}")
+
+    fname = ""
+    if isinstance(f, (str, Path)):
+        if isinstance(f, str):
+            f = Path(f)
+        fname = f.stem
+        f = f.open("r")
+
+    logger.info("reading -> {}".format(fname))
 
     p_meta = re.compile(
         "Locatie,Externe aanduiding,X-coordinaat,Y-coordinaat, Startdatum, Einddatum"
     )
     p_data = re.compile(r"Locatie,Peildatum,Stand \(cm t.o.v. NAP\),Bijzonderheid")
 
-    with open(fname, "r") as f:
+    line = f.readline()
+    while line != "":
         line = f.readline()
-        while line != "":
-            line = f.readline()
-            if p_meta.match(line):
-                meta = _read_dino_waterlvl_metadata(f, line)
-                if meta:
-                    meta["metadata_available"] = True
-                else:
-                    meta["metadata_available"] = False
-                meta["filename"] = fname
-                meta["source"] = "dino"
-            elif p_data.match(line):
-                if read_series:
-                    measurements = _read_dino_waterlvl_measurements(f, line)
-                    if to_mnap and measurements is not None:
-                        measurements["stand_m_tov_nap"] = (
-                            measurements["stand_cm_tov_nap"] / 100.0
-                        )
-                        meta["unit"] = "m NAP"
-                    elif not to_mnap:
-                        meta["unit"] = "cm NAP"
-                else:
-                    measurements = None
+        if p_meta.match(line):
+            meta = _read_dino_waterlvl_metadata(f, line)
+            if meta:
+                meta["metadata_available"] = True
+            else:
+                meta["metadata_available"] = False
+            meta["filename"] = fname
+            meta["source"] = "dino"
+        elif p_data.match(line):
+            if read_series:
+                measurements = _read_dino_waterlvl_measurements(f, line)
+                if to_mnap and measurements is not None:
+                    measurements["stand_m_tov_nap"] = (
+                        measurements["stand_cm_tov_nap"] / 100.0
+                    )
+                    meta["unit"] = "m NAP"
+                elif not to_mnap:
+                    meta["unit"] = "cm NAP"
+            else:
+                measurements = None
+
+    f.close()
 
-                return measurements, meta
+    return measurements, meta
 
 
 def read_dino_dir(
-    dirname,
-    ObsClass=None,
-    subdir="Boormonsterprofiel_Geologisch booronderzoek",
-    suffix=".txt",
-    unpackdir=None,
-    force_unpack=False,
-    preserve_datetime=False,
-    keep_all_obs=True,
-    **kwargs,
+    path: Union[str, Path],
+    ObsClass,
+    subdir: str = "Grondwaterstanden_Put",
+    suffix: str = "1.csv",
+    keep_all_obs: bool = True,
+    **kwargs: dict,
 ):
     """Read Dino directory with point observations.
 
     TODO:
     - Evt. nog verbeteren door meteen Dataframe te vullen op het moment dat een
     observatie wordt ingelezen. Nu wordt eerst alles ingelezen in een lijst en
     daar een dataframe van gemaakt.
     - aparte unzip functie maken en toch de juiste tijdelijke directory krijgen.
 
     Parameters
     ----------
-    dirname : str
+    path : str | Path
         directory name, can be a .zip file or the parent directory of subdir
     ObsClass : type
         class of the observations, e.g. GroundwaterObs or WaterlvlObs
     subdir : str
         subdirectory of dirname with data files
     suffix : str
         suffix of files in subdir that will be read
-    unpackdir : str
-        destination directory of the unzipped file
-    force_unpack : boolean, optional
-        force unpack if dst already exists
-    preserve_datetime : boolean, optional
-        use date of the zipfile for the destination file
     keep_all_obs : boolean, optional
         add all observation points to the collection, even without data or
         metadata
     **kwargs: dict, optional
         Extra arguments are passed to ObsClass.from_dino_file()
 
     Returns
     -------
     obs_df : pd.DataFrame
         collection of multiple point observations
     """
 
-    # unzip dir
-    if dirname.endswith(".zip"):
-        zipf = dirname
-        if unpackdir is None:
-            dirname = tempfile.TemporaryDirectory().name
-        else:
-            dirname = unpackdir
-        unzip_file(
-            zipf, dirname, force=force_unpack, preserve_datetime=preserve_datetime
-        )
-
-    # read filenames
-    files = os.listdir(os.path.join(dirname, subdir))
-    if suffix:
-        files = [file for file in files if file.endswith(suffix)]
-
-    if not files:
-        raise FileNotFoundError(
-            "no files were found in {} that end with {}".format(
-                os.path.join(dirname, subdir), suffix
-            )
-        )
+    path = Path(path)
 
-    # read individual files
     obs_list = []
-    for _, file in enumerate(files):
-        fname = os.path.join(dirname, subdir, file)
-        obs = ObsClass.from_dino(fname=fname, **kwargs)
+
+    def get_dino_obs(f: Union[str, FileIO]):
+        obs = ObsClass.from_dino(fname=f, **kwargs)
         if obs.metadata_available and (not obs.empty):
-            obs_list.append(obs)
+            return obs
         elif keep_all_obs:
-            obs_list.append(obs)
+            return obs
         else:
-            logging.info(f"not added to collection -> {fname}")
+            logging.info(f"not added to collection -> {f.name}")
+            return None
+
+    if path.suffix == ".zip":
+        with ZipFile(path) as zfile:
+            fnames = [x for x in zfile.namelist() if f"{subdir}/" in x]
+            if suffix:
+                if "0" in suffix:
+                    raise Exception(f"Cant read dino files with _{suffix}")
+                fnames = [x for x in fnames if suffix in x]
+            if len(fnames) == 0:
+                raise FileNotFoundError(
+                    f"no files were found in {path}, {subdir=} with {suffix=}"
+                )
+            for fname in fnames:
+                with zfile.open(fname) as fo:
+                    obs = get_dino_obs(TextIOWrapper(fo))
+                    if obs is not None:
+                        obs_list.append(obs)
+    elif path.is_dir():
+        subpath = path / subdir
+        if suffix:
+            if "0" in suffix:
+                raise Exception(f"Cant read dino files with _{suffix}")
+            elif "*" not in suffix:
+                suffix = f"*{suffix}"
+            files = list(subpath.glob(suffix))
+        else:
+            files = list(subpath.iterdir())
+
+        if len(files) == 0:
+            raise FileNotFoundError(f"no files were found in {subpath} with {suffix=}")
+
+        for file in files:
+            obs = get_dino_obs(file)
+            if obs is not None:
+                obs_list.append(obs)
+    else:
+        raise ValueError("Path must either be a .zip or directory")
 
     return obs_list
```

### Comparing `hydropandas-0.7.3/hydropandas/io/fews.py` & `hydropandas-0.8.0/hydropandas/io/fews.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import datetime
 import logging
 import os
 import xml.etree.ElementTree as etree
 from io import StringIO
+from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from lxml.etree import iterparse
 
-from ..observation import (
-    EvaporationObs,
-    GroundwaterObs,
-    MeteoObs,
-    PrecipitationObs,
-    WaterlvlObs,
-)
+from .. import observation
+from ..observation import Obs
 
 logger = logging.getLogger(__name__)
 
 
 def read_xml_fname(
-    fname,
-    ObsClass,
-    translate_dic=None,
-    low_memory=True,
-    locationIds=None,
-    filterdict=None,
-    return_events=True,
-    keep_flags=(0, 1),
-    return_df=False,
-    tags=("series", "header", "event"),
-    skip_errors=True,
-    remove_nan=False,
-    **kwargs,
+    fname: str,
+    ObsClass: Union[Obs, Dict[str, Obs]],
+    translate_dic: Optional[Dict[str, str]] = None,
+    low_memory: bool = True,
+    locationIds: Optional[List[str]] = None,
+    filterdict: Optional[Dict[str, List[str]]] = None,
+    return_events: bool = True,
+    keep_flags: Tuple[int] = (0, 1),
+    return_df: bool = False,
+    tags: Tuple[str] = ("series", "header", "event"),
+    remove_nan: bool = False,
+    **kwargs: dict,  # unused
 ):
     """Read an xml filename into a list of observations objects.
 
     Parameters
     ----------
     fname : str
         full path to file
-    ObsClass : type
+    ObsClass: Union[Obs, Dict[str, Obs]]
         class of the observations, e.g. GroundwaterObs or WaterlvlObs
     translate_dic : dic or None, optional
         translate names from fews. If None this default dictionary is used:
         {'locationId': 'monitoring_well'}.
     low_memory : bool, optional
         whether to use xml-parsing method with lower memory footprint,
         default is True
@@ -85,15 +80,14 @@
             translate_dic=translate_dic,
             locationIds=locationIds,
             filterdict=filterdict,
             return_events=return_events,
             keep_flags=keep_flags,
             return_df=return_df,
             tags=tags,
-            skip_errors=skip_errors,
         )
     else:
         tree = etree.parse(fname)
         root = tree.getroot()
         obs_list = read_xml_root(
             root,
             ObsClass,
@@ -102,32 +96,31 @@
             remove_nan=remove_nan,
         )
 
     return obs_list
 
 
 def iterparse_pi_xml(
-    fname,
-    ObsClass,
-    translate_dic=None,
-    filterdict=None,
-    locationIds=None,
-    return_events=True,
-    keep_flags=(0, 1),
-    return_df=False,
-    tags=("series", "header", "event"),
-    skip_errors=False,
+    fname: str,
+    ObsClass: Union[Obs, Dict[str, Obs]],
+    translate_dic: Optional[Dict[str, str]] = None,
+    filterdict: Optional[Dict[str, List[str]]] = None,
+    locationIds: Optional[List[str]] = None,
+    return_events: bool = True,
+    keep_flags: Tuple[int] = (0, 1),
+    return_df: bool = False,
+    tags: Tuple[str] = ("series", "header", "event"),
 ):
     """Read a FEWS XML-file with measurements, memory efficient.
 
     Parameters
     ----------
     fname : str
         full path to file
-    ObsClass : type
+    ObsClass: Union[Obs, Dict[str, Obs]],
         class of the observations, e.g. GroundwaterObs or WaterlvlObs
     translate_dic : dic or None, optional
         translate names from fews. If None this default dictionary is used:
         {'locationId': 'monitoring_well'}.
     locationIds : tuple or list of str, optional
         list of locationId's to read from XML file, others are skipped.
         If None (default) all locations are read.
@@ -278,30 +271,30 @@
             h["series"] = s
         return pd.DataFrame(header_list)
     else:
         return obs_list
 
 
 def read_xmlstring(
-    xmlstring,
-    ObsClass,
-    translate_dic=None,
-    filterdict=None,
-    locationIds=None,
-    low_memory=True,
-    remove_nan=False,
+    xmlstring: str,
+    ObsClass: Union[Obs, Dict[str, Obs]],
+    translate_dic: Optional[Dict[str, str]] = None,
+    filterdict: Optional[Dict[str, List[str]]] = None,
+    locationIds: Optional[List[str]] = None,
+    low_memory: bool = True,
+    remove_nan: bool = False,
 ):
     """Read xmlstring into an list of Obs objects. Xmlstrings are usually
     obtained using a fews api.
 
     Parameters
     ----------
     xmlstring : str
         xml string to be parsed. Typically from a fews api.
-    ObsClass : type
+    ObsClass: Union[Obs, Dict[str, Obs]]
         class of the observations, e.g. GroundwaterObs or WaterlvlObs
     translate_dic : dic or None, optional
         translate names from fews. If None this default dictionary is used:
         {'locationId': 'monitoring_well'}.
     locationIds : tuple or list of str, optional
         list of locationId's to read from XML file, others are skipped.
         If None (default) all locations are read.
@@ -338,27 +331,27 @@
             remove_nan=remove_nan,
         )
 
     return obs_list
 
 
 def read_xml_root(
-    root,
-    ObsClass,
-    translate_dic=None,
-    locationIds=None,
-    remove_nan=False,
+    root: etree.Element,
+    ObsClass: Union[Obs, Dict[str, Obs]],
+    translate_dic: Dict[str, str] = None,
+    locationIds: List[str] = None,
+    remove_nan: bool = False,
 ):
     """Read a FEWS XML-file with measurements, return list of ObsClass objects.
 
     Parameters
     ----------
     root : xml.etree.ElementTree.Element
         root element of a fews xml
-    ObsClass : type
+    ObsClass: Union[Obs, Dict[str, Obs]],
         class of the observations, e.g. GroundwaterObs or WaterlvlObs
     translate_dic : dic or None, optional
         translate names from fews. If None this default dictionary is used:
         {'locationId': 'monitoring_well'}.
     locationIds : tuple or list of str, optional
         list of locationId's to read from XML file, others are skipped.
         If None (default) all locations are read.
@@ -413,26 +406,31 @@
                     obs_list.append(o)
             else:
                 obs_list.append(o)
 
     return obs_list
 
 
-def _obs_from_meta(ts, header, translate_dic, ObsClass):
+def _obs_from_meta(
+    ts: pd.DataFrame,
+    header: Dict[str, str],
+    translate_dic: Dict[str, str],
+    ObsClass: Union[Obs, Dict[str, Obs]],
+):
     """Internal function to convert timeseries and header into Obs objects.
 
     Parameters
     ----------
     ts : pd.DataFrame
         timeseries data.
     header : dictionary
         metadata.
     translate_dic : dictionary
         translate dictionary.
-    ObsClass : type
+    ObsClass: Union[Obs, Dict[str, Obs]],
         class of the observations, e.g. GroundwaterObs or WaterlvlObs
 
     Returns
     -------
     o : GroundwaterObs or WaterlvlObs
         hyrdopandas observation object.
     header : dictionary
@@ -457,66 +455,78 @@
 
     if np.isnan(x) or np.isnan(y):
         metadata_available = False
     else:
         metadata_available = True
 
     if "parameterId" in header:
-        pid = header["parameterId"]
-        name = header["monitoring_well"] + "_" + pid
+        parid = header["parameterId"]
+        name = header["monitoring_well"] + "_" + parid
     else:
         name = header["monitoring_well"]
 
-    if ObsClass in (WaterlvlObs,):
-        o = ObsClass(
+    if isinstance(ObsClass, dict):
+        if parid in ObsClass.keys():
+            ObsC = ObsClass[parid]
+        else:
+            ObsC = Obs
+    else:
+        ObsC = ObsClass
+
+    if ObsC in (observation.WaterlvlObs,):
+        o = ObsC(
             ts,
             x=x,
             y=y,
             unit=unit,
             meta=header,
             name=name,
             monitoring_well=header["monitoring_well"],
             metadata_available=metadata_available,
             source="FEWS",
         )
-    elif ObsClass in (GroundwaterObs,):
+    elif ObsC in (observation.GroundwaterObs,):
         if "z" in header.keys():
             z = float(header["z"])
         else:
             z = np.nan
-        o = ObsClass(
+        o = ObsC(
             ts,
             x=x,
             y=y,
             ground_level=z,
             unit=unit,
             meta=header,
             name=name,
             monitoring_well=header["monitoring_well"],
             metadata_available=metadata_available,
             source="FEWS",
         )
-    elif ObsClass in (MeteoObs, PrecipitationObs, EvaporationObs):
-        o = ObsClass(
+    elif ObsC in (
+        observation.MeteoObs,
+        observation.PrecipitationObs,
+        observation.EvaporationObs,
+    ):
+        o = ObsC(
             ts,
             x=x,
             y=y,
             unit=unit,
             meta=header,
             name=name,
-            meteo_var=pid,
+            meteo_var=parid,
             source="FEWS",
         )
     else:
-        o = ObsClass(ts, x=x, y=y, unit=unit, meta=header, name=name, source="FEWS")
+        o = ObsC(ts, x=x, y=y, unit=unit, meta=header, name=name, source="FEWS")
 
     return o, header
 
 
-def write_pi_xml(obs_coll, fname, timezone=1.0, version="1.24"):
+def write_pi_xml(obs_coll, fname: str, timezone: float = 1.0, version: str = "1.24"):
     """Write TimeSeries object to PI-XML file.
 
     Parameters
     ----------
     fname: path
         path to XML file
     """
@@ -608,31 +618,31 @@
             # end series
             f.write("\t" + "</series>\n")
         # end Timeseries
         f.write("</TimeSeries>\n")
 
 
 def read_xml_filelist(
-    fnames,
-    ObsClass,
-    directory=None,
-    locations=None,
-    translate_dic=None,
-    filterdict=None,
-    remove_nan=False,
-    low_memory=True,
-    **kwargs,
+    fnames: List[str],
+    ObsClass: Union[Obs, Dict[str, Obs]],
+    directory: Optional[str] = None,
+    locations: Optional[List[str]] = None,
+    translate_dic: Optional[Dict[str, str]] = None,
+    filterdict: Optional[Dict[str, List[str]]] = None,
+    remove_nan: bool = False,
+    low_memory: bool = True,
+    **kwargs: dict,
 ):
     """Read a list of xml files into a list of observation objects.
 
     Parameters
     ----------
     fnames : TYPE
         DESCRIPTION.
-    ObsClass : type
+    ObsClass: Union[Obs, Dict[str, Obs]]
         class of the observations, e.g. GroundwaterObs or WaterlvlObs
     directory : TYPE, optional
         DESCRIPTION. The default is None.
     locations : tuple or list of str, optional
         list of locationId's to read from XML file, others are skipped.
         If None (default) all locations are read.
     translate_dic : dic or None, optional
@@ -673,11 +683,32 @@
         obs_list += read_xml_fname(
             fullpath,
             ObsClass,
             translate_dic=translate_dic,
             filterdict=filterdict,
             low_memory=low_memory,
             locationIds=locations,
+            remove_nan=remove_nan,
             **kwargs,
         )
 
     return obs_list
+
+
+def get_fews_pid(name: str) -> Dict[str, Obs]:
+    """Get matching ParameterId's and HydroPandas Observation Classes
+
+    Parameters
+    ----------
+    name : str
+        Waterboard name
+
+    Returns
+    -------
+    Dict[str, Obs]
+        Dictonary with ParameterId and the resulting Observation Class
+    """
+    from ..data.fews_parameterid import pid
+
+    pid_sel = pid[name.lower()]
+
+    return {key: getattr(observation, value) for (key, value) in pid_sel.items()}
```

### Comparing `hydropandas-0.7.3/hydropandas/io/knmi.py` & `hydropandas-0.8.0/hydropandas/io/knmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,15 +585,15 @@
         with open(fname_zip, "wb") as fd:
             for chunk in r.iter_content(chunk_size=128):
                 fd.write(chunk)
 
         # unzip file
         util.unzip_file(fname_zip, fname_dir, force=True, preserve_datetime=True)
 
-    return read_knmi_daily_rainfall_file(fname_txt, meteo_var, start=None, end=None)
+    return read_knmi_daily_rainfall_file(fname_txt, meteo_var, start=start, end=end)
 
 
 def read_knmi_daily_rainfall_file(fname_txt, meteo_var="RD", start=None, end=None):
     """read a knmi file with daily rainfall data.
 
     Parameters
     ----------
@@ -940,15 +940,15 @@
         with open(fname_zip, "wb") as fd:
             for chunk in r.iter_content(chunk_size=128):
                 fd.write(chunk)
 
         # unzip file
         util.unzip_file(fname_zip, fname_dir, force=True, preserve_datetime=True)
 
-    return read_knmi_daily_meteo_file(fname_txt, meteo_var, start=None, end=None)
+    return read_knmi_daily_meteo_file(fname_txt, meteo_var, start=start, end=end)
 
 
 def read_knmi_daily_meteo_file(fname, meteo_var, start=None, end=None):
     """read knmi daily meteo data from a file
 
     Parameters
     ----------
```

### Comparing `hydropandas-0.7.3/hydropandas/io/menyanthes.py` & `hydropandas-0.8.0/hydropandas/io/menyanthes.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/io/modflow.py` & `hydropandas-0.8.0/hydropandas/io/modflow.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/io/pastas.py` & `hydropandas-0.8.0/hydropandas/io/pastas.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/io/waterinfo.py` & `hydropandas-0.8.0/hydropandas/io/waterinfo.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/hydropandas/io/wiski.py` & `hydropandas-0.8.0/hydropandas/io/wiski.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 def read_wiski_file(
     fname,
     sep=";",
     header_sep=None,
     header_identifier="#",
     read_series=True,
-    infer_datetime_format=True,
     translate_dic=None,
     tz_localize=True,
     unit="",
     **kwargs,
 ):
     """
     Read data from a WISKI file.
@@ -53,16 +52,14 @@
     header_sep : str, optional (default=None)
         The delimiter used to separate fields in the header. If None, the
         function will try to automatically detect the separator.
     header_identifier : str, optional (default="#")
         The character used to identify header lines.
     read_series : bool, optional (default=True)
         Whether to read the time series data from the file.
-    infer_datetime_format : bool, optional (default=True)
-        Whether to infer the datetime format of the timestamp column.
     translate_dic : dict, optional (default=None)
         A dictionary mapping header field names to the desired output names.
     tz_localize : bool, optional (default=True)
         Whether to localize the datetime index to the machine's timezone.
     unit : str, optional (default="")
         The unit of measurement of the data.
     **kwargs : keyword arguments
@@ -120,15 +117,14 @@
         if read_series:
             # read data
             data = pd.read_csv(
                 f,
                 sep=sep,
                 header=None,
                 names=columns,
-                infer_datetime_format=infer_datetime_format,
                 **kwargs,
             )
 
             if tz_localize:
                 data.index = data.index.tz_localize(None)
 
             # convert Value to float
```

### Comparing `hydropandas-0.7.3/hydropandas/obs_collection.py` & `hydropandas-0.8.0/hydropandas/obs_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,14 @@
 
 
 def read_dino(
     dirname=None,
     ObsClass=obs.GroundwaterObs,
     subdir="Grondwaterstanden_Put",
     suffix="1.csv",
-    unpackdir=None,
-    force_unpack=False,
-    preserve_datetime=False,
     keep_all_obs=True,
     name=None,
     **kwargs,
 ):
     """Read dino observations within an extent from the server or from a
     directory with downloaded files.
 
@@ -105,51 +102,73 @@
         of subdir
     ObsClass : type
         class of the observations, so far only GroundwaterObs is supported
     subdir : str
         subdirectory of dirname with data files
     suffix : str
         suffix of files in subdir that will be read
-    unpackdir : str
-        destination directory of the unzipped file
-    force_unpack : boolean, optional
-        force unpack if dst already exists
-    preserve_datetime : boolean, optional
-        use date of the zipfile for the destination file
     keep_all_obs : boolean, optional
         add all observation points to the collection, even the points
         without measurements or metadata
     name : str, optional
         the name of the observation collection
     kwargs:
-        kwargs are passed to the hydropandas.io.dino.download_dino_within_extent() or
-        the hydropandas.io.dino.read_dino_dir() function
+        kwargs are passed to the hydropandas.io.dino.read_dino_dir() function
 
     Returns
     -------
     ObsCollection
         collection of multiple point observations
     """
 
     oc = ObsCollection.from_dino(
         dirname=dirname,
         ObsClass=ObsClass,
         subdir=subdir,
         suffix=suffix,
-        unpackdir=unpackdir,
-        force_unpack=force_unpack,
-        preserve_datetime=preserve_datetime,
         keep_all_obs=keep_all_obs,
         name=name,
         **kwargs,
     )
 
     return oc
 
 
+def read_excel(path, meta_sheet_name="metadata"):
+    """Create an observation collection from an excel file. The excel file
+    should have the same format as excel files created with the `to_excel`
+    method of an ObsCollection.
+
+    Parameters
+    ----------
+    path : str
+        full file path (including extension) of the excel file.
+    meta_sheet_name : str, optional
+        sheetname with metadata. The default is "metadata".
+
+    Returns
+    -------
+    ObsCollection
+
+    Notes
+    -----
+    if you write an excel file using the 'to_excel' method and read an excel
+    with the 'read_excel' method you lose this information:
+    - The 'name' and 'meta' attributes of the ObsCollection
+    - metadata of each Observation stored in the 'meta' attribute
+
+    If you don't want to lose this data consider using the `to_pickle` and
+    `read_pickle` function.
+    """
+
+    oc = ObsCollection.from_excel(path, meta_sheet_name=meta_sheet_name)
+
+    return oc
+
+
 def read_fews(
     file_or_dir=None,
     xmlstring=None,
     ObsClass=obs.GroundwaterObs,
     name="fews",
     translate_dic=None,
     filterdict=None,
@@ -529,14 +548,64 @@
         exclude_layers=exclude_layers,
         method=method,
     )
 
     return oc
 
 
+def read_pickle(
+    filepath_or_buffer,
+    compression="infer",
+    storage_options=None,
+):
+    """wrapper around pd.read_pickle
+
+    Parameters
+    ----------
+    filepath_or_buffer : str, path object, or file-like object
+        String, path object (implementing ``os.PathLike[str]``), or file-like
+        object implementing a binary ``readlines()`` function.
+
+        .. versionchanged:: 1.0.0
+        Accept URL. URL is not limited to S3 and GCS.
+
+    compression : str or dict, default 'infer'
+        For on-the-fly decompression of on-disk data. If 'infer' and
+        'filepath_or_buffer' is path-like, then detect compression from the
+        following extensions: '.gz','.bz2', '.zip', '.xz', or '.zst' (otherwise
+        no compression). If using 'zip', the ZIP file must contain only one data
+        file to be read in. Set to ``None`` for no decompression. Can also be a
+        dict with key ``'method'`` set to one of {``'zip'``, ``'gzip'``,
+        ``'bz2'``, ``'zstd'``} and other key-value pairs are forwarded to
+        ``zipfile.ZipFile``, ``gzip.GzipFile``, ``bz2.BZ2File``, or
+        ``zstandard.ZstdDecompressor``, respectively. As an example, the
+        following could be passed for Zstandard decompression using a custom
+        compression dictionary: ``compression={'method': 'zstd', 'dict_data':
+        my_compression_dict}``.
+
+        .. versionchanged:: 1.4.0 Zstandard support.
+
+    storage_options : dict, optional
+        Extra options that make sense for a particular storage connection, e.g.
+        host, port, username, password, etc. For HTTP(S) URLs the key-value
+        pairs are forwarded to ``urllib`` as header options. For other URLs
+        (e.g. starting with "s3://", and "gcs://") the key-value pairs are
+        forwarded to ``fsspec``. Please see ``fsspec`` and ``urllib`` for more
+        details.
+
+        .. versionadded:: 1.2.0
+
+    Returns
+    -------
+    ObsCollection : same type as object stored in file
+    """
+
+    return pd.read_pickle(filepath_or_buffer, compression, storage_options)
+
+
 def read_waterinfo(
     file_or_dir, name="", ObsClass=obs.WaterlvlObs, progressbar=True, **kwargs
 ):
     """Read waterinfo file or directory.
 
     Parameters
     ----------
@@ -622,41 +691,55 @@
 
     An ObsCollection object is a subclass of a pandas.DataFrame and allows for
     additional attributes and methods. Additional attributes are
     defined in the '_metadata' attribute.
 
     Parameters
     ----------
-    name : str
-        name of the observation collection
-    meta : dic
-        metadata of the observation collection
+    *args observations, list of observations or a pandas DataFrame,
+    **kwargs can be one of these:
+        name : str
+            name of the observation collection
+        meta : dic
+            metadata of the observation collection
+
     """
 
     # temporary properties
     _internal_names = pd.DataFrame._internal_names + ["none"]
     _internal_names_set = set(_internal_names)
 
     # normal properties
     _metadata = [
         "name",
         "meta",
     ]
 
     def __init__(self, *args, **kwargs):
-        """constructor of the ObsCollection.
-
-        *args must be input for the pandas.DataFrame constructor,
-        **kwargs can be one of the attributes listed in _metadata or
-        keyword arguments for the constructor of a pandas.DataFrame.
-        """
         self.name = kwargs.pop("name", "")
         self.meta = kwargs.pop("meta", {})
 
-        super(ObsCollection, self).__init__(*args, **kwargs)
+        if isinstance(args[0], (list, tuple)):
+            logger.debug("Convert list of observations to ObsCollection")
+            obs_df = util._obslist_to_frame(args[0])
+            super().__init__(obs_df, *args[1:], **kwargs)
+        elif isinstance(args[0], obs.Obs):
+            logger.debug("Convert observation(s) to ObsCollection")
+            obs_list = [o for o in args if isinstance(o, obs.Obs)]
+            remaining_args = [o for o in args if not isinstance(o, obs.Obs)]
+            obs_df = util._obslist_to_frame(obs_list)
+            super().__init__(obs_df, *remaining_args, **kwargs)
+        elif isinstance(args[0], pd.DataFrame):
+            if "obs" not in args[0].columns:
+                df = self.from_dataframe(*args)
+                super().__init__(df, **kwargs)
+            else:
+                super().__init__(*args, **kwargs)
+        else:
+            super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
         return ObsCollection
 
     def _infer_otype(self):
         """Infer observation type from the obs column.
@@ -722,16 +805,15 @@
             self.rename(index={iname: value}, inplace=True)
         else:
             self.loc[iname, att_name] = value
         logger.debug(f"set {iname}, {att_name} to {value} in obscollection")
 
         if add_to_meta:
             o.meta.update({att_name: value})
-            logger.debug(
-                f"add {att_name} of {iname} with value {value} to meta")
+            logger.debug(f"add {att_name} of {iname} with value {value} to meta")
 
     def _is_consistent(self, check_individual_obs=True):
         """check if an observation collection is consistent. An observation
         collection is consistent if:
             1. all observations have a unique name
             2. there are no nan values in the obs column
             3. (optional) the metadata of each observation has the same type
@@ -759,16 +841,15 @@
                            not unique. non unique indices are:"""
             )
             logger.warning(" ".join(self.index[self.index.duplicated()]))
             return False
 
         # check nan values in observations
         if self.obs.isna().any():
-            logger.warning(
-                f"missing observation object in collection -> {self.name} ")
+            logger.warning(f"missing observation object in collection -> {self.name} ")
             return False
 
         # check oc data with individual object attributes
         if check_individual_obs:
             for o in self.obs.values:
                 for att in o._metadata:
                     if att not in ["name", "meta"]:
@@ -849,16 +930,15 @@
 
         """
         if check_consistency:
             if not self._is_consistent():
                 raise RuntimeError("inconsistent observation collection")
 
         if not isinstance(o, obs.Obs):
-            raise TypeError(
-                "Observation should be of type hydropandas.observation.Obs")
+            raise TypeError("Observation should be of type hydropandas.observation.Obs")
 
         # add new observation to collection
         if o.name not in self.index:
             logger.info(f"adding {o.name} to collection")
             self.loc[o.name] = o.to_collection_dict()
         else:
             logger.info(
@@ -1039,61 +1119,88 @@
         """
 
         if isinstance(df, pd.DataFrame):
             if obs_list is None:
                 obs_list = [ObsClass() for i in range(len(df))]
             df["obs"] = obs_list
         else:
-            raise TypeError(
-                f"df should be type pandas.DataFrame not {type(df)}")
+            raise TypeError(f"df should be type pandas.DataFrame not {type(df)}")
+
+        return cls(df)
+
+    @classmethod
+    def from_excel(cls, path, meta_sheet_name="metadata"):
+        """Create an observation collection from an excel file. The excel file
+        should have the same format as excel files created with the `to_excel`
+        method of an ObsCollection.
+
+        Parameters
+        ----------
+        path : str
+            full file path (including extension) of the excel file.
+        meta_sheet_name : str, optional
+            sheetname with metadata. The default is "metadata".
+
+        Returns
+        -------
+        ObsCollection
+
+        Notes
+        -----
+        if you write an excel file using the 'to_excel' method and read an excel
+        with the 'read_excel' method you lose this information:
+        - The 'name' and 'meta' attributes of the ObsCollection
+        - metadata of each Observation stored in the 'meta' attribute
+
+        If you don't want to lose this data consider using the `to_pickle` and
+        `read_pickle` function.
+        """
+
+        df = pd.read_excel(path, meta_sheet_name, index_col=0)
+
+        for oname, row in df.iterrows():
+            measurements = pd.read_excel(path, oname, index_col=0)
+            all_metadata = row.to_dict()
+            obsclass = getattr(obs, row["obs"])
+            # get observation specific metadata
+            metadata = {
+                k: v for (k, v) in all_metadata.items() if k in obsclass._metadata
+            }
+            metadata["name"] = oname
+
+            o = obsclass(measurements, **metadata)
+            df.at[oname, "obs"] = o
 
         return cls(df)
 
     @classmethod
     def from_dino(
         cls,
         dirname=None,
         ObsClass=obs.GroundwaterObs,
         subdir="Grondwaterstanden_Put",
         suffix="1.csv",
-        unpackdir=None,
-        force_unpack=False,
-        preserve_datetime=False,
         keep_all_obs=True,
         name=None,
         **kwargs,
     ):
         """Read dino data within an extent from the server or from a directory
         with downloaded files.
 
         Parameters
         ----------
         dirname : str, optional
             directory name, can be a .zip file or the parent directory
             of subdir
-        extent : list, tuple or numpy-array (user must specify extent or bbox)
-            get dinodata online within this extent [xmin, xmax, ymin, ymax]
-        bbox : list, tuple or numpy-array (user must specify extent or bbox)
-            The bounding box, in RD-coordinates, for which you want to
-            retrieve locations [xmin, ymin, xmax, ymax]
-        locations : list of str, optional
-            list of names with location and filter number, separated by
-            'filtersep'
         ObsClass : type
             class of the observations, so far only GroundwaterObs is supported
         subdir : str
             subdirectory of dirname with data files
         suffix : str
             suffix of files in subdir that will be read
-        unpackdir : str
-            destination directory of the unzipped file
-        force_unpack : boolean, optional
-            force unpack if dst already exists
-        preserve_datetime : boolean, optional
-            use date of the zipfile for the destination file
         keep_all_obs : boolean, optional
             add all observation points to the collection, even the points
             without measurements or metadata
         name : str, optional
             the name of the observation collection
         kwargs:
             kwargs are passed to the hydropandas.io.dino.read_dino_dir() function
@@ -1109,28 +1216,22 @@
         if name is None:
             name = subdir
 
         meta = {
             "dirname": dirname,
             "type": ObsClass,
             "suffix": suffix,
-            "unpackdir": unpackdir,
-            "force_unpack": force_unpack,
-            "preserve_datetime": preserve_datetime,
             "keep_all_obs": keep_all_obs,
         }
 
         obs_list = read_dino_dir(
             dirname,
             ObsClass,
             subdir,
             suffix,
-            unpackdir,
-            force_unpack,
-            preserve_datetime,
             keep_all_obs,
             **kwargs,
         )
 
         obs_df = util._obslist_to_frame(obs_list)
         return cls(obs_df, name=name, meta=meta)
 
@@ -1316,16 +1417,15 @@
                 remove_nan=remove_nan,
                 **kwargs,
             )
             obs_df = util._obslist_to_frame(obs_list)
             return cls(obs_df, name=name, meta=meta)
 
         else:
-            raise ValueError(
-                "either specify variables file_or_dir or xmlstring")
+            raise ValueError("either specify variables file_or_dir or xmlstring")
 
     @classmethod
     def from_imod(
         cls,
         obs_collection,
         ml,
         runfile,
@@ -1532,16 +1632,15 @@
                 elif meteovar == "EV24":
                     ObsClasses.append(obs.EvaporationObs)
                 else:
                     ObsClasses.append(obs.MeteoObs)
 
         elif isinstance(ObsClasses, type):
             if issubclass(
-                ObsClasses, (obs.PrecipitationObs,
-                             obs.EvaporationObs, obs.MeteoObs)
+                ObsClasses, (obs.PrecipitationObs, obs.EvaporationObs, obs.MeteoObs)
             ):
                 ObsClasses = [ObsClasses] * len(meteo_vars)
             else:
                 TypeError(
                     "must be None, PrecipitationObs, EvaporationObs, MeteoObs, "
                     "list or tuple"
                 )
@@ -1722,56 +1821,61 @@
             keep_all_obs=keep_all_obs,
             **kwargs,
         )
         obs_df = util._obslist_to_frame(obs_list)
 
         return cls(obs_df, name=name, meta=meta)
 
-    def to_excel(self, path, main_sheet_name=None):
-        """write an ObsCollection to an excel, the first sheet in the
+    def to_excel(self, path, meta_sheet_name="metadata"):
+        """Write an ObsCollection to an excel, the first sheet in the
         excel contains the metadata, the other tabs are the timeseries of each
         observation.
 
+        The excel can be read using the read_excel function of hydropandas.
 
         Parameters
         ----------
         path : str
             full path of xlsx file.
-        main_sheet_name : str or None, optional
-            sheetname with metadata, if None the name of the ObsCollection is
-            used. The default is None.
+        meta_sheet_name : str, optional
+            sheetname with metadata. The default is "metadata".
 
         Raises
         ------
         RuntimeError
             If the ObsCollection is inconsistent.
 
         Returns
         -------
         None.
 
-        """
-
-        if main_sheet_name is None:
-            main_sheet_name = self.name
+        Notes
+        -----
+        The following data is NOT written to the excel file:
+        - The 'name' and 'meta' attributes of the ObsCollection
+        - metadata of each Observation stored in the 'meta' dictionary
 
-        if main_sheet_name == "":
-            main_sheet_name = "metadata"
+        If you don't want this consider using the `to_pickle` method.
+        """
 
         if not self._is_consistent():
             raise RuntimeError("inconsistent observation collection")
 
+        oc = self.copy(deep=True)
+
         with pd.ExcelWriter(path) as writer:
-            # write ObsCollection dataframe without observations to first sheet
-            super(ObsCollection, self.drop(columns="obs")).to_excel(
-                writer, main_sheet_name
-            )
+            # replace obs column by observation type
+            obseries = oc.pop("obs")
+            oc["obs"] = [type(o).__name__ for o in obseries]
+
+            # write ObsCollection dataframe to first sheet
+            super(ObsCollection, oc).to_excel(writer, meta_sheet_name)
 
             # write each observation time series to next sheets
-            for o in self.obs.values:
+            for o in obseries:
                 sheetname = o.name
                 for ch in ["[", "]", ":", "*", "?", "/", "\\"]:
                     sheetname = sheetname.replace(ch, "_")
                 o.to_excel(writer, sheetname)
 
     def to_pi_xml(self, fname, timezone="", version="1.24"):
         from .io import fews
@@ -1994,28 +2098,26 @@
 
         fill_df = util.interpolate(
             xy, obsdf, xy_oc, kernel=kernel, kernel2=kernel2, epsilon=epsilon
         )
 
         # add all metadata that is equal for all observations
         kwargs = {}
-        meta_att = set(otype._metadata) - \
-            set(["x", "y", "name", "source", "meta"])
+        meta_att = set(otype._metadata) - set(["x", "y", "name", "source", "meta"])
         for att in meta_att:
             if (self.loc[:, att] == self.iloc[0].loc[att]).all():
                 kwargs[att] = self.iloc[0].loc[att]
 
         obs_list = []
         for i, col in enumerate(fill_df.columns):
             o = otype(
                 fill_df.loc[:, [col]].copy(),
                 x=xy[i][0],
                 y=xy[i][1],
                 name=col,
                 source=f"interpolation {self.name}",
-                meta={"interpolation_kernel": kernel,
-                      "interpolation_epsilon": epsilon},
+                meta={"interpolation_kernel": kernel, "interpolation_epsilon": epsilon},
                 **kwargs,
             )
             obs_list.append(o)
 
         return self.from_list(obs_list)
```

### Comparing `hydropandas-0.7.3/hydropandas/observation.py` & `hydropandas-0.8.0/hydropandas/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,41 +245,41 @@
                     same_metadata = False
                     if overlap == "error":
                         raise ValueError(
                             f"existing observation {key} differs from new observation"
                         )
                     elif overlap == "use_left":
                         logger.info(
-                            f"existing observation {key} differs from new"
+                            f"existing observation {key} differs from new "
                             "observation, use existing"
                         )
                         new_metadata[key] = v1
                     elif overlap == "use_right":
                         logger.info(
-                            f"existing observation {key} differs from new"
+                            f"existing observation {key} differs from new "
                             "observation, use new"
                         )
                         new_metadata[key] = v2
                 else:
                     new_metadata[key] = v1
             except TypeError:
                 same_metadata = False
                 if overlap == "error":
                     raise ValueError(
                         f"existing observation {key} differs from new observation"
                     )
                 elif overlap == "use_left":
                     logger.info(
-                        f"existing observation {key} differs from new"
+                        f"existing observation {key} differs from new "
                         "observation, use existing"
                     )
                     new_metadata[key] = v1
                 elif overlap == "use_right":
                     logger.info(
-                        f"existing observation {key} differs from new"
+                        f"existing observation {key} differs from new "
                         "observation, use new"
                     )
                     new_metadata[key] = v2
         if same_metadata:
             logger.info("new and existing observation have the same metadata")
 
         return new_metadata
@@ -327,15 +327,15 @@
         dup_ind_o = right.loc[right.index.isin(self.index)]
         if not dup_ind_o.empty:
             # check if overlapping timeseries have different values
             if not self.loc[dup_ind_o.index, overlap_cols].equals(
                 dup_ind_o[overlap_cols]
             ):
                 logger.warning(
-                    f"timeseries of observation {right.name} overlap with"
+                    f"timeseries of observation {right.name} overlap with "
                     "different values"
                 )
                 if overlap == "error":
                     raise ValueError(
                         "observations have different values for same time steps"
                     )
                 elif overlap == "use_left":
@@ -404,17 +404,14 @@
             when the time series have different values on the same date or
             different values for the same metadata.
 
         Returns
         -------
         Observation object.
         """
-        logger.warning(
-            "function 'merge_observation' not thoroughly tested, please be carefull!"
-        )
 
         if overlap not in ["error", "use_left", "use_right"]:
             raise ValueError(
                 "invalid value for overlap, choose between error, use_left and"
                 "use_right"
             )
 
@@ -482,15 +479,15 @@
         self.tube_nr = kwargs.pop("tube_nr", "")
         self.ground_level = kwargs.pop("ground_level", np.nan)
         self.tube_top = kwargs.pop("tube_top", np.nan)
         self.screen_top = kwargs.pop("screen_top", np.nan)
         self.screen_bottom = kwargs.pop("screen_bottom", np.nan)
         self.metadata_available = kwargs.pop("metadata_available", np.nan)
 
-        super(GroundwaterObs, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
         return GroundwaterObs
 
     @classmethod
     def from_bro(
@@ -633,16 +630,16 @@
         from .io import wiski
 
         data, metadata = wiski.read_wiski_file(fname, **kwargs)
 
         return cls(data, meta=metadata, **metadata)
 
 
-class GroundwaterQualityObs(Obs):
-    """class for groundwater quality (grondwatersamenstelling) point
+class WaterQualityObs(Obs):
+    """class for water quality ((grond)watersamenstelling) point
     observations.
 
     Subclass of the Obs class
     """
 
     _metadata = Obs._metadata + [
         "monitoring_well",
@@ -651,33 +648,33 @@
         "metadata_available",
     ]
 
     def __init__(self, *args, **kwargs):
         if len(args) > 0:
             if isinstance(args[0], Obs):
                 for key in args[0]._metadata:
-                    if (key in GroundwaterQualityObs._metadata) and (
+                    if (key in WaterQualityObs._metadata) and (
                         key not in kwargs.keys()
                     ):
                         kwargs[key] = getattr(args[0], key)
 
         self.monitoring_well = kwargs.pop("monitoring_well", "")
         self.tube_nr = kwargs.pop("tube_nr", "")
         self.ground_level = kwargs.pop("ground_level", np.nan)
         self.metadata_available = kwargs.pop("metadata_available", np.nan)
 
-        super(GroundwaterQualityObs, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
-        return GroundwaterQualityObs
+        return WaterQualityObs
 
     @classmethod
     def from_dino(cls, fname, **kwargs):
-        """read ad dino file with groundwater quality data.
+        """read dino file with groundwater quality data.
 
         Parameters
         ----------
         fname : str
             dino txt filename
         kwargs : key-word arguments
             these arguments are passed to
@@ -704,15 +701,15 @@
                 for key in args[0]._metadata:
                     if (key in WaterlvlObs._metadata) and (key not in kwargs.keys()):
                         kwargs[key] = getattr(args[0], key)
 
         self.monitoring_well = kwargs.pop("monitoring_well", "")
         self.metadata_available = kwargs.pop("metadata_available", np.nan)
 
-        super(WaterlvlObs, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
         return WaterlvlObs
 
     @classmethod
     def from_dino(cls, fname, **kwargs):
@@ -771,15 +768,15 @@
             if isinstance(args[0], Obs):
                 for key in args[0]._metadata:
                     if (key in ModelObs._metadata) and (key not in kwargs.keys()):
                         kwargs[key] = getattr(args[0], key)
 
         self.model = kwargs.pop("model", "")
 
-        super(ModelObs, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
         return ModelObs
 
 
 class MeteoObs(Obs):
@@ -796,15 +793,15 @@
                 for key in args[0]._metadata:
                     if (key in MeteoObs._metadata) and (key not in kwargs.keys()):
                         kwargs[key] = getattr(args[0], key)
 
         self.station = kwargs.pop("station", np.nan)
         self.meteo_var = kwargs.pop("meteo_var", "")
 
-        super(MeteoObs, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
         return MeteoObs
 
     @classmethod
     def from_knmi(
@@ -1297,15 +1294,15 @@
     def __init__(self, *args, **kwargs):
         if len(args) > 0:
             if isinstance(args[0], Obs):
                 for key in args[0]._metadata:
                     if (key in EvaporationObs._metadata) and (key not in kwargs.keys()):
                         kwargs[key] = getattr(args[0], key)
 
-        super(EvaporationObs, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
         return EvaporationObs
 
     @classmethod
     def from_knmi(
@@ -1594,15 +1591,15 @@
             if isinstance(args[0], Obs):
                 for key in args[0]._metadata:
                     if (key in PrecipitationObs._metadata) and (
                         key not in kwargs.keys()
                     ):
                         kwargs[key] = getattr(args[0], key)
 
-        super(PrecipitationObs, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def _constructor(self):
         return PrecipitationObs
 
     @classmethod
     def from_knmi(cls, stn, stn_type="meteo", meteo_var=None, **kwargs):
```

### Comparing `hydropandas-0.7.3/hydropandas/util.py` & `hydropandas-0.8.0/hydropandas/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         (useful for checking whether data has changed)
     """
     # check if unpackdir is same as file_or_dir, if same, this can cause
     # problems when the unpackdir still contains zips that will be unpacked
     # again.
     if unpackdir is not None:
         if os.path.normcase(unpackdir) == os.path.normcase(file_or_dir):
-            raise ValueError("Please specify a different folder to unpack" " files!")
+            raise ValueError("Please specify a different folder to unpack files!")
     # identify whether file_or_dir started as zip
     if file_or_dir.endswith(".zip"):
         iszip = True
     else:
         iszip = False
 
     # unzip dir
```

### Comparing `hydropandas-0.7.3/hydropandas.egg-info/PKG-INFO` & `hydropandas-0.8.0/hydropandas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hydropandas
-Version: 0.7.3
+Version: 0.8.0
 Summary: Module by Artesia for loading observation data into custom DataFrames.
 Author-email: Onno Ebbens <o.ebbens@artesia-water.nl>
-Maintainer-email: "O. Ebbens" <o.ebbens@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
+Maintainer-email: "O.N. Ebbens" <o.ebbens@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 O.E. Ebbens, D.A. Brakenhoff, R. Calje
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -35,118 +35,121 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: rtd
 Provides-Extra: linting
 Provides-Extra: formatting
 Provides-Extra: pytesting
 Provides-Extra: coveraging
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="/docs/_static/Artesia_logo.jpg" alt="Artesia" width="200" align="right">
 
 [![PyPi](https://img.shields.io/pypi/v/hydropandas.svg)](https://pypi.python.org/pypi/hydropandas)
-[![PyPi Supported Python Versions](https://img.shields.io/pypi/pyversions/hydropandas)](https://pypi.org/project/spei/)
+[![PyPi Supported Python Versions](https://img.shields.io/pypi/pyversions/hydropandas)](https://pypi.python.org/pypi/hydropandas)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArtesiaWater/hydropandas/master)
 
 [![hydropandas](https://github.com/ArtesiaWater/hydropandas/workflows/hydropandas/badge.svg)](https://github.com/ArtesiaWater/hydropandas/actions?query=workflow%3Ahydropandas)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/c1b99f474bdc49b0a47e00e4e9f66c2f)](https://www.codacy.com/gh/ArtesiaWater/hydropandas/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ArtesiaWater/hydropandas&utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/c1b99f474bdc49b0a47e00e4e9f66c2f)](https://www.codacy.com/gh/ArtesiaWater/hydropandas/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ArtesiaWater/hydropandas&utm_campaign=Badge_Coverage)
 [![Documentation Status](https://readthedocs.org/projects/hydropandas/badge/?version=latest)](https://hydropandas.readthedocs.io/en/latest/?badge=latest)
 
 [![Format: isort](https://img.shields.io/badge/imports-isort-ef8336)](https://pycqa.github.io/isort/index.html)
 [![Format: Black](https://img.shields.io/badge/code_style-black-black)](https://github.com/psf/black)
 [![Linter: flake8](https://img.shields.io/badge/linter-flake8-yellowgreen)](https://flake8.pycqa.org/)
 [![Linter: ruff](https://img.shields.io/badge/linter-ruff-red)](https://github.com/charliermarsh/ruff)
 
-# hydropandas
+# HydroPandas
 
-The HydroPandas package allows users to store observation data at multiple locations in a single object (ObsCollection).
+Python tools for hydrological measurement data.
+
+## Introduction
+
+The HydroPandas package allows users to store observation data at multiple locations in a single object: ObsCollection.
+An ObsCollection makes it easier to analyse, visualise and export the observation data.
 An ObsCollection is a pandas DataFrame extended with custom methods and attributes related to hydrological timeseries.
+
 The HydroPandas package also provides convenient read functions for Dutch hydrological data from:
--   [BRO](https://www.broloket.nl)
--   [DINO](https://www.dinoloket.nl)
--   FEWS PI-XML
--   [KNMI](https://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script)
--   MODFLOW groundwater models
--   IMOD groundwater models
--   [Pastastore](https://github.com/pastas/pastastore)
--   [waterinfo](https://waterinfo.rws.nl/)
--   WISKI csv files
 
+- [BRO](https://www.broloket.nl)
+- [DINO](https://www.dinoloket.nl)
+- FEWS PI-XML
+- [KNMI](https://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script)
+- MODFLOW groundwater models
+- IMOD groundwater models
+- [Pastastore](https://github.com/pastas/pastastore)
+- [waterinfo](https://waterinfo.rws.nl/)
+- WISKI csv files
 
-## Installation
+## Install
 
 Install the module with pip:
 
 `pip install hydropandas`
 
-Hydropandas requires `numpy`, `scipy`, `matplotlib`, `pandas`, `requests` and `zeep`.
+HydroPandas requires `pandas`, `scipy`, `matplotlib`, `tqdm`, `requests` and `colorama`.
 
 For some functionality additional packages are required:
 
--   `geopandas`: for dealing with shapefiles
--   `pastastore`: for reading or storing data from PastaStore
--   `bokeh`, `branca`, `folium`: for interactive maps
--   `flopy`: for reading data from MODFLOW models
--   `xarray`: for loading data from REGIS
+- `geopandas`: for dealing with shapefiles
+- `pastastore`: for reading or storing data from PastaStore
+- `bokeh`, `branca`, `folium`: for interactive maps
+- `flopy`: for reading data from MODFLOW models
+- `xarray`: for loading data from REGIS
 
 For installing in development mode, clone the repository and install by
 typing `pip install -e .` from the module root directory.
-For installing all the optional packages use `pip install -e .[full]`
+For installing all the optional packages use `pip install -e .[full]`.
+
+## Get in touch
 
-If you have trouble installing HydroPandas, refer to the
-[Dependencies section](#dependencies) below.
+- Questions on HydroPandas ("How can I?") can be asked and answered on [Github Discussions](https://github.com/ArtesiaWater/hydropandas/discussions).
+- Bugs, feature requests and other improvements can be posted as [Github Issues](https://github.com/ArtesiaWater/hydropandas/issues).
+- Find out how to contribute to HydroPandas at our [Contribution page](https://hydropandas.readthedocs.io/en/stable/contribute.html).
 
-## Example usage
+## Examples
 
-Importing a single DINO csv file:
+Importing a groundwater time series from the BRO using the BRO-id and the tube number:
 
 ```python
 import hydropandas as hpd
-fname = './tests/data/2019-Dino-test/Grondwaterstanden_Put/B33F0080001_1.csv'
-gw = hpd.GroundwaterObs.from_dino(fname=fname)
+gw_bro = hpd.GroundwaterObs.from_bro("GMW000000041261", 1)
 ```
 
-Or for a zipfile:
+Or import all groundwater time series from the BRO within a certain extent:
 
 ```python
-import hydropandas as hpd
-dinozip = './tests/data/2019-Dino-test/dino.zip'
-dino_gw = hpd.read_dino(dirname=dinozip,
-			subdir='Grondwaterstanden_Put',
-                        suffix='1.csv',
-                        ObsClass=hpd.GroundwaterObs,
-                        keep_all_obs=False)
+oc = hpd.read_bro(extent=(117850, 118180, 439550, 439900))
 ```
 
 ## The Obs class
 
 The Obs class holds the measurements and metadata for one timeseries. There are
 currently 5 specific Obs classes for different types of measurements:
 
--   GroundwaterObs: for groundwater measurements
--   GroundwaterQualityObs: for groundwater quality measurements
--   WaterlvlObs: for surface water level measurements
--   ModelObs: for "observations" from a MODFLOW model
--   MeteoObs: for meteorological observations
--   PrecipitationObs: for precipitation observations, subclass of MeteoObs
--   EvaporationObs: for evaporation observations, subclass of MeteoObs
+- GroundwaterObs: for groundwater measurements
+- WaterQualityObs: for groundwater quality measurements
+- WaterlvlObs: for surface water level measurements
+- ModelObs: for "observations" from a MODFLOW model
+- MeteoObs: for meteorological observations
+- PrecipitationObs: for precipitation observations, subclass of MeteoObs
+- EvaporationObs: for evaporation observations, subclass of MeteoObs
 
 Each of these Obs classes is essentially a pandas DataFrame with additional
 methods and attributes related to the type of measurement that it holds.
-The classes also contain specific methods to read data from specific sources.
+Each Obs object also contain specific methods to read data from specific sources.
 
 ## The ObsCollection class
 
 The ObsCollection class, as the name implies, represents a collection of Obs
 classes, e.g. 10 timeseries of the groundwater level in a certain area. The
 ObsCollection is also a pandas DataFrame in which each timeseries is stored
 in a different row. Each row contains metadata (e.g. latitude and longitude
@@ -155,48 +158,13 @@
 type, e.g. to create an ObsCollection for 10 GroundwaterObs, and a separate
 ObsCollection for 5 PrecipitationObs.
 
 Like the Obs class, the ObsCollection class contains a bunch of methods for
 reading data from different sources. See the next section for supported data
 sources.
 
-## Dependencies
-
-Hydropandas (indirectly) uses some packages that cannot be installed
-automatically with `pip` on Windows. These packages are:
-
--   GDAL
--   Fiona
--   Shapely
-
-If you do not have these packages already it is recommended to first try
-installing them with `conda install <pkg>`. Otherwise, read the instructions
-below how to install them manually.
-
-Download the packages from [Christoph Gohlke's website](https://www.lfd.uci.edu/~gohlke/pythonlibs).
-Use CTRL+F to find the download link on the page. Be sure to download the
-correct version of the package. The Python version should match your Python
-version. Also the architecture should match (i.e. 64bits vs 32bits).
-For example:
-
--   GDAL-3.1.4-cp38-cp38-win_amd64.whl
-
-This is the GDAL version for Python 3.8 (as can be seen from the cp38 in the
-name), for 64-bits Python (as derived from the amd64 in the name).
-
-Once you have downloaded the correct files, navigate to the directory in which
-you saved your downloads. Now type the following commands (the order is
-important):
-
-1.  `pip install GDAL-3.1.4-cp38-cp38-win_amd64.whl`
-2.  `pip install Fiona-1.8.17-cp38-cp38-win_amd64.whl`
-3.  `pip install Shapely-1.7.1-cp38-cp38-win_amd64.whl`
-
-After you've done this you can install hydropandas using
-`pip install hydropandas`.
-
 ## Authors
 
--   Onno Ebbens, Artesia
--   Ruben Caljé, Artesia
--   Davíd Brakenhoff, Artesia
--   Martin Vonk, Artesia
+- Onno Ebbens, Artesia
+- Ruben Caljé, Artesia
+- Davíd Brakenhoff, Artesia
+- Martin Vonk, Artesia
```

### Comparing `hydropandas-0.7.3/hydropandas.egg-info/SOURCES.txt` & `hydropandas-0.8.0/hydropandas.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 hydropandas/util.py
 hydropandas/version.py
 hydropandas.egg-info/PKG-INFO
 hydropandas.egg-info/SOURCES.txt
 hydropandas.egg-info/dependency_links.txt
 hydropandas.egg-info/requires.txt
 hydropandas.egg-info/top_level.txt
+hydropandas/data/fews_parameterid.py
 hydropandas/data/knmi_meteostation.json
 hydropandas/data/knmi_neerslagstation.json
 hydropandas/extensions/__init__.py
 hydropandas/extensions/accessor.py
 hydropandas/extensions/geo.py
 hydropandas/extensions/gwobs.py
 hydropandas/extensions/plots.py
```

### Comparing `hydropandas-0.7.3/pyproject.toml` & `hydropandas-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,68 +6,63 @@
 name = "hydropandas"
 dynamic = ["version"]
 description = "Module by Artesia for loading observation data into custom DataFrames."
 license = { file = "LICENSE" }
 readme = "readme.md"
 authors = [{ name = "Onno Ebbens", email = "o.ebbens@artesia-water.nl" }]
 maintainers = [
-    { name = "O. Ebbens", email = "o.ebbens@artesia-water.nl" },
+    { name = "O.N. Ebbens", email = "o.ebbens@artesia-water.nl" },
     { name = "R. Calje", email = "r.calje@artesia-water.nl" },
     { name = "D.A. Brakenhoff", email = "d.brakenhoff@artesia-water.nl" },
     { name = "M.A. Vonk", email = "m.vonk@artesia-water.nl" },
 ]
 requires-python = ">=3.7"
-dependencies = [
-    "scipy",
-    "pandas",
-    "matplotlib",
-    "tqdm",
-    "requests",
-    "zeep",
-    "colorama",
-]
+dependencies = ["scipy", "pandas", "matplotlib", "tqdm", "requests", "colorama"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: MIT License",
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     "Operating System :: OS Independent",
+    'Topic :: Scientific/Engineering :: Hydrology',
 ]
 
 [project.urls]
 homepage = "https://www.artesia-water.nl"
 repository = "https://github.com/artesiawater/hydropandas"
 documentation = "https://hydropandas.readthedocs.io/en/stable/"
 
 [project.optional-dependencies]
 full = [
     "geopandas",
+    "openpyxl",
     "pastastore",
     "bokeh",
     "branca",
     "folium",
     "flopy",
     "xarray",
     "shapely",
     "pyproj",
+    "contextily"
 ]
 rtd = [
     "hydropandas[full]",
     "imod",
     "lxml",
     "requests",
     "Shapely",
     "nbconvert",
     "ipykernel",
-    "netCDF4>=1.5.7",
+    "netCDF4==1.5.8",
     "docutils<0.18",
     "sphinx_rtd_theme",
     "Ipython",
     "nbsphinx",
     "nbsphinx_link",
 ]
 linting = ["flake8", "ruff"]
@@ -119,16 +114,16 @@
             coverage xml
 
     [testenv:format]
     description = run formatters
     basepython = python3.9
     extras = formatting
     commands =
-            black .
-            isort .
+            black . --check --diff
+            isort . --check-only --diff
 
     [testenv:lint]
     description = run linters
     basepython = python3.9
     extras = linting
     commands =
             flake8 . --max-line-length=88 --ignore=E741,W503
```

### Comparing `hydropandas-0.7.3/readme.md` & `hydropandas-0.8.0/readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,102 @@
 <img src="/docs/_static/Artesia_logo.jpg" alt="Artesia" width="200" align="right">
 
 [![PyPi](https://img.shields.io/pypi/v/hydropandas.svg)](https://pypi.python.org/pypi/hydropandas)
-[![PyPi Supported Python Versions](https://img.shields.io/pypi/pyversions/hydropandas)](https://pypi.org/project/spei/)
+[![PyPi Supported Python Versions](https://img.shields.io/pypi/pyversions/hydropandas)](https://pypi.python.org/pypi/hydropandas)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ArtesiaWater/hydropandas/master)
 
 [![hydropandas](https://github.com/ArtesiaWater/hydropandas/workflows/hydropandas/badge.svg)](https://github.com/ArtesiaWater/hydropandas/actions?query=workflow%3Ahydropandas)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/c1b99f474bdc49b0a47e00e4e9f66c2f)](https://www.codacy.com/gh/ArtesiaWater/hydropandas/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ArtesiaWater/hydropandas&utm_campaign=Badge_Grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/c1b99f474bdc49b0a47e00e4e9f66c2f)](https://www.codacy.com/gh/ArtesiaWater/hydropandas/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ArtesiaWater/hydropandas&utm_campaign=Badge_Coverage)
 [![Documentation Status](https://readthedocs.org/projects/hydropandas/badge/?version=latest)](https://hydropandas.readthedocs.io/en/latest/?badge=latest)
 
 [![Format: isort](https://img.shields.io/badge/imports-isort-ef8336)](https://pycqa.github.io/isort/index.html)
 [![Format: Black](https://img.shields.io/badge/code_style-black-black)](https://github.com/psf/black)
 [![Linter: flake8](https://img.shields.io/badge/linter-flake8-yellowgreen)](https://flake8.pycqa.org/)
 [![Linter: ruff](https://img.shields.io/badge/linter-ruff-red)](https://github.com/charliermarsh/ruff)
 
-# hydropandas
+# HydroPandas
 
-The HydroPandas package allows users to store observation data at multiple locations in a single object (ObsCollection).
+Python tools for hydrological measurement data.
+
+## Introduction
+
+The HydroPandas package allows users to store observation data at multiple locations in a single object: ObsCollection.
+An ObsCollection makes it easier to analyse, visualise and export the observation data.
 An ObsCollection is a pandas DataFrame extended with custom methods and attributes related to hydrological timeseries.
+
 The HydroPandas package also provides convenient read functions for Dutch hydrological data from:
--   [BRO](https://www.broloket.nl)
--   [DINO](https://www.dinoloket.nl)
--   FEWS PI-XML
--   [KNMI](https://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script)
--   MODFLOW groundwater models
--   IMOD groundwater models
--   [Pastastore](https://github.com/pastas/pastastore)
--   [waterinfo](https://waterinfo.rws.nl/)
--   WISKI csv files
 
+- [BRO](https://www.broloket.nl)
+- [DINO](https://www.dinoloket.nl)
+- FEWS PI-XML
+- [KNMI](https://www.knmi.nl/kennis-en-datacentrum/achtergrond/data-ophalen-vanuit-een-script)
+- MODFLOW groundwater models
+- IMOD groundwater models
+- [Pastastore](https://github.com/pastas/pastastore)
+- [waterinfo](https://waterinfo.rws.nl/)
+- WISKI csv files
 
-## Installation
+## Install
 
 Install the module with pip:
 
 `pip install hydropandas`
 
-Hydropandas requires `numpy`, `scipy`, `matplotlib`, `pandas`, `requests` and `zeep`.
+HydroPandas requires `pandas`, `scipy`, `matplotlib`, `tqdm`, `requests` and `colorama`.
 
 For some functionality additional packages are required:
 
--   `geopandas`: for dealing with shapefiles
--   `pastastore`: for reading or storing data from PastaStore
--   `bokeh`, `branca`, `folium`: for interactive maps
--   `flopy`: for reading data from MODFLOW models
--   `xarray`: for loading data from REGIS
+- `geopandas`: for dealing with shapefiles
+- `pastastore`: for reading or storing data from PastaStore
+- `bokeh`, `branca`, `folium`: for interactive maps
+- `flopy`: for reading data from MODFLOW models
+- `xarray`: for loading data from REGIS
 
 For installing in development mode, clone the repository and install by
 typing `pip install -e .` from the module root directory.
-For installing all the optional packages use `pip install -e .[full]`
+For installing all the optional packages use `pip install -e .[full]`.
+
+## Get in touch
 
-If you have trouble installing HydroPandas, refer to the
-[Dependencies section](#dependencies) below.
+- Questions on HydroPandas ("How can I?") can be asked and answered on [Github Discussions](https://github.com/ArtesiaWater/hydropandas/discussions).
+- Bugs, feature requests and other improvements can be posted as [Github Issues](https://github.com/ArtesiaWater/hydropandas/issues).
+- Find out how to contribute to HydroPandas at our [Contribution page](https://hydropandas.readthedocs.io/en/stable/contribute.html).
 
-## Example usage
+## Examples
 
-Importing a single DINO csv file:
+Importing a groundwater time series from the BRO using the BRO-id and the tube number:
 
 ```python
 import hydropandas as hpd
-fname = './tests/data/2019-Dino-test/Grondwaterstanden_Put/B33F0080001_1.csv'
-gw = hpd.GroundwaterObs.from_dino(fname=fname)
+gw_bro = hpd.GroundwaterObs.from_bro("GMW000000041261", 1)
 ```
 
-Or for a zipfile:
+Or import all groundwater time series from the BRO within a certain extent:
 
 ```python
-import hydropandas as hpd
-dinozip = './tests/data/2019-Dino-test/dino.zip'
-dino_gw = hpd.read_dino(dirname=dinozip,
-			subdir='Grondwaterstanden_Put',
-                        suffix='1.csv',
-                        ObsClass=hpd.GroundwaterObs,
-                        keep_all_obs=False)
+oc = hpd.read_bro(extent=(117850, 118180, 439550, 439900))
 ```
 
 ## The Obs class
 
 The Obs class holds the measurements and metadata for one timeseries. There are
 currently 5 specific Obs classes for different types of measurements:
 
--   GroundwaterObs: for groundwater measurements
--   GroundwaterQualityObs: for groundwater quality measurements
--   WaterlvlObs: for surface water level measurements
--   ModelObs: for "observations" from a MODFLOW model
--   MeteoObs: for meteorological observations
--   PrecipitationObs: for precipitation observations, subclass of MeteoObs
--   EvaporationObs: for evaporation observations, subclass of MeteoObs
+- GroundwaterObs: for groundwater measurements
+- WaterQualityObs: for groundwater quality measurements
+- WaterlvlObs: for surface water level measurements
+- ModelObs: for "observations" from a MODFLOW model
+- MeteoObs: for meteorological observations
+- PrecipitationObs: for precipitation observations, subclass of MeteoObs
+- EvaporationObs: for evaporation observations, subclass of MeteoObs
 
 Each of these Obs classes is essentially a pandas DataFrame with additional
 methods and attributes related to the type of measurement that it holds.
-The classes also contain specific methods to read data from specific sources.
+Each Obs object also contain specific methods to read data from specific sources.
 
 ## The ObsCollection class
 
 The ObsCollection class, as the name implies, represents a collection of Obs
 classes, e.g. 10 timeseries of the groundwater level in a certain area. The
 ObsCollection is also a pandas DataFrame in which each timeseries is stored
 in a different row. Each row contains metadata (e.g. latitude and longitude
@@ -103,48 +105,13 @@
 type, e.g. to create an ObsCollection for 10 GroundwaterObs, and a separate
 ObsCollection for 5 PrecipitationObs.
 
 Like the Obs class, the ObsCollection class contains a bunch of methods for
 reading data from different sources. See the next section for supported data
 sources.
 
-## Dependencies
-
-Hydropandas (indirectly) uses some packages that cannot be installed
-automatically with `pip` on Windows. These packages are:
-
--   GDAL
--   Fiona
--   Shapely
-
-If you do not have these packages already it is recommended to first try
-installing them with `conda install <pkg>`. Otherwise, read the instructions
-below how to install them manually.
-
-Download the packages from [Christoph Gohlke's website](https://www.lfd.uci.edu/~gohlke/pythonlibs).
-Use CTRL+F to find the download link on the page. Be sure to download the
-correct version of the package. The Python version should match your Python
-version. Also the architecture should match (i.e. 64bits vs 32bits).
-For example:
-
--   GDAL-3.1.4-cp38-cp38-win_amd64.whl
-
-This is the GDAL version for Python 3.8 (as can be seen from the cp38 in the
-name), for 64-bits Python (as derived from the amd64 in the name).
-
-Once you have downloaded the correct files, navigate to the directory in which
-you saved your downloads. Now type the following commands (the order is
-important):
-
-1.  `pip install GDAL-3.1.4-cp38-cp38-win_amd64.whl`
-2.  `pip install Fiona-1.8.17-cp38-cp38-win_amd64.whl`
-3.  `pip install Shapely-1.7.1-cp38-cp38-win_amd64.whl`
-
-After you've done this you can install hydropandas using
-`pip install hydropandas`.
-
 ## Authors
 
--   Onno Ebbens, Artesia
--   Ruben Caljé, Artesia
--   Davíd Brakenhoff, Artesia
--   Martin Vonk, Artesia
+- Onno Ebbens, Artesia
+- Ruben Caljé, Artesia
+- Davíd Brakenhoff, Artesia
+- Martin Vonk, Artesia
```

### Comparing `hydropandas-0.7.3/tests/test_000_run_notebooks.py` & `hydropandas-0.8.0/tests/test_000_run_notebooks.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.7.3/tests/test_001_to_from.py` & `hydropandas-0.8.0/tests/test_001_to_from.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     # single observation
     bro_id = "GMN000000000163"
     hpd.read_bro(bro_id=bro_id, only_metadata=True)
     return
 
 
 def test_bro_extent():
-    extent = (210260, 213550, 459890, 473920)  # extent more than 1000 observations
-    extent = (213260, 213550, 473890, 473920)  # extent skip duplicates
+    # extent = (210260, 213550, 459890, 473920)  # extent more than 1000 observations
+    # extent = (213260, 213550, 473890, 473920)  # extent skip duplicates
     extent = (102395, 103121, 434331, 434750)  # 4 observations within extent
 
     hpd.read_bro(extent=extent, only_metadata=True)
     return
 
 
 def test_bro_extent_too_big():
@@ -41,15 +41,15 @@
 
 dinozip = "./tests/data/2019-Dino-test/dino.zip"
 
 
 def test_observation_gwq():
     # single observation
     fname = "./tests/data/2019-Dino-test/Grondwatersamenstellingen_Put/B52C0057.txt"
-    hpd.GroundwaterQualityObs.from_dino(fname)
+    hpd.WaterQualityObs.from_dino(fname)
     return
 
 
 def test_observation_wl():
     fname = "./tests/data/2019-Dino-test/Peilschaal/P58A0001.csv"
     hpd.WaterlvlObs.from_dino(fname)
     return
@@ -66,27 +66,29 @@
         dirname=dinozip,
         ObsClass=hpd.GroundwaterObs,
         subdir="Grondwaterstanden_Put",
         suffix="1.csv",
         keep_all_obs=True,
     )
     obs_list = [o for o in dino_gw.obs.values]
-    hpd.ObsCollection.from_list(obs_list)
+    hpd.ObsCollection(obs_list)
     return
 
 
 def test_obscollection_from_df():
     df = pd.DataFrame(index=["pb1", "pb2"], data={"tube_nr": [1, 1]})
 
-    hpd.ObsCollection.from_dataframe(df)
+    hpd.ObsCollection(df)
 
     return
 
 
 # read dino directories
+
+
 def test_obscollection_dinozip_gw():
     # groundwater quantity
     oc = hpd.read_dino(
         dirname=dinozip,
         ObsClass=hpd.GroundwaterObs,
         subdir="Grondwaterstanden_Put",
         suffix="1.csv",
@@ -116,15 +118,15 @@
     return oc
 
 
 def test_obscollection_dinozip_gwq():
     # groundwater quality
     hpd.read_dino(
         dirname=dinozip,
-        ObsClass=hpd.GroundwaterQualityObs,
+        ObsClass=hpd.WaterQualityObs,
         subdir="Grondwatersamenstellingen_Put",
         suffix=".txt",
     )
     return
 
 
 # %% FEWS
@@ -164,187 +166,176 @@
         header_sep=":",
         header_identifier=":",
         parse_dates={"datetime": [0, 1]},
         index_col=["datetime"],
         translate_dic={"name": "Station Number", "x": "GlobalX", "y": "GlobalY"},
     )
 
-    return
-
 
 @pytest.mark.slow
 def test_obscollection_wiskizip_gw():
     hpd.read_wiski(
         r"./tests/data/2019-WISKI-test/1016_PBF.zip",
         translate_dic={"name": "Station Number", "x": "GlobalX", "y": "GlobalY"},
         sep=r"\s+",
         header_sep=":",
         dayfirst=True,
         header_identifier=":",
         parse_dates={"datetime": [0, 1]},
         index_col=["datetime"],
     )
 
-    return
-
 
 # %% PASTASTORE
 def test_to_pastastore():
     dino_gw = test_obscollection_dinozip_gw()
     # drop duplicate
     dino_gw.drop("B22D0155-001", inplace=True)
     dino_gw.to_pastastore()
 
-    return
+
+# %% excel
+
+
+def test_to_excel():
+    oc = hpd.read_fews(
+        "./tests/data/2019-FEWS-test/WaalenBurg_201810-20190215_prod.zip",
+        locations=None,
+        low_memory=True,
+    )
+
+    oc.to_excel("tests/data/excel/test.xlsx")
+
+
+def test_from_excel():
+    hpd.read_excel("tests/data/excel/test.xlsx")
 
 
 # %% Meteo
 
 
 def test_pressure_obs_from_stn():
     hpd.MeteoObs.from_knmi(
         310, meteo_var="P", interval="hourly", fill_missing_obs=False
     )
 
-    return
-
 
 def test_pressure_read_knmi():
     hpd.read_knmi(
         stns=(310,),
         meteo_vars=("P",),
         settings={
             "interval": "hourly",
             "fill_missing_obs": False,
             "inseason": False,
             "normalize_index": True,
         },
     )
 
-    return
-
 
 # %% Evaporation
 
 
 def test_evap_obs_from_file():
     fname = "./tests/data/2023-KNMI-test/etmgeg_260.txt"
     hpd.EvaporationObs.from_knmi_file(fname)
 
-    return
-
 
 def test_evap_obs_from_stn():
     hpd.EvaporationObs.from_knmi(260, et_type="EV24")
-    return
 
 
 def test_evap_obs_from_stn_makkink():
     hpd.EvaporationObs.from_knmi(260, et_type="makkink")
-    return
 
 
 def test_evap_obs_from_stn_penman():
     hpd.EvaporationObs.from_knmi(260, et_type="penman")
-    return
 
 
 def test_evap_obs_from_stn_hargreaves():
     hpd.EvaporationObs.from_knmi(260, et_type="hargreaves")
-    return
 
 
 # %% Precipitation
 
 
 def test_precip_obs_from_file():
     fname = "./tests/data/2023-KNMI-test/neerslaggeg_ESBEEK_831.txt"
     hpd.PrecipitationObs.from_knmi_file(fname)
-    return
 
 
 def test_precip_obs_from_stn():
     hpd.PrecipitationObs.from_knmi(233, "precipitation")
-    return
 
 
 def test_knmi_obs_from_stn_no_api():
     hpd.PrecipitationObs.from_knmi(233, "precipitation", use_api=False)
-    return
 
 
 def test_knmi_obs_from_stn_without_any_data():
     hpd.EvaporationObs.from_knmi(
         210, startdate="19500101", enddate="19600101", fill_missing_obs=False
     )
 
-    return
-
 
 def test_knmi_obs_from_stn_with_missing_data_in_time_period():
     hpd.PrecipitationObs.from_knmi("441", "precipitation", startdate="2010-1-2")
-    return
 
 
 def test_knmi_obs_from_xy():
     hpd.PrecipitationObs.from_nearest_xy((100000, 350000))
-    return
 
 
 def test_knmi_obs_from_obs():
     pb = test_observation_gw()
-    o = hpd.PrecipitationObs.from_obs(pb, fill_missing_obs=False)
-    return o
+    hpd.PrecipitationObs.from_obs(pb, fill_missing_obs=False)
 
 
 # @pytest.xfail(
 #     "Station HEIBLOEM 967 not available. See issue"
 #     " https://github.com/ArtesiaWater/hydropandas/issues/103"
 # )
 def test_knmi_collection_from_locations():
     obsc = test_obscollection_dinozip_gw()
     try:
         hpd.read_knmi(
             locations=obsc, meteo_vars=["EV24", "RD"], starts="2010", ends="2015"
         )
     except ConnectionError:
         pass
-    return
 
 
 def test_knmi_collection_from_stns():
     stns = [344, 260]  # Rotterdam en de Bilt
     hpd.read_knmi(
         stns=stns,
         meteo_vars=["EV24", "RH"],
         starts=["2010", "2010"],
         ends=["2015", "2015"],
     )
-    return
 
 
 def test_knmi_collection_from_grid():
     # somewhere in Noord-Holland (near Castricum)
     xy = [[104150.0, 510150.0], [104550.0, 510550.0]]
     hpd.read_knmi(
         xy=xy,
         meteo_vars=["RH"],
         starts=["2010"],
         ends=["2015"],
     )
-    return
 
 
 # %% WATERINFO
 
 
 def test_waterinfo_from_dir():
     path = "./tests/data/waterinfo-test"
     hpd.read_waterinfo(path)
-    return
 
 
 # %% MENYANTHES (still need a small menyanthes file to do the test)
 
 # def test_obscollection_menyanthes():
 #
 #    fname = r'export_from_ADI.men'
```

### Comparing `hydropandas-0.7.3/tests/test_002_obs_objects.py` & `hydropandas-0.8.0/tests/test_002_obs_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         name="waterquality_obs1",
         monitoring_well="waterquality",
         x=3,
         y=4,
         filename="",
         meta={"info": "you can store additional information in this dictionary"},
     )
-    return
 
 
 def test_obscollection_from_list():
     o_list = []
     for i in range(10):
         o_list.append(test_groundwater_obs(name=f"groundwaterobs_00{i}", tube_nr=i))
 
@@ -156,16 +155,14 @@
     omerged = o.merge_observation(o2)
 
     assert omerged.shape == (
         20,
         1,
     ), "merged observation should have one column with 20 values"
 
-    return
-
 
 def test_merge_overlapping():
     # base
     o = test_groundwater_obs(name="groundwaterobs_010", tube_nr=10)
 
     # observation with partially overlapping time series and extra columns
     o2 = o.copy()
@@ -177,16 +174,14 @@
     omerged = o.merge_observation(o2)
 
     assert omerged.shape == (
         15,
         3,
     ), "merged observation should have one column with 20 values"
 
-    return
-
 
 def test_merge_errors():
     # base
     o = test_groundwater_obs(name="groundwaterobs_010", tube_nr=10)
 
     # observation with partially overlapping time series and extra columns
     o2 = test_waterlvl_obs()
```

### Comparing `hydropandas-0.7.3/tests/test_003_calculations.py` & `hydropandas-0.8.0/tests/test_003_calculations.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,68 +2,60 @@
 
 
 def test_within_extent():
     dino_gw = ttf.test_obscollection_dinozip_gw()
     extent = [210350, 213300, 473300, 474000]
     dino_gw.geo.within_extent(extent, inplace=True)
     assert dino_gw.shape[0] == 4
-    return
 
 
 # %% stats
 
 
 def test_obscollection_consecutive_obs_years():
     gw = ttf.test_obscollection_dinozip_gw_keep_all_obs()
     gw.stats.consecutive_obs_years()
-    return
 
 
 def test_obscollection_get_number_of_obs():
     gw = ttf.test_obscollection_dinozip_gw_keep_all_obs()
     gw.stats.get_no_of_observations()
-    return
 
 
 def test_obscollection_get_first_last_obs_date():
     gw = ttf.test_obscollection_dinozip_gw_keep_all_obs()
     gw.stats.get_first_last_obs_date()
-    return
 
 
 def test_obscollection_get_seasonal_stats():
     gw = ttf.test_obscollection_dinozip_gw_keep_all_obs()
     gw.stats.get_seasonal_stat(stat="mean")
-    return
 
 
 def test_obscollection_get_min():
     gw = ttf.test_obscollection_dinozip_gw_keep_all_obs()
     gw.stats.get_min()
-    return
 
 
 def test_obscollection_get_max():
     gw = ttf.test_obscollection_dinozip_gw_keep_all_obs()
     gw.stats.get_max()
-    return
 
 
 # %% geo
 
 
 def test_get_nearest_point():
     # check two of the same observation collections
     # every point must find itself as the nearest point
     dino_gw = ttf.test_obscollection_dinozip_gw()
     fl = ttf.test_obscollection_dinozip_wl()
     dino_gw[
         ["nearest point", "distance nearest point"]
     ] = dino_gw.geo.get_nearest_point(fl)
-    return
 
 
 def test_get_nearest_polygon():
     import geopandas as gpd
     from shapely.geometry import Polygon
 
     # check two of the same observation collections
@@ -92,32 +84,28 @@
 
     dino_gw[
         ["nearest polygon", "distance nearest polygon"]
     ] = dino_gw.geo.get_nearest_polygon(gdf)
     assert (dino_gw["nearest polygon"] == 0.0).all()
     assert (dino_gw["distance nearest polygon"] == 0.0).all()
 
-    return
-
 
 def test_get_ground_level_oc():
     try:
         from art_tools import hpd_extension  # noqa: F401
 
         gw = ttf.test_obscollection_fews_lowmemory()
         gw.art.geo_get_ground_level()
         return
     except ModuleNotFoundError as e:
         print(e)
-    return
 
 
 def test_get_ground_level_gwobs():
     try:
         from art_tools import hpd_extension  # noqa: F401
 
         gw = ttf.test_observation_gw()
         gw.art.geo_get_ground_level()
         return
     except ModuleNotFoundError as e:
         print(e)
-        return
```

### Comparing `hydropandas-0.7.3/tests/test_004_gwobs.py` & `hydropandas-0.8.0/tests/test_004_gwobs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import numpy as np
 import test_001_to_from as ttf
 
 
 def test_set_tube_nr():
     dino_gw = ttf.test_obscollection_dinozip_gw()
     dino_gw.gwobs.set_tube_nr(if_exists="replace")
-    return
 
 
 def test_set_tube_nr_monitoring_well():
     fews_gw_prod = ttf.test_obscollection_fews_lowmemory()
     fews_gw_prod.gwobs.set_tube_nr_monitoring_well(
         "monitoring_well", if_exists="replace"
     )
-    return
 
 
 def test_get_modellayers_mf2005():
     import flopy
 
     modelname = "test_mf2005"
     ml = flopy.modflow.Modflow(modelname, exe_name="mf2005")
@@ -45,29 +43,25 @@
         xul=0,
         yul=700000,
     )
 
     dino_gw = ttf.test_obscollection_dinozip_gw()
     dino_gw.gwobs.get_modellayers(ml)
 
-    return
-
 
 def test_get_modellayers_mf6_structured():
     import flopy
 
     # Create the Flopy simulation object
     model_name = "test_mf6_structured"
-    sim = flopy.mf6.MFSimulation(
-        sim_name=model_name, exe_name="mf6", version="mf6")
+    sim = flopy.mf6.MFSimulation(sim_name=model_name, exe_name="mf6", version="mf6")
 
     # Create the Flopy groundwater flow (gwf) model object
     model_nam_file = "{}.nam".format(model_name)
-    gwf = flopy.mf6.ModflowGwf(
-        sim, modelname=model_name, model_nam_file=model_nam_file)
+    gwf = flopy.mf6.ModflowGwf(sim, modelname=model_name, model_nam_file=model_nam_file)
     Lx = 300000.0
     Ly = 400000.0
     ztop = 50.0
     zbot = -150.0
     nlay = 4
     nrow = 40
     ncol = 30
@@ -84,20 +78,11 @@
         delc=Ly / nrow,
         top=ztop,
         botm=botm[1:],
     )
     dino_gw = ttf.test_obscollection_dinozip_gw()
     dino_gw.gwobs.get_modellayers(gwf)
 
-    return
-
 
 def test_get_regis_layer():
-    # TODO: E   OSError: [Errno -68] NetCDF: I/O failure:
-    # 'http://www.dinodata.nl:80/opendap/REGIS/REGIS.nc'
-
-    try:
-        dino_gw = ttf.test_obscollection_dinozip_gw()
-        dino_gw.gwobs.get_regis_layers()
-    except OSError:
-        pass
-    return
+    dino_gw = ttf.test_obscollection_dinozip_gw()
+    dino_gw.gwobs.get_regis_layers()
```

### Comparing `hydropandas-0.7.3/tests/test_005_dino.py` & `hydropandas-0.8.0/tests/test_005_dino.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_dino_csv():
     fname = "./tests/data/2019-Dino-test/Grondwaterstanden_Put/" "B33F0080001_1.csv"
     dino.read_dino_groundwater_csv(fname)
 
-    return
-
 
 def test_dino_csv_duplicate_index():
     # contains 1 duplicate index 2019-11-19
     fname = "./tests/data/2019-Dino-test/Grondwaterstanden_Put/" "B22D0155001_1.csv"
     measurements, meta = dino.read_dino_groundwater_csv(fname)
 
     # check if measurements contains duplicate indices
@@ -27,9 +25,7 @@
 
     measurements, meta = dino.read_dino_groundwater_csv(
         fname, remove_duplicates=True, keep_dup="last"
     )
 
     # check if measurements contains no duplicate indices
     assert ~measurements.index.duplicated().any()
-
-    return
```

### Comparing `hydropandas-0.7.3/tests/test_006_knmi.py` & `hydropandas-0.8.0/tests/test_006_knmi.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,231 +9,195 @@
 
 
 def test_read_knmi_file1():
     # De Bilt neerslagstation
     fname = "./tests/data/2023-KNMI-test/neerslaggeg_ESBEEK_831.txt"
     knmi.read_knmi_daily_rainfall_file(fname)
 
-    return
-
 
 def test_read_knmi_file2():
     # De Bilt neerslagstation
     fname = "./tests/data/2023-KNMI-test/neerslaggeg_VILSTEREN_342.txt"
     knmi.read_knmi_daily_rainfall_file(fname)
 
-    return
-
 
 def test_read_knmi_file3():
     # De Bilt neerslagstation
     fname = "./tests/data/2023-KNMI-test/precipitation_st_anthonis.txt"
     knmi.read_knmi_daily_rainfall_file(fname)
 
-    return
-
 
 def test_get_knmi_precip_neerslagstation():
     # De Bilt neerslagstation
     knmi.get_knmi_timeseries_stn(
         "550", "RD", start="2010-1-1", end="2010-1-10", settings=None
     )
-    return
 
 
 def test_read_knmi_meteostation_file():
     fname = "./tests/data/2023-KNMI-test/etmgeg_260.txt"
     knmi.read_knmi_daily_meteo_file(fname, "EV24")
 
-    return
-
 
 def test_get_knmi_precip_meteostation_fill_missing():
     # De Bilt meteostation
     knmi.get_knmi_timeseries_stn(
         260, "RH", start="2010-1-1", end="2010-1-10", settings=None
     )
-    return
 
 
 def test_get_knmi_precip_meteostation_hourly():
     # De Bilt meteostation uurlijks
     knmi.get_knmi_timeseries_stn(
         260,
         "RH",
         start="2010-1-1",
         end="2010-1-10",
         settings={"interval": "hourly", "fill_missing_obs": False},
     )
-    return
 
 
 def test_get_pressure_hourly():
     # De Bilt meteostation uurlijks
     knmi.get_knmi_timeseries_stn(
         310,
         "P",
         start="2010-1-1",
         end="2010-1-10",
         settings={"interval": "hourly", "fill_missing_obs": False},
     )
-    return
 
 
 def test_get_knmi_precip_neerslagstation_no_api():
     # De Bilt neerslagstation
     knmi.get_knmi_timeseries_stn(
         "550", "RD", start="2010-1-1", end="2010-1-10", settings={"use_api": False}
     )
-    return
 
 
 def test_get_knmi_precip_meteostation_no_api():
     # De Bilt neerslagstation
     knmi.get_knmi_timeseries_stn(
         260, "RH", start="2010-1-1", end="2010-1-10", settings={"use_api": False}
     )
-    return
 
 
 def test_get_knmi_precip_neerslagstation_fill_missing():
     settings = knmi._get_default_settings(None)
     knmi.download_knmi_data(
         "550", meteo_var="RD", start="1952", end=None, settings=settings
     )
-    return
 
 
 def test_download_rd_550_no_api():
     settings = knmi._get_default_settings(None)
     settings["use_api"] = False
     knmi.download_knmi_data(
         "550",
         stn_name="DE-BILT",
         meteo_var="RD",
         start="1952",
         end=None,
         settings=settings,
     )
-    return
 
 
 def test_download_rd_12():
     settings = knmi._get_default_settings(None)
     knmi.download_knmi_data(
         "12", meteo_var="RD", start="2010", end=None, settings=settings
     )
-    return
 
 
 def test_download_without_data():
     settings = knmi._get_default_settings(None)
     try:
         knmi.download_knmi_data(
             "324", meteo_var="RD", start="2018", end="2020", settings=settings
         )
     except ValueError:
         pass
 
-    return
-
 
 def test_download_without_data_no_error():
     settings = knmi._get_default_settings(settings={"raise_exceptions": False})
 
     knmi_df, variables, stations = knmi.download_knmi_data(
         "324", meteo_var="RD", start="2018", end="2020", settings=settings
     )
 
     assert (knmi_df.empty, variables == {}, stations.empty) == (True, True, True)
 
-    return
-
 
 def test_download_ev24_210():
     settings = knmi._get_default_settings(None)
 
     knmi.download_knmi_data(
         210, meteo_var="EV24", start="1952", end=None, settings=settings
     )
-    return
 
 
 def test_download_ev24_210_no_api():
     settings = knmi._get_default_settings({"use_api": False})
     knmi.download_knmi_data(
         210, meteo_var="EV24", start="1952", end=None, settings=settings
     )
-    return
 
 
 def test_get_knmi_daily_meteo_ev24_empty():
     start, end = knmi._start_end_to_datetime("1959", "1963")
     knmi.get_knmi_daily_meteo_api(knmi.URL_DAILY_METEO, 265, "EV24", start, end, False)
 
-    return
-
 
 def test_fill_missing_measurements_ev24_278():
     knmi.fill_missing_measurements(278, meteo_var="EV24", start="1959", end="1963")
-    return
 
 
 def test_fill_missing_measurements_rh_273():
     knmi.fill_missing_measurements(273, meteo_var="RH", start="1995", end="2000")
-    return
 
 
 def test_fill_missing_measurements_rh_278():
     settings = knmi._get_default_settings({"exclude_neerslag_stn": True})
     knmi.fill_missing_measurements(
         278, meteo_var="RH", start="1990", end=None, settings=settings
     )
-    return
 
 
 def test_obslist_from_grid():
     xy = [[x, y] for x in [104150.0, 104550.0] for y in [510150.0, 510550.0]]
 
     knmi.get_knmi_obslist(
         xy=xy,
         meteo_vars=["RH", "EV24"],
         starts=["2010", "2010"],
         ObsClasses=[hpd.PrecipitationObs, hpd.EvaporationObs],
     )
 
-    return
-
 
 def test_obslist_from_locations():
     locations = pd.DataFrame(data={"x": [100000], "y": [350000]})
     knmi.get_knmi_obslist(
         locations, meteo_vars=["EV24"], ObsClasses=[hpd.EvaporationObs]
     )
 
-    return
-
 
 def test_obslist_from_stns():
     stns = [344, 260]  # Rotterdam en de Bilt
     knmi.get_knmi_obslist(
         stns=stns,
         meteo_vars=["RH", "EV24"],
         starts=["2010", "2010"],
         ends=["2015", "2015"],
         ObsClasses=[hpd.PrecipitationObs, hpd.EvaporationObs],
     )
 
-    return
-
 
 def test_obslist_from_stns_single_startdate():
     stns = [344, 260]  # Rotterdam en de Bilt
     knmi.get_knmi_obslist(
         stns=stns,
         meteo_vars=["RH", "EV24"],
         starts="2010",
         ends="2015",
         ObsClasses=[hpd.PrecipitationObs, hpd.EvaporationObs],
     )
-
-    return
```

### Comparing `hydropandas-0.7.3/tests/test_007_wiski.py` & `hydropandas-0.8.0/tests/test_007_wiski.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,66 @@
-# -*- coding: utf-8 -*-
-"""Created on Mon Jun 24 11:43:27 2019.
-
-@author: oebbe
-"""
+from pathlib import Path
 
 import hydropandas as hpd
 from hydropandas.io import wiski
 
+wiski_data_path = Path(__file__).parent / "data/2019-WISKI-test"
+
 
-def test_read_wiski_csv():
+def test_read_wiski_csv() -> None:
     # download single file
 
     wiski.read_wiski_file(
-        "./tests/data/2019-WISKI-test/1016_PBF.csv",
+        wiski_data_path / "1016_PBF.csv",
         sep=r"\s+",
         header_sep=":",
         header_identifier=":",
         verbose=True,
         parse_dates={"datetime": [0, 1]},
         infer_datetime_format=True,
         index_col=["datetime"],
         translate_dic={"name": "Station Number", "x": "GlobalX", "y": "GlobalY"},
     )
 
-    return
-
 
-def test_read_wiski_csv2():
+def test_read_wiski_csv2() -> None:
     # download single file
 
     wiski.read_wiski_file(
-        "./tests/data/2019-WISKI-test/8137_PBF.csv",
+        wiski_data_path / "8137_PBF.csv",
         sep=r"\s+",
         header_sep=":",
         header_identifier=":",
         verbose=True,
         parse_dates={"datetime": [0, 1]},
         infer_datetime_format=False,
         dayfirst=True,
         index_col=["datetime"],
         translate_dic={"name": "Station Number", "x": "GlobalX", "y": "GlobalY"},
     )
 
-    return
 
-
-def test_read_wiski_zip():
+def test_read_wiski_zip() -> None:
     wiski.read_wiski_dir(
-        "./tests/data/2019-WISKI-test/1016_PBF.zip",
+        str(wiski_data_path / "1016_PBF.zip"),
         ObsClass=hpd.GroundwaterObs,
         sep=r"\s+",
         header_sep=":",
         header_identifier=":",
         parse_dates={"datetime": [0, 1]},
         index_col=["datetime"],
         translate_dic={"name": "Station Number", "x": "GlobalX", "y": "GlobalY"},
         verbose=True,
+        dayfirst=True,
     )
 
-    return
-
 
-def test_rijnenijssel_wiski_format():
+def test_rijnenijssel_wiski_format() -> None:
     hpd.GroundwaterObs.from_wiski(
-        (
-            "./tests/data/2019-WISKI-test/"
-            "Zwiepse Horstweg Barchem_1024_FT1_WNS9040_MomentaanO.csv"
-        ),
+        wiski_data_path / "Zwiepse Horstweg Barchem_1024_FT1_WNS9040_MomentaanO.csv",
         header_sep=";",
         end_header_str="#Timestamp",
         parse_dates=[0],
         index_col=[0],
         infer_datetime_format=True,
         tz_localize=False,
     )
-    return
```

### Comparing `hydropandas-0.7.3/tests/test_008_visualisation.py` & `hydropandas-0.8.0/tests/test_008_visualisation.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,60 +13,55 @@
     gw = ttf.test_observation_gw()
     gw.plots.interactive_plot(
         savedir=plot_dir,
         cols=("stand_m_tov_nap",),
         hoover_date_format="{%F}",
         add_screen_to_legend=True,
     )
-    return
 
 
 def test_obscollection_dino_to_imap():
     dino_gw = ttf.test_obscollection_dinozip_gw()
     dino_gw.geo.set_lat_lon()
     dino_gw.plots.interactive_map(
         plot_dir,
         cols=("stand_m_tov_nap",),
         fname="imap.html",
         legend_name="grondwater DINO",
         add_screen_to_legend=True,
         hoover_names=("gws",),
         zoom_start=9,
     )
-    return
 
 
 def test_obscollection_dino_to_mapgraph():
     try:
         from art_tools import hpd_extension  # noqa: F401
 
         gw = ttf.test_obscollection_dinozip_gw()
         gw.art.plot_mapgraphs(plot_ylim="min_dy")
         return
     except ModuleNotFoundError as e:
         print(e)
-        return
 
 
 def test_obscollection_dino_to_section_plot():
     dino_gw = ttf.test_obscollection_dinozip_gw()
     dino_gw.plots.section_plot()
-    return
 
 
 def test_obscollection_to_map():
     try:
         from art_tools import hpd_extension  # noqa: F401
 
         fews_gw_prod = ttf.test_obscollection_fews_lowmemory()
         fews_gw_prod.art.plot_mapfig()
         return
     except ModuleNotFoundError as e:
         print(e)
-        return
 
 
 def test_obscollection_to_imap():
     fname = "texel_fews.html"
     fews_gw_prod = ttf.test_obscollection_fews_lowmemory()
     # add metadata to obscollection DF
     fews_gw_prod.add_meta_to_df("lat")
@@ -84,8 +79,7 @@
         plot_columns=("value",),
         fname=fname,
         plot_freq="D",
         legend_name="opp water FEWS",
         map_label="locationId",
         map_label_size=10,
     )
-    return
```

### Comparing `hydropandas-0.7.3/tests/test_011_bro.py` & `hydropandas-0.8.0/tests/test_011_bro.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,68 +7,54 @@
 
 
 def test_metadata():
     # single observation
     bro_id = "GMW000000036287"
     bro.get_metadata_from_gmw(bro_id, 1)
 
-    return
-
 
 def test_metadata_full():
     # single observation
     bro_id = "GMW000000036287"
     bro.get_full_metadata_from_gmw(bro_id, 1)
 
-    return
-
 
 def test_groundwater_monitoring_net_metadata():
     bro_id = "GMN000000000163"
     bro.get_obs_list_from_gmn(bro_id, hpd.GroundwaterObs, only_metadata=True)
 
-    return
-
 
 def test_groundwater_observations():
     bro_id = "GLD000000012893"
     bro.get_bro_groundwater(bro_id, tube_nr=None, only_metadata=False)
-    return
 
 
 def test_gld_no_monitoringnet():
     bro_id = "GLD000000013128"
     bro.get_bro_groundwater(bro_id, tube_nr=None, only_metadata=False)
-    return
 
 
 def test_groundwater_observations2():
     bro_id = "GLD000000008061"
     measurements, _ = bro.get_bro_groundwater(bro_id, tube_nr=None, only_metadata=False)
 
     measurements["values"].plot(color="blue", marker=".")
     measurements.loc[measurements["qualifier"] == "goedgekeurd", "values"].plot(
         color="green", marker="."
     )
 
-    return
-
 
 def test_get_gld_ids_from_gmw():
     bro_id = "GMW000000036287"
     bro_id = "GMW000000055372"
     bro_id = "GMW000000059186"
     bro_id = "GMW000000063853"  # two gld ids
     bro_id = "GMW000000030953"  # three gld ids
     bro.get_gld_ids_from_gmw(bro_id, tube_nr=1)
 
-    return
-
 
 def test_obs_list_from_extent():
     extent = (102395, 103121, 434331, 434750)
     extent = [116500, 120000, 439000, 442000]
     bro.get_obs_list_from_extent(
         extent, hpd.GroundwaterObs, tmin=None, tmax=None, epsg=28992, only_metadata=True
     )
-
-    return
```

