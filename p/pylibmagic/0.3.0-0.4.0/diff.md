# Comparing `tmp/pylibmagic-0.3.0.tar.gz` & `tmp/pylibmagic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibmagic-0.3.0.tar", last modified: Thu Apr  6 19:42:10 2023, max compression
+gzip compressed data, was "pylibmagic-0.4.0.tar", last modified: Fri May 19 01:15:29 2023, max compression
```

## Comparing `pylibmagic-0.3.0.tar` & `pylibmagic-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:42:10.627747 pylibmagic-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-06 19:42:10.627747 pylibmagic-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-06 19:42:10.631748 pylibmagic-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:42:10.627747 pylibmagic-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:42:10.627747 pylibmagic-0.3.0/src/pylibmagic/
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/src/pylibmagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 19:42:10.000000 pylibmagic-0.3.0/src/pylibmagic/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/src/pylibmagic/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/src/pylibmagic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:42:10.627747 pylibmagic-0.3.0/src/pylibmagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-06 19:42:10.000000 pylibmagic-0.3.0/src/pylibmagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-06 19:42:10.000000 pylibmagic-0.3.0/src/pylibmagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 19:42:10.000000 pylibmagic-0.3.0/src/pylibmagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-06 19:42:10.000000 pylibmagic-0.3.0/src/pylibmagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 19:42:10.000000 pylibmagic-0.3.0/src/pylibmagic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 19:42:10.627747 pylibmagic-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/tests/test_compiled.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-06 19:41:56.000000 pylibmagic-0.3.0/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:15:29.564531 pylibmagic-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-19 01:15:29.564531 pylibmagic-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-19 01:15:29.564531 pylibmagic-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:15:29.560531 pylibmagic-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:15:29.560531 pylibmagic-0.4.0/src/pylibmagic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/src/pylibmagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-19 01:15:29.000000 pylibmagic-0.4.0/src/pylibmagic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/src/pylibmagic/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/src/pylibmagic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:15:29.564531 pylibmagic-0.4.0/src/pylibmagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-19 01:15:29.000000 pylibmagic-0.4.0/src/pylibmagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-19 01:15:29.000000 pylibmagic-0.4.0/src/pylibmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 01:15:29.000000 pylibmagic-0.4.0/src/pylibmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-19 01:15:29.000000 pylibmagic-0.4.0/src/pylibmagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 01:15:29.000000 pylibmagic-0.4.0/src/pylibmagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:15:29.564531 pylibmagic-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/tests/test_compiled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 01:15:18.000000 pylibmagic-0.4.0/tests/test_package.py
```

### Comparing `pylibmagic-0.3.0/LICENSE` & `pylibmagic-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibmagic-0.3.0/PKG-INFO` & `pylibmagic-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibmagic
-Version: 0.3.0
+Version: 0.4.0
 Summary: scikit-build project with CMake for compiling libmagic
 Home-page: https://github.com/kratsg/pylibmagic
 Author: Giordon Stark
 Author-email: kratsg@gmail.com
 Maintainer: Giordon Stark
 Maintainer-email: kratsg@gmail.com
 License: BSD-3-Clause
@@ -29,21 +29,21 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
-pylibmagic v0.3.0
+pylibmagic v0.4.0
 =================
 
 A lightweight, minimal python package that ships ``magic`` libraries
 using automake, CMake, scikit-build, and cibuildwheel.
 
-|Actions Status| |Documentation Status| |Code style: black|
+|Actions Status| |Cirrus Status| |Documentation Status| |Code style: black|
 
 |PyPI version| |Conda-Forge| |PyPI platforms|
 
 |GitHub Discussion| |Gitter|
 
 Why?
 ----
@@ -96,14 +96,16 @@
 .. code:: bash
 
     $ python -c "import pylibmagic; print(pylibmagic.data)"
 
 
 .. |Actions Status| image:: https://github.com/kratsg/pylibmagic/workflows/CI/badge.svg
    :target: https://github.com/kratsg/pylibmagic/actions
+.. |Cirrus Status| image:: https://api.cirrus-ci.com/github/kratsg/pylibmagic.svg?branch=main
+   :target: https://cirrus-ci.com/github/kratsg/pylibmagic
 .. |Documentation Status| image:: https://readthedocs.org/projects/pylibmagic/badge/?version=latest
    :target: https://pylibmagic.readthedocs.io/en/latest/?badge=latest
 .. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 .. |PyPI version| image:: https://badge.fury.io/py/pylibmagic.svg
    :target: https://pypi.org/project/pylibmagic/
 .. |Conda-Forge| image:: https://img.shields.io/conda/vn/conda-forge/pylibmagic
