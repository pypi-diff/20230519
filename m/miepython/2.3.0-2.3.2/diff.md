# Comparing `tmp/miepython-2.3.0.tar.gz` & `tmp/miepython-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miepython-2.3.0.tar", last modified: Wed Jul 27 19:39:45 2022, max compression
+gzip compressed data, was "miepython-2.3.2.tar", last modified: Thu May 18 22:25:29 2023, max compression
```

## Comparing `miepython-2.3.0.tar` & `miepython-2.3.2.tar`

### file list

```diff
@@ -1,31 +1,61 @@
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2022-07-27 19:39:45.235571 miepython-2.3.0/
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2022-07-27 19:39:45.166217 miepython-2.3.0/.github/
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2022-07-27 19:39:45.173688 miepython-2.3.0/.github/workflows/
--rw-r--r--   0 prahl      (502) staff       (20)      713 2022-01-26 22:36:27.000000 miepython-2.3.0/.github/workflows/test.yml
--rw-r--r--   0 prahl      (502) staff       (20)     5297 2022-07-27 19:36:37.000000 miepython-2.3.0/CHANGELOG.rst
--rw-r--r--   0 prahl      (502) staff       (20)     1055 2021-11-17 18:49:05.000000 miepython-2.3.0/LICENSE.txt
--rw-r--r--   0 prahl      (502) staff       (20)      310 2022-01-26 23:01:59.000000 miepython-2.3.0/MANIFEST.in
--rw-r--r--   0 prahl      (502) staff       (20)     4265 2022-07-27 19:39:45.235808 miepython-2.3.0/PKG-INFO
--rw-r--r--   0 prahl      (502) staff       (20)     3485 2022-07-27 18:49:31.000000 miepython-2.3.0/README.rst
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2022-07-27 19:39:45.174983 miepython-2.3.0/miepython/
--rw-r--r--   0 prahl      (502) staff       (20)     1432 2022-07-27 18:52:41.000000 miepython-2.3.0/miepython/__init__.py
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2022-07-27 19:39:45.232510 miepython-2.3.0/miepython/data/
--rw-r--r--   0 prahl      (502) staff       (20)     1337 2022-01-26 18:53:40.000000 miepython-2.3.0/miepython/data/Johnson.txt
--rw-r--r--   0 prahl      (502) staff       (20)     1337 2022-01-26 20:40:40.000000 miepython-2.3.0/miepython/data/ag-Johnson.txt
--rw-r--r--   0 prahl      (502) staff       (20)    36719 2017-08-05 17:05:42.000000 miepython-2.3.0/miepython/data/segelstein81_index.txt
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2022-07-27 19:39:45.234996 miepython-2.3.0/miepython/examples/
--rwxr-xr-x   0 prahl      (502) staff       (20)      684 2021-11-17 18:49:06.000000 miepython-2.3.0/miepython/examples/01_dielectric.py
--rwxr-xr-x   0 prahl      (502) staff       (20)      804 2021-11-17 18:49:06.000000 miepython-2.3.0/miepython/examples/02_glass.py
--rwxr-xr-x   0 prahl      (502) staff       (20)      921 2021-11-17 18:49:06.000000 miepython-2.3.0/miepython/examples/03_droplets.py
--rwxr-xr-x   0 prahl      (502) staff       (20)     2717 2022-07-05 18:09:58.000000 miepython-2.3.0/miepython/examples/04_gold.py
--rw-r--r--   0 prahl      (502) staff       (20)    26737 2022-07-26 20:03:48.000000 miepython-2.3.0/miepython/miepython.py
--rw-r--r--   0 prahl      (502) staff       (20)    24387 2022-07-05 18:09:58.000000 miepython-2.3.0/miepython/miepython_nojit.py
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2022-07-27 19:39:45.231377 miepython-2.3.0/miepython.egg-info/
--rw-r--r--   0 prahl      (502) staff       (20)     4265 2022-07-27 19:39:45.000000 miepython-2.3.0/miepython.egg-info/PKG-INFO
--rw-r--r--   0 prahl      (502) staff       (20)      573 2022-07-27 19:39:45.000000 miepython-2.3.0/miepython.egg-info/SOURCES.txt
--rw-r--r--   0 prahl      (502) staff       (20)        1 2022-07-27 19:39:45.000000 miepython-2.3.0/miepython.egg-info/dependency_links.txt
--rw-r--r--   0 prahl      (502) staff       (20)       23 2022-07-27 19:39:45.000000 miepython-2.3.0/miepython.egg-info/requires.txt
--rw-r--r--   0 prahl      (502) staff       (20)       10 2022-07-27 19:39:45.000000 miepython-2.3.0/miepython.egg-info/top_level.txt
--rw-r--r--   0 prahl      (502) staff       (20)      569 2022-07-05 18:09:58.000000 miepython-2.3.0/pyproject.toml
--rw-r--r--   0 prahl      (502) staff       (20)      986 2022-07-27 19:39:45.236661 miepython-2.3.0/setup.cfg
--rw-r--r--   0 prahl      (502) staff       (20)     1095 2022-07-05 18:09:58.000000 miepython-2.3.0/setup.py
+drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.628378 miepython-2.3.2/
+drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.397087 miepython-2.3.2/.github/
+drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.404818 miepython-2.3.2/.github/workflows/
+-rw-r--r--   0 prahl      (502) staff       (20)      713 2022-01-26 22:36:27.000000 miepython-2.3.2/.github/workflows/test.yml
+-rw-r--r--   0 prahl      (502) staff       (20)      164 2022-01-26 22:27:48.000000 miepython-2.3.2/.gitignore
+-rw-r--r--   0 prahl      (502) staff       (20)      398 2021-11-17 18:49:05.000000 miepython-2.3.2/.readthedocs.yaml
+-rw-r--r--   0 prahl      (502) staff       (20)       48 2022-01-25 19:27:23.000000 miepython-2.3.2/.testignore
+-rw-r--r--   0 prahl      (502) staff       (20)     5500 2023-05-18 22:21:25.000000 miepython-2.3.2/CHANGELOG.rst
+-rw-r--r--   0 prahl      (502) staff       (20)     1098 2023-05-18 22:23:49.000000 miepython-2.3.2/CITATION.cff
+-rw-r--r--   0 prahl      (502) staff       (20)     1055 2021-11-17 18:49:05.000000 miepython-2.3.2/LICENSE.txt
+-rw-r--r--   0 prahl      (502) staff       (20)      161 2023-05-18 22:09:45.000000 miepython-2.3.2/MANIFEST.in
+-rw-r--r--   0 prahl      (502) staff       (20)     1797 2022-07-05 18:09:58.000000 miepython-2.3.2/Makefile
+-rw-r--r--   0 prahl      (502) staff       (20)     4364 2023-05-18 22:25:29.628605 miepython-2.3.2/PKG-INFO
+-rw-r--r--   0 prahl      (502) staff       (20)     3584 2023-05-18 22:03:55.000000 miepython-2.3.2/README.rst
+drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.555198 miepython-2.3.2/docs/
+-rw-r--r--   0 prahl      (502) staff       (20)   190191 2022-07-27 18:07:30.000000 miepython-2.3.2/docs/01_basics.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)    34904 2021-11-17 18:49:05.000000 miepython-2.3.2/docs/01_plot.png
+-rw-r--r--   0 prahl      (502) staff       (20)   123686 2022-08-03 16:28:32.000000 miepython-2.3.2/docs/02_efficiencies.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)    47794 2021-11-17 18:49:05.000000 miepython-2.3.2/docs/02_plot.png
+-rw-r--r--   0 prahl      (502) staff       (20)   478393 2022-01-31 19:21:59.000000 miepython-2.3.2/docs/03_angular_scattering.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)    34095 2021-11-17 18:49:05.000000 miepython-2.3.2/docs/03_plot.png
+-rw-r--r--   0 prahl      (502) staff       (20)   165954 2022-07-27 19:14:22.000000 miepython-2.3.2/docs/03a_normalization.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)    54959 2022-07-05 18:09:58.000000 miepython-2.3.2/docs/04_plot.png
+-rw-r--r--   0 prahl      (502) staff       (20)   133775 2021-11-17 18:49:05.000000 miepython-2.3.2/docs/04_rayleigh.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)   264354 2022-01-26 21:48:56.000000 miepython-2.3.2/docs/05_fog.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)    88000 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/06_random_deviates.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)    43928 2022-01-25 19:22:34.000000 miepython-2.3.2/docs/07_algorithm.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)   565045 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/08_large_spheres.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)    33297 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/09_backscattering.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)    21271 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/10_basic_tests.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)   111396 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/11_performance.ipynb
+-rw-r--r--   0 prahl      (502) staff       (20)       29 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/changelog.rst
+-rw-r--r--   0 prahl      (502) staff       (20)     1953 2022-07-05 18:09:58.000000 miepython-2.3.2/docs/conf.py
+-rw-r--r--   0 prahl      (502) staff       (20)     3407 2022-07-27 18:48:20.000000 miepython-2.3.2/docs/index.rst
+-rw-r--r--   0 prahl      (502) staff       (20)      136 2022-01-28 00:11:47.000000 miepython-2.3.2/docs/miepython.rst
+-rw-r--r--   0 prahl      (502) staff       (20)       76 2022-07-05 18:09:58.000000 miepython-2.3.2/docs/requirements.txt
+drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.557592 miepython-2.3.2/miepython/
+-rw-r--r--   0 prahl      (502) staff       (20)     1432 2023-05-18 22:21:35.000000 miepython-2.3.2/miepython/__init__.py
+drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.607507 miepython-2.3.2/miepython/data/
+-rw-r--r--   0 prahl      (502) staff       (20)     1337 2022-01-26 18:53:40.000000 miepython-2.3.2/miepython/data/Johnson.txt
+-rw-r--r--   0 prahl      (502) staff       (20)     1337 2022-01-26 20:40:40.000000 miepython-2.3.2/miepython/data/ag-Johnson.txt
+-rw-r--r--   0 prahl      (502) staff       (20)    36719 2017-08-05 17:05:42.000000 miepython-2.3.2/miepython/data/segelstein81_index.txt
+drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.627297 miepython-2.3.2/miepython/examples/
+-rwxr-xr-x   0 prahl      (502) staff       (20)      684 2021-11-17 18:49:06.000000 miepython-2.3.2/miepython/examples/01_dielectric.py
+-rwxr-xr-x   0 prahl      (502) staff       (20)      804 2021-11-17 18:49:06.000000 miepython-2.3.2/miepython/examples/02_glass.py
+-rwxr-xr-x   0 prahl      (502) staff       (20)      921 2021-11-17 18:49:06.000000 miepython-2.3.2/miepython/examples/03_droplets.py
+-rwxr-xr-x   0 prahl      (502) staff       (20)     2717 2022-07-05 18:09:58.000000 miepython-2.3.2/miepython/examples/04_gold.py
+-rw-r--r--   0 prahl      (502) staff       (20)    26737 2022-07-26 20:03:48.000000 miepython-2.3.2/miepython/miepython.py
+-rw-r--r--   0 prahl      (502) staff       (20)    24387 2022-07-05 18:09:58.000000 miepython-2.3.2/miepython/miepython_nojit.py
+drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.560825 miepython-2.3.2/miepython.egg-info/
+-rw-r--r--   0 prahl      (502) staff       (20)     4364 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/PKG-INFO
+-rw-r--r--   0 prahl      (502) staff       (20)     1156 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/SOURCES.txt
+-rw-r--r--   0 prahl      (502) staff       (20)        1 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/dependency_links.txt
+-rw-r--r--   0 prahl      (502) staff       (20)       23 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/requires.txt
+-rw-r--r--   0 prahl      (502) staff       (20)       10 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/top_level.txt
+-rw-r--r--   0 prahl      (502) staff       (20)      569 2022-07-05 18:09:58.000000 miepython-2.3.2/pyproject.toml
+-rw-r--r--   0 prahl      (502) staff       (20)      602 2022-03-11 18:19:27.000000 miepython-2.3.2/release.txt
+-rw-r--r--   0 prahl      (502) staff       (20)      182 2022-01-26 22:23:15.000000 miepython-2.3.2/requirements-dev.txt
+-rw-r--r--   0 prahl      (502) staff       (20)       22 2022-01-26 22:23:09.000000 miepython-2.3.2/requirements.txt
+-rw-r--r--   0 prahl      (502) staff       (20)      986 2023-05-18 22:25:29.629541 miepython-2.3.2/setup.cfg
+-rw-r--r--   0 prahl      (502) staff       (20)     1095 2022-07-05 18:09:58.000000 miepython-2.3.2/setup.py
```

### Comparing `miepython-2.3.0/.github/workflows/test.yml` & `miepython-2.3.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/CHANGELOG.rst` & `miepython-2.3.2/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+v2.3.2
+-------------------
+*   fix typo in README.rst that prevented pypi upload
+*   add CITATION.cff to base level of miepython repository
+
+v2.3.1
+-------------------
+*   add DOI for citation purposes
+
 v2.3.0
 -------------------
 *   add optional argument to change scattering function normalization
 *   document normalization in new notebook
 *   store data in correct place
 *   store version __init__.py so scripts can query it
 *   fix typo in header of gold sphere example script
