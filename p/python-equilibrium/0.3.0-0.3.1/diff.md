# Comparing `tmp/python_equilibrium-0.3.0.tar.gz` & `tmp/python_equilibrium-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.3.0.tar", max compression
+gzip compressed data, was "python_equilibrium-0.3.1.tar", max compression
```

## Comparing `python_equilibrium-0.3.0.tar` & `python_equilibrium-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/LICENSE
--rw-r--r--   0        0        0     1648 2023-05-16 21:42:27.224180 python_equilibrium-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-16 21:42:27.224180 python_equilibrium-0.3.0/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/py.typed
--rw-r--r--   0        0        0      741 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/AdmissionController.py
--rw-r--r--   0        0        0     8497 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/CrudResourceController.py
--rw-r--r--   0        0        0    12910 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/JsonResourceStore.py
--rw-r--r--   0        0        0     8298 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/JsonResourceStore_test.py
--rw-r--r--   0        0        0      616 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/Namespace.py
--rw-r--r--   0        0        0    13234 2023-05-16 21:15:49.967795 python_equilibrium-0.3.0/src/equilibrium/resource/Resource.py
--rw-r--r--   0        0        0    15490 2023-05-16 21:33:14.798476 python_equilibrium-0.3.0/src/equilibrium/resource/ResourceContext.py
--rw-r--r--   0        0        0      500 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/ResourceController.py
--rw-r--r--   0        0        0     4849 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/ResourceStore.py
--rw-r--r--   0        0        0     2198 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/resource/Resource_test.py
--rw-r--r--   0        0        0     3046 2023-05-16 21:27:19.982844 python_equilibrium-0.3.0/src/equilibrium/resource/Service.py
--rw-r--r--   0        0        0      989 2023-05-16 21:27:24.034885 python_equilibrium-0.3.0/src/equilibrium/resource/__init__.py
--rw-r--r--   0        0        0     2031 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Cache.py
--rw-r--r--   0        0        0     3161 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Executor.py
--rw-r--r--   0        0        0      853 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/HashSupport.py
--rw-r--r--   0        0        0     5223 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Params.py
--rw-r--r--   0        0        0      898 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Params_test.py
--rw-r--r--   0        0        0     3699 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Rule.py
--rw-r--r--   0        0        0      417 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Rule_test.py
--rw-r--r--   0        0        0     3111 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/RulesEngine.py
--rw-r--r--   0        0        0     2682 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/RulesEngine_test.py
--rw-r--r--   0        0        0     3054 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/RulesGraph.py
--rw-r--r--   0        0        0     2639 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/RulesGraph_test.py
--rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/Signature.py
--rw-r--r--   0        0        0      689 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/__init__.py
--rw-r--r--   0        0        0     1415 2023-05-16 21:13:35.338396 python_equilibrium-0.3.0/src/equilibrium/rules/errors.py
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 python_equilibrium-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1740 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/README.md
+-rw-r--r--   0        0        0     1669 2023-05-19 08:34:15.489955 python_equilibrium-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-19 08:34:15.489955 python_equilibrium-0.3.1/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/py.typed
+-rw-r--r--   0        0        0      741 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/resource/AdmissionController.py
+-rw-r--r--   0        0        0     8497 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/resource/CrudResourceController.py
+-rw-r--r--   0        0        0    12910 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/resource/JsonResourceStore.py
+-rw-r--r--   0        0        0     8298 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/resource/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      616 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/resource/Namespace.py
+-rw-r--r--   0        0        0    13234 2023-05-16 21:15:49.967795 python_equilibrium-0.3.1/src/equilibrium/resource/Resource.py
+-rw-r--r--   0        0        0    15490 2023-05-16 21:33:14.798476 python_equilibrium-0.3.1/src/equilibrium/resource/ResourceContext.py
+-rw-r--r--   0        0        0      500 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/resource/ResourceController.py
+-rw-r--r--   0        0        0     4849 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/resource/ResourceStore.py
+-rw-r--r--   0        0        0     2198 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/resource/Resource_test.py
+-rw-r--r--   0        0        0     3046 2023-05-16 21:27:19.982844 python_equilibrium-0.3.1/src/equilibrium/resource/Service.py
+-rw-r--r--   0        0        0      989 2023-05-16 21:27:24.034885 python_equilibrium-0.3.1/src/equilibrium/resource/__init__.py
+-rw-r--r--   0        0        0     2031 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/Cache.py
+-rw-r--r--   0        0        0     3161 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/Executor.py
+-rw-r--r--   0        0        0      853 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/HashSupport.py
+-rw-r--r--   0        0        0     5223 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/Params.py
+-rw-r--r--   0        0        0      898 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/Params_test.py
+-rw-r--r--   0        0        0     3699 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/Rule.py
+-rw-r--r--   0        0        0      417 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/Rule_test.py
+-rw-r--r--   0        0        0     3111 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/RulesEngine.py
+-rw-r--r--   0        0        0     2682 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/RulesEngine_test.py
+-rw-r--r--   0        0        0     3054 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/RulesGraph.py
+-rw-r--r--   0        0        0     2639 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/RulesGraph_test.py
+-rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/Signature.py
+-rw-r--r--   0        0        0      689 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/__init__.py
+-rw-r--r--   0        0        0     1415 2023-05-16 21:13:35.338396 python_equilibrium-0.3.1/src/equilibrium/rules/errors.py
+-rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 python_equilibrium-0.3.1/PKG-INFO
```

### Comparing `python_equilibrium-0.3.0/LICENSE` & `python_equilibrium-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/pyproject.toml` & `python_equilibrium-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
+readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/python-equilibrium/issues"
 # Documentation = ""
```

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/AdmissionController.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/AdmissionController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/CrudResourceController.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/JsonResourceStore.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/JsonResourceStore_test.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/Namespace.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/Resource.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/Resource.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/ResourceContext.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/ResourceContext.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/ResourceStore.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/Resource_test.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/Service.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/resource/__init__.py` & `python_equilibrium-0.3.1/src/equilibrium/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/Cache.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/Cache.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/Executor.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/Executor.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/HashSupport.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/HashSupport.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/Params.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/Params.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/Params_test.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/Params_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/Rule.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/Rule.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/RulesEngine.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/RulesEngine.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/RulesEngine_test.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/RulesEngine_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/RulesGraph.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/RulesGraph.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/RulesGraph_test.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/RulesGraph_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/__init__.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.3.0/src/equilibrium/rules/errors.py` & `python_equilibrium-0.3.1/src/equilibrium/rules/errors.py`

 * *Files identical despite different names*

