# Comparing `tmp/psrqpy-1.2.6.tar.gz` & `tmp/psrqpy-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/psrqpy/psrqpy/dist/.tmp-a_9xzl3o/psrqpy-1.2.6.tar", last modified: Mon Apr 24 16:27:02 2023, max compression
+gzip compressed data, was "/home/runner/work/psrqpy/psrqpy/dist/.tmp-_enqseps/psrqpy-1.2.7.tar", last modified: Fri May 19 08:28:46 2023, max compression
```

## Comparing `psrqpy-1.2.6.tar` & `psrqpy-1.2.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-24 16:26:51.000000 psrqpy-1.2.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-24 16:26:51.000000 psrqpy-1.2.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 16:26:51.000000 psrqpy-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-04-24 16:27:02.000000 psrqpy-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-24 16:26:51.000000 psrqpy-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   187239 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/images/PvsPdot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   141497 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/images/ppdot.png
--rw-r--r--   0 runner    (1001) docker     (123)    18282 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/pulsar.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/query.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/paper.tex
--rw-r--r--   0 runner    (1001) docker     (123)   141497 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/ppdot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/pulsar.py
--rw-r--r--   0 runner    (1001) docker     (123)   122264 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/derived_catalogue.db
--rw-r--r--   0 runner    (1001) docker     (123)    28442 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/query_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/test_catalogue.db
--rw-r--r--   0 runner    (1001) docker     (123)    76496 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 16:26:51.000000 psrqpy-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 16:26:51.000000 psrqpy-1.2.6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-24 16:27:02.000000 psrqpy-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 16:26:51.000000 psrqpy-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-19 08:28:33.000000 psrqpy-1.2.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-19 08:28:33.000000 psrqpy-1.2.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-19 08:28:33.000000 psrqpy-1.2.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 08:28:33.000000 psrqpy-1.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 08:28:33.000000 psrqpy-1.2.7/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 08:28:33.000000 psrqpy-1.2.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-19 08:28:33.000000 psrqpy-1.2.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-19 08:28:33.000000 psrqpy-1.2.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 08:28:33.000000 psrqpy-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-19 08:28:46.000000 psrqpy-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-19 08:28:33.000000 psrqpy-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   187239 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/images/PvsPdot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   141497 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/images/ppdot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18282 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/pulsar.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/query.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 08:28:33.000000 psrqpy-1.2.7/docs/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-19 08:28:33.000000 psrqpy-1.2.7/paper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-19 08:28:33.000000 psrqpy-1.2.7/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-19 08:28:33.000000 psrqpy-1.2.7/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-05-19 08:28:33.000000 psrqpy-1.2.7/paper/paper.tex
+-rw-r--r--   0 runner    (1001) docker     (123)   141497 2023-05-19 08:28:33.000000 psrqpy-1.2.7/paper/ppdot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122264 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/tests/derived_catalogue.db
+-rw-r--r--   0 runner    (1001) docker     (123)    28442 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/tests/query_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/tests/test_catalogue.db
+-rw-r--r--   0 runner    (1001) docker     (123)    76496 2023-05-19 08:28:33.000000 psrqpy-1.2.7/psrqpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 08:28:46.000000 psrqpy-1.2.7/psrqpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-19 08:28:33.000000 psrqpy-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 08:28:33.000000 psrqpy-1.2.7/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-19 08:28:46.000000 psrqpy-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-19 08:28:33.000000 psrqpy-1.2.7/setup.py
```

### Comparing `psrqpy-1.2.6/.github/workflows/build.yml` & `psrqpy-1.2.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/.github/workflows/pypi.yml` & `psrqpy-1.2.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/CHANGELOG.md` & `psrqpy-1.2.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Notable changes between versions
 
