# Comparing `tmp/python_adjudicator-0.1.0.post0.tar.gz` & `tmp/python_adjudicator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_adjudicator-0.1.0.post0.tar", max compression
+gzip compressed data, was "python_adjudicator-0.1.1.tar", max compression
```

## Comparing `python_adjudicator-0.1.0.post0.tar` & `python_adjudicator-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      988 2023-05-19 08:45:58.545191 python_adjudicator-0.1.0.post0/LICENSE
--rw-r--r--   0        0        0     2560 2023-05-19 09:34:38.810342 python_adjudicator-0.1.0.post0/README.md
--rw-r--r--   0        0        0     1858 2023-05-19 09:36:05.134752 python_adjudicator-0.1.0.post0/pyproject.toml
--rw-r--r--   0        0        0     2019 2023-05-19 08:50:35.058438 python_adjudicator-0.1.0.post0/src/adjudicator/Cache.py
--rw-r--r--   0        0        0     3137 2023-05-19 08:50:35.058438 python_adjudicator-0.1.0.post0/src/adjudicator/Executor.py
--rw-r--r--   0        0        0      853 2023-05-16 21:13:35.338396 python_adjudicator-0.1.0.post0/src/adjudicator/HashSupport.py
--rw-r--r--   0        0        0     5211 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/Params.py
--rw-r--r--   0        0        0      892 2023-05-19 08:51:12.194651 python_adjudicator-0.1.0.post0/src/adjudicator/Params_test.py
--rw-r--r--   0        0        0     3687 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/Rule.py
--rw-r--r--   0        0        0      411 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/Rule_test.py
--rw-r--r--   0        0        0     3069 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/RulesEngine.py
--rw-r--r--   0        0        0     2652 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/RulesEngine_test.py
--rw-r--r--   0        0        0     3036 2023-05-19 08:50:35.090438 python_adjudicator-0.1.0.post0/src/adjudicator/RulesGraph.py
--rw-r--r--   0        0        0     2615 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/RulesGraph_test.py
--rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_adjudicator-0.1.0.post0/src/adjudicator/Signature.py
--rw-r--r--   0        0        0      688 2023-05-19 09:36:05.134752 python_adjudicator-0.1.0.post0/src/adjudicator/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-19 08:50:35.062438 python_adjudicator-0.1.0.post0/src/adjudicator/errors.py
--rw-r--r--   0        0        0        0 2023-05-19 08:45:58.549191 python_adjudicator-0.1.0.post0/src/adjudicator/py.typed
--rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 python_adjudicator-0.1.0.post0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-19 08:45:58.545191 python_adjudicator-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2560 2023-05-19 09:34:38.810342 python_adjudicator-0.1.1/README.md
+-rw-r--r--   0        0        0     1852 2023-05-19 09:52:38.123361 python_adjudicator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2019 2023-05-19 08:50:35.058438 python_adjudicator-0.1.1/src/adjudicator/Cache.py
+-rw-r--r--   0        0        0     3137 2023-05-19 08:50:35.058438 python_adjudicator-0.1.1/src/adjudicator/Executor.py
+-rw-r--r--   0        0        0     1530 2023-05-19 09:42:57.372585 python_adjudicator-0.1.1/src/adjudicator/HashSupport.py
+-rw-r--r--   0        0        0     5579 2023-05-19 09:50:25.658731 python_adjudicator-0.1.1/src/adjudicator/Params.py
+-rw-r--r--   0        0        0      892 2023-05-19 08:51:12.194651 python_adjudicator-0.1.1/src/adjudicator/Params_test.py
+-rw-r--r--   0        0        0     3687 2023-05-19 08:50:35.062438 python_adjudicator-0.1.1/src/adjudicator/Rule.py
+-rw-r--r--   0        0        0      411 2023-05-19 08:50:35.062438 python_adjudicator-0.1.1/src/adjudicator/Rule_test.py
+-rw-r--r--   0        0        0     4385 2023-05-19 09:51:54.739163 python_adjudicator-0.1.1/src/adjudicator/RulesEngine.py
+-rw-r--r--   0        0        0     2643 2023-05-19 09:37:37.623158 python_adjudicator-0.1.1/src/adjudicator/RulesEngine_test.py
+-rw-r--r--   0        0        0     3036 2023-05-19 08:50:35.090438 python_adjudicator-0.1.1/src/adjudicator/RulesGraph.py
+-rw-r--r--   0        0        0     2615 2023-05-19 08:50:35.062438 python_adjudicator-0.1.1/src/adjudicator/RulesGraph_test.py
+-rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_adjudicator-0.1.1/src/adjudicator/Signature.py
+-rw-r--r--   0        0        0      682 2023-05-19 09:52:38.123361 python_adjudicator-0.1.1/src/adjudicator/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-19 08:50:35.062438 python_adjudicator-0.1.1/src/adjudicator/errors.py
+-rw-r--r--   0        0        0        0 2023-05-19 08:45:58.549191 python_adjudicator-0.1.1/src/adjudicator/py.typed
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 python_adjudicator-0.1.1/PKG-INFO
```

### Comparing `python_adjudicator-0.1.0.post0/LICENSE` & `python_adjudicator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/README.md` & `python_adjudicator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/pyproject.toml` & `python_adjudicator-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-adjudicator"
-version = "0.1.0.post0"
+version = "0.1.1"
 description = ""
 authors = ["Unknown <me@unknown.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "adjudicator", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/Cache.py` & `python_adjudicator-0.1.1/src/adjudicator/Cache.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/Executor.py` & `python_adjudicator-0.1.1/src/adjudicator/Executor.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/Params.py` & `python_adjudicator-0.1.1/src/adjudicator/Params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Collection, Generic, KeysView, Mapping, Sequence, TypeAlias, TypeVar, cast, overload
+from typing import Any, Collection, Generic, Iterable, KeysView, Mapping, Sequence, TypeAlias, TypeVar, cast, overload
 
 from adjudicator.HashSupport import Hasher
 from adjudicator.Signature import Signature
 
 T = TypeVar("T")
 U = TypeVar("U")
 
@@ -92,14 +92,21 @@
     def __or__(self, params: Params) -> Params:
         """
         Merge two parameter sets, taking precedence of the parameters in the right hand side.
         """
 
         return Params({**self._params, **params._params}, self._hasher)
 
+    def __sub__(self, types: Collection[type[Any]]) -> Params:
+        """
+        Remove the parameters in the right hand side from the left hand side.
+        """
+
+        return Params({k: v for k, v in self._params.items() if k not in types}, self._hasher)
+
     def __len__(self) -> int:
         return len(self._params)
 
     def __bool__(self) -> bool:
         return bool(self._params)
 
     @overload
@@ -114,14 +121,17 @@
         try:
             return cast(T, self._params[param_type])
         except KeyError:
             if default is _Sentinel:
                 raise KeyError(f"Parameter of type {param_type} not found")
             return cast(U, default)
 
+    def items(self) -> Iterable[tuple[type[Any], object]]:
+        return self._params.items()
+
     def types(self) -> KeysView[type[Any]]:
         return self._params.keys()
 
     def filter(self, types: Collection[type[Any]], total: bool = False) -> Params:
         """
         Return a new Params instance containing only the parameters of the specified types.
         """
```

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/Params_test.py` & `python_adjudicator-0.1.1/src/adjudicator/Params_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/Rule.py` & `python_adjudicator-0.1.1/src/adjudicator/Rule.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/RulesEngine_test.py` & `python_adjudicator-0.1.1/src/adjudicator/RulesEngine_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,34 +64,34 @@
             Rule(
                 func=lambda p: int(p.get(bool)),
                 input_types={bool},
                 output_type=int,
                 id="r2",
             ),
         ],
-        subjects=[],
+        facts=[],
     )
 
     assert engine.get(int, Params(["42"])) == 42
     assert engine.get(int, Params([True])) == 1
     assert engine.get(int, Params([False])) == 0
 
 
-def test__RulesEngine__injects_subjects() -> None:
+def test__RulesEngine__injects_facts() -> None:
     @dataclass(frozen=True)
     class CustomType:
         v: int
 
     engine = RulesEngine(
         rules=[
             Rule(
                 func=lambda p: p.get(CustomType).v,
                 input_types={CustomType},
                 output_type=int,
                 id="r1",
             )
         ],
-        subjects=[CustomType(42)],
+        facts=[CustomType(42)],
     )
 
     assert engine.get(int, Params()) == 42
     assert engine.get(int, Params([CustomType(33)])) == 33
```

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/RulesGraph.py` & `python_adjudicator-0.1.1/src/adjudicator/RulesGraph.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/RulesGraph_test.py` & `python_adjudicator-0.1.1/src/adjudicator/RulesGraph_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/__init__.py` & `python_adjudicator-0.1.1/src/adjudicator/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     "rule",
     "Rule",
     "RuleResolveError",
     "RulesEngine",
     "RulesGraph",
 ]
 
-__version__ = "0.1.0.post0"
+__version__ = "0.1.1"
```

### Comparing `python_adjudicator-0.1.0.post0/src/adjudicator/errors.py` & `python_adjudicator-0.1.1/src/adjudicator/errors.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.1.0.post0/PKG-INFO` & `python_adjudicator-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adjudicator
-Version: 0.1.0.post0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Unknown
 Author-email: me@unknown.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

