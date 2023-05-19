# Comparing `tmp/cssfinder_backend_numpy-0.4.0.tar.gz` & `tmp/cssfinder_backend_numpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssfinder_backend_numpy-0.4.0.tar", max compression
+gzip compressed data, was "cssfinder_backend_numpy-0.5.0.tar", max compression
```

## Comparing `cssfinder_backend_numpy-0.4.0.tar` & `cssfinder_backend_numpy-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6342 2023-04-27 17:47:58.937753 cssfinder_backend_numpy-0.4.0/README.md
--rw-r--r--   0        0        0     1104 2023-04-27 17:47:58.937753 cssfinder_backend_numpy-0.4.0/build.py
--rw-r--r--   0        0        0     2557 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/__init__.py
--rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/__init__.py
--rw-r--r--   0        0        0    13392 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/_complex128.py
--rw-r--r--   0        0        0    13432 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/_complex64.py
--rw-r--r--   0        0        0    11378 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/base.py
--rw-r--r--   0        0        0     3534 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/complex128.py
--rw-r--r--   0        0        0     3499 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/complex64.py
--rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/cython/__init__.py
--rw-r--r--   0        0        0     8266 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/impl.py
--rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/__init__.py
--rw-r--r--   0        0        0    13392 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/_complex128.py
--rw-r--r--   0        0        0    13432 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/_complex64.py
--rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/__init__.py
--rw-r--r--   0        0        0    16988 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/_complex128.py
--rw-r--r--   0        0        0    16964 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/_complex64.py
--rw-r--r--   0        0        0     1241 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/__init__.py
--rw-r--r--   0        0        0    14359 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/_complex128.py
--rw-r--r--   0        0        0    14399 2023-04-27 17:47:58.941753 cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/_complex64.py
--rw-r--r--   0        0        0    16962 2023-04-27 17:47:58.945753 cssfinder_backend_numpy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7171 1970-01-01 00:00:00.000000 cssfinder_backend_numpy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6342 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/README.md
+-rw-r--r--   0        0        0     1104 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/build.py
+-rw-r--r--   0        0        0     2557 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/_cython/__init__.py
+-rw-r--r--   0        0        0    16121 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/_cython/_complex128.py
+-rw-r--r--   0        0        0    16155 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/_cython/_complex64.py
+-rw-r--r--   0        0        0    12353 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/base.py
+-rw-r--r--   0        0        0     3534 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/complex128.py
+-rw-r--r--   0        0        0     3499 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/complex64.py
+-rw-r--r--   0        0        0     1241 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/cython/__init__.py
+-rw-r--r--   0        0        0     9201 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/impl.py
+-rw-r--r--   0        0        0     1241 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy/__init__.py
+-rw-r--r--   0        0        0    16121 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy/_complex128.py
+-rw-r--r--   0        0        0    16155 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy/_complex64.py
+-rw-r--r--   0        0        0     1241 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_debug/__init__.py
+-rw-r--r--   0        0        0    19931 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_debug/_complex128.py
+-rw-r--r--   0        0        0    19898 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_debug/_complex64.py
+-rw-r--r--   0        0        0     1241 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_jit/__init__.py
+-rw-r--r--   0        0        0    17216 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_jit/_complex128.py
+-rw-r--r--   0        0        0    17250 2023-05-19 12:47:33.081342 cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_jit/_complex64.py
+-rw-r--r--   0        0        0    16887 2023-05-19 12:47:33.085342 cssfinder_backend_numpy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7171 1970-01-01 00:00:00.000000 cssfinder_backend_numpy-0.5.0/PKG-INFO
```

### Comparing `cssfinder_backend_numpy-0.4.0/README.md` & `cssfinder_backend_numpy-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -67,36 +67,36 @@
 
 ```
 poe build
 ```
 
 ![poe_build](https://user-images.githubusercontent.com/56170852/223251363-61fc4d00-68ad-429c-9fbb-8ab7f4712451.png)
 
-This will create `dist/` directory with `cssfinder_backend_numpy-0.4.0` or
+This will create `dist/` directory with `cssfinder_backend_numpy-0.5.0` or
 alike inside.
 
 Wheel file can be installed with
 
 ```
-pip install ./dist/cssfinder_backend_numpy-0.4.0
+pip install ./dist/cssfinder_backend_numpy-0.5.0
 ```
 
 What you expect is
 
 ```
-Successfully installed cssfinder_backend_numpy-0.4.0
+Successfully installed cssfinder_backend_numpy-0.5.0
 ```
 
 or rather something like
 
 ```
-Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder_backend_numpy-0.4.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
+Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder_backend_numpy-0.5.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
 ```
 
-But `cssfinder_backend_numpy-0.4.0` should be included in this list.
+But `cssfinder_backend_numpy-0.5.0` should be included in this list.
 
 ## Code quality
 
 To ensure that all code follow same style guidelines and code quality rules,
 multiple static analysis tools are used. For simplicity, all of them are
 configured as `pre-commit` ([learn about pre-commit](https://pre-commit.com/))
 hooks. Most of them however are listed as development dependencies.
```

### Comparing `cssfinder_backend_numpy-0.4.0/build.py` & `cssfinder_backend_numpy-0.5.0/build.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/__init__.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from cssfinder_backend_numpy.complex64 import NumPyC64, NumPyC64Debug, NumPyC64Jit
 from cssfinder_backend_numpy.complex128 import HAS_CYTHON as HAS_CYTHON_128
 from cssfinder_backend_numpy.complex128 import NumPyC128, NumPyC128Debug, NumPyC128Jit
 
 if TYPE_CHECKING:
     from cssfinder.algorithm.backend import BackendBase
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 
 def export_backend() -> dict[tuple[str, Precision], BackendBase]:
     """Export mapping of available backends in this package."""
     backends = {
         ("numpy_jit", Precision.SINGLE): NumPyC64Jit,
         ("numpy_jit", Precision.DOUBLE): NumPyC128Jit,
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/__init__.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/_cython/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/_complex128.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_jit/_complex128.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
+from numba import jit, types  # type: ignore[attr-defined]
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
 
 #    █████  ██████  ███    ███ ███    ███  ██████  ███    ██
 #   ██     ██    ██ ████  ████ ████  ████ ██    ██ ████   ██
@@ -55,61 +56,67 @@
 
 
 _REAL = np.cos(0.01 * np.pi)
 _IMAG = 1j * np.sin(0.01 * np.pi)
 _VALUE = (_REAL + _IMAG - 1).astype(np.complex128)
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def product(
     matrix1: npt.NDArray[np.complex128], matrix2: npt.NDArray[np.complex128]
 ) -> np.float64:
     """Calculate scalar product of two matrices."""
     retval = np.trace(np.dot(matrix1, matrix2)).real
 
     return retval  # type: ignore[no-any-return]
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def get_random_haar_1d(depth: int) -> npt.NDArray[np.complex128]:
     """Generate a random vector with Haar measure."""
     real = np.random.uniform(0, 1, depth)  # noqa: NPY002
     imag = np.random.uniform(0, 1, depth)  # noqa: NPY002
 
     retval = np.exp(2 * np.pi * 1j * real) * np.sqrt(-np.log(imag))
 
     return retval  # type: ignore[no-any-return]
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def get_random_haar_2d(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Generate multiple random vectors with Haar measure in form of matrix."""
     real = np.random.uniform(0, 1, (quantity, depth))  # noqa: NPY002
     imag = np.random.uniform(0, 1, (quantity, depth))  # noqa: NPY002
 
     retval = np.exp(2 * np.pi * 1j * real) * np.sqrt(-np.log(imag))
 
     return retval  # type: ignore[no-any-return]
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def normalize(mtx: npt.NDArray[np.complex128]) -> npt.NDArray[np.complex128]:
     """Normalize a vector."""
     mtx2 = np.dot(mtx, np.conj(mtx))
 
     val = np.sqrt(np.real(mtx2))
 
     retval = mtx / val
 
     return retval  # type: ignore[no-any-return]
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def project(mtx1: npt.NDArray[np.complex128]) -> npt.NDArray[np.complex128]:
     """Build a projection from a vector."""
     retval = np.outer(mtx1, np.conj(mtx1))
 
     return retval  # type: ignore[no-any-return]
 
 
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def kronecker(
     mtx: npt.NDArray[np.complex128], mtx1: npt.NDArray[np.complex128]
 ) -> npt.NDArray[np.complex128]:
     """Kronecker Product."""
     ddd1 = len(mtx)
     ddd2 = len(mtx1)
 
@@ -120,28 +127,30 @@
     out_mtx = np.swapaxes(dot_0_1, 1, 2)
 
     retval = out_mtx.reshape(output_shape).astype(np.complex128, copy=False)
 
     return retval  # type: ignore[no-any-return]
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def rotate(
     rho2: npt.NDArray[np.complex128], unitary: npt.NDArray[np.complex128]
 ) -> npt.NDArray[np.complex128]:
     """Sandwich an operator with a unitary."""
     rho2a = np.dot(rho2, np.conj(unitary).T)  # matmul replaced with dot
 
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
 
     return rho2a  # type: ignore[no-any-return]
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def apply_symmetries(
     rho: npt.NDArray[np.complex128],
-    symmetries: list[list[npt.NDArray[np.complex128]]],
+    symmetries: types.ListType[types.ListType[npt.NDArray[np.complex128]]],
 ) -> npt.NDArray[np.complex128]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex128]
         Density matrix to which we want to apply symmetries.
@@ -174,73 +183,76 @@
 #   ██████     ███████    ███████            ███    ███     ██████     ██████     ███████   # noqa: E501
 #   ██   ██    ██         ██                 ████  ████    ██    ██    ██   ██    ██        # noqa: E501
 #   ██   ██    █████      ███████            ██ ████ ██    ██    ██    ██   ██    █████     # noqa: E501
 #   ██   ██    ██              ██            ██  ██  ██    ██    ██    ██   ██    ██        # noqa: E501
 #   ██████     ██         ███████            ██      ██     ██████     ██████     ███████   # noqa: E501
 
 
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def optimize_d_fs(
     new_state: npt.NDArray[np.complex128],
     visibility_state: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex128]:
     """Optimize implementation for FSnQd mode."""
-    product_2_3 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
-    # To make sure rotated_2 is not unbound
+    # To make sure return_state is not unbound
     unitary = random_unitary_d_fs(depth, quantity, 0)
 
-    rotated_2 = rotate(new_state, unitary)
+    return_state = rotate(new_state, unitary)
 
-    for idx in range(updates_count):
+    for idx in range(20 * depth * depth * quantity):
         idx_mod = idx % int(quantity)
         unitary = random_unitary_d_fs(depth, quantity, idx_mod)
 
-        rotated_2 = rotate(new_state, unitary)
+        return_state = rotate(new_state, unitary)
 
-        product_rot2_3 = product(rotated_2, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        if product_2_3 > product_rot2_3:
+        if loss > new_loss:
             unitary = unitary.conj().T
-            rotated_2 = rotate(new_state, unitary)
+            return_state = rotate(new_state, unitary)
 
-        while product_rot2_3 > product_2_3:
-            product_2_3 = product_rot2_3
-            rotated_2 = rotate(rotated_2, unitary)
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
 
-            product_rot2_3 = product(rotated_2, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
-    return rotated_2.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
+    return return_state.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
 
 
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def random_unitary_d_fs(
     depth: int, quantity: int, idx: int
 ) -> npt.NDArray[np.complex128]:
     """N quDits."""
     value = _random_unitary_d_fs(depth)
 
     mtx = expand_d_fs(value, depth, quantity, idx)
 
     return mtx  # type: ignore[no-any-return]
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def _random_unitary_d_fs(depth: int) -> npt.NDArray[np.complex128]:
     random_mtx = random_d_fs(depth, 1)
 
     identity_mtx = np.identity(depth).astype(np.complex128)
 
     rand_mul = np.multiply(_VALUE, random_mtx)
 
     value = np.add(rand_mul, identity_mtx)
 
     return value  # type: ignore[no-any-return]
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
 
     for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
@@ -248,14 +260,15 @@
         vector = np.outer(vector, idx_vector).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
 
 
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def expand_d_fs(
     value: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
     idx: int,
 ) -> npt.NDArray[np.complex128]:
     """Expand an operator to n quDits."""
@@ -275,26 +288,28 @@
 #   ██████     ███████            ███    ███     ██████     ██████     ███████
 #   ██   ██    ██                 ████  ████    ██    ██    ██   ██    ██
 #   ██████     ███████            ██ ████ ██    ██    ██    ██   ██    █████
 #   ██   ██         ██            ██  ██  ██    ██    ██    ██   ██    ██
 #   ██████     ███████            ██      ██     ██████     ██████     ███████
 
 
+@jit(nopython=True, nogil=True, cache=True)
 def random_bs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Draw random biseparable state."""
     random_vector_1 = normalize(get_random_haar_1d(depth))
     random_vector_2 = normalize(get_random_haar_1d(quantity))
 
     vector = np.outer(random_vector_1, random_vector_2).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
 
 
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def random_unitary_bs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
 
     random_matrix = project(random_vector)
 
     identity_depth = np.identity(depth).astype(np.complex128)
@@ -304,15 +319,16 @@
     unitary_biseparable = _VALUE * random_matrix + identity_depth
 
     retval = kronecker(unitary_biseparable, identity_quantity)
 
     return retval  # type: ignore[no-any-return]
 
 
-def random_unitary_bs_reverse(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
+def random_unitary_bs_reverse(quantity: int, depth: int) -> npt.NDArray[np.complex128]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
 
     random_matrix = project(random_vector)
 
     identity_depth = np.identity(depth).astype(np.complex128)
 
@@ -321,20 +337,20 @@
     unitary_biseparable = _VALUE * random_matrix + identity_depth
 
     retval = kronecker(identity_quantity, unitary_biseparable)
 
     return retval  # type: ignore[no-any-return]
 
 
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def optimize_bs(
     new_state: npt.NDArray[np.complex128],
     visibility_state: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex128]:
     """Run the minimization algorithm to optimize the biseparable state.
 
     Parameters
     ----------
     new_state : npt.NDArray[np.complex128]
         Randomly drawn state to be optimized.
@@ -349,31 +365,105 @@
 
     Returns
     -------
     npt.NDArray[np.complex128]
         Optimized state.
 
     """
-    pp1 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
     return_state = new_state.copy()
 
-    for index in range(updates_count):
+    for index in range(5 * depth * quantity):
         if index % 2:
             unitary = random_unitary_bs(depth, quantity)
         else:
             unitary = random_unitary_bs_reverse(depth, quantity)
 
         return_state = rotate(new_state, unitary)
 
-        if pp1 > product(return_state, visibility_state):
+        if loss > product(return_state, visibility_state):
             unitary = unitary.conj().T
             return_state = rotate(new_state, unitary)
 
-        pp2 = product(return_state, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        while pp2 > pp1:
-            pp1 = pp2
+        while new_loss > loss:
+            loss = new_loss
             return_state = rotate(return_state, unitary)
-            pp2 = product(return_state, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
     return return_state
+
+
+#    ███████   █████▄   ██████     █████    ███████   ██████▄    ██████    ██████
+#   ██             ██   ██   ██   ██   ██   ██             ██   ██    ██   ██   ██
+#   ██   ███   █████    ██████    ███████   █████      █████    ██    ██   ██   ██
+#   ██    ██       ██   ██        ██   ██   ██             ██   ██ ▄▄ ██   ██   ██
+#    ███████   █████▀   ██        ██   ██   ███████   ██████▀    ██████    ██████
+#                                                                   ▀▀
+
+
+@jit(nopython=True, nogil=True, cache=True)
+def random_3p(
+    depth: int,
+    swaps: types.ListType[npt.NDArray[np.complex128]],
+    index: int,
+) -> npt.NDArray[np.complex128]:
+    """Draw random biseparable state."""
+    if index == 0:
+        return random_bs(depth, depth * depth)  # type: ignore[no-any-return]
+    if index == 1:
+        return rotate(  # type: ignore[no-any-return]
+            random_bs(depth, depth * depth),
+            swaps[0],
+        )
+
+    return random_bs(depth * depth, depth)  # type: ignore[no-any-return]
+
+
+OPTIMIZE_3P_OPT_0 = 0
+OPTIMIZE_3P_OPT_1 = 1
+OPTIMIZE_3P_OPT_2 = 2
+
+
+OPTIMIZE_3P_JUMP_TABLE = [random_unitary_bs, random_unitary_bs_reverse]
+
+
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
+def optimize_3p(
+    new_state: npt.NDArray[np.complex128],
+    visibility_state: npt.NDArray[np.complex128],
+    depth: int,
+    swaps: types.ListType[npt.NDArray[np.complex128]],
+    index: int,
+) -> npt.NDArray[np.complex128]:
+    return_state = new_state.copy()
+    loss = product(new_state, visibility_state)
+
+    for i in range(5 * depth**6):
+        if index == OPTIMIZE_3P_OPT_0:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+
+        elif index == OPTIMIZE_3P_OPT_1:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+            unitary = rotate(unitary, swaps[0])
+
+        elif index == OPTIMIZE_3P_OPT_2:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth * depth, depth)
+
+        return_state = rotate(new_state, unitary)
+
+        new_loss = product(return_state, visibility_state)
+
+        if loss > new_loss:
+            unitary = unitary.conj().T
+            return_state = rotate(new_state, unitary)
+            new_loss = product(return_state, visibility_state)
+
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+
+            new_loss = product(return_state, visibility_state)
+
+    return return_state  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/_cython/_complex64.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/_cython/_complex64.py`

 * *Files 12% similar despite different names*

```diff
@@ -183,43 +183,42 @@
 
 
 def optimize_d_fs(
     new_state: npt.NDArray[np.complex64],
     visibility_state: npt.NDArray[np.complex64],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex64]:
     """Optimize implementation for FSnQd mode."""
-    product_2_3 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
-    # To make sure rotated_2 is not unbound
+    # To make sure return_state is not unbound
     unitary = random_unitary_d_fs(depth, quantity, 0)
 
-    rotated_2 = rotate(new_state, unitary)
+    return_state = rotate(new_state, unitary)
 
-    for idx in range(updates_count):
+    for idx in range(20 * depth * depth * quantity):
         idx_mod = idx % int(quantity)
         unitary = random_unitary_d_fs(depth, quantity, idx_mod)
 
-        rotated_2 = rotate(new_state, unitary)
+        return_state = rotate(new_state, unitary)
 
-        product_rot2_3 = product(rotated_2, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        if product_2_3 > product_rot2_3:
+        if loss > new_loss:
             unitary = unitary.conj().T
-            rotated_2 = rotate(new_state, unitary)
+            return_state = rotate(new_state, unitary)
 
-        while product_rot2_3 > product_2_3:
-            product_2_3 = product_rot2_3
-            rotated_2 = rotate(rotated_2, unitary)
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
 
-            product_rot2_3 = product(rotated_2, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
-    return rotated_2.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
+    return return_state.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
 
 
 def random_unitary_d_fs(
     depth: int, quantity: int, idx: int
 ) -> npt.NDArray[np.complex64]:
     """N quDits."""
     value = _random_unitary_d_fs(depth)
@@ -308,15 +307,15 @@
     unitary_biseparable = _VALUE * random_matrix + identity_depth
 
     retval = kronecker(unitary_biseparable, identity_quantity)
 
     return retval  # type: ignore[no-any-return]
 
 
-def random_unitary_bs_reverse(depth: int, quantity: int) -> npt.NDArray[np.complex64]:
+def random_unitary_bs_reverse(quantity: int, depth: int) -> npt.NDArray[np.complex64]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
 
     random_matrix = project(random_vector)
 
     identity_depth = np.identity(depth).astype(np.complex64)
 
@@ -330,15 +329,14 @@
 
 
 def optimize_bs(
     new_state: npt.NDArray[np.complex64],
     visibility_state: npt.NDArray[np.complex64],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex64]:
     """Run the minimization algorithm to optimize the biseparable state.
 
     Parameters
     ----------
     new_state : npt.NDArray[np.complex64]
         Randomly drawn state to be optimized.
@@ -353,31 +351,103 @@
 
     Returns
     -------
     npt.NDArray[np.complex64]
         Optimized state.
 
     """
-    pp1 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
     return_state = new_state.copy()
 
-    for index in range(updates_count):
+    for index in range(5 * depth * quantity):
         if index % 2:
             unitary = random_unitary_bs(depth, quantity)
         else:
             unitary = random_unitary_bs_reverse(depth, quantity)
 
         return_state = rotate(new_state, unitary)
 
-        if pp1 > product(return_state, visibility_state):
+        if loss > product(return_state, visibility_state):
             unitary = unitary.conj().T
             return_state = rotate(new_state, unitary)
 
-        pp2 = product(return_state, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        while pp2 > pp1:
-            pp1 = pp2
+        while new_loss > loss:
+            loss = new_loss
             return_state = rotate(return_state, unitary)
-            pp2 = product(return_state, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
     return return_state
+
+
+#    ███████   █████▄   ██████     █████    ███████   ██████▄    ██████    ██████
+#   ██             ██   ██   ██   ██   ██   ██             ██   ██    ██   ██   ██
+#   ██   ███   █████    ██████    ███████   █████      █████    ██    ██   ██   ██
+#   ██    ██       ██   ██        ██   ██   ██             ██   ██ ▄▄ ██   ██   ██
+#    ███████   █████▀   ██        ██   ██   ███████   ██████▀    ██████    ██████
+#                                                                   ▀▀
+
+
+def random_3p(
+    depth: int,
+    swaps: list[npt.NDArray[np.complex64]],
+    index: int,
+) -> npt.NDArray[np.complex64]:
+    """Draw random biseparable state."""
+    if index == 0:
+        return random_bs(depth, depth * depth)  # type: ignore[no-any-return]
+    if index == 1:
+        return rotate(  # type: ignore[no-any-return]
+            random_bs(depth, depth * depth),
+            swaps[0],
+        )
+
+    return random_bs(depth * depth, depth)  # type: ignore[no-any-return]
+
+
+OPTIMIZE_3P_OPT_0 = 0
+OPTIMIZE_3P_OPT_1 = 1
+OPTIMIZE_3P_OPT_2 = 2
+
+
+OPTIMIZE_3P_JUMP_TABLE = [random_unitary_bs, random_unitary_bs_reverse]
+
+
+def optimize_3p(
+    new_state: npt.NDArray[np.complex64],
+    visibility_state: npt.NDArray[np.complex64],
+    depth: int,
+    swaps: list[npt.NDArray[np.complex64]],
+    index: int,
+) -> npt.NDArray[np.complex64]:
+    return_state = new_state.copy()
+    loss = product(new_state, visibility_state)
+
+    for i in range(5 * depth**6):
+        if index == OPTIMIZE_3P_OPT_0:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+
+        elif index == OPTIMIZE_3P_OPT_1:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+            unitary = rotate(unitary, swaps[0])
+
+        elif index == OPTIMIZE_3P_OPT_2:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth * depth, depth)
+
+        return_state = rotate(new_state, unitary)
+
+        new_loss = product(return_state, visibility_state)
+
+        if loss > new_loss:
+            unitary = unitary.conj().T
+            return_state = rotate(new_state, unitary)
+            new_loss = product(return_state, visibility_state)
+
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+
+            new_loss = product(return_state, visibility_state)
+
+    return return_state  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/base.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 specific precision.
 """
 
 from __future__ import annotations
 
 import logging
 from types import MethodType
-from typing import TYPE_CHECKING, Callable, Generic, Optional, TypeVar, cast
+from typing import TYPE_CHECKING, Generic, Optional, TypeVar, cast
 
 import numpy as np
 import numpy.typing as npt
 from cssfinder.algorithm.backend.base import BackendBase
 from cssfinder.cssfproject import AlgoMode
 from numba import jit, typed  # type: ignore[attr-defined]
 
 if TYPE_CHECKING:
-    from cssfinder.algorithm.backend.numpy.impl import Implementation
+    from cssfinder_backend_numpy.impl import Implementation
 
 PRIMARY = TypeVar("PRIMARY", np.complex128, np.complex64)
 SECONDARY_co = TypeVar("SECONDARY_co", np.float64, np.float32, covariant=True)
 
 
 class NumPyBase(Generic[PRIMARY, SECONDARY_co], BackendBase):
     """Implementation of Gilbert algorithm using python numpy library."""
@@ -53,18 +53,15 @@
     _symmetries: list[list[npt.NDArray[PRIMARY]]]
     _projection: Optional[npt.NDArray[PRIMARY]]
 
     impl: Implementation[PRIMARY, SECONDARY_co]
     primary_t: type[PRIMARY]
     secondary_t: type[SECONDARY_co]
 
-    optimize_callback: Callable[
-        [npt.NDArray[PRIMARY], npt.NDArray[PRIMARY], int, int, int],
-        npt.NDArray[PRIMARY],
-    ]
+    swaps: list[npt.NDArray[PRIMARY]]
 
     def __init__(  # noqa: PLR0913
         self,
         initial: npt.NDArray[np.complex128],
         depth: int,
         quantity: int,
         mode: AlgoMode,
@@ -95,19 +92,31 @@
             npt.NDArray[PRIMARY],
             (self._visibility - self._intermediate),
         )
         self._dd1: SECONDARY_co = self.impl.product(
             self._intermediate,
             self._visibility_reduced,
         )
-
-        if self.mode == AlgoMode.FSnQd:
-            self.optimize_callback = self.impl.optimize_d_fs
-        elif self.mode == AlgoMode.SBiPa:
-            self.optimize_callback = self.impl.optimize_bs
+        if self.mode == AlgoMode.G3PaE3qD:
+            self.swaps = [self._get_swap123(depth)]
+        elif self.mode == AlgoMode.G4PaE3qD:
+            self.swaps = []
+        else:
+            self.swaps = []
+
+    def _get_swap123(self, depth: int) -> npt.NDArray[PRIMARY]:
+        swap_matrix = np.zeros((depth**3, depth**3), dtype=self.primary_t)
+        depth2 = depth**2
+        for i in range(depth):
+            for j in range(depth):
+                for k in range(depth):
+                    swap_matrix[i * depth2 + j * depth + k][
+                        j * depth2 + i * depth + k
+                    ] = (1.0 + 0.0j)
+        return swap_matrix
 
     def _create_visibility_matrix(self) -> npt.NDArray[PRIMARY]:
         vis_state = self.visibility * self.initial
         inv_vis_ident = (1 - self.visibility) * np.identity(
             len(self.initial),
             dtype=np.complex128,
         )
@@ -172,52 +181,71 @@
         """Return number of all corrections found during optimization."""
         return len(self._corrections)
 
     def run_epoch(self, iterations: int, epoch_index: int) -> None:
         """Run sequence of iterations without stopping to check any stop conditions."""
         depth = self.depth
         quantity = self.quantity
-        epochs = 20 * depth * depth * quantity
 
-        for iteration_index in range(iterations):
+        begin = epoch_index * iterations
+        end = epoch_index * iterations + iterations
+
+        for iteration_index in range(begin, end):
             if self.mode == AlgoMode.FSnQd:
                 alternative_state = self.impl.random_d_fs(depth, quantity)
+
             elif self.mode == AlgoMode.SBiPa:
                 alternative_state = self.impl.random_bs(depth, quantity)
 
+            elif self.mode == AlgoMode.G3PaE3qD:
+                alternative_state = self.impl.random_3p(
+                    depth, self.swaps, iteration_index % 3
+                )
+
             if (
                 self.impl.product(alternative_state, self._visibility_reduced)
                 > self._dd1
             ):
                 self._update_state(
                     alternative_state,
-                    iterations,
-                    epoch_index,
-                    epochs,
                     iteration_index,
                 )
 
-    def _update_state(  # noqa: PLR0913
+    def _update_state(
         self,
         alternative_state: npt.NDArray[PRIMARY],
-        iterations: int,
-        epoch_index: int,
-        epochs: int,
         iteration_index: int,
     ) -> None:
         depth = self.depth
         quantity = self.quantity
 
-        alternative_state = self.optimize_callback(
-            alternative_state,
-            self._visibility_reduced,
-            depth,
-            quantity,
-            epochs,
-        )
+        if self.mode == AlgoMode.FSnQd:
+            alternative_state = self.impl.optimize_d_fs(
+                alternative_state,
+                self._visibility_reduced,
+                depth,
+                quantity,
+            )
+
+        elif self.mode == AlgoMode.SBiPa:
+            alternative_state = self.impl.optimize_bs(
+                alternative_state,
+                self._visibility_reduced,
+                depth,
+                quantity,
+            )
+
+        elif self.mode == AlgoMode.G3PaE3qD:
+            alternative_state = self.impl.optimize_3p(
+                alternative_state,
+                self._visibility_reduced,
+                depth,
+                self.swaps,
+                iteration_index % 3,
+            )
 
         if self._symmetries:
             self._intermediate = self.impl.apply_symmetries(
                 self._intermediate, self._symmetries
             )
         if self._projection is not None:
             self._intermediate = self.impl.rotate(self._intermediate, self._projection)
@@ -242,15 +270,15 @@
             )
             self._aa4 = 2 * self.impl.product(self._visibility, self._intermediate)
             self._aa6 = self.impl.product(self._intermediate, self._intermediate)
             self._dd1 = self._aa4 / 2 - self._aa6
 
             self._corrections.append(
                 (
-                    epoch_index * iterations + iteration_index + 1,
+                    iteration_index + 1,
                     len(self._corrections) + 1,
                     float(
                         self.impl.product(
                             self._visibility_reduced,
                             self._visibility_reduced,
                         ),
                     ),
@@ -268,14 +296,15 @@
         quantity: int,
         mode: AlgoMode,
         visibility: float,
         *,
         is_debug: bool = False,
     ) -> None:
         super().__init__(initial, depth, quantity, mode, visibility, is_debug=is_debug)
+        self.swaps = typed.List(s for s in self.swaps)
         if not self.is_debug:
             self.jit()
 
     def set_symmetries(
         self, symmetries: list[list[npt.NDArray[np.complex128]]]
     ) -> None:
         """Set symmetries to use during calculations.
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/complex128.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/complex128.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/complex64.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/complex64.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/cython/__init__.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/cython/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/impl.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,15 +124,14 @@
 
     @staticmethod
     def optimize_d_fs(
         new_state: npt.NDArray[PRIMARY],
         visibility_state: npt.NDArray[PRIMARY],
         depth: int,
         quantity: int,
-        epochs: int,
     ) -> npt.NDArray[PRIMARY]:
         """Optimize implementation for FSnQd mode."""
         ...
 
     @staticmethod
     def random_unitary_d_fs(
         depth: int,
@@ -180,31 +179,68 @@
 
     @staticmethod
     def optimize_bs(
         new_state: npt.NDArray[PRIMARY],
         visibility_state: npt.NDArray[PRIMARY],
         depth: int,
         quantity: int,
-        updates_count: int,
     ) -> npt.NDArray[PRIMARY]:
         """Run the minimization algorithm to optimize the biseparable state.
 
         Parameters
         ----------
         new_state : npt.NDArray[np.complex128]
             Randomly drawn state to be optimized.
         visibility_state : npt.NDArray[np.complex128]
             Visibility matrix.
         depth : int
             Depth of analyzed system.
         quantity : int
             Quantity of quDits in system.
-        updates_count : int
-            Number of optimizer iterations to execute.
 
         Returns
         -------
         npt.NDArray[np.complex128]
             Optimized state.
 
         """
         ...
+
+    @staticmethod
+    def optimize_3p(
+        new_state: npt.NDArray[PRIMARY],
+        visibility_state: npt.NDArray[PRIMARY],
+        depth: int,
+        swaps: list[npt.NDArray[PRIMARY]],
+        index: int,
+    ) -> npt.NDArray[PRIMARY]:
+        """Run the minimization algorithm to optimize the biseparable state.
+
+        Parameters
+        ----------
+        new_state : npt.NDArray[PRIMARY]
+            Randomly drawn state to be optimized.
+        visibility_state : npt.NDArray[PRIMARY]
+            Visibility matrix.
+        depth : int
+            Depth of analyzed system.
+        swaps : list[npt.NDArray[PRIMARY]]
+            Swap gates array.
+        index : int
+            Index of variant of unitary generator.
+
+        Returns
+        -------
+        npt.NDArray[PRIMARY]
+            Optimized state.
+
+        """
+        ...
+
+    @staticmethod
+    def random_3p(
+        depth: int,
+        swaps: list[npt.NDArray[PRIMARY]],
+        index: int,
+    ) -> npt.NDArray[PRIMARY]:
+        """Draw biseparable state with three quDits."""
+        ...
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/__init__.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/_complex128.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/_cython/_complex128.py`

 * *Files 14% similar despite different names*

```diff
@@ -179,43 +179,42 @@
 
 
 def optimize_d_fs(
     new_state: npt.NDArray[np.complex128],
     visibility_state: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex128]:
     """Optimize implementation for FSnQd mode."""
-    product_2_3 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
-    # To make sure rotated_2 is not unbound
+    # To make sure return_state is not unbound
     unitary = random_unitary_d_fs(depth, quantity, 0)
 
-    rotated_2 = rotate(new_state, unitary)
+    return_state = rotate(new_state, unitary)
 
-    for idx in range(updates_count):
+    for idx in range(20 * depth * depth * quantity):
         idx_mod = idx % int(quantity)
         unitary = random_unitary_d_fs(depth, quantity, idx_mod)
 
-        rotated_2 = rotate(new_state, unitary)
+        return_state = rotate(new_state, unitary)
 
-        product_rot2_3 = product(rotated_2, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        if product_2_3 > product_rot2_3:
+        if loss > new_loss:
             unitary = unitary.conj().T
-            rotated_2 = rotate(new_state, unitary)
+            return_state = rotate(new_state, unitary)
 
-        while product_rot2_3 > product_2_3:
-            product_2_3 = product_rot2_3
-            rotated_2 = rotate(rotated_2, unitary)
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
 
-            product_rot2_3 = product(rotated_2, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
-    return rotated_2.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
+    return return_state.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
 
 
 def random_unitary_d_fs(
     depth: int, quantity: int, idx: int
 ) -> npt.NDArray[np.complex128]:
     """N quDits."""
     value = _random_unitary_d_fs(depth)
@@ -304,15 +303,15 @@
     unitary_biseparable = _VALUE * random_matrix + identity_depth
 
     retval = kronecker(unitary_biseparable, identity_quantity)
 
     return retval  # type: ignore[no-any-return]
 
 
-def random_unitary_bs_reverse(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
+def random_unitary_bs_reverse(quantity: int, depth: int) -> npt.NDArray[np.complex128]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
 
     random_matrix = project(random_vector)
 
     identity_depth = np.identity(depth).astype(np.complex128)
 
@@ -326,15 +325,14 @@
 
 
 def optimize_bs(
     new_state: npt.NDArray[np.complex128],
     visibility_state: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex128]:
     """Run the minimization algorithm to optimize the biseparable state.
 
     Parameters
     ----------
     new_state : npt.NDArray[np.complex128]
         Randomly drawn state to be optimized.
@@ -349,31 +347,103 @@
 
     Returns
     -------
     npt.NDArray[np.complex128]
         Optimized state.
 
     """
-    pp1 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
     return_state = new_state.copy()
 
-    for index in range(updates_count):
+    for index in range(5 * depth * quantity):
         if index % 2:
             unitary = random_unitary_bs(depth, quantity)
         else:
             unitary = random_unitary_bs_reverse(depth, quantity)
 
         return_state = rotate(new_state, unitary)
 
-        if pp1 > product(return_state, visibility_state):
+        if loss > product(return_state, visibility_state):
             unitary = unitary.conj().T
             return_state = rotate(new_state, unitary)
 
-        pp2 = product(return_state, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        while pp2 > pp1:
-            pp1 = pp2
+        while new_loss > loss:
+            loss = new_loss
             return_state = rotate(return_state, unitary)
-            pp2 = product(return_state, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
     return return_state
+
+
+#    ███████   █████▄   ██████     █████    ███████   ██████▄    ██████    ██████
+#   ██             ██   ██   ██   ██   ██   ██             ██   ██    ██   ██   ██
+#   ██   ███   █████    ██████    ███████   █████      █████    ██    ██   ██   ██
+#   ██    ██       ██   ██        ██   ██   ██             ██   ██ ▄▄ ██   ██   ██
+#    ███████   █████▀   ██        ██   ██   ███████   ██████▀    ██████    ██████
+#                                                                   ▀▀
+
+
+def random_3p(
+    depth: int,
+    swaps: list[npt.NDArray[np.complex128]],
+    index: int,
+) -> npt.NDArray[np.complex128]:
+    """Draw random biseparable state."""
+    if index == 0:
+        return random_bs(depth, depth * depth)  # type: ignore[no-any-return]
+    if index == 1:
+        return rotate(  # type: ignore[no-any-return]
+            random_bs(depth, depth * depth),
+            swaps[0],
+        )
+
+    return random_bs(depth * depth, depth)  # type: ignore[no-any-return]
+
+
+OPTIMIZE_3P_OPT_0 = 0
+OPTIMIZE_3P_OPT_1 = 1
+OPTIMIZE_3P_OPT_2 = 2
+
+
+OPTIMIZE_3P_JUMP_TABLE = [random_unitary_bs, random_unitary_bs_reverse]
+
+
+def optimize_3p(
+    new_state: npt.NDArray[np.complex128],
+    visibility_state: npt.NDArray[np.complex128],
+    depth: int,
+    swaps: list[npt.NDArray[np.complex128]],
+    index: int,
+) -> npt.NDArray[np.complex128]:
+    return_state = new_state.copy()
+    loss = product(new_state, visibility_state)
+
+    for i in range(5 * depth**6):
+        if index == OPTIMIZE_3P_OPT_0:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+
+        elif index == OPTIMIZE_3P_OPT_1:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+            unitary = rotate(unitary, swaps[0])
+
+        elif index == OPTIMIZE_3P_OPT_2:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth * depth, depth)
+
+        return_state = rotate(new_state, unitary)
+
+        new_loss = product(return_state, visibility_state)
+
+        if loss > new_loss:
+            unitary = unitary.conj().T
+            return_state = rotate(new_state, unitary)
+            new_loss = product(return_state, visibility_state)
+
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+
+            new_loss = product(return_state, visibility_state)
+
+    return return_state  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy/_complex64.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy/_complex64.py`

 * *Files 12% similar despite different names*

```diff
@@ -183,43 +183,42 @@
 
 
 def optimize_d_fs(
     new_state: npt.NDArray[np.complex64],
     visibility_state: npt.NDArray[np.complex64],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex64]:
     """Optimize implementation for FSnQd mode."""
-    product_2_3 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
-    # To make sure rotated_2 is not unbound
+    # To make sure return_state is not unbound
     unitary = random_unitary_d_fs(depth, quantity, 0)
 
-    rotated_2 = rotate(new_state, unitary)
+    return_state = rotate(new_state, unitary)
 
-    for idx in range(updates_count):
+    for idx in range(20 * depth * depth * quantity):
         idx_mod = idx % int(quantity)
         unitary = random_unitary_d_fs(depth, quantity, idx_mod)
 
-        rotated_2 = rotate(new_state, unitary)
+        return_state = rotate(new_state, unitary)
 
-        product_rot2_3 = product(rotated_2, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        if product_2_3 > product_rot2_3:
+        if loss > new_loss:
             unitary = unitary.conj().T
-            rotated_2 = rotate(new_state, unitary)
+            return_state = rotate(new_state, unitary)
 
-        while product_rot2_3 > product_2_3:
-            product_2_3 = product_rot2_3
-            rotated_2 = rotate(rotated_2, unitary)
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
 
-            product_rot2_3 = product(rotated_2, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
-    return rotated_2.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
+    return return_state.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
 
 
 def random_unitary_d_fs(
     depth: int, quantity: int, idx: int
 ) -> npt.NDArray[np.complex64]:
     """N quDits."""
     value = _random_unitary_d_fs(depth)
@@ -308,15 +307,15 @@
     unitary_biseparable = _VALUE * random_matrix + identity_depth
 
     retval = kronecker(unitary_biseparable, identity_quantity)
 
     return retval  # type: ignore[no-any-return]
 
 
-def random_unitary_bs_reverse(depth: int, quantity: int) -> npt.NDArray[np.complex64]:
+def random_unitary_bs_reverse(quantity: int, depth: int) -> npt.NDArray[np.complex64]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
 
     random_matrix = project(random_vector)
 
     identity_depth = np.identity(depth).astype(np.complex64)
 
@@ -330,15 +329,14 @@
 
 
 def optimize_bs(
     new_state: npt.NDArray[np.complex64],
     visibility_state: npt.NDArray[np.complex64],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex64]:
     """Run the minimization algorithm to optimize the biseparable state.
 
     Parameters
     ----------
     new_state : npt.NDArray[np.complex64]
         Randomly drawn state to be optimized.
@@ -353,31 +351,103 @@
 
     Returns
     -------
     npt.NDArray[np.complex64]
         Optimized state.
 
     """
-    pp1 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
     return_state = new_state.copy()
 
-    for index in range(updates_count):
+    for index in range(5 * depth * quantity):
         if index % 2:
             unitary = random_unitary_bs(depth, quantity)
         else:
             unitary = random_unitary_bs_reverse(depth, quantity)
 
         return_state = rotate(new_state, unitary)
 
-        if pp1 > product(return_state, visibility_state):
+        if loss > product(return_state, visibility_state):
             unitary = unitary.conj().T
             return_state = rotate(new_state, unitary)
 
-        pp2 = product(return_state, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        while pp2 > pp1:
-            pp1 = pp2
+        while new_loss > loss:
+            loss = new_loss
             return_state = rotate(return_state, unitary)
-            pp2 = product(return_state, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
     return return_state
+
+
+#    ███████   █████▄   ██████     █████    ███████   ██████▄    ██████    ██████
+#   ██             ██   ██   ██   ██   ██   ██             ██   ██    ██   ██   ██
+#   ██   ███   █████    ██████    ███████   █████      █████    ██    ██   ██   ██
+#   ██    ██       ██   ██        ██   ██   ██             ██   ██ ▄▄ ██   ██   ██
+#    ███████   █████▀   ██        ██   ██   ███████   ██████▀    ██████    ██████
+#                                                                   ▀▀
+
+
+def random_3p(
+    depth: int,
+    swaps: list[npt.NDArray[np.complex64]],
+    index: int,
+) -> npt.NDArray[np.complex64]:
+    """Draw random biseparable state."""
+    if index == 0:
+        return random_bs(depth, depth * depth)  # type: ignore[no-any-return]
+    if index == 1:
+        return rotate(  # type: ignore[no-any-return]
+            random_bs(depth, depth * depth),
+            swaps[0],
+        )
+
+    return random_bs(depth * depth, depth)  # type: ignore[no-any-return]
+
+
+OPTIMIZE_3P_OPT_0 = 0
+OPTIMIZE_3P_OPT_1 = 1
+OPTIMIZE_3P_OPT_2 = 2
+
+
+OPTIMIZE_3P_JUMP_TABLE = [random_unitary_bs, random_unitary_bs_reverse]
+
+
+def optimize_3p(
+    new_state: npt.NDArray[np.complex64],
+    visibility_state: npt.NDArray[np.complex64],
+    depth: int,
+    swaps: list[npt.NDArray[np.complex64]],
+    index: int,
+) -> npt.NDArray[np.complex64]:
+    return_state = new_state.copy()
+    loss = product(new_state, visibility_state)
+
+    for i in range(5 * depth**6):
+        if index == OPTIMIZE_3P_OPT_0:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+
+        elif index == OPTIMIZE_3P_OPT_1:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+            unitary = rotate(unitary, swaps[0])
+
+        elif index == OPTIMIZE_3P_OPT_2:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth * depth, depth)
+
+        return_state = rotate(new_state, unitary)
+
+        new_loss = product(return_state, visibility_state)
+
+        if loss > new_loss:
+            unitary = unitary.conj().T
+            return_state = rotate(new_state, unitary)
+            new_loss = product(return_state, visibility_state)
+
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+
+            new_loss = product(return_state, visibility_state)
+
+    return return_state  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/__init__.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_debug/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/_complex128.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_debug/_complex128.py`

 * *Files 16% similar despite different names*

```diff
@@ -226,51 +226,50 @@
 
 
 def optimize_d_fs(
     new_state: npt.NDArray[np.complex128],
     visibility_state: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex128]:
     """Optimize implementation for FSnQd mode."""
     assert_dtype(new_state, np.complex128)
     assert_dtype(visibility_state, np.complex128)
 
-    product_2_3 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
-    # To make sure rotated_2 is not unbound
+    # To make sure return_state is not unbound
     unitary = random_unitary_d_fs(depth, quantity, 0)
     assert_dtype(unitary, np.complex128)
 
-    rotated_2 = rotate(new_state, unitary)
+    return_state = rotate(new_state, unitary)
 
-    for idx in range(updates_count):
+    for idx in range(20 * depth * depth * quantity):
         idx_mod = idx % int(quantity)
         unitary = random_unitary_d_fs(depth, quantity, idx_mod)
         assert_dtype(unitary, np.complex128)
 
-        rotated_2 = rotate(new_state, unitary)
-        assert_dtype(rotated_2, np.complex128)
+        return_state = rotate(new_state, unitary)
+        assert_dtype(return_state, np.complex128)
 
-        product_rot2_3 = product(rotated_2, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        if product_2_3 > product_rot2_3:
+        if loss > new_loss:
             unitary = unitary.conj().T
-            rotated_2 = rotate(new_state, unitary)
-            assert_dtype(rotated_2, np.complex128)
+            return_state = rotate(new_state, unitary)
+            assert_dtype(return_state, np.complex128)
 
-        while product_rot2_3 > product_2_3:
-            product_2_3 = product_rot2_3
-            rotated_2 = rotate(rotated_2, unitary)
-            assert_dtype(rotated_2, np.complex128)
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+            assert_dtype(return_state, np.complex128)
 
-            product_rot2_3 = product(rotated_2, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
-    return rotated_2.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
+    return return_state.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
 
 
 def random_unitary_d_fs(
     depth: int, quantity: int, idx: int
 ) -> npt.NDArray[np.complex128]:
     """N quDits."""
     value = _random_unitary_d_fs(depth)
@@ -382,15 +381,15 @@
 
     retval = kronecker(unitary_biseparable, identity_quantity)
     assert_dtype(retval, np.complex128)
 
     return retval  # type: ignore[no-any-return]
 
 
-def random_unitary_bs_reverse(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
+def random_unitary_bs_reverse(quantity: int, depth: int) -> npt.NDArray[np.complex128]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
     assert_dtype(random_vector, np.complex128)
 
     random_matrix = project(random_vector)
     assert_dtype(random_matrix, np.complex128)
 
@@ -410,15 +409,14 @@
 
 
 def optimize_bs(
     new_state: npt.NDArray[np.complex128],
     visibility_state: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex128]:
     """Run the minimization algorithm to optimize the biseparable state.
 
     Parameters
     ----------
     new_state : npt.NDArray[np.complex128]
         Randomly drawn state to be optimized.
@@ -436,39 +434,117 @@
     npt.NDArray[np.complex128]
         Optimized state.
 
     """
     assert_dtype(new_state, np.complex128)
     assert_dtype(visibility_state, np.complex128)
 
-    pp1 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
     return_state = new_state.copy()
 
-    for index in range(updates_count):
+    for index in range(5 * depth * quantity):
         if index % 2:
             unitary = random_unitary_bs(depth, quantity)
         else:
             unitary = random_unitary_bs_reverse(depth, quantity)
         assert_dtype(unitary, np.complex128)
 
         return_state = rotate(new_state, unitary)
         assert_dtype(return_state, np.complex128)
 
-        if pp1 > product(return_state, visibility_state):
+        if loss > product(return_state, visibility_state):
             unitary = unitary.conj().T
             return_state = rotate(new_state, unitary)
             assert_dtype(return_state, np.complex128)
 
-        pp2 = product(return_state, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        while pp2 > pp1:
-            pp1 = pp2
+        while new_loss > loss:
+            loss = new_loss
             return_state = rotate(return_state, unitary)
-            pp2 = product(return_state, visibility_state)
+            new_loss = product(return_state, visibility_state)
             assert_dtype(return_state, np.complex128)
 
         assert_dtype(return_state, np.complex128)
 
     assert_dtype(return_state, np.complex128)
 
     return return_state
+
+
+#    ███████   █████▄   ██████     █████    ███████   ██████▄    ██████    ██████
+#   ██             ██   ██   ██   ██   ██   ██             ██   ██    ██   ██   ██
+#   ██   ███   █████    ██████    ███████   █████      █████    ██    ██   ██   ██
+#   ██    ██       ██   ██        ██   ██   ██             ██   ██ ▄▄ ██   ██   ██
+#    ███████   █████▀   ██        ██   ██   ███████   ██████▀    ██████    ██████
+#                                                                   ▀▀
+
+
+def random_3p(
+    depth: int,
+    swaps: list[npt.NDArray[np.complex128]],
+    index: int,
+) -> npt.NDArray[np.complex128]:
+    """Draw random biseparable state."""
+    if index == 0:
+        return random_bs(depth, depth * depth)  # type: ignore[no-any-return]
+    if index == 1:
+        return rotate(  # type: ignore[no-any-return]
+            random_bs(depth, depth * depth),
+            swaps[0],
+        )
+
+    return random_bs(depth * depth, depth)  # type: ignore[no-any-return]
+
+
+OPTIMIZE_3P_OPT_0 = 0
+OPTIMIZE_3P_OPT_1 = 1
+OPTIMIZE_3P_OPT_2 = 2
+
+
+OPTIMIZE_3P_JUMP_TABLE = [random_unitary_bs, random_unitary_bs_reverse]
+
+
+def optimize_3p(
+    new_state: npt.NDArray[np.complex128],
+    visibility_state: npt.NDArray[np.complex128],
+    depth: int,
+    swaps: list[npt.NDArray[np.complex128]],
+    index: int,
+) -> npt.NDArray[np.complex128]:
+    return_state = new_state.copy()
+    loss = product(new_state, visibility_state)
+
+    for i in range(5 * depth**6):
+        if index == OPTIMIZE_3P_OPT_0:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+
+        elif index == OPTIMIZE_3P_OPT_1:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+            unitary = rotate(unitary, swaps[0])
+
+        elif index == OPTIMIZE_3P_OPT_2:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth * depth, depth)
+
+        else:
+            raise AssertionError(index)
+
+        return_state = rotate(new_state, unitary)
+
+        new_loss = product(return_state, visibility_state)
+
+        if loss > new_loss:
+            unitary = unitary.conj().T
+            return_state = rotate(new_state, unitary)
+            new_loss = product(return_state, visibility_state)
+
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+            assert_dtype(return_state, np.complex128)
+            new_loss = product(return_state, visibility_state)
+
+        assert_dtype(return_state, np.complex128)
+
+    assert_dtype(return_state, np.complex128)
+    return return_state  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_debug/_complex64.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_debug/_complex64.py`

 * *Files 10% similar despite different names*

```diff
@@ -230,51 +230,50 @@
 
 
 def optimize_d_fs(
     new_state: npt.NDArray[np.complex64],
     visibility_state: npt.NDArray[np.complex64],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex64]:
     """Optimize implementation for FSnQd mode."""
     assert_dtype(new_state, np.complex64)
     assert_dtype(visibility_state, np.complex64)
 
-    product_2_3 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
-    # To make sure rotated_2 is not unbound
+    # To make sure return_state is not unbound
     unitary = random_unitary_d_fs(depth, quantity, 0)
     assert_dtype(unitary, np.complex64)
 
-    rotated_2 = rotate(new_state, unitary)
+    return_state = rotate(new_state, unitary)
 
-    for idx in range(updates_count):
+    for idx in range(20 * depth * depth * quantity):
         idx_mod = idx % int(quantity)
         unitary = random_unitary_d_fs(depth, quantity, idx_mod)
         assert_dtype(unitary, np.complex64)
 
-        rotated_2 = rotate(new_state, unitary)
-        assert_dtype(rotated_2, np.complex64)
+        return_state = rotate(new_state, unitary)
+        assert_dtype(return_state, np.complex64)
 
-        product_rot2_3 = product(rotated_2, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        if product_2_3 > product_rot2_3:
+        if loss > new_loss:
             unitary = unitary.conj().T
-            rotated_2 = rotate(new_state, unitary)
-            assert_dtype(rotated_2, np.complex64)
+            return_state = rotate(new_state, unitary)
+            assert_dtype(return_state, np.complex64)
 
-        while product_rot2_3 > product_2_3:
-            product_2_3 = product_rot2_3
-            rotated_2 = rotate(rotated_2, unitary)
-            assert_dtype(rotated_2, np.complex64)
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+            assert_dtype(return_state, np.complex64)
 
-            product_rot2_3 = product(rotated_2, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
-    return rotated_2.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
+    return return_state.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
 
 
 def random_unitary_d_fs(
     depth: int, quantity: int, idx: int
 ) -> npt.NDArray[np.complex64]:
     """N quDits."""
     value = _random_unitary_d_fs(depth)
@@ -386,15 +385,15 @@
 
     retval = kronecker(unitary_biseparable, identity_quantity)
     assert_dtype(retval, np.complex64)
 
     return retval  # type: ignore[no-any-return]
 
 
-def random_unitary_bs_reverse(depth: int, quantity: int) -> npt.NDArray[np.complex64]:
+def random_unitary_bs_reverse(quantity: int, depth: int) -> npt.NDArray[np.complex64]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
     assert_dtype(random_vector, np.complex64)
 
     random_matrix = project(random_vector)
     assert_dtype(random_matrix, np.complex64)
 
@@ -414,15 +413,14 @@
 
 
 def optimize_bs(
     new_state: npt.NDArray[np.complex64],
     visibility_state: npt.NDArray[np.complex64],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex64]:
     """Run the minimization algorithm to optimize the biseparable state.
 
     Parameters
     ----------
     new_state : npt.NDArray[np.complex64]
         Randomly drawn state to be optimized.
@@ -440,39 +438,117 @@
     npt.NDArray[np.complex64]
         Optimized state.
 
     """
     assert_dtype(new_state, np.complex64)
     assert_dtype(visibility_state, np.complex64)
 
-    pp1 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
     return_state = new_state.copy()
 
-    for index in range(updates_count):
+    for index in range(5 * depth * quantity):
         if index % 2:
             unitary = random_unitary_bs(depth, quantity)
         else:
             unitary = random_unitary_bs_reverse(depth, quantity)
         assert_dtype(unitary, np.complex64)
 
         return_state = rotate(new_state, unitary)
         assert_dtype(return_state, np.complex64)
 
-        if pp1 > product(return_state, visibility_state):
+        if loss > product(return_state, visibility_state):
             unitary = unitary.conj().T
             return_state = rotate(new_state, unitary)
             assert_dtype(return_state, np.complex64)
 
-        pp2 = product(return_state, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        while pp2 > pp1:
-            pp1 = pp2
+        while new_loss > loss:
+            loss = new_loss
             return_state = rotate(return_state, unitary)
-            pp2 = product(return_state, visibility_state)
+            new_loss = product(return_state, visibility_state)
             assert_dtype(return_state, np.complex64)
 
         assert_dtype(return_state, np.complex64)
 
     assert_dtype(return_state, np.complex64)
 
     return return_state
+
+
+#    ███████   █████▄   ██████     █████    ███████   ██████▄    ██████    ██████
+#   ██             ██   ██   ██   ██   ██   ██             ██   ██    ██   ██   ██
+#   ██   ███   █████    ██████    ███████   █████      █████    ██    ██   ██   ██
+#   ██    ██       ██   ██        ██   ██   ██             ██   ██ ▄▄ ██   ██   ██
+#    ███████   █████▀   ██        ██   ██   ███████   ██████▀    ██████    ██████
+#                                                                   ▀▀
+
+
+def random_3p(
+    depth: int,
+    swaps: list[npt.NDArray[np.complex64]],
+    index: int,
+) -> npt.NDArray[np.complex64]:
+    """Draw random biseparable state."""
+    if index == 0:
+        return random_bs(depth, depth * depth)  # type: ignore[no-any-return]
+    if index == 1:
+        return rotate(  # type: ignore[no-any-return]
+            random_bs(depth, depth * depth),
+            swaps[0],
+        )
+
+    return random_bs(depth * depth, depth)  # type: ignore[no-any-return]
+
+
+OPTIMIZE_3P_OPT_0 = 0
+OPTIMIZE_3P_OPT_1 = 1
+OPTIMIZE_3P_OPT_2 = 2
+
+
+OPTIMIZE_3P_JUMP_TABLE = [random_unitary_bs, random_unitary_bs_reverse]
+
+
+def optimize_3p(
+    new_state: npt.NDArray[np.complex64],
+    visibility_state: npt.NDArray[np.complex64],
+    depth: int,
+    swaps: list[npt.NDArray[np.complex64]],
+    index: int,
+) -> npt.NDArray[np.complex64]:
+    return_state = new_state.copy()
+    loss = product(new_state, visibility_state)
+
+    for i in range(5 * depth**6):
+        if index == OPTIMIZE_3P_OPT_0:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+
+        elif index == OPTIMIZE_3P_OPT_1:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+            unitary = rotate(unitary, swaps[0])
+
+        elif index == OPTIMIZE_3P_OPT_2:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth * depth, depth)
+
+        else:
+            raise AssertionError(index)
+
+        return_state = rotate(new_state, unitary)
+
+        new_loss = product(return_state, visibility_state)
+
+        if loss > new_loss:
+            unitary = unitary.conj().T
+            return_state = rotate(new_state, unitary)
+            new_loss = product(return_state, visibility_state)
+
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+            assert_dtype(return_state, np.complex64)
+            new_loss = product(return_state, visibility_state)
+
+        assert_dtype(return_state, np.complex64)
+
+    assert_dtype(return_state, np.complex64)
+    return return_state  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/__init__.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_jit/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/_complex128.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy/_complex128.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
-from numba import jit, types  # type: ignore[attr-defined]
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
 
 #    █████  ██████  ███    ███ ███    ███  ██████  ███    ██
 #   ██     ██    ██ ████  ████ ████  ████ ██    ██ ████   ██
@@ -56,67 +55,61 @@
 
 
 _REAL = np.cos(0.01 * np.pi)
 _IMAG = 1j * np.sin(0.01 * np.pi)
 _VALUE = (_REAL + _IMAG - 1).astype(np.complex128)
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def product(
     matrix1: npt.NDArray[np.complex128], matrix2: npt.NDArray[np.complex128]
 ) -> np.float64:
     """Calculate scalar product of two matrices."""
     retval = np.trace(np.dot(matrix1, matrix2)).real
 
     return retval  # type: ignore[no-any-return]
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def get_random_haar_1d(depth: int) -> npt.NDArray[np.complex128]:
     """Generate a random vector with Haar measure."""
     real = np.random.uniform(0, 1, depth)  # noqa: NPY002
     imag = np.random.uniform(0, 1, depth)  # noqa: NPY002
 
     retval = np.exp(2 * np.pi * 1j * real) * np.sqrt(-np.log(imag))
 
     return retval  # type: ignore[no-any-return]
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def get_random_haar_2d(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Generate multiple random vectors with Haar measure in form of matrix."""
     real = np.random.uniform(0, 1, (quantity, depth))  # noqa: NPY002
     imag = np.random.uniform(0, 1, (quantity, depth))  # noqa: NPY002
 
     retval = np.exp(2 * np.pi * 1j * real) * np.sqrt(-np.log(imag))
 
     return retval  # type: ignore[no-any-return]
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def normalize(mtx: npt.NDArray[np.complex128]) -> npt.NDArray[np.complex128]:
     """Normalize a vector."""
     mtx2 = np.dot(mtx, np.conj(mtx))
 
     val = np.sqrt(np.real(mtx2))
 
     retval = mtx / val
 
     return retval  # type: ignore[no-any-return]
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def project(mtx1: npt.NDArray[np.complex128]) -> npt.NDArray[np.complex128]:
     """Build a projection from a vector."""
     retval = np.outer(mtx1, np.conj(mtx1))
 
     return retval  # type: ignore[no-any-return]
 
 
-@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def kronecker(
     mtx: npt.NDArray[np.complex128], mtx1: npt.NDArray[np.complex128]
 ) -> npt.NDArray[np.complex128]:
     """Kronecker Product."""
     ddd1 = len(mtx)
     ddd2 = len(mtx1)
 
@@ -127,30 +120,28 @@
     out_mtx = np.swapaxes(dot_0_1, 1, 2)
 
     retval = out_mtx.reshape(output_shape).astype(np.complex128, copy=False)
 
     return retval  # type: ignore[no-any-return]
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def rotate(
     rho2: npt.NDArray[np.complex128], unitary: npt.NDArray[np.complex128]
 ) -> npt.NDArray[np.complex128]:
     """Sandwich an operator with a unitary."""
     rho2a = np.dot(rho2, np.conj(unitary).T)  # matmul replaced with dot
 
     rho2a = np.dot(unitary, rho2a)  # matmul replaced with dot
 
     return rho2a  # type: ignore[no-any-return]
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def apply_symmetries(
     rho: npt.NDArray[np.complex128],
-    symmetries: types.ListType[types.ListType[npt.NDArray[np.complex128]]],
+    symmetries: list[list[npt.NDArray[np.complex128]]],
 ) -> npt.NDArray[np.complex128]:
     """Apply symmetries to density matrix.
 
     Parameters
     ----------
     rho : npt.NDArray[np.complex128]
         Density matrix to which we want to apply symmetries.
@@ -183,77 +174,72 @@
 #   ██████     ███████    ███████            ███    ███     ██████     ██████     ███████   # noqa: E501
 #   ██   ██    ██         ██                 ████  ████    ██    ██    ██   ██    ██        # noqa: E501
 #   ██   ██    █████      ███████            ██ ████ ██    ██    ██    ██   ██    █████     # noqa: E501
 #   ██   ██    ██              ██            ██  ██  ██    ██    ██    ██   ██    ██        # noqa: E501
 #   ██████     ██         ███████            ██      ██     ██████     ██████     ███████   # noqa: E501
 
 
-@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def optimize_d_fs(
     new_state: npt.NDArray[np.complex128],
     visibility_state: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex128]:
     """Optimize implementation for FSnQd mode."""
-    product_2_3 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
-    # To make sure rotated_2 is not unbound
+    # To make sure return_state is not unbound
     unitary = random_unitary_d_fs(depth, quantity, 0)
 
-    rotated_2 = rotate(new_state, unitary)
+    return_state = rotate(new_state, unitary)
 
-    for idx in range(updates_count):
+    for idx in range(20 * depth * depth * quantity):
         idx_mod = idx % int(quantity)
         unitary = random_unitary_d_fs(depth, quantity, idx_mod)
 
-        rotated_2 = rotate(new_state, unitary)
+        return_state = rotate(new_state, unitary)
 
-        product_rot2_3 = product(rotated_2, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        if product_2_3 > product_rot2_3:
+        if loss > new_loss:
             unitary = unitary.conj().T
-            rotated_2 = rotate(new_state, unitary)
+            return_state = rotate(new_state, unitary)
 
-        while product_rot2_3 > product_2_3:
-            product_2_3 = product_rot2_3
-            rotated_2 = rotate(rotated_2, unitary)
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
 
-            product_rot2_3 = product(rotated_2, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
-    return rotated_2.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
+    return return_state.astype(np.complex128, copy=False)  # type: ignore[no-any-return]
 
 
-@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def random_unitary_d_fs(
     depth: int, quantity: int, idx: int
 ) -> npt.NDArray[np.complex128]:
     """N quDits."""
     value = _random_unitary_d_fs(depth)
 
     mtx = expand_d_fs(value, depth, quantity, idx)
 
     return mtx  # type: ignore[no-any-return]
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def _random_unitary_d_fs(depth: int) -> npt.NDArray[np.complex128]:
     random_mtx = random_d_fs(depth, 1)
 
     identity_mtx = np.identity(depth).astype(np.complex128)
 
     rand_mul = np.multiply(_VALUE, random_mtx)
 
     value = np.add(rand_mul, identity_mtx)
 
     return value  # type: ignore[no-any-return]
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def random_d_fs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Random n quDit state."""
     rand_vectors = get_random_haar_2d(depth, quantity)
     vector = normalize(rand_vectors[0])
 
     for i in range(1, quantity):
         idx_vector = normalize(rand_vectors[i])
@@ -261,15 +247,14 @@
         vector = np.outer(vector, idx_vector).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
 
 
-@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def expand_d_fs(
     value: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
     idx: int,
 ) -> npt.NDArray[np.complex128]:
     """Expand an operator to n quDits."""
@@ -289,28 +274,26 @@
 #   ██████     ███████            ███    ███     ██████     ██████     ███████
 #   ██   ██    ██                 ████  ████    ██    ██    ██   ██    ██
 #   ██████     ███████            ██ ████ ██    ██    ██    ██   ██    █████
 #   ██   ██         ██            ██  ██  ██    ██    ██    ██   ██    ██
 #   ██████     ███████            ██      ██     ██████     ██████     ███████
 
 
-@jit(nopython=True, nogil=True, cache=True)
 def random_bs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Draw random biseparable state."""
     random_vector_1 = normalize(get_random_haar_1d(depth))
     random_vector_2 = normalize(get_random_haar_1d(quantity))
 
     vector = np.outer(random_vector_1, random_vector_2).flatten()
 
     vector = project(vector)
 
     return vector  # type: ignore[no-any-return]
 
 
-@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def random_unitary_bs(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
 
     random_matrix = project(random_vector)
 
     identity_depth = np.identity(depth).astype(np.complex128)
@@ -320,16 +303,15 @@
     unitary_biseparable = _VALUE * random_matrix + identity_depth
 
     retval = kronecker(unitary_biseparable, identity_quantity)
 
     return retval  # type: ignore[no-any-return]
 
 
-@jit(nopython=False, forceobj=True, cache=True, looplift=False)
-def random_unitary_bs_reverse(depth: int, quantity: int) -> npt.NDArray[np.complex128]:
+def random_unitary_bs_reverse(quantity: int, depth: int) -> npt.NDArray[np.complex128]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
 
     random_matrix = project(random_vector)
 
     identity_depth = np.identity(depth).astype(np.complex128)
 
@@ -338,21 +320,19 @@
     unitary_biseparable = _VALUE * random_matrix + identity_depth
 
     retval = kronecker(identity_quantity, unitary_biseparable)
 
     return retval  # type: ignore[no-any-return]
 
 
-@jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def optimize_bs(
     new_state: npt.NDArray[np.complex128],
     visibility_state: npt.NDArray[np.complex128],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex128]:
     """Run the minimization algorithm to optimize the biseparable state.
 
     Parameters
     ----------
     new_state : npt.NDArray[np.complex128]
         Randomly drawn state to be optimized.
@@ -367,31 +347,103 @@
 
     Returns
     -------
     npt.NDArray[np.complex128]
         Optimized state.
 
     """
-    pp1 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
     return_state = new_state.copy()
 
-    for index in range(updates_count):
+    for index in range(5 * depth * quantity):
         if index % 2:
             unitary = random_unitary_bs(depth, quantity)
         else:
             unitary = random_unitary_bs_reverse(depth, quantity)
 
         return_state = rotate(new_state, unitary)
 
-        if pp1 > product(return_state, visibility_state):
+        if loss > product(return_state, visibility_state):
             unitary = unitary.conj().T
             return_state = rotate(new_state, unitary)
 
-        pp2 = product(return_state, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        while pp2 > pp1:
-            pp1 = pp2
+        while new_loss > loss:
+            loss = new_loss
             return_state = rotate(return_state, unitary)
-            pp2 = product(return_state, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
     return return_state
+
+
+#    ███████   █████▄   ██████     █████    ███████   ██████▄    ██████    ██████
+#   ██             ██   ██   ██   ██   ██   ██             ██   ██    ██   ██   ██
+#   ██   ███   █████    ██████    ███████   █████      █████    ██    ██   ██   ██
+#   ██    ██       ██   ██        ██   ██   ██             ██   ██ ▄▄ ██   ██   ██
+#    ███████   █████▀   ██        ██   ██   ███████   ██████▀    ██████    ██████
+#                                                                   ▀▀
+
+
+def random_3p(
+    depth: int,
+    swaps: list[npt.NDArray[np.complex128]],
+    index: int,
+) -> npt.NDArray[np.complex128]:
+    """Draw random biseparable state."""
+    if index == 0:
+        return random_bs(depth, depth * depth)  # type: ignore[no-any-return]
+    if index == 1:
+        return rotate(  # type: ignore[no-any-return]
+            random_bs(depth, depth * depth),
+            swaps[0],
+        )
+
+    return random_bs(depth * depth, depth)  # type: ignore[no-any-return]
+
+
+OPTIMIZE_3P_OPT_0 = 0
+OPTIMIZE_3P_OPT_1 = 1
+OPTIMIZE_3P_OPT_2 = 2
+
+
+OPTIMIZE_3P_JUMP_TABLE = [random_unitary_bs, random_unitary_bs_reverse]
+
+
+def optimize_3p(
+    new_state: npt.NDArray[np.complex128],
+    visibility_state: npt.NDArray[np.complex128],
+    depth: int,
+    swaps: list[npt.NDArray[np.complex128]],
+    index: int,
+) -> npt.NDArray[np.complex128]:
+    return_state = new_state.copy()
+    loss = product(new_state, visibility_state)
+
+    for i in range(5 * depth**6):
+        if index == OPTIMIZE_3P_OPT_0:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+
+        elif index == OPTIMIZE_3P_OPT_1:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+            unitary = rotate(unitary, swaps[0])
+
+        elif index == OPTIMIZE_3P_OPT_2:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth * depth, depth)
+
+        return_state = rotate(new_state, unitary)
+
+        new_loss = product(return_state, visibility_state)
+
+        if loss > new_loss:
+            unitary = unitary.conj().T
+            return_state = rotate(new_state, unitary)
+            new_loss = product(return_state, visibility_state)
+
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+
+            new_loss = product(return_state, visibility_state)
+
+    return return_state  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.4.0/cssfinder_backend_numpy/numpy_jit/_complex64.py` & `cssfinder_backend_numpy-0.5.0/cssfinder_backend_numpy/numpy_jit/_complex64.py`

 * *Files 14% similar despite different names*

```diff
@@ -193,43 +193,42 @@
 
 @jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def optimize_d_fs(
     new_state: npt.NDArray[np.complex64],
     visibility_state: npt.NDArray[np.complex64],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex64]:
     """Optimize implementation for FSnQd mode."""
-    product_2_3 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
-    # To make sure rotated_2 is not unbound
+    # To make sure return_state is not unbound
     unitary = random_unitary_d_fs(depth, quantity, 0)
 
-    rotated_2 = rotate(new_state, unitary)
+    return_state = rotate(new_state, unitary)
 
-    for idx in range(updates_count):
+    for idx in range(20 * depth * depth * quantity):
         idx_mod = idx % int(quantity)
         unitary = random_unitary_d_fs(depth, quantity, idx_mod)
 
-        rotated_2 = rotate(new_state, unitary)
+        return_state = rotate(new_state, unitary)
 
-        product_rot2_3 = product(rotated_2, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        if product_2_3 > product_rot2_3:
+        if loss > new_loss:
             unitary = unitary.conj().T
-            rotated_2 = rotate(new_state, unitary)
+            return_state = rotate(new_state, unitary)
 
-        while product_rot2_3 > product_2_3:
-            product_2_3 = product_rot2_3
-            rotated_2 = rotate(rotated_2, unitary)
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
 
-            product_rot2_3 = product(rotated_2, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
-    return rotated_2.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
+    return return_state.astype(np.complex64, copy=False)  # type: ignore[no-any-return]
 
 
 @jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def random_unitary_d_fs(
     depth: int, quantity: int, idx: int
 ) -> npt.NDArray[np.complex64]:
     """N quDits."""
@@ -325,15 +324,15 @@
 
     retval = kronecker(unitary_biseparable, identity_quantity)
 
     return retval  # type: ignore[no-any-return]
 
 
 @jit(nopython=False, forceobj=True, cache=True, looplift=False)
-def random_unitary_bs_reverse(depth: int, quantity: int) -> npt.NDArray[np.complex64]:
+def random_unitary_bs_reverse(quantity: int, depth: int) -> npt.NDArray[np.complex64]:
     """Draw random unitary for biseparable state."""
     random_vector = normalize(get_random_haar_1d(depth))
 
     random_matrix = project(random_vector)
 
     identity_depth = np.identity(depth).astype(np.complex64)
 
@@ -348,15 +347,14 @@
 
 @jit(nopython=False, forceobj=True, cache=True, looplift=False)
 def optimize_bs(
     new_state: npt.NDArray[np.complex64],
     visibility_state: npt.NDArray[np.complex64],
     depth: int,
     quantity: int,
-    updates_count: int,
 ) -> npt.NDArray[np.complex64]:
     """Run the minimization algorithm to optimize the biseparable state.
 
     Parameters
     ----------
     new_state : npt.NDArray[np.complex64]
         Randomly drawn state to be optimized.
@@ -371,31 +369,105 @@
 
     Returns
     -------
     npt.NDArray[np.complex64]
         Optimized state.
 
     """
-    pp1 = product(new_state, visibility_state)
+    loss = product(new_state, visibility_state)
 
     return_state = new_state.copy()
 
-    for index in range(updates_count):
+    for index in range(5 * depth * quantity):
         if index % 2:
             unitary = random_unitary_bs(depth, quantity)
         else:
             unitary = random_unitary_bs_reverse(depth, quantity)
 
         return_state = rotate(new_state, unitary)
 
-        if pp1 > product(return_state, visibility_state):
+        if loss > product(return_state, visibility_state):
             unitary = unitary.conj().T
             return_state = rotate(new_state, unitary)
 
-        pp2 = product(return_state, visibility_state)
+        new_loss = product(return_state, visibility_state)
 
-        while pp2 > pp1:
-            pp1 = pp2
+        while new_loss > loss:
+            loss = new_loss
             return_state = rotate(return_state, unitary)
-            pp2 = product(return_state, visibility_state)
+            new_loss = product(return_state, visibility_state)
 
     return return_state
+
+
+#    ███████   █████▄   ██████     █████    ███████   ██████▄    ██████    ██████
+#   ██             ██   ██   ██   ██   ██   ██             ██   ██    ██   ██   ██
+#   ██   ███   █████    ██████    ███████   █████      █████    ██    ██   ██   ██
+#   ██    ██       ██   ██        ██   ██   ██             ██   ██ ▄▄ ██   ██   ██
+#    ███████   █████▀   ██        ██   ██   ███████   ██████▀    ██████    ██████
+#                                                                   ▀▀
+
+
+@jit(nopython=True, nogil=True, cache=True)
+def random_3p(
+    depth: int,
+    swaps: types.ListType[npt.NDArray[np.complex64]],
+    index: int,
+) -> npt.NDArray[np.complex64]:
+    """Draw random biseparable state."""
+    if index == 0:
+        return random_bs(depth, depth * depth)  # type: ignore[no-any-return]
+    if index == 1:
+        return rotate(  # type: ignore[no-any-return]
+            random_bs(depth, depth * depth),
+            swaps[0],
+        )
+
+    return random_bs(depth * depth, depth)  # type: ignore[no-any-return]
+
+
+OPTIMIZE_3P_OPT_0 = 0
+OPTIMIZE_3P_OPT_1 = 1
+OPTIMIZE_3P_OPT_2 = 2
+
+
+OPTIMIZE_3P_JUMP_TABLE = [random_unitary_bs, random_unitary_bs_reverse]
+
+
+@jit(nopython=False, forceobj=True, cache=True, looplift=False)
+def optimize_3p(
+    new_state: npt.NDArray[np.complex64],
+    visibility_state: npt.NDArray[np.complex64],
+    depth: int,
+    swaps: types.ListType[npt.NDArray[np.complex64]],
+    index: int,
+) -> npt.NDArray[np.complex64]:
+    return_state = new_state.copy()
+    loss = product(new_state, visibility_state)
+
+    for i in range(5 * depth**6):
+        if index == OPTIMIZE_3P_OPT_0:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+
+        elif index == OPTIMIZE_3P_OPT_1:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth, depth * depth)
+            unitary = rotate(unitary, swaps[0])
+
+        elif index == OPTIMIZE_3P_OPT_2:
+            unitary = OPTIMIZE_3P_JUMP_TABLE[i % 2](depth * depth, depth)
+
+        return_state = rotate(new_state, unitary)
+
+        new_loss = product(return_state, visibility_state)
+
+        if loss > new_loss:
+            unitary = unitary.conj().T
+            return_state = rotate(new_state, unitary)
+            new_loss = product(return_state, visibility_state)
+
+        while new_loss > loss:
+            loss = new_loss
+            return_state = rotate(return_state, unitary)
+
+            new_loss = product(return_state, visibility_state)
+
+    return return_state  # type: ignore[no-any-return]
```

### Comparing `cssfinder_backend_numpy-0.4.0/pyproject.toml` & `cssfinder_backend_numpy-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry] # ANCHOR: tool.poetry
 name = "cssfinder_backend_numpy"
-version = "0.4.0"
+version = "0.5.0"
 description = "Implementation of CSSFinder backend using NumPy library."
 authors = [
     "Krzysztof Wiśniewski <argmaster.world@gmail.com>",
     "Marcin Wieśniak <marcin.wiesniak@ug.edu.pl>",
 ]
 repository = "https://github.com/argmaster/cssfinder_backend_numpy"
 readme = "README.md"
@@ -54,16 +54,15 @@
     { cmd = "pre-commit run --all-files -v" },
 ]
 build = [
     { cmd = "poetry build --format=wheel --no-ansi" },
     { cmd = "poetry build --format=sdist --no-ansi" },
 ]
 gen-numpy-impl = { script = "scripts.gen_numpy_impl:main" }
-test-system = { cmd = "pytest test/test_system -v --cov" }
-test-reports = { cmd = "pytest test/test_reports -v --cov" }
+test-unit = { cmd = "pytest test -v --cov" }
 type-check = [
     { cmd = "poetry install --sync --no-ansi" },
     { cmd = "mypy cssfinder_backend_numpy test scripts" },
 ]
 
 [build-system]
 requires = ["poetry-core", "cython>=3.0.0b1", "setuptools>=67.0.0,<68.0.0"]
```

### Comparing `cssfinder_backend_numpy-0.4.0/PKG-INFO` & `cssfinder_backend_numpy-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssfinder-backend-numpy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Implementation of CSSFinder backend using NumPy library.
 Home-page: https://github.com/argmaster/cssfinder_backend_numpy
 Author: Krzysztof Wiśniewski
 Author-email: argmaster.world@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -87,36 +87,36 @@
 
 ```
 poe build
 ```
 
 ![poe_build](https://user-images.githubusercontent.com/56170852/223251363-61fc4d00-68ad-429c-9fbb-8ab7f4712451.png)
 
-This will create `dist/` directory with `cssfinder_backend_numpy-0.4.0` or
+This will create `dist/` directory with `cssfinder_backend_numpy-0.5.0` or
 alike inside.
 
 Wheel file can be installed with
 
 ```
-pip install ./dist/cssfinder_backend_numpy-0.4.0
+pip install ./dist/cssfinder_backend_numpy-0.5.0
 ```
 
 What you expect is
 
 ```
-Successfully installed cssfinder_backend_numpy-0.4.0
+Successfully installed cssfinder_backend_numpy-0.5.0
 ```
 
 or rather something like
 
 ```
-Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder_backend_numpy-0.4.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
+Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder_backend_numpy-0.5.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
 ```
 
-But `cssfinder_backend_numpy-0.4.0` should be included in this list.
+But `cssfinder_backend_numpy-0.5.0` should be included in this list.
 
 ## Code quality
 
 To ensure that all code follow same style guidelines and code quality rules,
 multiple static analysis tools are used. For simplicity, all of them are
 configured as `pre-commit` ([learn about pre-commit](https://pre-commit.com/))
 hooks. Most of them however are listed as development dependencies.
```

