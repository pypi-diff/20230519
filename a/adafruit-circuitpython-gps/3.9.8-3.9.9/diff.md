# Comparing `tmp/adafruit-circuitpython-gps-3.9.8.tar.gz` & `tmp/adafruit-circuitpython-gps-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-gps-3.9.8.tar", last modified: Wed May 25 20:02:05 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-gps-3.9.9.tar", last modified: Tue Jun  7 16:51:22 2022, max compression
```

## Comparing `adafruit-circuitpython-gps-3.9.8.tar` & `adafruit-circuitpython-gps-3.9.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.517840 adafruit-circuitpython-gps-3.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.509840 adafruit-circuitpython-gps-3.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.513840 adafruit-circuitpython-gps-3.9.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.513840 adafruit-circuitpython-gps-3.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16274 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.513840 adafruit-circuitpython-gps-3.9.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-05-25 20:02:05.517840 adafruit-circuitpython-gps-3.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.513840 adafruit-circuitpython-gps-3.9.8/adafruit_circuitpython_gps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-05-25 20:02:05.000000 adafruit-circuitpython-gps-3.9.8/adafruit_circuitpython_gps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-05-25 20:02:05.000000 adafruit-circuitpython-gps-3.9.8/adafruit_circuitpython_gps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 20:02:05.000000 adafruit-circuitpython-gps-3.9.8/adafruit_circuitpython_gps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-25 20:02:05.000000 adafruit-circuitpython-gps-3.9.8/adafruit_circuitpython_gps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-25 20:02:05.000000 adafruit-circuitpython-gps-3.9.8/adafruit_circuitpython_gps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    22687 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/adafruit_gps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.517840 adafruit-circuitpython-gps-3.9.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.517840 adafruit-circuitpython-gps-3.9.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/details.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/details.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.517840 adafruit-circuitpython-gps-3.9.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/examples/gps_datalogging.py
--rw-r--r--   0 runner    (1001) docker     (121)     2807 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/examples/gps_echotest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/examples/gps_satellitefix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4681 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/examples/gps_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/examples/gps_time_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-25 20:02:05.517840 adafruit-circuitpython-gps-3.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 20:02:05.517840 adafruit-circuitpython-gps-3.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16003 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/tests/adafruit_gps_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-25 20:01:49.000000 adafruit-circuitpython-gps-3.9.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.824610 adafruit-circuitpython-gps-3.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.832610 adafruit-circuitpython-gps-3.9.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.832610 adafruit-circuitpython-gps-3.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16275 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/adafruit_circuitpython_gps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-06-07 16:51:22.000000 adafruit-circuitpython-gps-3.9.9/adafruit_circuitpython_gps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-07 16:51:22.000000 adafruit-circuitpython-gps-3.9.9/adafruit_circuitpython_gps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 16:51:22.000000 adafruit-circuitpython-gps-3.9.9/adafruit_circuitpython_gps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-07 16:51:22.000000 adafruit-circuitpython-gps-3.9.9/adafruit_circuitpython_gps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-07 16:51:22.000000 adafruit-circuitpython-gps-3.9.9/adafruit_circuitpython_gps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    22687 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/adafruit_gps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/details.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/details.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/examples/gps_datalogging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2807 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/examples/gps_echotest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/examples/gps_satellitefix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4681 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/examples/gps_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/examples/gps_time_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:22.836610 adafruit-circuitpython-gps-3.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16003 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/tests/adafruit_gps_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-06-07 16:51:08.000000 adafruit-circuitpython-gps-3.9.9/tox.ini
```

### Comparing `adafruit-circuitpython-gps-3.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-gps-3.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/.github/workflows/build.yml` & `adafruit-circuitpython-gps-3.9.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/.github/workflows/release.yml` & `adafruit-circuitpython-gps-3.9.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/.gitignore` & `adafruit-circuitpython-gps-3.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/.pre-commit-config.yaml` & `adafruit-circuitpython-gps-3.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/.pylintrc` & `adafruit-circuitpython-gps-3.9.9/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-gps-3.9.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-gps-3.9.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/LICENSE` & `adafruit-circuitpython-gps-3.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-gps-3.9.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/LICENSES/MIT.txt` & `adafruit-circuitpython-gps-3.9.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-gps-3.9.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/PKG-INFO` & `adafruit-circuitpython-gps-3.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-gps
-Version: 3.9.8
+Version: 3.9.9
 Summary: CircuitPython library for GPS modules.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_GPS
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit gps module latitude longitude breakout hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-gps-3.9.8/README.rst` & `adafruit-circuitpython-gps-3.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/adafruit_circuitpython_gps.egg-info/PKG-INFO` & `adafruit-circuitpython-gps-3.9.9/adafruit_circuitpython_gps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-gps
-Version: 3.9.8
+Version: 3.9.9
 Summary: CircuitPython library for GPS modules.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_GPS
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit gps module latitude longitude breakout hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-gps-3.9.8/adafruit_circuitpython_gps.egg-info/SOURCES.txt` & `adafruit-circuitpython-gps-3.9.9/adafruit_circuitpython_gps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/adafruit_gps.py` & `adafruit-circuitpython-gps-3.9.9/adafruit_gps.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/docs/_static/favicon.ico` & `adafruit-circuitpython-gps-3.9.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/docs/conf.py` & `adafruit-circuitpython-gps-3.9.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-gps-3.9.8/docs/details.rst` & `adafruit-circuitpython-gps-3.9.9/docs/details.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/docs/examples.rst` & `adafruit-circuitpython-gps-3.9.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/docs/index.rst` & `adafruit-circuitpython-gps-3.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/examples/gps_datalogging.py` & `adafruit-circuitpython-gps-3.9.9/examples/gps_datalogging.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/examples/gps_echotest.py` & `adafruit-circuitpython-gps-3.9.9/examples/gps_echotest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/examples/gps_satellitefix.py` & `adafruit-circuitpython-gps-3.9.9/examples/gps_satellitefix.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/examples/gps_simpletest.py` & `adafruit-circuitpython-gps-3.9.9/examples/gps_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/examples/gps_time_source.py` & `adafruit-circuitpython-gps-3.9.9/examples/gps_time_source.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/setup.py` & `adafruit-circuitpython-gps-3.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gps-3.9.8/tests/adafruit_gps_test.py` & `adafruit-circuitpython-gps-3.9.9/tests/adafruit_gps_test.py`

 * *Files identical despite different names*

