# Comparing `tmp/netto-0.0.2.tar.gz` & `tmp/netto-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/martin/Projects/netto/dist/.tmp-qdruujcg/netto-0.0.2.tar", last modified: Sat Nov 26 22:55:06 2022, max compression
+gzip compressed data, was "/Users/martin/Projects/netto/dist/.tmp-08szw15w/netto-0.1.0.tar", last modified: Fri May 19 12:32:37 2023, max compression
```

## Comparing `netto-0.0.2.tar` & `netto-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-11-26 22:55:06.026808 netto-0.0.2/
--rw-r--r--   0 martin     (501) staff       (20)     1069 2022-11-02 20:33:13.000000 netto-0.0.2/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)     2503 2022-11-26 22:55:06.023765 netto-0.0.2/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1901 2022-11-26 22:18:24.000000 netto-0.0.2/README.md
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-11-26 22:55:05.951907 netto-0.0.2/netto/
--rw-r--r--   0 martin     (501) staff       (20)      126 2022-11-26 17:16:01.000000 netto-0.0.2/netto/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      417 2022-11-18 21:37:12.000000 netto-0.0.2/netto/config.py
--rw-r--r--   0 martin     (501) staff       (20)     4855 2022-11-25 19:45:04.000000 netto-0.0.2/netto/const.py
--rw-r--r--   0 martin     (501) staff       (20)     1436 2022-11-26 22:18:24.000000 netto-0.0.2/netto/main.py
--rw-r--r--   0 martin     (501) staff       (20)     2649 2022-11-26 17:16:05.000000 netto-0.0.2/netto/social_security.py
--rw-r--r--   0 martin     (501) staff       (20)     2581 2022-11-26 17:16:05.000000 netto-0.0.2/netto/taxes_income.py
--rw-r--r--   0 martin     (501) staff       (20)      527 2022-11-26 17:16:05.000000 netto-0.0.2/netto/taxes_other.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-11-26 22:55:05.985916 netto-0.0.2/netto.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     2503 2022-11-26 22:55:05.000000 netto-0.0.2/netto.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      377 2022-11-26 22:55:05.000000 netto-0.0.2/netto.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2022-11-26 22:55:05.000000 netto-0.0.2/netto.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)        6 2022-11-26 22:55:05.000000 netto-0.0.2/netto.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)      667 2022-11-26 22:49:59.000000 netto-0.0.2/pyproject.toml
--rw-r--r--   0 martin     (501) staff       (20)       38 2022-11-26 22:55:06.033429 netto-0.0.2/setup.cfg
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-11-26 22:55:06.018533 netto-0.0.2/test/
--rw-r--r--   0 martin     (501) staff       (20)     1693 2022-11-26 17:14:40.000000 netto-0.0.2/test/test_main.py
--rw-r--r--   0 martin     (501) staff       (20)     4318 2022-11-26 17:14:40.000000 netto-0.0.2/test/test_social_security.py
--rw-r--r--   0 martin     (501) staff       (20)     1416 2022-11-26 17:14:40.000000 netto-0.0.2/test/test_taxes_income.py
--rw-r--r--   0 martin     (501) staff       (20)     1050 2022-11-26 17:14:40.000000 netto-0.0.2/test/test_taxes_other.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-19 12:32:37.556297 netto-0.1.0/
+-rw-r--r--   0 martin     (501) staff       (20)     1069 2022-11-02 20:33:13.000000 netto-0.1.0/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)     2315 2023-05-19 12:32:37.551731 netto-0.1.0/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     1713 2023-05-19 12:10:44.000000 netto-0.1.0/README.md
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-19 12:32:37.527930 netto-0.1.0/netto/
+-rw-r--r--   0 martin     (501) staff       (20)      126 2022-11-26 17:16:01.000000 netto-0.1.0/netto/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      988 2023-05-18 08:48:46.000000 netto-0.1.0/netto/config.py
+-rw-r--r--   0 martin     (501) staff       (20)     4826 2023-05-16 10:43:19.000000 netto-0.1.0/netto/const.py
+-rw-r--r--   0 martin     (501) staff       (20)     3377 2023-05-19 12:08:56.000000 netto-0.1.0/netto/main.py
+-rw-r--r--   0 martin     (501) staff       (20)     2669 2022-12-12 18:09:34.000000 netto-0.1.0/netto/social_security.py
+-rw-r--r--   0 martin     (501) staff       (20)     5658 2023-05-17 18:22:28.000000 netto-0.1.0/netto/taxes_income.py
+-rw-r--r--   0 martin     (501) staff       (20)      594 2023-05-16 13:13:22.000000 netto-0.1.0/netto/taxes_other.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-19 12:32:37.540266 netto-0.1.0/netto.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     2315 2023-05-19 12:32:37.000000 netto-0.1.0/netto.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      397 2023-05-19 12:32:37.000000 netto-0.1.0/netto.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-05-19 12:32:37.000000 netto-0.1.0/netto.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        6 2023-05-19 12:32:37.000000 netto-0.1.0/netto.egg-info/top_level.txt
+-rw-r--r--   0 martin     (501) staff       (20)      667 2023-05-19 12:30:06.000000 netto-0.1.0/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)       38 2023-05-19 12:32:37.557597 netto-0.1.0/setup.cfg
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-19 12:32:37.548812 netto-0.1.0/test/
+-rw-r--r--   0 martin     (501) staff       (20)     1350 2023-05-18 08:48:49.000000 netto-0.1.0/test/test_config.py
+-rw-r--r--   0 martin     (501) staff       (20)     2253 2023-05-19 12:08:43.000000 netto-0.1.0/test/test_main.py
+-rw-r--r--   0 martin     (501) staff       (20)     4318 2022-12-12 16:48:37.000000 netto-0.1.0/test/test_social_security.py
+-rw-r--r--   0 martin     (501) staff       (20)     2193 2023-05-17 18:22:32.000000 netto-0.1.0/test/test_taxes_income.py
+-rw-r--r--   0 martin     (501) staff       (20)     1050 2022-12-12 16:48:37.000000 netto-0.1.0/test/test_taxes_other.py
```

### Comparing `netto-0.0.2/LICENSE` & `netto-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netto-0.0.2/PKG-INFO` & `netto-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netto
-Version: 0.0.2
+Version: 0.1.0
 Summary: German income tax (Einkommensteuer) and social security (Sozialabgaben) calculator
 Author-email: Martin Klein <hi@martinklein.co>
 Project-URL: Homepage, https://github.com/0-k/netto
 Project-URL: Documentation, https://netto.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/0-k/netto/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,40 +15,36 @@
 
 # netto
 
 [![Documentation Status](https://readthedocs.org/projects/netto/badge/?version=latest)](https://netto.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/netto.svg)](https://pypi.python.org/pypi/netto)
 [![CI](https://github.com/0-k/netto/actions/workflows/workflow.yml/badge.svg)](https://github.com/0-k/netto/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/0-k/netto/branch/master/graph/badge.svg)](https://codecov.io/gh/0-k/netto)
-[![License](https://img.shields.io/pypi/l/netto.svg)](LICENSE.txt)
+[![License](https://img.shields.io/pypi/l/netto.svg)](LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 German income tax (Einkommensteuer) and social security (Sozialabgaben) calculator.
 
 Currently tested against the following assumptions:
-* Tax class I/IV
 * Public health and pension insurance
 * West-German pension deduction
 * Optional: Church tax
-* Supported tax years: 2018-2023
+* Optional: Married 
+* Supported tax years: 2018-2024
 
 ### TODO list
 
-* Implement tax class II & III/V
 * Calculate support for children (Kindergeld/Kinderfreibetrag)
-* Implement fields for private health insurance
-* Implement fields for private pension insurance
 * Implement correct pension deductible for East Germany
-* Convenience function to calculate church tax (by state)
 
 ## Sources
 
 * [German tax curve](https://www.bmf-steuerrechner.de/Tarifhistorie_Steuerrechner.pdf?__blob=publicationFile&v=1)
 * [Wage tax (Lohnsteuer)](https://www.bmf-steuerrechner.de/bl/bl2022/eingabeformbl2022.xhtml)
 * [Social security deductable (Vorsorgepauschale)](https://www.lohn-info.de/vorsorgepauschale.html)
 * [Social security rates](https://www.lohn-info.de/sozialversicherungsbeitraege2022.html)
 * [Taxable income calculator](https://udo-brechtel.de/mathe/est_gsv/reverse_zve_brutto.htm)
 * [Solidarity tax (Solidaritätszuschlag)](https://www.lohn-info.de/solizuschlag.html)
 
 ## Credits
 
-Martin Klein, 2022
+Martin Klein, 2023
```

### Comparing `netto-0.0.2/README.md` & `netto-0.1.0/netto.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,50 @@
+Metadata-Version: 2.1
+Name: netto
+Version: 0.1.0
+Summary: German income tax (Einkommensteuer) and social security (Sozialabgaben) calculator
+Author-email: Martin Klein <hi@martinklein.co>
+Project-URL: Homepage, https://github.com/0-k/netto
+Project-URL: Documentation, https://netto.readthedocs.io/en/latest/
+Project-URL: Bug Tracker, https://github.com/0-k/netto/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # netto
 
 [![Documentation Status](https://readthedocs.org/projects/netto/badge/?version=latest)](https://netto.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/netto.svg)](https://pypi.python.org/pypi/netto)
 [![CI](https://github.com/0-k/netto/actions/workflows/workflow.yml/badge.svg)](https://github.com/0-k/netto/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/0-k/netto/branch/master/graph/badge.svg)](https://codecov.io/gh/0-k/netto)
-[![License](https://img.shields.io/pypi/l/netto.svg)](LICENSE.txt)
+[![License](https://img.shields.io/pypi/l/netto.svg)](LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 German income tax (Einkommensteuer) and social security (Sozialabgaben) calculator.
 
 Currently tested against the following assumptions:
-* Tax class I/IV
 * Public health and pension insurance
 * West-German pension deduction
 * Optional: Church tax
-* Supported tax years: 2018-2023
+* Optional: Married 
+* Supported tax years: 2018-2024
 
 ### TODO list
 
-* Implement tax class II & III/V
 * Calculate support for children (Kindergeld/Kinderfreibetrag)
-* Implement fields for private health insurance
-* Implement fields for private pension insurance
 * Implement correct pension deductible for East Germany
-* Convenience function to calculate church tax (by state)
 
 ## Sources
 
 * [German tax curve](https://www.bmf-steuerrechner.de/Tarifhistorie_Steuerrechner.pdf?__blob=publicationFile&v=1)
 * [Wage tax (Lohnsteuer)](https://www.bmf-steuerrechner.de/bl/bl2022/eingabeformbl2022.xhtml)
 * [Social security deductable (Vorsorgepauschale)](https://www.lohn-info.de/vorsorgepauschale.html)
 * [Social security rates](https://www.lohn-info.de/sozialversicherungsbeitraege2022.html)
 * [Taxable income calculator](https://udo-brechtel.de/mathe/est_gsv/reverse_zve_brutto.htm)
 * [Solidarity tax (Solidaritätszuschlag)](https://www.lohn-info.de/solizuschlag.html)
 
 ## Credits
 
-Martin Klein, 2022
+Martin Klein, 2023
```

### Comparing `netto-0.0.2/netto/const.py` & `netto-0.1.0/netto/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-tax_curve = {
+__tax_curve = {
     2018: {
         0: {"step": 9000, "rate": 0.14},
         1: {"step": 13996, "rate": 0.2397, "const": [997.8, 1400]},
         2: {"step": 54949, "rate": 0.42, "const": [220.13, 2397, 948.49]},
         3: {"step": 260533, "rate": 0.45, "const": [8621.75, 16437.7]},
     },
     2019: {
@@ -26,54 +26,53 @@
     2022: {
         0: {"step": 10347, "rate": 0.14},
         1: {"step": 14926, "rate": 0.2397, "const": [1088.67, 1400]},
         2: {"step": 58596, "rate": 0.42, "const": [206.43, 2397, 869.32]},
         3: {"step": 277826, "rate": 0.45, "const": [9336.45, 17671.20]},
     },
     2023: {
-        0: {"step": 10633, "rate": 0.14},
+        0: {"step": 10909, "rate": 0.14},
         1: {
-            "step": 15786,
+            "step": 15999,
             "rate": 0.2397,
-            "const": [NotImplementedError, NotImplementedError],
+            "const": [None, None],
         },
         2: {
-            "step": 61971,
+            "step": 62809,
             "rate": 0.42,
-            "const": [NotImplementedError, NotImplementedError, NotImplementedError],
+            "const": [None, None, None],
         },
         3: {
             "step": 277826,
             "rate": 0.45,
-            "const": [NotImplementedError, NotImplementedError],
+            "const": [None, None],
         },
     },
     2024: {
-        0: {"step": 10933, "rate": 0.14},
+        0: {"step": 11605, "rate": 0.14},
         1: {
-            "step": 16179,
+            "step": 17005,
             "rate": 0.2397,
-            "const": [NotImplementedError, NotImplementedError],
+            "const": [None, None],
         },
         2: {
-            "step": 63514,
+            "step": 66760,
             "rate": 0.42,
-            "const": [NotImplementedError, NotImplementedError, NotImplementedError],
+            "const": [None, None, None],
         },
         3: {
             "step": 277826,
             "rate": 0.45,
-            "const": [NotImplementedError, NotImplementedError],
+            "const": [None, None],
         },
     },
-    2025: NotImplementedError,
 }
 
 
-social_security_curve = {
+__social_security_curve = {
     2018: {
         "pension": {"limit": 78000, "rate": 0.093},
         "unemployment": {"limit": 78000, "rate": 0.015},
         "health": {"limit": 53100, "rate": 0.073},
         "nursing": {"limit": 53100, "rate": 0.01275, "extra": 0.0025},
     },
     2019: {
@@ -102,32 +101,37 @@
     },
     2023: {
         "pension": {"limit": 87600, "rate": 0.093},
         "unemployment": {"limit": 87600, "rate": 0.012},
         "health": {"limit": 59850, "rate": 0.073},
         "nursing": {"limit": 59850, "rate": 0.01525, "extra": 0.0035},
     },
-    2024: NotImplementedError,
+    2024: {
+        "pension": {"limit": 87600, "rate": 0.093},
+        "unemployment": {"limit": 87600, "rate": 0.012},
+        "health": {"limit": 59850, "rate": 0.073},
+        "nursing": {"limit": 59850, "rate": 0.01525, "extra": 0.0035},
+    },
     2025: NotImplementedError,
 }
 
 
-soli_curve = {
+__soli_curve = {
     2018: {"start_taxable_income": 972, "start_fraction": 0.2, "end_rate": 0.055},
     2019: {"start_taxable_income": 972, "start_fraction": 0.2, "end_rate": 0.055},
     2020: {"start_taxable_income": 972, "start_fraction": 0.2, "end_rate": 0.055},
     2021: {"start_taxable_income": 16956, "start_fraction": 0.119, "end_rate": 0.055},
     2022: {"start_taxable_income": 16956, "start_fraction": 0.119, "end_rate": 0.055},
     2023: {"start_taxable_income": 17543, "start_fraction": 0.119, "end_rate": 0.055},
     2024: {"start_taxable_income": 18130, "start_fraction": 0.119, "end_rate": 0.055},
-    2025: NotImplementedError,
+    2025: None,
 }
 
 
-correction_factor_pensions = {
+__correction_factor_pensions = {
     2018: 0.72,
     2019: 0.76,
     2020: 0.8,
     2021: 0.84,
     2022: 0.88,
     2023: 0.92,
     2024: 0.96,
```

### Comparing `netto-0.0.2/netto/social_security.py` & `netto-0.1.0/netto/social_security.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 import math
 
 from scipy.integrate import quad
 
 import netto.config as config
-from netto.const import correction_factor_pensions, social_security_curve
+from netto.const import __correction_factor_pensions, __social_security_curve
+
+
+def get_rate_pension(salary):
+    return __get_rate(salary, "pension")
 
 
 def __get_rate(salary, type, extra=0):
     return (
-        social_security_curve[config.YEAR][type]["rate"] + extra
-        if 0 < salary <= social_security_curve[config.YEAR][type]["limit"]
+        __social_security_curve[config.year][type]["rate"] + extra
+        if 0 < salary <= __social_security_curve[config.year][type]["limit"]
         else 0
     )
 
 
-def __get_value(salary, type, extra=0):
-    return min(
-        salary * (social_security_curve[config.YEAR][type]["rate"] + extra),
-        social_security_curve[config.YEAR][type]["limit"]
-        * (social_security_curve[config.YEAR][type]["rate"] + extra),
-    )
-
-
-def get_rate_pension(salary):
-    return __get_rate(salary, "pension")
-
-
 def get_rate_unemployment(salary):
     return __get_rate(salary, "unemployment")
 
 
 def get_rate_health(salary):
-    extra = config.EXTRA_HEALTH_INSURANCE / 2
+    extra = config.extra_health_insurance / 2
     return __get_rate(salary, "health", extra)
 
 
 def get_rate_nursing(salary):
     extra = (
         0
-        if config.HAS_CHILDREN
-        else social_security_curve[config.YEAR]["nursing"]["extra"]
+        if config.has_children
+        else __social_security_curve[config.year]["nursing"]["extra"]
     )
     return __get_rate(salary, "nursing", extra)
 
 
 def calc_insurance_pension(salary):
     return __get_value(salary, "pension")
 
 
+def __get_value(salary, type, extra=0):
+    return min(
+        salary * (__social_security_curve[config.year][type]["rate"] + extra),
+        __social_security_curve[config.year][type]["limit"]
+        * (__social_security_curve[config.year][type]["rate"] + extra),
+    )
+
+
 def calc_insurance_unemployment(salary):
     return __get_value(salary, "unemployment")
 
 
 def calc_insurance_health(salary):
-    extra = config.EXTRA_HEALTH_INSURANCE / 2
+    extra = config.extra_health_insurance / 2
     return __get_value(salary, "health", extra)
 
 
 def calc_insurance_health_deductable(salary):
-    extra = config.EXTRA_HEALTH_INSURANCE / 2
+    extra = config.extra_health_insurance / 2
     return __get_value(salary, "health", extra - 0.003)
 
 
 def calc_insurance_nursing(salary):
     extra = (
         0
-        if config.HAS_CHILDREN
-        else social_security_curve[config.YEAR]["nursing"]["extra"]
+        if config.has_children
+        else __social_security_curve[config.year]["nursing"]["extra"]
     )
     return __get_value(salary, "nursing", extra)
 
 
-def calc_deductable_social_security(salary):
+def calc_deductible_social_security(salary):
     return (
         math.ceil(
-            calc_insurance_pension(salary) * correction_factor_pensions[config.YEAR]
+            calc_insurance_pension(salary) * __correction_factor_pensions[config.year]
         )
         + math.ceil(calc_insurance_health_deductable(salary))
         + math.ceil(calc_insurance_nursing(salary))
     )
 
 
 def calc_social_security(salary):
```

### Comparing `netto-0.0.2/netto.egg-info/PKG-INFO` & `netto-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,35 @@
-Metadata-Version: 2.1
-Name: netto
-Version: 0.0.2
-Summary: German income tax (Einkommensteuer) and social security (Sozialabgaben) calculator
-Author-email: Martin Klein <hi@martinklein.co>
-Project-URL: Homepage, https://github.com/0-k/netto
-Project-URL: Documentation, https://netto.readthedocs.io/en/latest/
-Project-URL: Bug Tracker, https://github.com/0-k/netto/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # netto
 
 [![Documentation Status](https://readthedocs.org/projects/netto/badge/?version=latest)](https://netto.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://img.shields.io/pypi/v/netto.svg)](https://pypi.python.org/pypi/netto)
 [![CI](https://github.com/0-k/netto/actions/workflows/workflow.yml/badge.svg)](https://github.com/0-k/netto/actions/workflows/workflow.yml)
 [![codecov](https://codecov.io/gh/0-k/netto/branch/master/graph/badge.svg)](https://codecov.io/gh/0-k/netto)
-[![License](https://img.shields.io/pypi/l/netto.svg)](LICENSE.txt)
+[![License](https://img.shields.io/pypi/l/netto.svg)](LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 German income tax (Einkommensteuer) and social security (Sozialabgaben) calculator.
 
 Currently tested against the following assumptions:
-* Tax class I/IV
 * Public health and pension insurance
 * West-German pension deduction
 * Optional: Church tax
-* Supported tax years: 2018-2023
+* Optional: Married 
+* Supported tax years: 2018-2024
 
 ### TODO list
 
-* Implement tax class II & III/V
 * Calculate support for children (Kindergeld/Kinderfreibetrag)
-* Implement fields for private health insurance
-* Implement fields for private pension insurance
 * Implement correct pension deductible for East Germany
-* Convenience function to calculate church tax (by state)
 
 ## Sources
 
 * [German tax curve](https://www.bmf-steuerrechner.de/Tarifhistorie_Steuerrechner.pdf?__blob=publicationFile&v=1)
 * [Wage tax (Lohnsteuer)](https://www.bmf-steuerrechner.de/bl/bl2022/eingabeformbl2022.xhtml)
 * [Social security deductable (Vorsorgepauschale)](https://www.lohn-info.de/vorsorgepauschale.html)
 * [Social security rates](https://www.lohn-info.de/sozialversicherungsbeitraege2022.html)
 * [Taxable income calculator](https://udo-brechtel.de/mathe/est_gsv/reverse_zve_brutto.htm)
 * [Solidarity tax (Solidaritätszuschlag)](https://www.lohn-info.de/solizuschlag.html)
 
 ## Credits
 
-Martin Klein, 2022
+Martin Klein, 2023
```

### Comparing `netto-0.0.2/pyproject.toml` & `netto-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netto"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Martin Klein", email="hi@martinklein.co" },
 ]
 description = "German income tax (Einkommensteuer) and social security (Sozialabgaben) calculator"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `netto-0.0.2/test/test_social_security.py` & `netto-0.1.0/test/test_social_security.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import netto.config as config
 import netto.social_security as social_security
 
 
 class TestSocialSecurity(unittest.TestCase):
     def setUp(self):
-        config.EXTRA_HEALTH_INSURANCE = 0.014
-        config.CHURCH_TAX = 0.09
-        config.HAS_CHILDREN = False
+        config.extra_health_insurance = 0.014
+        config.church_tax = 0.09
+        config.has_children = False
 
     def tearDown(self):
         pass
 
     def test_get_rate_pension(self):
         self.assertEqual(social_security.get_rate_pension(0), 0)
         self.assertEqual(social_security.get_rate_pension(10000), 0.093)
@@ -38,52 +38,52 @@
         self.assertEqual(social_security.calc_insurance_health(0), 0)
         self.assertEqual(social_security.calc_insurance_health(10000), 0.08 * 10000)
         self.assertEqual(social_security.calc_insurance_health(58050), 0.08 * 58050)
         self.assertEqual(social_security.calc_insurance_health(58051), 0.08 * 58050)
         self.assertEqual(social_security.calc_insurance_health(100000), 0.08 * 58050)
 
     def test_calc_deductable_social_security(self):
-        self.assertEqual(social_security.calc_deductable_social_security(0), 0)
+        self.assertEqual(social_security.calc_deductible_social_security(0), 0)
         self.assertEqual(
-            social_security.calc_deductable_social_security(30000),
+            social_security.calc_deductible_social_security(30000),
             2456 + 2310 + 563,  # https://www.lohn-info.de/vorsorgepauschale.html
         )
 
     def test_sameness_of_calc_social_security(self):
         for salary in range(0, 100001, 10000):
             self.assertEqual(
                 social_security.calc_social_security(salary),
                 social_security.calc_social_security_by_integration(salary),
             )
 
     def test_sameness_of_calc_social_security_different_config(self):
-        config.EXTRA_HEALTH_INSURANCE = 0.015
-        config.HAS_CHILDREN = True
+        config.extra_health_insurance = 0.015
+        config.has_children = True
         for salary in range(0, 100001, 10000):
             self.assertEqual(
                 social_security.calc_social_security(salary),
                 social_security.calc_social_security_by_integration(salary),
             )
 
     def test_get_rate_health_different_config(self):
-        config.EXTRA_HEALTH_INSURANCE = 0.015
+        config.extra_health_insurance = 0.015
         self.assertEqual(social_security.get_rate_health(0), 0)
         self.assertAlmostEqual(social_security.get_rate_health(10000), 0.0805)
         self.assertAlmostEqual(social_security.get_rate_health(58050), 0.0805)
         self.assertEqual(social_security.get_rate_health(58051), 0)
         self.assertEqual(social_security.get_rate_health(100000), 0)
 
     def test_get_rate_nursing(self):
-        config.HAS_CHILDREN = False
+        config.has_children = False
         self.assertEqual(social_security.get_rate_nursing(0), 0)
         self.assertEqual(social_security.get_rate_nursing(10000), 0.01875)
         self.assertEqual(social_security.get_rate_nursing(58050), 0.01875)
         self.assertEqual(social_security.get_rate_nursing(58051), 0)
         self.assertEqual(social_security.get_rate_nursing(100000), 0)
 
     def test_get_rate_nursing_different_config(self):
-        config.HAS_CHILDREN = True
+        config.has_children = True
         self.assertEqual(social_security.get_rate_nursing(0), 0)
         self.assertEqual(social_security.get_rate_nursing(10000), 0.01525)
         self.assertEqual(social_security.get_rate_nursing(58050), 0.01525)
         self.assertEqual(social_security.get_rate_nursing(58051), 0)
         self.assertEqual(social_security.get_rate_nursing(100000), 0)
```

### Comparing `netto-0.0.2/test/test_taxes_income.py` & `netto-0.1.0/test/test_taxes_income.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import netto.config as config
 import netto.taxes_income as taxes_income
 
 
 class TestTaxesIncome(unittest.TestCase):
     def setUp(self):
-        config.EXTRA_HEALTH_INSURANCE = 0.014
-        config.CHURCH_TAX = 0.09
-        config.HAS_CHILDREN = False
+        config.extra_health_insurance = 0.014
+        config.church_tax = 0.09
+        config.has_children = False
 
     def tearDown(self):
         pass
 
     def test_valid_get_marginal_tax_rate(self):
         self.assertEqual(taxes_income.get_marginal_tax_rate(-1000), 0)
         self.assertEqual(taxes_income.get_marginal_tax_rate(0), 0)
@@ -21,14 +21,32 @@
         self.assertEqual(taxes_income.get_marginal_tax_rate(14926), 0.2397)
         self.assertEqual(taxes_income.get_marginal_tax_rate(58596), 0.42)
         self.assertEqual(taxes_income.get_marginal_tax_rate(58597), 0.42)
         self.assertEqual(taxes_income.get_marginal_tax_rate(100000), 0.42)
         self.assertEqual(taxes_income.get_marginal_tax_rate(277826), 0.45)
         self.assertEqual(taxes_income.get_marginal_tax_rate(277827), 0.45)
 
+    def test_valid_get_marginal_tax_rate_married(self):
+        config.is_married = True
+        self.assertEqual(taxes_income.get_marginal_tax_rate(10346), 0)
+        self.assertEqual(taxes_income.get_marginal_tax_rate(10347), 0)
+        self.assertEqual(taxes_income.get_marginal_tax_rate(10346 * 2), 0)
+        self.assertEqual(taxes_income.get_marginal_tax_rate(10347 * 2), 0.14)
+        config.is_married = False
+
     def test_sameness_of_calc_income_tax_methods(self):
+        self.assertAlmostEqual(
+            taxes_income.calc_income_tax(12000),
+            taxes_income.calc_income_tax_by_integration(12000),
+            delta=0.1,
+        )
         for taxable_income in range(0, 100001, 10000):
             self.assertAlmostEqual(
                 taxes_income.calc_income_tax(taxable_income),
                 taxes_income.calc_income_tax_by_integration(taxable_income),
                 delta=0.1,
             )
+        self.assertAlmostEqual(
+            taxes_income.calc_income_tax(300000),
+            taxes_income.calc_income_tax_by_integration(300000),
+            delta=0.1,
+        )
```

### Comparing `netto-0.0.2/test/test_taxes_other.py` & `netto-0.1.0/test/test_taxes_other.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import netto.config as config
 import netto.taxes_other as taxes_other
 
 
 class TestTaxesOther(unittest.TestCase):
     def setUp(self):
-        config.EXTRA_HEALTH_INSURANCE = 0.014
-        config.CHURCH_TAX = 0.09
-        config.HAS_CHILDREN = False
+        config.extra_health_insurance = 0.014
+        config.church_tax = 0.09
+        config.has_children = False
 
     def tearDown(self):
         pass
 
     def test_valid_calc_soli(self):
         self.assertEqual(taxes_other.calc_soli(-1000), 0)
         self.assertEqual(taxes_other.calc_soli(0), 0)
```