```

### Comparing `miepython-2.3.0/LICENSE.txt` & `miepython-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/PKG-INFO` & `miepython-2.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miepython
-Version: 2.3.0
+Version: 2.3.2
 Summary: Mie scattering of a plane wave by a sphere
 Home-page: https://github.com/scottprahl/miepython.git
 Author: Scott Prahl
 Author-email: scott.prahl@oit.edu
 License: MIT
 Keywords: mie,scattering,rainbow,droplet,backscatter,sphere,nanoparticle,sphere,cloud,phase function,efficiency,rayleigh,backscattering
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,14 +36,17 @@
 
 .. image:: https://img.shields.io/badge/MIT-license-yellow.svg
    :target: https://github.com/scottprahl/miepython/blob/master/LICENSE.txt
 
 .. image:: https://github.com/scottprahl/miepython/actions/workflows/test.yml/badge.svg
    :target: https://github.com/scottprahl/miepython/actions/workflows/test.yml
 
+.. image:: https://zenodo.org/badge/99259684.svg
+   :target: https://zenodo.org/badge/latestdoi/99259684
+
 __________
 
 ``miepython`` is a pure Python module to calculate light scattering for
 non-absorbing, partially-absorbing, or perfectly-conducting spheres. Mie
 theory is used, following `the procedure described by Wiscombe
 <http://opensky.ucar.edu/islandora/object/technotes:232>`_. This code has
 been validated against his results. 
