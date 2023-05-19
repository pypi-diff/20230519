# Comparing `tmp/einsum_pipe-0.2.0.tar.gz` & `tmp/einsum_pipe-0.2.1.tar.gz`

## Comparing `einsum_pipe-0.2.0.tar` & `einsum_pipe-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/src/einsum_pipe/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/src/einsum_pipe/bidict.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/src/einsum_pipe/einsum_pipe.py
--rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/src/einsum_pipe/einsum_script.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/src/einsum_pipe/ops.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/tests/test_einsum_pipe.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/tests/test_ops.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/LICENSE
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 einsum_pipe-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/bidict.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/einsum_pipe.py
+-rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/einsum_script.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/src/einsum_pipe/ops.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/tests/test_einsum_pipe.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/tests/test_ops.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 einsum_pipe-0.2.1/PKG-INFO
```

### Comparing `einsum_pipe-0.2.0/src/einsum_pipe/bidict.py` & `einsum_pipe-0.2.1/src/einsum_pipe/bidict.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.0/src/einsum_pipe/einsum_pipe.py` & `einsum_pipe-0.2.1/src/einsum_pipe/einsum_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,24 @@
         output_script.simplify()
     elif simplify:
         output_script.simplify(input_shapes)
     return output_script, output_shape
 
 
 @overload
-def einsum_pipe(*args, simplify=True, **kwargs): ...
+def einsum_pipe(*args, simplify=True, **kwargs) -> np.ndarray: ...
 
 
 @overload
 def einsum_pipe(*args, simplify=True,
-                script: EinsumScript, output_shape: Tuple[int, ...], **kwargs): ...
+                script: EinsumScript, output_shape: Tuple[int, ...], **kwargs) -> np.ndarray: ...
 
 
 def einsum_pipe(*args, simplify=True,
-                script: Optional[EinsumScript] = None, output_shape: Optional[Tuple[int, ...]] = None, **kwargs):
+                script: Optional[EinsumScript] = None, output_shape: Optional[Tuple[int, ...]] = None, **kwargs) -> np.ndarray:
     assert (script is None and output_shape is None) or (
         script is not None and output_shape is not None)
     subs = []
     ops: List[np.ndarray] = []
     for arg in args:
         if isinstance(arg, (str, list, tuple)) or callable(arg):
             if isinstance(arg, list) and not isinstance(arg[0], int):
```

### Comparing `einsum_pipe-0.2.0/src/einsum_pipe/einsum_script.py` & `einsum_pipe-0.2.1/src/einsum_pipe/einsum_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
 import copy
 import math
-from typing import Generator, List, Optional, Self, Tuple, TypeVar, Union, cast
+from typing import Generator, List, Optional, Tuple, TypeVar, Union, cast
 from .bidict import _BiDict
 
 
 class EinsumComp:
     def __init__(self, size: int) -> None:
         self.size = size
 
@@ -21,15 +22,15 @@
 class EinsumScript:
     def __init__(self, inputs: List[List[EinsumComp]], outputs: List[EinsumComp]) -> None:
         self.inputs = inputs
         self.outputs = outputs
         self._parsed_script: Optional[str] = None
 
     @classmethod
-    def parse(cls, input_shapes: List[List[int]], subscripts: str) -> Self:
+    def parse(cls, input_shapes: List[List[int]], subscripts: str) -> EinsumScript:
         parsed_subscripts = subscripts
         subscripts = subscripts.replace(' ', '')
         # Easier to deal with broadcasting as a single character
         subscripts = subscripts.replace('...', '?')
         # The broadcasting character is automatically sorted to the start
         letters = sorted(subscripts.replace(',', '').replace('->', ''))
         if '->' not in subscripts:
@@ -165,15 +166,15 @@
                         else:
                             self.split_comp(inp_in_val, [
                                 inp_in_val.size // input_shape_val, input_shape_val])
                             input_shape_val = next(input_shape_iter)
                 except StopIteration:
                     pass
 
-    def simplified(self, keep_shape: Optional[List[Tuple[int, ...]]] = None) -> Self:
+    def simplified(self, keep_shape: Optional[List[Tuple[int, ...]]] = None) -> EinsumScript:
         val = copy.deepcopy(self)
         val.simplify(keep_shape)
         return val
 
     def __repr__(self) -> str:
         if self._parsed_script is None:
             return f'"{self}"'
@@ -188,15 +189,15 @@
             subs.append(''.join(_get_char(comps.index(comp)) for comp in inp))
 
         output_str = ''.join(_get_char(comps.index(comp))
                              for comp in self.outputs)
 
         return ','.join(subs) + '->' + output_str
 
-    def __add__(self, rhs: Self) -> Self:
+    def __add__(self, rhs: EinsumScript) -> EinsumScript:
         lhs = copy.deepcopy(self)
         rhs = copy.deepcopy(rhs)
         lhs_out_iter = rev_mut_iter(lhs.outputs)
         rhs_in_iter = rev_mut_iter(rhs.inputs[0])
 
         try:
             lhs_out_val = next(lhs_out_iter)
@@ -213,14 +214,17 @@
                 else:
                     rhs.split_comp(rhs_in_val, [
                         rhs_in_val.size // lhs_out_val.size, lhs_out_val.size])
                     lhs_out_val = next(lhs_out_iter)
         except StopIteration:
             pass
 
+        rhs.remove_ones()
+        lhs.remove_ones()
+
         assert len(lhs.outputs) == len(
             rhs.inputs[0]), f'Incompatible shapes between {repr(lhs)} and {repr(rhs)}: {lhs.output_shape} and {rhs.input_shapes[0]}'
         assert all(x.size == y.size for x, y in zip(
             lhs.outputs, rhs.inputs[0]))
 
         for i, x in enumerate(rhs.inputs[0]):
             val = lhs.outputs[i]
```

### Comparing `einsum_pipe-0.2.0/src/einsum_pipe/ops.py` & `einsum_pipe-0.2.1/src/einsum_pipe/ops.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.0/tests/test_einsum_pipe.py` & `einsum_pipe-0.2.1/tests/test_einsum_pipe.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.0/tests/test_ops.py` & `einsum_pipe-0.2.1/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.0/LICENSE` & `einsum_pipe-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.0/README.md` & `einsum_pipe-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `einsum_pipe-0.2.0/pyproject.toml` & `einsum_pipe-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "einsum_pipe"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="David Armstrong" },
 ]
 description = "A Python package to compile multiple Numpy einsum operations into one"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `einsum_pipe-0.2.0/PKG-INFO` & `einsum_pipe-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einsum_pipe
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package to compile multiple Numpy einsum operations into one
 Project-URL: Homepage, https://github.com/davystrong/Einsum-Pipe
 Project-URL: Bug Tracker, https://github.com/davystrong/Einsum-Pipe/issues
 Author: David Armstrong
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

