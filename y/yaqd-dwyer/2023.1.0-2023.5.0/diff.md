# Comparing `tmp/yaqd-dwyer-2023.1.0.tar.gz` & `tmp/yaqd_dwyer-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaqd-dwyer-2023.1.0.tar", last modified: Fri Jan 27 22:24:27 2023, max compression
+gzip compressed data, was "yaqd_dwyer-2023.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `yaqd-dwyer-2023.1.0.tar` & `yaqd_dwyer-2023.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      426 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/.github/workflows/python-mypy.yml
--rw-r--r--   0        0        0      794 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      738 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/.github/workflows/run-entry-points.yml
--rw-r--r--   0        0        0      447 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/.gitignore
--rw-r--r--   0        0        0      659 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      614 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     7633 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/LICENSE
--rw-r--r--   0        0        0      840 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/README.md
--rw-r--r--   0        0        0     1253 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/pyproject.toml
--rw-r--r--   0        0        0        9 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/VERSION
--rw-r--r--   0        0        0       82 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/__init__.py
--rw-r--r--   0        0        0      493 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/__version__.py
--rw-r--r--   0        0        0     4968 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/_dwyer_16b.py
--rw-r--r--   0        0        0     2438 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/_dwyer_16c.py
--rw-r--r--   0        0        0    11079 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/dwyer-16b.avpr
--rw-r--r--   0        0        0     1093 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/dwyer-16b.toml
--rw-r--r--   0        0        0    10832 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/dwyer-16c.avpr
--rw-r--r--   0        0        0      901 2023-01-27 22:24:20.467901 yaqd-dwyer-2023.1.0/yaqd_dwyer/dwyer-16c.toml
--rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 yaqd-dwyer-2023.1.0/PKG-INFO
+-rw-r--r--   0        0        0      426 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/.github/workflows/python-mypy.yml
+-rw-r--r--   0        0        0      794 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      738 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/.github/workflows/run-entry-points.yml
+-rw-r--r--   0        0        0      447 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/.gitignore
+-rw-r--r--   0        0        0      658 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1102 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     7633 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/LICENSE
+-rw-r--r--   0        0        0      840 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/README.md
+-rw-r--r--   0        0        0      153 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/example-yaq-configs/dwyer-16b/simple.toml
+-rw-r--r--   0        0        0     1253 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/pyproject.toml
+-rw-r--r--   0        0        0        9 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/VERSION
+-rw-r--r--   0        0        0       82 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/__version__.py
+-rw-r--r--   0        0        0     7487 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/_dwyer_16b.py
+-rw-r--r--   0        0        0     2438 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/_dwyer_16c.py
+-rw-r--r--   0        0        0    17387 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/dwyer-16b.avpr
+-rw-r--r--   0        0        0     4762 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/dwyer-16b.toml
+-rw-r--r--   0        0        0    10832 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/dwyer-16c.avpr
+-rw-r--r--   0        0        0      901 2023-05-19 16:26:02.645993 yaqd_dwyer-2023.5.0/yaqd_dwyer/dwyer-16c.toml
+-rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 yaqd_dwyer-2023.5.0/PKG-INFO
```

### Comparing `yaqd-dwyer-2023.1.0/.github/workflows/python-publish.yml` & `yaqd_dwyer-2023.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yaqd-dwyer-2023.1.0/.github/workflows/run-entry-points.yml` & `yaqd_dwyer-2023.5.0/.github/workflows/run-entry-points.yml`

 * *Files identical despite different names*

### Comparing `yaqd-dwyer-2023.1.0/.pre-commit-config.yaml` & `yaqd_dwyer-2023.5.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
     hooks:
     -   id: trailing-whitespace
     -   id: check-toml
     -   id: no-commit-to-branch
         args: [-b, master]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
         entry: black
         require_serial: true
         types: [python]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.3.0
     hooks:
       - id: mypy
         exclude: ^docs/conf.py
 
   - repo: https://github.com/yaq-project/yaq-traits
     rev: v2022.11.0
     hooks:
```

### Comparing `yaqd-dwyer-2023.1.0/CHANGELOG.md` & `yaqd_dwyer-2023.5.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.5.0]
+
+### Added
+- 16b: temperature regulation value now exposed via properties
+
+### Fixed
+- 16b: added forgotten dictionarys converting parameters from config into minimalmodbus
+- 16b: broken ramping
+
+## [2023.3.0]
+
+### Added
+- 16b: extra properties for PID settings
+- 16b: now forces usage of PID profile 0 only
+
 ## [2023.1.0]
 
 ### Changed
 - now ramps are parametrized using time delay, not rate
 
 ### Fixed
 - various fixes from production involving infrequent error conditions
 
 ## [2022.7.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/yaq-project/yaqd-dwyer/compare/v2023.1.0...main
+[Unreleased]: https://github.com/yaq-project/yaqd-dwyer/compare/v2023.5.0...main
+[2023.5.0]: https://github.com/yaq-project/yaqd-dwyer/compare/v2023.3.0...2023.5.0
+[2023.3.0]: https://github.com/yaq-project/yaqd-dwyer/compare/v2023.1.0...2023.3.0
 [2023.1.0]: https://github.com/yaq-project/yaqd-dwyer/compare/v2022.7.0...2023.1.0
 [2022.7.0]: https://gihub.com/yaq-project/yaqd-dwyer/tags/v2022.7.0
-
```

### Comparing `yaqd-dwyer-2023.1.0/LICENSE` & `yaqd_dwyer-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaqd-dwyer-2023.1.0/README.md` & `yaqd_dwyer-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `yaqd-dwyer-2023.1.0/pyproject.toml` & `yaqd_dwyer-2023.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaqd-dwyer-2023.1.0/yaqd_dwyer/_dwyer_16c.py` & `yaqd_dwyer-2023.5.0/yaqd_dwyer/_dwyer_16c.py`

 * *Files identical despite different names*

### Comparing `yaqd-dwyer-2023.1.0/yaqd_dwyer/dwyer-16b.avpr` & `yaqd_dwyer-2023.5.0/yaqd_dwyer/dwyer-16c.avpr`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 {
     "config": {
         "baud_rate": {
             "origin": "uses-uart",
             "type": "int"
         },
+        "byte_size": {
+            "doc": "Byte size of your instrument.",
+            "type": "int"
+        },
         "enable": {
             "default": true,
             "doc": "Disable this daemon. The kind entry-point will not attempt to start this daemon.",
             "origin": "is-daemon",
             "type": "boolean"
         },
         "limits": {
@@ -49,14 +53,24 @@
             "default": null,
             "origin": "is-daemon",
             "type": [
                 "null",
                 "string"
             ]
         },
+        "modbus_address": {
+            "default": 1,
+            "doc": "Unique address in the modbus network.",
+            "type": "int"
+        },
+        "modbus_handle_echo": {
+            "default": true,
+            "doc": "Configure echo handling.",
+            "type": "boolean"
+        },
         "model": {
             "default": null,
             "origin": "is-daemon",
             "type": [
                 "null",
                 "string"
             ]
@@ -69,14 +83,27 @@
             "symbols": [
                 "closest",
                 "ignore",
                 "error"
             ],
             "type": "enum"
         },
+        "parity": {
+            "default": "none",
+            "doc": "Modbus parity.",
+            "type": {
+                "name": "parity",
+                "symbols": [
+                    "even",
+                    "odd",
+                    "none"
+                ],
+                "type": "enum"
+            }
+        },
         "port": {
             "doc": "TCP port for daemon to occupy.",
             "origin": "is-daemon",
             "type": "int"
         },
         "serial": {
             "default": null,
@@ -86,19 +113,32 @@
                 "null",
                 "string"
             ]
         },
         "serial_port": {
             "origin": "uses-uart",
             "type": "string"
+        },
+        "stop_bits": {
+            "default": "one",
+            "doc": "Number of stop bits.",
+            "type": {
+                "name": "stop_bits",
+                "symbols": [
+                    "one",
+                    "one_and_half",
+                    "two"
+                ],
+                "type": "enum"
+            }
         }
     },
     "doc": "",
     "hardware": [
-        "dwyer:16b"
+        "dwyer:16c"
     ],
     "installation": {
         "PyPI": "https://pypi.org/project/yaqd-dwyer"
     },
     "links": {
         "bugtracker": "https://gitlab.com/yaq-project/yaqd-dwyer/-/issues",
         "source": "https://github.com/yaq-project/yaqd-dwyer"
@@ -150,32 +190,14 @@
         },
         "get_position": {
             "doc": "Get current daemon position.",
             "origin": "has-position",
             "request": [],
             "response": "double"
         },