@@ -64,15 +67,15 @@
 
 
 Using miepython
 ---------------
 
 1. You can install locally using pip::
     
-    pip install --user miepython
+    pip install miepython
 
 2. or `run this code in the cloud using Google Collaboratory <https://colab.research.google.com/github/scottprahl/miepython/blob/master>`_ by selecting the Jupyter notebook that interests you.
 
 An example
 ----------
 
 The following code::
```

### Comparing `miepython-2.3.0/README.rst` & `miepython-2.3.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 .. image:: https://img.shields.io/badge/MIT-license-yellow.svg
    :target: https://github.com/scottprahl/miepython/blob/master/LICENSE.txt
 
 .. image:: https://github.com/scottprahl/miepython/actions/workflows/test.yml/badge.svg
    :target: https://github.com/scottprahl/miepython/actions/workflows/test.yml
 
+.. image:: https://zenodo.org/badge/99259684.svg
+   :target: https://zenodo.org/badge/latestdoi/99259684
+
 __________
 
 ``miepython`` is a pure Python module to calculate light scattering for
 non-absorbing, partially-absorbing, or perfectly-conducting spheres. Mie
 theory is used, following `the procedure described by Wiscombe
 <http://opensky.ucar.edu/islandora/object/technotes:232>`_. This code has
 been validated against his results. 
