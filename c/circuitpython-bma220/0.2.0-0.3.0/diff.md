# Comparing `tmp/circuitpython-bma220-0.2.0.tar.gz` & `tmp/circuitpython-bma220-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bma220-0.2.0.tar", last modified: Thu May 18 20:39:54 2023, max compression
+gzip compressed data, was "circuitpython-bma220-0.3.0.tar", last modified: Fri May 19 16:13:07 2023, max compression
```

## Comparing `circuitpython-bma220-0.2.0.tar` & `circuitpython-bma220-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.123404 circuitpython-bma220-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.115404 circuitpython-bma220-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-18 20:39:54.123404 circuitpython-bma220-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/bma220/
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/bma220/bma220.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/bma220/bma220_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/bma220/bma220_slope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.123404 circuitpython-bma220-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_filter_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_latched_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_sleep_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_slope_slope_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_slope_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 20:39:54.123404 circuitpython-bma220-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.996886 circuitpython-bma220-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.988886 circuitpython-bma220-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.988886 circuitpython-bma220-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-19 16:13:07.996886 circuitpython-bma220-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.992886 circuitpython-bma220-0.3.0/bma220/
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/bma220/bma220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/bma220/bma220_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/bma220/bma220_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/bma220/bma220_tap_sensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.992886 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.992886 circuitpython-bma220-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.992886 circuitpython-bma220-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.996886 circuitpython-bma220-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_double_tap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_filter_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_latched_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_sleep_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_slope_slope_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_slope_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:13:07.996886 circuitpython-bma220-0.3.0/setup.cfg
```

### Comparing `circuitpython-bma220-0.2.0/.github/workflows/build.yml` & `circuitpython-bma220-0.3.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/.github/workflows/release_gh.yml` & `circuitpython-bma220-0.3.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/.gitignore` & `circuitpython-bma220-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/.pre-commit-config.yaml` & `circuitpython-bma220-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/.pylintrc` & `circuitpython-bma220-0.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/LICENSE` & `circuitpython-bma220-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/PKG-INFO` & `circuitpython-bma220-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bma220
-Version: 0.2.0
+Version: 0.3.0
 Summary: BMA220 Bosch Circuitpython Driver library
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMA220
 Keywords: sensor,blinka,circuitpython,micropython,bma220,acceleration,digital,bosch,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bma220-0.2.0/README.rst` & `circuitpython-bma220-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/bma220/bma220.py` & `circuitpython-bma220-0.3.0/bma220/bma220.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     from busio import I2C
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 
 _REG_WHOAMI = const(0x00)
 _FILTER_CONF = const(0x20)
 _ACC_RANGE = const(0x22)
 _SLEEP_CONF = const(0x0F)
@@ -171,15 +171,18 @@
             raise RuntimeError("Failed to find BMA220")
 
         self._acc_range_mem = self._acc_range
 
     @property
     def acc_range(self) -> str:
         """
-        Sensor acc_range
+        The BMA220 has four different range settings for the full scale acceleration range.
+        In dependence of the use case always the lowest full scale range with the maximum
+        resolution should be selected. Please refer to literature to find out, which full
+        scale acceleration range, which sensitivity or which resolution is the ideal one.
 
         +---------------------------------+------------------+
         | Mode                            | Value            |
         +=================================+==================+
         | :py:const:`bma220.ACC_RANGE_2`  | :py:const:`0b00` |
         +---------------------------------+------------------+
         | :py:const:`bma220.ACC_RANGE_4`  | :py:const:`0b01` |
@@ -203,15 +206,19 @@
             raise ValueError("Value must be a valid acc_range setting")
         self._acc_range = value
         self._acc_range_mem = value
 
     @property
     def sleep_enabled(self) -> str:
         """
-        Sensor sleep_enabled
+        The BMA220 supports a low-power mode. In this low-power mode, the chip wakes up
+        periodically, enables the interrupt controller and goes back to sleep if no
+        interrupt has occurred.
+        The low-power mode can be enabled by setting :attr:`sleep_enabled` and by enabling
+        the data ready interrupt (or any other interrupt, see chapter 5 in the datasheet)
 
         +-----------------------------------+-----------------+
         | Mode                              | Value           |
         +===================================+=================+
         | :py:const:`bma220.SLEEP_DISABLED` | :py:const:`0b0` |
         +-----------------------------------+-----------------+
         | :py:const:`bma220.SLEEP_ENABLED`  | :py:const:`0b1` |
