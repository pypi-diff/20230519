# Comparing `tmp/circuitpython-bmp384-0.1.0.tar.gz` & `tmp/circuitpython-bmp384-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bmp384-0.1.0.tar", last modified: Wed May  3 17:09:22 2023, max compression
+gzip compressed data, was "circuitpython-bmp384-0.1.1.tar", last modified: Fri May 19 13:15:04 2023, max compression
```

## Comparing `circuitpython-bmp384-0.1.0.tar` & `circuitpython-bmp384-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:09:22.098446 circuitpython-bmp384-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:09:22.094446 circuitpython-bmp384-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:09:22.094446 circuitpython-bmp384-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-03 17:09:22.098446 circuitpython-bmp384-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-05-03 17:09:14.000000 circuitpython-bmp384-0.1.0/bmp384.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:09:22.094446 circuitpython-bmp384-0.1.0/circuitpython_bmp384.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-03 17:09:22.000000 circuitpython-bmp384-0.1.0/circuitpython_bmp384.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-03 17:09:22.000000 circuitpython-bmp384-0.1.0/circuitpython_bmp384.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:09:22.000000 circuitpython-bmp384-0.1.0/circuitpython_bmp384.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 17:09:22.000000 circuitpython-bmp384-0.1.0/circuitpython_bmp384.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 17:09:22.000000 circuitpython-bmp384-0.1.0/circuitpython_bmp384.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:09:22.098446 circuitpython-bmp384-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:09:22.098446 circuitpython-bmp384-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:09:22.098446 circuitpython-bmp384-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-03 17:09:14.000000 circuitpython-bmp384-0.1.0/examples/bmp384_filter_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-03 17:09:14.000000 circuitpython-bmp384-0.1.0/examples/bmp384_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-03 17:09:14.000000 circuitpython-bmp384-0.1.0/examples/bmp384_pressure_oversample.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 17:09:14.000000 circuitpython-bmp384-0.1.0/examples/bmp384_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-03 17:09:14.000000 circuitpython-bmp384-0.1.0/examples/bmp384_temperature_oversample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-03 17:09:14.000000 circuitpython-bmp384-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 17:09:05.000000 circuitpython-bmp384-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:09:22.098446 circuitpython-bmp384-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:15:04.618317 circuitpython-bmp384-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:15:04.614317 circuitpython-bmp384-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:15:04.618317 circuitpython-bmp384-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-19 13:15:04.618317 circuitpython-bmp384-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14647 2023-05-19 13:14:57.000000 circuitpython-bmp384-0.1.1/bmp384.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:15:04.618317 circuitpython-bmp384-0.1.1/circuitpython_bmp384.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-19 13:15:04.000000 circuitpython-bmp384-0.1.1/circuitpython_bmp384.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-19 13:15:04.000000 circuitpython-bmp384-0.1.1/circuitpython_bmp384.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:15:04.000000 circuitpython-bmp384-0.1.1/circuitpython_bmp384.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 13:15:04.000000 circuitpython-bmp384-0.1.1/circuitpython_bmp384.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 13:15:04.000000 circuitpython-bmp384-0.1.1/circuitpython_bmp384.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:15:04.618317 circuitpython-bmp384-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:15:04.618317 circuitpython-bmp384-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:15:04.618317 circuitpython-bmp384-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-19 13:14:57.000000 circuitpython-bmp384-0.1.1/examples/bmp384_filter_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-19 13:14:57.000000 circuitpython-bmp384-0.1.1/examples/bmp384_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-19 13:14:57.000000 circuitpython-bmp384-0.1.1/examples/bmp384_pressure_oversample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 13:14:57.000000 circuitpython-bmp384-0.1.1/examples/bmp384_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-19 13:14:57.000000 circuitpython-bmp384-0.1.1/examples/bmp384_temperature_oversample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-19 13:14:57.000000 circuitpython-bmp384-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 13:14:49.000000 circuitpython-bmp384-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:15:04.618317 circuitpython-bmp384-0.1.1/setup.cfg
```

### Comparing `circuitpython-bmp384-0.1.0/.github/workflows/build.yml` & `circuitpython-bmp384-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/.github/workflows/release_gh.yml` & `circuitpython-bmp384-0.1.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/.gitignore` & `circuitpython-bmp384-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/.pre-commit-config.yaml` & `circuitpython-bmp384-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/.pylintrc` & `circuitpython-bmp384-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/LICENSE` & `circuitpython-bmp384-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/PKG-INFO` & `circuitpython-bmp384-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmp384
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython Driver for the Bosch BMP384 Pressure and Temperature sensor
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMP384
 Keywords: sensor,blinka,circuitpython,micropython,bmp384,pressure,temperature,driver,sensor,bosch,bmp384
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -81,37 +81,14 @@
 .. code-block:: shell
 
     mkdir project-name && cd project-name
     python3 -m venv .venv
     source .env/bin/activate
     pip3 install circuitpython-bmp384
 