@@ -45,15 +48,15 @@
 
 
 Using miepython
 ---------------
 
 1. You can install locally using pip::
     
-    pip install --user miepython
+    pip install miepython
 
 2. or `run this code in the cloud using Google Collaboratory <https://colab.research.google.com/github/scottprahl/miepython/blob/master>`_ by selecting the Jupyter notebook that interests you.
 
 An example
 ----------
 
 The following code::
```

### Comparing `miepython-2.3.0/miepython/__init__.py` & `miepython-2.3.2/miepython/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 Mie scattering intensities normalized to one when integrated over all angles::
 
     miepython.i_per(m, x, mu, norm='one')
     miepython.i_par(m, x, mu, norm='one')
     miepython.i_unpolarized(m, x, mu, norm='one')
 """
-__version__ = '2.3.0'
+__version__ = '2.3.2'
 __author__ = 'Scott Prahl'
 __email__ = 'scott.prahl@oit.edu'
-__copyright__ = 'Copyright 2017-22, Scott Prahl'
+__copyright__ = 'Copyright 2017-23, Scott Prahl'
 __license__ = 'MIT'
 __url__ = 'https://github.com/scottprahl/miepython.git'
 
 from .miepython import *
```

### Comparing `miepython-2.3.0/miepython/data/Johnson.txt` & `miepython-2.3.2/miepython/data/Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython/data/ag-Johnson.txt` & `miepython-2.3.2/miepython/data/ag-Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython/data/segelstein81_index.txt` & `miepython-2.3.2/miepython/data/segelstein81_index.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython/examples/01_dielectric.py` & `miepython-2.3.2/miepython/examples/01_dielectric.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython/examples/02_glass.py` & `miepython-2.3.2/miepython/examples/02_glass.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython/examples/03_droplets.py` & `miepython-2.3.2/miepython/examples/03_droplets.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython/examples/04_gold.py` & `miepython-2.3.2/miepython/examples/04_gold.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython/miepython.py` & `miepython-2.3.2/miepython/miepython.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython/miepython_nojit.py` & `miepython-2.3.2/miepython/miepython_nojit.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/miepython.egg-info/PKG-INFO` & `miepython-2.3.2/miepython.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miepython
-Version: 2.3.0
+Version: 2.3.2
 Summary: Mie scattering of a plane wave by a sphere
 Home-page: https://github.com/scottprahl/miepython.git
 Author: Scott Prahl
 Author-email: scott.prahl@oit.edu
 License: MIT
 Keywords: mie,scattering,rainbow,droplet,backscatter,sphere,nanoparticle,sphere,cloud,phase function,efficiency,rayleigh,backscattering
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,14 +36,17 @@
 
 .. image:: https://img.shields.io/badge/MIT-license-yellow.svg
    :target: https://github.com/scottprahl/miepython/blob/master/LICENSE.txt
 
 .. image:: https://github.com/scottprahl/miepython/actions/workflows/test.yml/badge.svg
    :target: https://github.com/scottprahl/miepython/actions/workflows/test.yml
 
+.. image:: https://zenodo.org/badge/99259684.svg
+   :target: https://zenodo.org/badge/latestdoi/99259684
+
 __________
 
 ``miepython`` is a pure Python module to calculate light scattering for
 non-absorbing, partially-absorbing, or perfectly-conducting spheres. Mie
 theory is used, following `the procedure described by Wiscombe
 <http://opensky.ucar.edu/islandora/object/technotes:232>`_. This code has
 been validated against his results. 
@@ -64,15 +67,15 @@
 
 
 Using miepython
 ---------------
 
 1. You can install locally using pip::
     
-    pip install --user miepython
+    pip install miepython
 
 2. or `run this code in the cloud using Google Collaboratory <https://colab.research.google.com/github/scottprahl/miepython/blob/master>`_ by selecting the Jupyter notebook that interests you.
 
 An example
 ----------
 
 The following code::
```

### Comparing `miepython-2.3.0/pyproject.toml` & `miepython-2.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/setup.cfg` & `miepython-2.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `miepython-2.3.0/setup.py` & `miepython-2.3.2/setup.py`

 * *Files identical despite different names*

