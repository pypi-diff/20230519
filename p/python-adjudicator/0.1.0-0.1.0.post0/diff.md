# Comparing `tmp/python_adjudicator-0.1.0.tar.gz` & `tmp/python_adjudicator-0.1.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_adjudicator-0.1.0.tar", max compression
+gzip compressed data, was "python_adjudicator-0.1.0.post0.tar", max compression
```

## Comparing `python_adjudicator-0.1.0.tar` & `python_adjudicator-0.1.0.post0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      988 2023-05-19 08:45:58.545191 python_adjudicator-0.1.0/LICENSE
--rw-r--r--   0        0        0     2560 2023-05-19 09:34:38.810342 python_adjudicator-0.1.0/README.md
--rw-r--r--   0        0        0     1689 2023-05-19 09:35:26.946560 python_adjudicator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2019 2023-05-19 08:50:35.058438 python_adjudicator-0.1.0/src/adjudicator/Cache.py
--rw-r--r--   0        0        0     3137 2023-05-19 08:50:35.058438 python_adjudicator-0.1.0/src/adjudicator/Executor.py
--rw-r--r--   0        0        0      853 2023-05-16 21:13:35.338396 python_adjudicator-0.1.0/src/adjudicator/HashSupport.py
--rw-r--r--   0        0        0     5211 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0/src/adjudicator/Params.py
--rw-r--r--   0        0        0      892 2023-05-19 08:51:12.194651 python_adjudicator-0.1.0/src/adjudicator/Params_test.py
--rw-r--r--   0        0        0     3687 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0/src/adjudicator/Rule.py
--rw-r--r--   0        0        0      411 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0/src/adjudicator/Rule_test.py
--rw-r--r--   0        0        0     3069 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0/src/adjudicator/RulesEngine.py
--rw-r--r--   0        0        0     2652 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0/src/adjudicator/RulesEngine_test.py
--rw-r--r--   0        0        0     3036 2023-05-19 08:50:35.090438 python_adjudicator-0.1.0/src/adjudicator/RulesGraph.py
--rw-r--r--   0        0        0     2615 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0/src/adjudicator/RulesGraph_test.py
--rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_adjudicator-0.1.0/src/adjudicator/Signature.py
--rw-r--r--   0        0        0      682 2023-05-19 09:35:26.946560 python_adjudicator-0.1.0/src/adjudicator/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0/src/adjudicator/errors.py
--rw-r--r--   0        0        0        0 2023-05-19 08:45:58.549191 python_adjudicator-0.1.0/src/adjudicator/py.typed
--rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 python_adjudicator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-19 08:45:58.545191 python_adjudicator-0.1.0.post0/LICENSE
+-rw-r--r--   0        0        0     2560 2023-05-19 09:34:38.810342 python_adjudicator-0.1.0.post0/README.md
+-rw-r--r--   0        0        0     1858 2023-05-19 09:36:05.134752 python_adjudicator-0.1.0.post0/pyproject.toml
+-rw-r--r--   0        0        0     2019 2023-05-19 08:50:35.058438 python_adjudicator-0.1.0.post0/src/adjudicator/Cache.py
+-rw-r--r--   0        0        0     3137 2023-05-19 08:50:35.058438 python_adjudicator-0.1.0.post0/src/adjudicator/Executor.py
+-rw-r--r--   0        0        0      853 2023-05-16 21:13:35.338396 python_adjudicator-0.1.0.post0/src/adjudicator/HashSupport.py
+-rw-r--r--   0        0        0     5211 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/Params.py
+-rw-r--r--   0        0        0      892 2023-05-19 08:51:12.194651 python_adjudicator-0.1.0.post0/src/adjudicator/Params_test.py
+-rw-r--r--   0        0        0     3687 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/Rule.py
+-rw-r--r--   0        0        0      411 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/Rule_test.py
+-rw-r--r--   0        0        0     3069 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/RulesEngine.py
+-rw-r--r--   0        0        0     2652 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/RulesEngine_test.py
+-rw-r--r--   0        0        0     3036 2023-05-19 08:50:35.090438 python_adjudicator-0.1.0.post0/src/adjudicator/RulesGraph.py
+-rw-r--r--   0        0        0     2615 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/RulesGraph_test.py
+-rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_adjudicator-0.1.0.post0/src/adjudicator/Signature.py
+-rw-r--r--   0        0        0      688 2023-05-19 09:36:05.134752 python_adjudicator-0.1.0.post0/src/adjudicator/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/errors.py
+-rw-r--r--   0        0        0        0 2023-05-19 08:45:58.549191 python_adjudicator-0.1.0.post0/src/adjudicator/py.typed
+-rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 python_adjudicator-0.1.0.post0/PKG-INFO
```

### Comparing `python_adjudicator-0.1.0/LICENSE` & `python_adjudicator-0.1.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/README.md` & `python_adjudicator-0.1.0.post0/README.md`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/pyproject.toml` & `python_adjudicator-0.1.0.post0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-adjudicator"
-version = "0.1.0"
+version = "0.1.0.post0"
 description = ""
 authors = ["Unknown <me@unknown.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "adjudicator", from = "src" }]
 classifiers = []
 keywords = []
 
 [tool.poetry.urls]
-# "Bug Tracker" = ""
+"Bug Tracker" = "https://github.com/NiklasRosenstein/python-adjudicator/issues"
 # Documentation = ""
-# Homepage = ""
-# Repository = ""
+Homepage = "https://github.com/NiklasRosenstein/python-adjudicator"
+Repository = "https://github.com/NiklasRosenstein/python-adjudicator"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 networkx = "^3.1"
 typeapi = "^1.4.2"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `python_adjudicator-0.1.0/src/adjudicator/Cache.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/Cache.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/Executor.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/Executor.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/HashSupport.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/HashSupport.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/Params.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/Params.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/Params_test.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/Params_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/Rule.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/Rule.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/RulesEngine.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/RulesEngine.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/RulesEngine_test.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/RulesEngine_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/RulesGraph.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/RulesGraph.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/RulesGraph_test.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/RulesGraph_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/src/adjudicator/__init__.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     "rule",
     "Rule",
     "RuleResolveError",
     "RulesEngine",
     "RulesGraph",
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.0.post0"
```

### Comparing `python_adjudicator-0.1.0/src/adjudicator/errors.py` & `python_adjudicator-0.1.0.post0/src/adjudicator/errors.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0/PKG-INFO` & `python_adjudicator-0.1.0.post0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: python-adjudicator
-Version: 0.1.0
+Version: 0.1.0.post0
 Summary: 
 License: MIT
 Author: Unknown
 Author-email: me@unknown.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: typeapi (>=1.4.2,<2.0.0)
+Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-adjudicator/issues
+Project-URL: Homepage, https://github.com/NiklasRosenstein/python-adjudicator
+Project-URL: Repository, https://github.com/NiklasRosenstein/python-adjudicator
 Description-Content-Type: text/markdown
 
 # adjudicator
 
 > __Adjudicator__ _(nount_): An adjudicator is a person or body that makes formal judgments on a disputed matter. They
 > are the ones who settle disputes or decide who is right in a disagreement. This could be a judge in a courtroom, an
 > arbitrator in a negotiation, or any person or system given the power to make decisions of this type.
```