@@ -225,15 +232,15 @@
         if value not in sleep_enabled_values:
             raise ValueError("Value must be a valid sleep_enabled setting")
         self._sleep_enabled = value
 
     @property
     def sleep_duration(self) -> str:
         """
-        Sensor sleep_duration
+        Sensor sleep_duration.
 
         +--------------------------------+-------------------+
         | Mode                           | Value             |
         +================================+===================+
         | :py:const:`bma220.SLEEP_2MS`   | :py:const:`0b000` |
         +--------------------------------+-------------------+
         | :py:const:`bma220.SLEEP_10MS`  | :py:const:`0b001` |
@@ -269,14 +276,16 @@
             raise ValueError("Value must be a valid sleep_duration setting")
         self._sleep_duration = value
 
     @property
     def x_enabled(self) -> str:
         """
         Sensor x_enabled
+        In order to optimize further power consumption of the BMA220, data evaluation
+        of individual axes can be deactivated. Per default, all three axes are active.
 
         +-------------------------------+-----------------+
         | Mode                          | Value           |
         +===============================+=================+
         | :py:const:`bma220.X_DISABLED` | :py:const:`0b0` |
         +-------------------------------+-----------------+
         | :py:const:`bma220.X_ENABLED`  | :py:const:`0b1` |
@@ -294,14 +303,16 @@
             raise ValueError("Value must be a valid x_enabled setting")
         self._x_enabled = value
 
     @property
     def y_enabled(self) -> str:
         """
         Sensor y_enabled
+        In order to optimize further power consumption of the BMA220, data evaluation
+        of individual axes can be deactivated. Per default, all three axes are active.
 
         +-------------------------------+-----------------+
         | Mode                          | Value           |
         +===============================+=================+
         | :py:const:`bma220.Y_DISABLED` | :py:const:`0b0` |
         +-------------------------------+-----------------+
         | :py:const:`bma220.Y_ENABLED`  | :py:const:`0b1` |
@@ -319,14 +330,16 @@
             raise ValueError("Value must be a valid y_enabled setting")
         self._y_enabled = value
 
     @property
     def z_enabled(self) -> str:
         """
         Sensor z_enabled
+        In order to optimize further power consumption of the BMA220, data evaluation
+        of individual axes can be deactivated. Per default, all three axes are active.
 
         +-------------------------------+-----------------+
         | Mode                          | Value           |
         +===============================+=================+
         | :py:const:`bma220.Z_DISABLED` | :py:const:`0b0` |
         +-------------------------------+-----------------+
         | :py:const:`bma220.Z_ENABLED`  | :py:const:`0b1` |
@@ -343,15 +356,17 @@
         if value not in axis_enabled_values:
             raise ValueError("Value must be a valid z_enabled setting")
         self._z_enabled = value
 
     @property
     def filter_bandwidth(self) -> str:
         """
-        Sensor filter_bandwidth
+        The BMA220 has a digital filter that can be configured. To always ensure
+         an ideal cut off frequency of the filter the BMA220 is adjusting the
+         sample rate automatically.
 
         +---------------------------------+------------------+
         | Mode                            | Value            |
         +=================================+==================+
         | :py:const:`bma220.ACCEL_32HZ`   | :py:const:`0x05` |
         +---------------------------------+------------------+
         | :py:const:`bma220.ACCEL_64HZ`   | :py:const:`0x04` |
@@ -382,33 +397,45 @@
         self._filter_bandwidth = value
 
     @property
     def latched_mode(self) -> str:
         """
         Sensor latched_mode
 
