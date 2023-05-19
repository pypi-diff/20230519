# Comparing `tmp/redcat-0.0.1.tar.gz` & `tmp/redcat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcat-0.0.1.tar", max compression
+gzip compressed data, was "redcat-0.0.2.tar", max compression
```

## Comparing `redcat-0.0.1.tar` & `redcat-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     1501 2023-05-18 08:42:29.653615 redcat-0.0.1/LICENSE
--rw-r--r--   0        0        0     2156 2023-05-18 08:42:29.653615 redcat-0.0.1/README.md
--rw-r--r--   0        0        0     4378 2023-05-18 08:42:29.653615 redcat-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      354 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/__init__.py
--rw-r--r--   0        0        0    17532 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/base.py
--rw-r--r--   0        0        0    16464 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/batchdict.py
--rw-r--r--   0        0        0     6626 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/batchlist.py
--rw-r--r--   0        0        0     2428 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/comparators.py
--rw-r--r--   0        0        0   140058 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/tensor.py
--rw-r--r--   0        0        0    50335 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/tensorseq.py
--rw-r--r--   0        0        0        0 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/utils/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/utils/format.py
--rw-r--r--   0        0        0     1446 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/utils/imports.py
--rw-r--r--   0        0        0    12069 2023-05-18 08:42:29.653615 redcat-0.0.1/src/redcat/utils/tensor.py
--rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 redcat-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-19 18:45:14.291732 redcat-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2156 2023-05-19 18:45:14.291732 redcat-0.0.2/README.md
+-rw-r--r--   0        0        0     4347 2023-05-19 18:45:14.291732 redcat-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/__init__.py
+-rw-r--r--   0        0        0    17532 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/base.py
+-rw-r--r--   0        0        0    16464 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/batchdict.py
+-rw-r--r--   0        0        0     6626 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/batchlist.py
+-rw-r--r--   0        0        0     2428 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/comparators.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/iter/__init__.py
+-rw-r--r--   0        0        0     4071 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/iter/batching.py
+-rw-r--r--   0        0        0     3729 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/iter/joining.py
+-rw-r--r--   0        0        0     2111 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/datapipes/iter/shuffling.py
+-rw-r--r--   0        0        0   140956 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/tensor.py
+-rw-r--r--   0        0        0    51250 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/tensorseq.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:45:14.291732 redcat-0.0.2/src/redcat/utils/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-19 18:45:14.295733 redcat-0.0.2/src/redcat/utils/format.py
+-rw-r--r--   0        0        0     1446 2023-05-19 18:45:14.295733 redcat-0.0.2/src/redcat/utils/imports.py
+-rw-r--r--   0        0        0    10154 2023-05-19 18:45:14.295733 redcat-0.0.2/src/redcat/utils/tensor.py
+-rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 redcat-0.0.2/PKG-INFO
```

### Comparing `redcat-0.0.1/LICENSE` & `redcat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1/README.md` & `redcat-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1/pyproject.toml` & `redcat-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "redcat"
-version = "0.0.1"
+version = "0.0.2"
 description = "A library to manipulate batches of examples"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/redcat"
 repository = "https://github.com/durandtibo/redcat"
 keywords = ["batch"]
 license = "BSD-3-Clause"
 
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -26,18 +26,18 @@
 
 packages = [
     { include = "redcat", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
-coola = "^0.0.7"
+coola = "^0.0, >=0.0.7"
+numpy = "^1.24"
 python = "^3.9"
-torch = "^2.0"  # make optional
-numpy = "^1.24"  # make optional
+torch = "^2.0"
 polars = { version = "^0.17", optional = true }
 
 [tool.poetry.extras]
 all = [
     "polars",
 ]
```

### Comparing `redcat-0.0.1/src/redcat/base.py` & `redcat-0.0.2/src/redcat/base.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1/src/redcat/batchdict.py` & `redcat-0.0.2/src/redcat/batchdict.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1/src/redcat/batchlist.py` & `redcat-0.0.2/src/redcat/batchlist.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1/src/redcat/comparators.py` & `redcat-0.0.2/src/redcat/comparators.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1/src/redcat/tensor.py` & `redcat-0.0.2/src/redcat/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
-__all__ = ["BatchedTensor", "check_data_and_dim"]
+__all__ = ["BatchedTensor", "check_data_and_dim", "check_batch_dims", "get_batch_dims"]
 
 import functools
-from collections.abc import Callable, Iterable, Sequence
+from collections.abc import Callable, Iterable, Mapping, Sequence
 from itertools import chain
 from typing import Any, TypeVar, Union, overload
 
 import torch
 from torch import Tensor
 
 from redcat.base import BaseBatch
-from redcat.utils.tensor import check_batch_dims, get_batch_dims, permute_along_dim
+from redcat.utils.tensor import permute_along_dim
 
 # Workaround because Self is not available for python 3.9 and 3.10
 # https://peps.python.org/pep-0673/
 TBatchedTensor = TypeVar("TBatchedTensor", bound="BatchedTensor")
 
 HANDLED_FUNCTIONS = {}
 
@@ -4009,14 +4009,43 @@
         raise RuntimeError(f"data needs at least 1 dimensions (received: {data.dim()})")
     if batch_dim < 0 or batch_dim >= data.dim():
         raise RuntimeError(
             f"Incorrect batch_dim ({batch_dim}) but the value should be in [0, {data.dim() - 1}]"
         )
 
 
+def check_batch_dims(dims: set[int]) -> None:
+    r"""Gets the batch dimensions from the inputs.
+
+    Args:
+        dims (set): Specifies the batch dims to check.
+
+    Raises:
+        RuntimeError if there are more than one batch dimension.
+    """
+    if len(dims) != 1:
+        raise RuntimeError(f"The batch dimensions do not match. Received multiple values: {dims}")
+
+
+def get_batch_dims(args: Iterable[Any], kwargs: Mapping[str, Any] | None = None) -> set[int]:
+    r"""Gets the batch dimensions from the inputs.
+
+    Args:
+        args: Variable length argument list.
+        kwargs: Arbitrary keyword arguments.
+
+    Returns:
+        set: The batch dimensions.
+    """
+    kwargs = kwargs or {}
+    dims = {val._batch_dim for val in args if hasattr(val, "_batch_dim")}
+    dims.update({val._batch_dim for val in kwargs.values() if hasattr(val, "_batch_dim")})
+    return dims
+
+
 def implements(torch_function: Callable) -> Callable:
     """Register a torch function override for BatchedTensor."""
 
     def decorator(func: Callable) -> Callable:
         functools.update_wrapper(func, torch_function)
         HANDLED_FUNCTIONS[torch_function] = func
         return func
```

### Comparing `redcat-0.0.1/src/redcat/tensorseq.py` & `redcat-0.0.2/src/redcat/tensorseq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from __future__ import annotations
 
-__all__ = ["BatchedTensorSeq", "check_data_and_dims"]
+__all__ = ["BatchedTensorSeq", "check_data_and_dims", "check_seq_dims", "get_seq_dims"]
 
 import functools
-from collections.abc import Callable, Iterable, Sequence
+from collections.abc import Callable, Iterable, Mapping, Sequence
 from typing import Any, overload
 
 import torch
 from torch import Tensor
 
 from redcat import BaseBatch, tensor
-from redcat.tensor import BatchedTensor
+from redcat.tensor import BatchedTensor, check_batch_dims, get_batch_dims
 from redcat.utils.tensor import (
     align_to_batch_seq,
     align_to_seq_batch,
-    check_batch_dims,
-    check_seq_dims,
     compute_batch_seq_permutation,
-    get_batch_dims,
-    get_seq_dims,
 )
 
 HANDLED_FUNCTIONS = {
     torch.max: tensor.torchmax,
     torch.mean: tensor.mean,
     torch.median: tensor.median,
     torch.min: tensor.torchmin,
@@ -1243,14 +1239,45 @@
         raise RuntimeError(
             f"Incorrect seq_dim ({seq_dim}) but the value should be in [0, {data.dim() - 1}]"
         )
     if batch_dim == seq_dim:
         raise RuntimeError(f"batch_dim ({batch_dim}) and seq_dim ({seq_dim}) have to be different")
 
 
+def check_seq_dims(dims: set[int]) -> None:
+    r"""Gets the sequence dimensions from the inputs.
+
+    Args:
+        dims (set): Specifies the sequence dims to check.
+
+    Raises:
+        RuntimeError if there are more than one sequence dimension.
+    """
+    if len(dims) != 1:
+        raise RuntimeError(
+            f"The sequence dimensions do not match. Received multiple values: {dims}"
+        )
+
+
+def get_seq_dims(args: Iterable[Any, ...], kwargs: Mapping[str, Any] | None = None) -> set[int]:
+    r"""Gets the sequence dimensions from the inputs.
+
+    Args:
+        args: Variable length argument list.
+        kwargs: Arbitrary keyword arguments.
+
+    Returns:
+        set: The sequence dimensions.
+    """
+    kwargs = kwargs or {}
+    dims = {val._seq_dim for val in args if hasattr(val, "_seq_dim")}
+    dims.update({val._seq_dim for val in kwargs.values() if hasattr(val, "_seq_dim")})
+    return dims
+
+
 def implements(torch_function: Callable) -> Callable:
     """Register a torch function override for BatchedTensor."""
 
     def decorator(func: Callable) -> Callable:
         functools.update_wrapper(func, torch_function)
         HANDLED_FUNCTIONS[torch_function] = func
         return func
```

### Comparing `redcat-0.0.1/src/redcat/utils/format.py` & `redcat-0.0.2/src/redcat/utils/format.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1/src/redcat/utils/imports.py` & `redcat-0.0.2/src/redcat/utils/imports.py`

 * *Files identical despite different names*

### Comparing `redcat-0.0.1/src/redcat/utils/tensor.py` & `redcat-0.0.2/src/redcat/utils/tensor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from __future__ import annotations
 
 __all__ = [
     "DeviceType",
     "align_to_batch_first",
     "align_to_batch_seq",
     "align_to_seq_batch",
-    "check_batch_dims",
-    "check_seq_dims",
     "compute_batch_seq_permutation",
     "get_available_devices",
-    "get_batch_dims",
-    "get_seq_dims",
     "get_torch_generator",
     "permute_along_dim",
     "swap2",
 ]
 
 import copy
-from collections.abc import Iterable, Mapping, MutableSequence
-from typing import Any, Union, overload
+from collections.abc import MutableSequence
+from typing import Union, overload
 
 import numpy as np
 import torch
 from torch import Tensor
 
 DeviceType = Union[torch.device, str, int]
 
@@ -111,42 +107,14 @@
             old_seq_dim=seq_dim,
             new_batch_dim=1,
             new_seq_dim=0,
         )
     )
 
 
-def check_batch_dims(dims: set[int]) -> None:
-    r"""Gets the batch dimensions from the inputs.
-
-    Args:
-        dims (set): Specifies the batch dims to check.
-
-    Raises:
-        RuntimeError if there are more than one batch dimension.
-    """
-    if len(dims) != 1:
-        raise RuntimeError(f"The batch dimensions do not match. Received multiple values: {dims}")
-
-
-def check_seq_dims(dims: set[int]) -> None:
-    r"""Gets the sequence dimensions from the inputs.
-
-    Args:
-        dims (set): Specifies the sequence dims to check.
-
-    Raises:
-        RuntimeError if there are more than one sequence dimension.
-    """
-    if len(dims) != 1:
-        raise RuntimeError(
-            f"The sequence dimensions do not match. Received multiple values: {dims}"
-        )
-
-
 def compute_batch_seq_permutation(
     num_dims: int,
     old_batch_dim: int,
     old_seq_dim: int,
     new_batch_dim: int,
     new_seq_dim: int,
 ) -> list[int]:
@@ -217,46 +185,14 @@
     if torch.cuda.is_available():
         return ("cpu", "cuda:0")
     if torch.backends.mps.is_available():
         return ("cpu", "mps:0")
     return ("cpu",)
 
 
-def get_batch_dims(args: Iterable[Any], kwargs: Mapping[str, Any] | None = None) -> set[int]:
-    r"""Gets the batch dimensions from the inputs.
-
-    Args:
-        args: Variable length argument list.
-        kwargs: Arbitrary keyword arguments.
-
-    Returns:
-        set: The batch dimensions.
-    """
-    kwargs = kwargs or {}
-    dims = {val._batch_dim for val in args if hasattr(val, "_batch_dim")}
-    dims.update({val._batch_dim for val in kwargs.values() if hasattr(val, "_batch_dim")})
-    return dims
-
-
-def get_seq_dims(args: Iterable[Any, ...], kwargs: Mapping[str, Any] | None = None) -> set[int]:
-    r"""Gets the sequence dimensions from the inputs.
-
-    Args:
-        args: Variable length argument list.
-        kwargs: Arbitrary keyword arguments.
-
-    Returns:
-        set: The sequence dimensions.
-    """
-    kwargs = kwargs or {}
-    dims = {val._seq_dim for val in args if hasattr(val, "_seq_dim")}
-    dims.update({val._seq_dim for val in kwargs.values() if hasattr(val, "_seq_dim")})
-    return dims
-
-
 def get_torch_generator(
     random_seed: int = 1, device: torch.device | str | None = "cpu"
 ) -> torch.Generator:
     r"""Creates a ``torch.Generator`` initialized with a given seed.
 
     Args:
     ----
```

### Comparing `redcat-0.0.1/PKG-INFO` & `redcat-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: redcat
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to manipulate batches of examples
 Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause
 Keywords: batch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
-Requires-Dist: coola (>=0.0.7,<0.0.8)
+Requires-Dist: coola (>=0.0.7,<0.1)
 Requires-Dist: numpy (>=1.24,<2.0)
 Requires-Dist: polars (>=0.17,<0.18) ; extra == "all"
 Requires-Dist: torch (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/durandtibo/redcat
 Description-Content-Type: text/markdown
 
 # redcat
```

#### html2text {}

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1 Name: redcat Version: 0.0.1 Summary: A library to
+Metadata-Version: 2.1 Name: redcat Version: 0.0.2 Summary: A library to
 manipulate batches of examples Home-page: https://github.com/durandtibo/redcat
 License: BSD-3-Clause Keywords: batch Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
+Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries Provides-Extra: all Requires-Dist: coola
-(>=0.0.7,<0.0.8) Requires-Dist: numpy (>=1.24,<2.0) Requires-Dist: polars
+(>=0.0.7,<0.1) Requires-Dist: numpy (>=1.24,<2.0) Requires-Dist: polars
 (>=0.17,<0.18) ; extra == "all" Requires-Dist: torch (>=2.0,<3.0) Project-URL:
 Repository, https://github.com/durandtibo/redcat Description-Content-Type:
 text/markdown # redcat
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  0987ab26fe4d52025085/maintainability] [https://api.codeclimate.com/v1/badges/
                      0987ab26fe4d52025085/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
```

