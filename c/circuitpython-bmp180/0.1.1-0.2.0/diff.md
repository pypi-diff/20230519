# Comparing `tmp/circuitpython-bmp180-0.1.1.tar.gz` & `tmp/circuitpython-bmp180-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bmp180-0.1.1.tar", last modified: Sat Apr 22 20:16:38 2023, max compression
+gzip compressed data, was "circuitpython-bmp180-0.2.0.tar", last modified: Fri May 19 00:03:26 2023, max compression
```

## Comparing `circuitpython-bmp180-0.1.1.tar` & `circuitpython-bmp180-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.841069 circuitpython-bmp180-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.841069 circuitpython-bmp180-0.1.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-04-22 20:16:31.000000 circuitpython-bmp180-0.1.1/bmp180.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/circuitpython_bmp180.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-22 20:16:38.000000 circuitpython-bmp180-0.1.1/circuitpython_bmp180.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 20:16:38.000000 circuitpython-bmp180-0.1.1/circuitpython_bmp180.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:16:38.000000 circuitpython-bmp180-0.1.1/circuitpython_bmp180.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-22 20:16:38.000000 circuitpython-bmp180-0.1.1/circuitpython_bmp180.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-22 20:16:38.000000 circuitpython-bmp180-0.1.1/circuitpython_bmp180.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-22 20:16:31.000000 circuitpython-bmp180-0.1.1/examples/bmp180_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-22 20:16:31.000000 circuitpython-bmp180-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-22 20:16:22.000000 circuitpython-bmp180-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 20:16:38.845069 circuitpython-bmp180-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.950479 circuitpython-bmp180-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.930478 circuitpython-bmp180-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.938478 circuitpython-bmp180-0.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.938478 circuitpython-bmp180-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.938478 circuitpython-bmp180-0.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-19 00:03:26.950479 circuitpython-bmp180-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-19 00:03:17.000000 circuitpython-bmp180-0.2.0/bmp180.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.942479 circuitpython-bmp180-0.2.0/circuitpython_bmp180.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-19 00:03:26.000000 circuitpython-bmp180-0.2.0/circuitpython_bmp180.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-19 00:03:26.000000 circuitpython-bmp180-0.2.0/circuitpython_bmp180.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:03:26.000000 circuitpython-bmp180-0.2.0/circuitpython_bmp180.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 00:03:26.000000 circuitpython-bmp180-0.2.0/circuitpython_bmp180.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 00:03:26.000000 circuitpython-bmp180-0.2.0/circuitpython_bmp180.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.946479 circuitpython-bmp180-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.946479 circuitpython-bmp180-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:03:26.946479 circuitpython-bmp180-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 00:03:17.000000 circuitpython-bmp180-0.2.0/examples/bmp180_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-19 00:03:17.000000 circuitpython-bmp180-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 00:03:06.000000 circuitpython-bmp180-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:03:26.950479 circuitpython-bmp180-0.2.0/setup.cfg
```

### Comparing `circuitpython-bmp180-0.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-bmp180-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/.github/workflows/build.yml` & `circuitpython-bmp180-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/.gitignore` & `circuitpython-bmp180-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/.pre-commit-config.yaml` & `circuitpython-bmp180-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/.pylintrc` & `circuitpython-bmp180-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/CODE_OF_CONDUCT.md` & `circuitpython-bmp180-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/LICENSE` & `circuitpython-bmp180-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-bmp180-0.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/LICENSES/MIT.txt` & `circuitpython-bmp180-0.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/LICENSES/Unlicense.txt` & `circuitpython-bmp180-0.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/PKG-INFO` & `circuitpython-bmp180-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmp180
-Version: 0.1.1
+Version: 0.2.0
 Summary: CircuitPython driver for the bmp180 sensor
 Author-email: "Jose D. Montoya" <qmc@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_bmp180
 Keywords: adafruit,blinka,circuitpython,micropython,bmp180,barometric,pressure,driver,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bmp180-0.1.1/README.rst` & `circuitpython-bmp180-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/bmp180.py` & `circuitpython-bmp180-0.2.0/bmp180.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,27 +30,15 @@
 _CHIP_ID = const(0x255)
 _I2C_ADDR = const(0x77)
 
 _REGISTER_CHIPID = const(0xD0)
 _REGISTER_SOFTRESET = const(0xE0)
 _REGISTER_CONTROL = const(0xF4)
 _REGISTER_DATA = const(0xF6)
-
-"""calibration coefficients register"""
 _REGISTER_AC1 = const(0xAA)
-_REGISTER_AC2 = const(0xAC)
-_REGISTER_AC3 = const(0xAE)
-_REGISTER_AC4 = const(0xB0)
-_REGISTER_AC5 = const(0xB2)
-_REGISTER_AC6 = const(0xB4)
-_REGISTER_B1 = const(0xB6)
-_REGISTER_B2 = const(0xB8)
-_REGISTER_MB = const(0xBA)
-_REGISTER_MC = const(0xBC)
-_REGISTER_MD = const(0xBE)
 
 _BMP180_PRESSURE_MIN_HPA = const(300)
 _BMP180_PRESSURE_MAX_HPA = const(1100)
 
 
 """oversampling values for temperature, pressure, and humidity"""
 TEMPERATURE_CMD = const(0x2E)
