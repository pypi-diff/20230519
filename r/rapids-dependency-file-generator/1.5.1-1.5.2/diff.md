# Comparing `tmp/rapids-dependency-file-generator-1.5.1.tar.gz` & `tmp/rapids-dependency-file-generator-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids-dependency-file-generator-1.5.1.tar", last modified: Wed Mar  8 00:24:05 2023, max compression
+gzip compressed data, was "rapids-dependency-file-generator-1.5.2.tar", last modified: Fri May 19 13:36:37 2023, max compression
```

## Comparing `rapids-dependency-file-generator-1.5.1.tar` & `rapids-dependency-file-generator-1.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 00:24:05.274241 rapids-dependency-file-generator-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28348 2023-03-08 00:24:05.274241 rapids-dependency-file-generator-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 00:24:05.274241 rapids-dependency-file-generator-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 00:24:05.270241 rapids-dependency-file-generator-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 00:24:05.270241 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-08 00:23:56.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/rapids_dependency_file_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/rapids_dependency_file_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-03-08 00:23:56.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 00:24:05.270241 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28348 2023-03-08 00:24:05.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-08 00:24:05.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 00:24:05.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-08 00:24:05.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-08 00:24:05.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-08 00:24:05.000000 rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 00:24:05.274241 rapids-dependency-file-generator-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/tests/test_rapids_dependency_file_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-08 00:23:46.000000 rapids-dependency-file-generator-1.5.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:36:37.566235 rapids-dependency-file-generator-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28348 2023-05-19 13:36:37.566235 rapids-dependency-file-generator-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:36:37.566235 rapids-dependency-file-generator-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:36:37.562235 rapids-dependency-file-generator-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:36:37.562235 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 13:36:25.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/rapids_dependency_file_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/rapids_dependency_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-19 13:36:25.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:36:37.562235 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28348 2023-05-19 13:36:37.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-19 13:36:37.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:36:37.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 13:36:37.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 13:36:37.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 13:36:37.000000 rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:36:37.566235 rapids-dependency-file-generator-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/tests/test_rapids_dependency_file_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 13:36:15.000000 rapids-dependency-file-generator-1.5.2/tests/test_schema.py
```

### Comparing `rapids-dependency-file-generator-1.5.1/LICENSE` & `rapids-dependency-file-generator-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/PKG-INFO` & `rapids-dependency-file-generator-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids-dependency-file-generator
-Version: 1.5.1
+Version: 1.5.2
 Summary: Tool for generating RAPIDS environment files
 Author-email: RAPIDS Development Team <pypi@rapids.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rapids-dependency-file-generator-1.5.1/README.md` & `rapids-dependency-file-generator-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/pyproject.toml` & `rapids-dependency-file-generator-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/cli.py` & `rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/cli.py`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/constants.py` & `rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/constants.py`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/rapids_dependency_file_generator.py` & `rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/rapids_dependency_file_generator.py`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/rapids_dependency_file_validator.py` & `rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/rapids_dependency_file_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Logic for validating dependency files."""
 
 import json
+import sys
 import textwrap
 
 import jsonschema
 import pkg_resources
 from jsonschema.exceptions import best_match
 
 SCHEMA = json.loads(pkg_resources.resource_string(__name__, "schema.json"))
@@ -22,11 +23,13 @@
     ------
     jsonschema.exceptions.ValidationError
         If the dependencies do not conform to the schema
     """
     validator = jsonschema.Draft7Validator(SCHEMA)
     errors = list(validator.iter_errors(dependencies))
     if len(errors) > 0:
-        print("The provided dependency file contains schema errors.")
+        print("The provided dependency file contains schema errors.", file=sys.stderr)
         best_matching_error = best_match(errors)
-        print("\n", textwrap.indent(str(best_matching_error), "\t"), "\n")
+        print(
+            "\n", textwrap.indent(str(best_matching_error), "\t"), "\n", file=sys.stderr
+        )
         raise RuntimeError("The provided dependencies data is invalid.")
```

### Comparing `rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator/schema.json` & `rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator/schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/rapidsai/dependency-file-generator/v1.5.2/src/rapids_dependency_file_generator/schema.json'"}*

```diff
@@ -166,15 +166,15 @@
             "items": {
                 "$ref": "#/$defs/requirement"
             },
             "minItems": 1,
             "type": "array"
         }
     },
-    "$id": "https://raw.githubusercontent.com/rapidsai/dependency-file-generator/v1.5.1/src/rapids_dependency_file_generator/schema.json",
+    "$id": "https://raw.githubusercontent.com/rapidsai/dependency-file-generator/v1.5.2/src/rapids_dependency_file_generator/schema.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "description": "Consolidated specification of RAPIDS project dependencies",
     "properties": {
         "channels": {
             "$ref": "#/$defs/channels"
         },
```

### Comparing `rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/PKG-INFO` & `rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids-dependency-file-generator
-Version: 1.5.1
+Version: 1.5.2
 Summary: Tool for generating RAPIDS environment files
 Author-email: RAPIDS Development Team <pypi@rapids.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rapids-dependency-file-generator-1.5.1/src/rapids_dependency_file_generator.egg-info/SOURCES.txt` & `rapids-dependency-file-generator-1.5.2/src/rapids_dependency_file_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/tests/test_cli.py` & `rapids-dependency-file-generator-1.5.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/tests/test_examples.py` & `rapids-dependency-file-generator-1.5.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.5.1/tests/test_rapids_dependency_file_generator.py` & `rapids-dependency-file-generator-1.5.2/tests/test_rapids_dependency_file_generator.py`

 * *Files identical despite different names*