-Installing to a Connected CircuitPython Device with Circup
-==========================================================
-
-Make sure that you have ``circup`` installed in your Python environment.
-Install it with the following command if necessary:
-
-.. code-block:: shell
-
-    pip3 install circup
-
-With ``circup`` installed and your CircuitPython device connected use the
-following command to install:
-
-.. code-block:: shell
-
-    circup install bmp384
-
-Or the following command to update an existing version:
-
-.. code-block:: shell
-
-    circup update
-
 Usage Example
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
```

### Comparing `circuitpython-bmp384-0.1.0/README.rst` & `circuitpython-bmp384-0.1.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -63,37 +63,14 @@
 .. code-block:: shell
 
     mkdir project-name && cd project-name
     python3 -m venv .venv
     source .env/bin/activate
     pip3 install circuitpython-bmp384
 
-Installing to a Connected CircuitPython Device with Circup
-==========================================================
-
-Make sure that you have ``circup`` installed in your Python environment.
-Install it with the following command if necessary:
-
-.. code-block:: shell
-
-    pip3 install circup
-
-With ``circup`` installed and your CircuitPython device connected use the
-following command to install:
-
-.. code-block:: shell
-
-    circup install bmp384
-
-Or the following command to update an existing version:
-
-.. code-block:: shell
-
-    circup update
-
 Usage Example
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
```

### Comparing `circuitpython-bmp384-0.1.0/bmp384.py` & `circuitpython-bmp384-0.1.1/bmp384.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from adafruit_register.i2c_bit import RWBit
 
 try:
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMP384.git"
 
 _REG_WHOAMI = const(0x00)
 _PWR_CTRL = const(0x1B)
 _OSR_CONFIG = const(0x1C)
 _ODR_CONFIG = const(0x1D)
 _CONFIG = const(0x1F)
@@ -111,15 +111,15 @@
         import bmp384
 
     Once this is done you can define your `board.I2C` object and define your sensor object
 
     .. code-block:: python
 
         i2c = board.I2C()  # uses board.SCL and board.SDA
-        bmp = BMP384.bmp384(i2c)
+        bmp = bmp384.BMP384(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
         press = bmp.pressure
         temp = bmp.temperature
@@ -166,21 +166,21 @@
         +--------------------------------+------------------+
         """
         values = (
             "SLEEP_MODE",
             "FORCED_MODE",
             "NORMAL_MODE",
         )
-        return values[self._power_mode]
+        return values[self._operation_mode]
 
     @power_mode.setter
     def power_mode(self, value: int) -> None:
         if value not in power_mode_values:
             raise ValueError("Value must be a valid power_mode setting")
-        self._power_mode = value
+        self._operation_mode = value
 
     @property
     def temperature_mode(self) -> str:
         """
         Sensor temperature_mode
 
         +---------------------------------+------------------+
```

### Comparing `circuitpython-bmp384-0.1.0/circuitpython_bmp384.egg-info/PKG-INFO` & `circuitpython-bmp384-0.1.1/circuitpython_bmp384.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmp384
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython Driver for the Bosch BMP384 Pressure and Temperature sensor
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMP384
 Keywords: sensor,blinka,circuitpython,micropython,bmp384,pressure,temperature,driver,sensor,bosch,bmp384
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -81,37 +81,14 @@
 .. code-block:: shell
 
     mkdir project-name && cd project-name
     python3 -m venv .venv
     source .env/bin/activate
     pip3 install circuitpython-bmp384
 
-Installing to a Connected CircuitPython Device with Circup
-==========================================================
-
-Make sure that you have ``circup`` installed in your Python environment.
-Install it with the following command if necessary:
-
-.. code-block:: shell
-
-    pip3 install circup
-
-With ``circup`` installed and your CircuitPython device connected use the
-following command to install:
-
-.. code-block:: shell
-
-    circup install bmp384
-
-Or the following command to update an existing version:
-
-.. code-block:: shell
-
-    circup update
-
 Usage Example
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
```

### Comparing `circuitpython-bmp384-0.1.0/circuitpython_bmp384.egg-info/SOURCES.txt` & `circuitpython-bmp384-0.1.1/circuitpython_bmp384.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/docs/_static/Logo.png` & `circuitpython-bmp384-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/docs/_static/favicon.ico` & `circuitpython-bmp384-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/docs/conf.py` & `circuitpython-bmp384-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/docs/examples.rst` & `circuitpython-bmp384-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/examples/bmp384_filter_coefficients.py` & `circuitpython-bmp384-0.1.1/examples/bmp384_filter_coefficients.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/examples/bmp384_power_mode.py` & `circuitpython-bmp384-0.1.1/examples/bmp384_power_mode.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/examples/bmp384_pressure_oversample.py` & `circuitpython-bmp384-0.1.1/examples/bmp384_pressure_oversample.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/examples/bmp384_temperature_oversample.py` & `circuitpython-bmp384-0.1.1/examples/bmp384_temperature_oversample.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp384-0.1.0/pyproject.toml` & `circuitpython-bmp384-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bmp384"
 description = "CircuitPython Driver for the Bosch BMP384 Pressure and Temperature sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_BMP384"}
 keywords = [
     "sensor",
```