-        +-----------------------------------+-------------------+
-        | Mode                              | Value             |
-        +===================================+===================+
-        | :py:const:`bma220.UNLATCHED`      | :py:const:`0b000` |
-        +-----------------------------------+-------------------+
-        | :py:const:`bma220.LATCH_FOR_025S` | :py:const:`0b001` |
-        +-----------------------------------+-------------------+
-        | :py:const:`bma220.LATCH_FOR_050S` | :py:const:`0b010` |
-        +-----------------------------------+-------------------+
-        | :py:const:`bma220.LATCH_FOR_1S`   | :py:const:`0b011` |
-        +-----------------------------------+-------------------+
-        | :py:const:`bma220.LATCH_FOR_2S`   | :py:const:`0b100` |
-        +-----------------------------------+-------------------+
-        | :py:const:`bma220.LATCH_FOR_4S`   | :py:const:`0b101` |
-        +-----------------------------------+-------------------+
-        | :py:const:`bma220.LATCH_FOR_8S`   | :py:const:`0b110` |
-        +-----------------------------------+-------------------+
-        | :py:const:`bma220.LATCHED`        | :py:const:`0b111` |
-        +-----------------------------------+-------------------+
+        The interrupt controller can be used in two modes
+
+        - **Latched mode**: Once one of the configured interrupt conditions applies,
+          the INT pin is asserted and must be reset by the external master through
+          the digital interface.
+
+        - **Non-Latched mode**: The interrupt controller clears the INT signal once
+          the interrupt condition no longer applies.
+
+        The interrupt output can be programmed by :attr:`latched_mode` to be either
+        unlatched (‘000’) or latched permanently (‘111’) or have different latching times.
+
+        +-----------------------------------+--------------------------------+
+        | Mode                              | Value                          |
+        +===================================+================================+
+        | :py:const:`bma220.UNLATCHED`      | :py:const:`0b000`              |
+        +-----------------------------------+--------------------------------+
+        | :py:const:`bma220.LATCH_FOR_025S` | :py:const:`0b001` 0.25 seconds |
+        +-----------------------------------+--------------------------------+
+        | :py:const:`bma220.LATCH_FOR_050S` | :py:const:`0b010` 0.5 seconds  |
+        +-----------------------------------+--------------------------------+
+        | :py:const:`bma220.LATCH_FOR_1S`   | :py:const:`0b011` 1 second     |
+        +-----------------------------------+--------------------------------+
+        | :py:const:`bma220.LATCH_FOR_2S`   | :py:const:`0b100` 2 seconds    |
+        +-----------------------------------+--------------------------------+
+        | :py:const:`bma220.LATCH_FOR_4S`   | :py:const:`0b101` 4 seconds    |
+        +-----------------------------------+--------------------------------+
+        | :py:const:`bma220.LATCH_FOR_8S`   | :py:const:`0b110` 8 seconds    |
+        +-----------------------------------+--------------------------------+
+        | :py:const:`bma220.LATCHED`        | :py:const:`0b111`              |
+        +-----------------------------------+--------------------------------+
         """
         values = (
             "UNLATCHED",
             "LATCH_FOR_025S",
             "LATCH_FOR_050S",
             "LATCH_FOR_1S",
             "LATCH_FOR_2S",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `circuitpython-bma220-0.2.0/bma220/bma220_const.py` & `circuitpython-bma220-0.3.0/bma220/bma220_const.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * Author(s): Jose D. Montoya
 
 
 """
 
 from micropython import const
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 # pylint: disable=duplicate-code
 # Acceleration range
 ACC_RANGE_2 = const(0b00)
 ACC_RANGE_4 = const(0b01)
 ACC_RANGE_8 = const(0b10)
```

### Comparing `circuitpython-bma220-0.2.0/bma220/bma220_slope.py` & `circuitpython-bma220-0.3.0/bma220/bma220_slope.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 _CONF = const(0x1A)
 _SLOPE_INFO = const(0x12)
 _SLOPE_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
 
@@ -47,22 +47,37 @@
 SLOPE_SIGN_POSITIVE = const(0b00)
 SLOPE_SIGN_NEGATIVE = const(0b01)
 slope_sign_values = (SLOPE_SIGN_POSITIVE, SLOPE_SIGN_NEGATIVE)
 
 
 class BMA220_SLOPE(BMA220):
     """
-    BMA220 Slope mode class.
-    The any-motion detection uses the slope between two successive acceleration
-    signals to detect changes in motion. It generates an interrupt when a preset
-    threshold slope_th is exceeded. The threshold can be configured between 0 and
-    the maximum acceleration value corresponding to the selected measurement range.
-    The time difference between the successive acceleration signals depends on
-    the bandwidth of the configurable low pass filter and corresponds roughly
-    to 1/(2*bandwidth) (Δt=1/(2*bw)).
+    The any-motion detection uses the slope between two successive acceleration signals to detect
+    changes in motion. It generates an interrupt when a preset threshold slope_th is exceeded. The
+    threshold can be configured between 0 and the maximum acceleration value corresponding to
+    the selected measurement range. The time difference between the successive acceleration
+    signals depends on the bandwidth of the configurable low pass filter and corresponds roughly to
+    1/(2*bandwidth) (Δt=1/(2*bw)).
+    In order to suppress failure signals, the interrupt is only generated if a certain number
+    :attr:`slope_duration` of consecutive slope data points is above the slope threshold
+    :attr:`slope_threshold`.
+    If the same number of data points falls below the threshold, the interrupt is reset.
+    The criteria for any-motion detection are fulfilled and the slope interrupt is
+    generated if any of the enabled channels exceeds the threshold :attr:`slope_threshold`
+    for :attr:`slope_threshold` consecutive times. As soon as all the enabled channels fall
+    or stay below this threshold for :attr:`slope_threshold` consecutive times the interrupt
+    is reset unless interrupt signal is latched.
+    The any-motion interrupt logic sends out the signals of the axis that has triggered
+    the interrupt (:attr:`slope_interrupt_info`) and the signal of motion
+    direction (:attr:`slope_sign`).
+    When serial interface is active, any-motion detection logic is enabled if any of
+    the any-motion enable register bits is set. To disable the any-motion interrupt,
+    clear all the axis enable bits.
+    In the dedicated wake-up mode (6.1), all three axes are enabled for any-motion detection
+    whether the individual axis enable bits are set or not.
     """
 
     _slope_z_enabled = RWBit(_CONF, 3)
     _slope_y_enabled = RWBit(_CONF, 4)
     _slope_x_enabled = RWBit(_CONF, 5)
     _slope_int = ROBit(_INTERRUPTS, 0)
     _slope_threshold = RWBits(4, _SLOPE_INFO, 2)