```

### Comparing `pylibmagic-0.3.0/README.rst` & `pylibmagic-0.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-pylibmagic v0.3.0
+pylibmagic v0.4.0
 =================
 
 A lightweight, minimal python package that ships ``magic`` libraries
 using automake, CMake, scikit-build, and cibuildwheel.
 
-|Actions Status| |Documentation Status| |Code style: black|
+|Actions Status| |Cirrus Status| |Documentation Status| |Code style: black|
 
 |PyPI version| |Conda-Forge| |PyPI platforms|
 
 |GitHub Discussion| |Gitter|
 
 Why?
 ----
@@ -61,14 +61,16 @@
 .. code:: bash
 
     $ python -c "import pylibmagic; print(pylibmagic.data)"
 
 
 .. |Actions Status| image:: https://github.com/kratsg/pylibmagic/workflows/CI/badge.svg
    :target: https://github.com/kratsg/pylibmagic/actions
+.. |Cirrus Status| image:: https://api.cirrus-ci.com/github/kratsg/pylibmagic.svg?branch=main
+   :target: https://cirrus-ci.com/github/kratsg/pylibmagic
 .. |Documentation Status| image:: https://readthedocs.org/projects/pylibmagic/badge/?version=latest
    :target: https://pylibmagic.readthedocs.io/en/latest/?badge=latest
 .. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 .. |PyPI version| image:: https://badge.fury.io/py/pylibmagic.svg
    :target: https://pypi.org/project/pylibmagic/
 .. |Conda-Forge| image:: https://img.shields.io/conda/vn/conda-forge/pylibmagic
```

### Comparing `pylibmagic-0.3.0/pyproject.toml` & `pylibmagic-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylibmagic-0.3.0/setup.cfg` & `pylibmagic-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibmagic-0.3.0/src/pylibmagic/__init__.py` & `pylibmagic-0.4.0/src/pylibmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `pylibmagic-0.3.0/src/pylibmagic.egg-info/PKG-INFO` & `pylibmagic-0.4.0/src/pylibmagic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibmagic
-Version: 0.3.0
+Version: 0.4.0
 Summary: scikit-build project with CMake for compiling libmagic
 Home-page: https://github.com/kratsg/pylibmagic
 Author: Giordon Stark
 Author-email: kratsg@gmail.com
 Maintainer: Giordon Stark
 Maintainer-email: kratsg@gmail.com
 License: BSD-3-Clause
@@ -29,21 +29,21 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
-pylibmagic v0.3.0
+pylibmagic v0.4.0
 =================
 
 A lightweight, minimal python package that ships ``magic`` libraries
 using automake, CMake, scikit-build, and cibuildwheel.
 
-|Actions Status| |Documentation Status| |Code style: black|
+|Actions Status| |Cirrus Status| |Documentation Status| |Code style: black|
 
 |PyPI version| |Conda-Forge| |PyPI platforms|
 
 |GitHub Discussion| |Gitter|
 
 Why?
 ----
@@ -96,14 +96,16 @@
 .. code:: bash
 
     $ python -c "import pylibmagic; print(pylibmagic.data)"
 
 
 .. |Actions Status| image:: https://github.com/kratsg/pylibmagic/workflows/CI/badge.svg
    :target: https://github.com/kratsg/pylibmagic/actions
+.. |Cirrus Status| image:: https://api.cirrus-ci.com/github/kratsg/pylibmagic.svg?branch=main
+   :target: https://cirrus-ci.com/github/kratsg/pylibmagic
 .. |Documentation Status| image:: https://readthedocs.org/projects/pylibmagic/badge/?version=latest
    :target: https://pylibmagic.readthedocs.io/en/latest/?badge=latest
 .. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 .. |PyPI version| image:: https://badge.fury.io/py/pylibmagic.svg
    :target: https://pypi.org/project/pylibmagic/
 .. |Conda-Forge| image:: https://img.shields.io/conda/vn/conda-forge/pylibmagic
```

### Comparing `pylibmagic-0.3.0/tests/test_compiled.py` & `pylibmagic-0.4.0/tests/test_compiled.py`

 * *Files identical despite different names*