-## [1.2.6] 2023-04-24]
+## [1.2.7] 2023-05-19
+
+- Fix URL for the Globular Cluster pulsar catalogue, which recently moved to [here](https://www3.mpifr-bonn.mpg.de/staff/pfreire/GCpsr.txt). See [#123](https://github.com/mattpitkin/psrqpy/issues/123).
+
+## [1.2.6] 2023-04-24
 
 - Make the `NAME` attribute default to using the PSRB name if available to be consistent with `psrcat`. See [#122](https://github.com/mattpitkin/psrqpy/pull/122).
 - Fix parsing of the glitch catalogue table. See [#121](https://github.com/mattpitkin/psrqpy/pull/121).
 
 ## [1.2.5] 2023-01-16
 
 - Update `get_gc_catalogue` for parsing the [Globular Cluster pulsar catalogue](https://www.naic.edu/~pfreire/GCpsr.txt) to allow the "Offset" value to have an associated error value.
```

### Comparing `psrqpy-1.2.6/Dockerfile` & `psrqpy-1.2.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/LICENSE` & `psrqpy-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/PKG-INFO` & `psrqpy-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrqpy
-Version: 1.2.6
+Version: 1.2.7
 Summary: A Python module for querying the ATNF pulsar catalogue
 Home-page: https://github.com/mattpitkin/psrqpy
 Author: Matthew Pitkin
 Author-email: matthew.pitkin@ligo.org
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psrqpy-1.2.6/README.md` & `psrqpy-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/docs/Makefile` & `psrqpy-1.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/docs/source/CHANGELOG.md` & `psrqpy-1.2.7/docs/source/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Notable changes between versions
 
-## [1.2.6] 2023-04-24]
+## [1.2.7] 2023-05-19
+
+- Fix URL for the Globular Cluster pulsar catalogue, which recently moved to [here](https://www3.mpifr-bonn.mpg.de/staff/pfreire/GCpsr.txt). See [#123](https://github.com/mattpitkin/psrqpy/issues/123).
+
+## [1.2.6] 2023-04-24
 
 - Make the `NAME` attribute default to using the PSRB name if available to be consistent with `psrcat`. See [#122](https://github.com/mattpitkin/psrqpy/pull/122).
 - Fix parsing of the glitch catalogue table. See [#121](https://github.com/mattpitkin/psrqpy/pull/121).
 
 ## [1.2.5] 2023-01-16
 
 - Update `get_gc_catalogue` for parsing the [Globular Cluster pulsar catalogue](https://www.naic.edu/~pfreire/GCpsr.txt) to allow the "Offset" value to have an associated error value.
```

### Comparing `psrqpy-1.2.6/docs/source/conf.py` & `psrqpy-1.2.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/docs/source/images/PvsPdot.ipynb` & `psrqpy-1.2.7/docs/source/images/PvsPdot.ipynb`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/docs/source/images/ppdot.png` & `psrqpy-1.2.7/docs/source/images/ppdot.png`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/docs/source/index.rst` & `psrqpy-1.2.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/paper/Makefile` & `psrqpy-1.2.7/paper/Makefile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/paper/paper.bib` & `psrqpy-1.2.7/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/paper/paper.md` & `psrqpy-1.2.7/paper/paper.md`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/paper/paper.tex` & `psrqpy-1.2.7/paper/paper.tex`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/paper/ppdot.png` & `psrqpy-1.2.7/paper/ppdot.png`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/psrqpy/__init__.py` & `psrqpy-1.2.7/psrqpy/__init__.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/psrqpy/config.py` & `psrqpy-1.2.7/psrqpy/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # be added).
 ATNF_VERSION_TARBALL = ATNF_BASE_URL + r"downloads/psrcat_pkg.v{}.tar.gz"
 
 #: The Jodrell Bank glitch catalogue table URL.
 GLITCH_URL = r"https://www.jb.man.ac.uk/pulsar/glitches/gTable.html"
 
 #: Paolo Freire's globular cluster pulsar table URL
-GC_URL = r"https://www.naic.edu/~pfreire/GCpsr.txt"
+GC_URL = r"https://www3.mpifr-bonn.mpg.de/staff/pfreire/GCpsr.txt"
 
 #: Dunc Lorimer's MSP table URL
 MSP_URL = r"http://astro.phys.wvu.edu/GalacticMSPs/GalacticMSPs.txt"
 
 # Pulsar parameters (http://www.atnf.csiro.au/research/pulsar/psrcat/psrcat_help.html) that can be
 # queried. For each parameter there is a dictionary giving:
 #  - 'ref': True if the parameter can have an associated reference in the ATNF catalogue
```

### Comparing `psrqpy-1.2.6/psrqpy/pulsar.py` & `psrqpy-1.2.7/psrqpy/pulsar.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/psrqpy/search.py` & `psrqpy-1.2.7/psrqpy/search.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/psrqpy/tests/derived_catalogue.db` & `psrqpy-1.2.7/psrqpy/tests/derived_catalogue.db`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/psrqpy/tests/query_test.py` & `psrqpy-1.2.7/psrqpy/tests/query_test.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/psrqpy/tests/test_catalogue.db` & `psrqpy-1.2.7/psrqpy/tests/test_catalogue.db`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/psrqpy/utils.py` & `psrqpy-1.2.7/psrqpy/utils.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/psrqpy.egg-info/PKG-INFO` & `psrqpy-1.2.7/psrqpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrqpy
-Version: 1.2.6
+Version: 1.2.7
 Summary: A Python module for querying the ATNF pulsar catalogue
 Home-page: https://github.com/mattpitkin/psrqpy
 Author: Matthew Pitkin
 Author-email: matthew.pitkin@ligo.org
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psrqpy-1.2.6/psrqpy.egg-info/SOURCES.txt` & `psrqpy-1.2.7/psrqpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.6/setup.cfg` & `psrqpy-1.2.7/setup.cfg`

 * *Files identical despite different names*