-        "get_ramp_time": {
-            "doc": "Ramp time, in minutes.",
-            "request": [],
-            "response": "double"
-        },
-        "get_ramp_time_limits": {
-            "doc": "Ramp time limits in minutes.",
-            "request": [],
-            "response": {
-                "items": "double",
-                "type": "array"
-            }
-        },
-        "get_ramp_time_units": {
-            "doc": "Ramp time units.",
-            "request": [],
-            "response": "string"
-        },
         "get_state": {
             "doc": "Get version of the running daemon",
             "origin": "is-daemon",
             "request": [],
             "response": "string"
         },
         "get_units": {
@@ -217,24 +239,14 @@
                 {
                     "name": "position",
                     "type": "double"
                 }
             ],
             "response": "null"
         },
-        "set_ramp_time": {
-            "doc": "Ramp time, in minutes. Set to zero to disable ramping.",
-            "request": [
-                {
-                    "name": "ramp_time",
-                    "type": "float"
-                }
-            ],
-            "response": "null"
-        },
         "set_relative": {
             "doc": "Give the daemon a new destination relative to its current position. Daemon will immediately begin motion towards new destination. Returns new destination.",
             "origin": "has-position",
             "request": [
                 {
                     "name": "distance",
                     "type": "double"
@@ -273,28 +285,17 @@
             "getter": "get_position",
             "limits_getter": "get_limits",
             "options_getter": null,
             "record_kind": "data",
             "setter": null,
             "type": "double",
             "units_getter": "get_units"
-        },
-        "ramp_time": {
-            "control_kind": "hinted",
-            "dynamic": true,
-            "getter": "get_ramp_time",
-            "limits_getter": "get_ramp_time_limits",
-            "options_getter": null,
-            "record_kind": "metadata",
-            "setter": "set_ramp_time",
-            "type": "float",
-            "units_getter": "get_ramp_time_units"
         }
     },
-    "protocol": "dwyer-16b",
+    "protocol": "dwyer-16c",
     "requires": [],
     "state": {
         "destination": {
             "default": NaN,
             "origin": "has-position",
             "type": "double"
         },
@@ -307,19 +308,14 @@
             "origin": "has-limits",
             "type": "array"
         },
         "position": {
             "default": NaN,
             "origin": "has-position",
             "type": "double"
-        },
-        "ramp_time": {
-            "default": 0.0,
-            "doc": "Ramp time, in minutes.",
-            "type": "double"
         }
     },
     "traits": [
         "has-limits",
         "has-position",
         "is-daemon",
         "uses-serial",
```

### Comparing `yaqd-dwyer-2023.1.0/yaqd_dwyer/dwyer-16c.toml` & `yaqd_dwyer-2023.5.0/yaqd_dwyer/dwyer-16c.toml`

 * *Files identical despite different names*

### Comparing `yaqd-dwyer-2023.1.0/PKG-INFO` & `yaqd_dwyer-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaqd-dwyer
-Version: 2023.1.0
+Version: 2023.5.0
 Summary: yaq daemons for Dwyer instruments & controllers
 Home-page: https://yaq.fyi
 Author: yaq developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