@@ -85,78 +73,85 @@
 
     _device_id = ROUnaryStruct(_REGISTER_CHIPID, "H")
     _reg_control = UnaryStruct(_REGISTER_CONTROL, "H")
     _reg_soft_reset = UnaryStruct(_REGISTER_SOFTRESET, "H")
     _regdata_MSB = UnaryStruct(_REGISTER_DATA, "H")
     _regdata_LSB = UnaryStruct(_REGISTER_DATA + 1, "H")
     _regdata_XLSB = UnaryStruct(_REGISTER_DATA + 2, "H")
-    _register_AC1 = UnaryStruct(_REGISTER_AC1, "H")
 
-    def __init__(self, i2c_bus: I2C, address: int = _I2C_ADDR) -> None:
+    _coeffs = Struct(_REGISTER_AC1, ">hhhHHHhhhhh")
+    _raw_temperature = UnaryStruct(_REGISTER_DATA, ">H")
+
+    def __init__(self, i2c_bus: I2C, address: int = 0x77) -> None:
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
-        print(self._device_id)
+
         if self._device_id != _CHIP_ID:
-            raise RuntimeError("Failed to find BMP180! Chip ID 0x%x" % self._device_id)
+            raise RuntimeError(
+                "Failed to find BMP180! Chip ID {}".format(self._device_id)
+            )
 
         self._oversampling_setting = PRESSURE_OVERSAMPLING_X8
         self._mode = MODE_HIGHRES
 
-        self._read_coefficients()
+        self.coeffs_mem = self._coeffs
 
         self.sea_level_pressure = 1013.25
 
     def _reset(self):
         """Soft reset the sensor"""
         self._reg_soft_reset = 0xB6  # reset the device
         sleep(0.004)  # Datasheet says 2ms.  Using 4ms just to be safe
 
     @property
     def temperature(self):
         """The compensated temperature in Celsius."""
-        UT = self._read_raw_temperature()
-        X1 = int(((UT - self._AC6) * self._AC5) >> 15)
-        X2 = int((self._MC << 11) / (X1 + self._MD))
+        self._reg_control = TEMPERATURE_CMD
+        sleep(0.005)  # Wait 5ms
+        UT = self._raw_temperature
+        X1 = int(((UT - self.coeffs_mem[5]) * self.coeffs_mem[4]) >> 15)
+        X2 = int((self.coeffs_mem[9] << 11) / (X1 + self.coeffs_mem[10]))
         B5 = X1 + X2
         temp = ((B5 + 8) >> 4) / 10.0
         return temp
 
-    def _read_raw_temperature(self):
-        self._reg_control = TEMPERATURE_CMD
-        sleep(0.005)  # Wait 5ms
-        return self._readU16(_REGISTER_DATA)
-
     @property
     def altitude(self):
         """The altitude based on the sea level pressure - which you must
-        enter ahead of time)"""
+        enter ahead of time"""
         altitude = 44330.0 * (
-            1.0 - pow(self.pressure / self.sea_level_pressure, 0.1903)
+            1.0 - ((self.pressure / self.sea_level_pressure) ** 0.19025)
         )
         return round(altitude, 1)
 
+    @altitude.setter
+    def altitude(self, value: float) -> None:
+        self.sea_level_pressure = self.pressure / (1.0 - value / 44330.0) ** 5.255
+
     @property
     def pressure(self):
         """The compensated pressure in hectoPascals."""
-        UT = self._read_raw_temperature()
+        self._reg_control = TEMPERATURE_CMD
+        sleep(0.005)  # Wait 5ms
+        UT = self._raw_temperature
         UP = self._read_raw_pressure()
 
-        X1 = int(((UT - self._AC6) * self._AC5) >> 15)
-        X2 = int((self._MC << 11) / (X1 + self._MD))
+        X1 = int(((UT - self.coeffs_mem[5]) * self.coeffs_mem[4]) >> 15)
+        X2 = int((self.coeffs_mem[9] << 11) / (X1 + self.coeffs_mem[10]))
         B5 = X1 + X2
 
         B6 = B5 - 4000
-        X1 = int((self._B2 * (B6 * B6) >> 12) >> 11)
-        X2 = int((self._AC2 * B6) >> 11)
+        X1 = int((self.coeffs_mem[7] * (B6 * B6) >> 12) >> 11)
+        X2 = int((self.coeffs_mem[1] * B6) >> 11)
         X3 = X1 + X2
-        B3 = int((((self._AC1 * 4 + X3) << self._mode) + 2) / 4)
+        B3 = int((((self.coeffs_mem[0] * 4 + X3) << self._mode) + 2) / 4)
 
-        X1 = int((self._AC3 * B6) >> 13)
-        X2 = int((self._B1 * ((B6 * B6) >> 12)) >> 16)
+        X1 = int((self.coeffs_mem[2] * B6) >> 13)
+        X2 = int((self.coeffs_mem[6] * ((B6 * B6) >> 12)) >> 16)
         X3 = int(((X1 + X2) + 2) >> 2)
-        B4 = int((self._AC4 * (X3 + 32768)) >> 15)
+        B4 = int((self.coeffs_mem[3] * (X3 + 32768)) >> 15)
         B7 = int((UP - B3) * (50000 >> self._mode))
 
         if B7 < 0x80000000:
             p = int((B7 * 2) / B4)
         else:
             p = int((B7 / B4) * 2)
 
@@ -217,61 +212,23 @@
         """
         return self._mode
 
     @mode.setter
     def mode(self, value):
 
         if not value in _BMP180_MODES:
-            raise ValueError("Mode '%s' not supported" % (value))
+            raise ValueError("Mode {} not supported".format(value))
         self._mode = value
 
     @property
     def oversampling_setting(self):
         """
         Oversampling setting
         Allowed values are set in the OVERSAMPLES enum class
         """
         return self._oversampling_setting
 
     @oversampling_setting.setter
     def oversampling_setting(self, value):
-        print("oss")
         if not value in _BMP180_PRESSURE_CMD:
-            raise ValueError("Overscan value '%s' not supported" % (value))
+            raise ValueError("Overscan value {} not supported".format(value))
         self._overscan_temperature = value
-
-    def _read_coefficients(self):
-        """Read & save the calibration coefficients"""
-
-        self._AC1 = self._readS16(_REGISTER_AC1)
-        self._AC2 = self._readS16(_REGISTER_AC2)
-        self._AC3 = self._readS16(_REGISTER_AC3)
-        self._AC4 = self._readU16(_REGISTER_AC4)
-        self._AC5 = self._readU16(_REGISTER_AC5)
-        self._AC6 = self._readU16(_REGISTER_AC6)
-        self._B1 = self._readS16(_REGISTER_B1)
-        self._B2 = self._readS16(_REGISTER_B2)
-        self._MB = self._readS16(_REGISTER_MB)
-        self._MC = self._readS16(_REGISTER_MC)
-        self._MD = self._readS16(_REGISTER_MD)
-
-    def _read_byte(self, register):
-        """Read a byte register value and return it"""
-        return self._read_register(register, 1)[0]
-
-    def _readS16(self, register):
-        msb = self._read_byte(register)
-        if msb > 127:
-            msb -= 256
-        return msb * 256 + self._read_byte(register + 1)
-
-    def _readU16(self, register):
-
-        return self._read_byte(register) * 256 + self._read_byte(register + 1)
-
-    def _read_register(self, register, length):
-        """Low level register reading over I2C, returns a list of values"""
-        with self.i2c_device as i2c:
-            i2c.write(bytes([register & 0xFF]))
-            result = bytearray(length)
-            i2c.readinto(result)
-            return result
```

### Comparing `circuitpython-bmp180-0.1.1/circuitpython_bmp180.egg-info/PKG-INFO` & `circuitpython-bmp180-0.2.0/circuitpython_bmp180.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmp180
-Version: 0.1.1
+Version: 0.2.0
 Summary: CircuitPython driver for the bmp180 sensor
 Author-email: "Jose D. Montoya" <qmc@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_bmp180
 Keywords: adafruit,blinka,circuitpython,micropython,bmp180,barometric,pressure,driver,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bmp180-0.1.1/circuitpython_bmp180.egg-info/SOURCES.txt` & `circuitpython-bmp180-0.2.0/circuitpython_bmp180.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/docs/_static/Logo.png` & `circuitpython-bmp180-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/docs/_static/favicon.ico` & `circuitpython-bmp180-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp180-0.1.1/docs/conf.py` & `circuitpython-bmp180-0.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,25 +104,25 @@
         "search.share",
     ],
     # Set the color and the accent color
     "palette": [
         {
             "media": "(prefers-color-scheme: light)",
             "scheme": "default",
-            "primary": "green",
+            "primary": "purple",
             "accent": "light-blue",
             "toggle": {
                 "icon": "material/lightbulb-outline",
                 "name": "Switch to dark mode",
             },
         },
         {
             "media": "(prefers-color-scheme: dark)",
             "scheme": "slate",
-            "primary": "green",
+            "primary": "purple",
             "accent": "light-blue",
             "toggle": {
                 "icon": "material/lightbulb",
                 "name": "Switch to light mode",
             },
         },
     ],
@@ -187,15 +187,15 @@
 }
 
 object_description_options = [
     ("py:.*", dict(generate_synopses="first_sentence")),
 ]
 
 # Set link name generated in the top bar.
-html_title = "CircuitPython QMC5883L"
+html_title = "CircuitPython BMP180"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # These paths are either relative to html_static_path
```

### Comparing `circuitpython-bmp180-0.1.1/pyproject.toml` & `circuitpython-bmp180-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bmp180"
 description = "CircuitPython driver for the bmp180 sensor"
-version = "0.1.1"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "qmc@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_bmp180"}
 keywords = [
     "adafruit",
```