```

### Comparing `circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/PKG-INFO` & `circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bma220
-Version: 0.2.0
+Version: 0.3.0
 Summary: BMA220 Bosch Circuitpython Driver library
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMA220
 Keywords: sensor,blinka,circuitpython,micropython,bma220,acceleration,digital,bosch,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/SOURCES.txt` & `circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release_gh.yml
 .github/workflows/release_pypi.yml
 bma220/bma220.py
 bma220/bma220_const.py
 bma220/bma220_slope.py
+bma220/bma220_tap_sensing.py
 circuitpython_bma220.egg-info/PKG-INFO
 circuitpython_bma220.egg-info/SOURCES.txt
 circuitpython_bma220.egg-info/dependency_links.txt
 circuitpython_bma220.egg-info/requires.txt
 circuitpython_bma220.egg-info/top_level.txt
 docs/api.rst
 docs/conf.py
@@ -26,13 +27,14 @@
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/bma220_acc_range.py
+examples/bma220_double_tap_test.py
 examples/bma220_filter_bandwidth.py
 examples/bma220_latched_mode.py
 examples/bma220_simpletest.py
 examples/bma220_sleep_duration.py
 examples/bma220_slope_slope_sign.py
 examples/bma220_slope_test.py
```

### Comparing `circuitpython-bma220-0.2.0/docs/_static/Logo.png` & `circuitpython-bma220-0.3.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/docs/_static/favicon.ico` & `circuitpython-bma220-0.3.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/docs/conf.py` & `circuitpython-bma220-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/docs/examples.rst` & `circuitpython-bma220-0.3.0/docs/examples.rst`

 * *Files 3% similar despite different names*

```diff
@@ -56,7 +56,16 @@
 --------------------
 
 Example showing the Slope sign setting
 
 .. literalinclude:: ../examples/bma220_slope_slope_sign.py
     :caption: examples/bma220_slope_slope_sign.py
     :linenos:
+
+Double Tap Example
+--------------------
+
+Example showing the Double Tap Setting
+
+.. literalinclude:: ../examples/bma220_double_tap_test.py
+    :caption: examples/bma220_double_tap_test.py
+    :linenos:
```

### Comparing `circuitpython-bma220-0.2.0/examples/bma220_acc_range.py` & `circuitpython-bma220-0.3.0/examples/bma220_acc_range.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/examples/bma220_filter_bandwidth.py` & `circuitpython-bma220-0.3.0/examples/bma220_filter_bandwidth.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/examples/bma220_latched_mode.py` & `circuitpython-bma220-0.3.0/examples/bma220_latched_mode.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/examples/bma220_sleep_duration.py` & `circuitpython-bma220-0.3.0/examples/bma220_sleep_duration.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/examples/bma220_slope_slope_sign.py` & `circuitpython-bma220-0.3.0/examples/bma220_slope_slope_sign.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.2.0/pyproject.toml` & `circuitpython-bma220-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bma220"
 description = "BMA220 Bosch Circuitpython Driver library"
-version = "0.2.0"
+version = "0.3.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_BMA220"}
 keywords = [
     "sensor",
```

