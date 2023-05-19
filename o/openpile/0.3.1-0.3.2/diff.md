# Comparing `tmp/openpile-0.3.1.tar.gz` & `tmp/openpile-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-8svl9kor/openpile-0.3.1.tar", last modified: Tue May 16 18:48:55 2023, max compression
+gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-ptali4vv/openpile-0.3.2.tar", last modified: Thu May 18 21:04:44 2023, max compression
```

## Comparing `openpile-0.3.1.tar` & `openpile-0.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 18:48:46.000000 openpile-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-16 18:48:55.000000 openpile-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-16 18:48:46.000000 openpile-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 18:48:46.000000 openpile-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-16 18:48:55.000000 openpile-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-16 18:48:46.000000 openpile-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)    54305 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/soilmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/Hb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/Mb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/mt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/py_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/qz_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/tz_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-16 18:48:46.000000 openpile-0.3.1/test/test_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-16 18:48:46.000000 openpile-0.3.1/test/test_pycurves.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-16 18:48:46.000000 openpile-0.3.1/test/test_utils_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:44.000000 openpile-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 21:04:35.000000 openpile-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-18 21:04:44.000000 openpile-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-18 21:04:35.000000 openpile-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-18 21:04:35.000000 openpile-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-18 21:04:44.000000 openpile-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-18 21:04:35.000000 openpile-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:44.000000 openpile-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54305 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29182 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/core/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/core/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/core/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/soilmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/utils/Hb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/utils/Mb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/utils/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/utils/mt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/utils/py_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/utils/qz_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-18 21:04:35.000000 openpile-0.3.2/src/openpile/utils/tz_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 21:04:44.000000 openpile-0.3.2/src/openpile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:04:44.000000 openpile-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-18 21:04:35.000000 openpile-0.3.2/test/test_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-18 21:04:35.000000 openpile-0.3.2/test/test_pycurves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 21:04:35.000000 openpile-0.3.2/test/test_utils_misc.py
```

### Comparing `openpile-0.3.1/LICENSE.txt` & `openpile-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/PKG-INFO` & `openpile-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
```

### Comparing `openpile-0.3.1/README.md` & `openpile-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/setup.cfg` & `openpile-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/setup.py` & `openpile-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/analyses.py` & `openpile-0.3.2/src/openpile/analyses.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/construct.py` & `openpile-0.3.2/src/openpile/construct.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/core/kernel.py` & `openpile-0.3.2/src/openpile/core/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,19 +625,21 @@
                     raise UserInputError(
                         "Error: Distributed moment cannot be calculated without distributed lateral springs."
                     )
                 k += elem_mt_stiffness_matrix(model, u, kind)
 
     K = jit_build(k, ndim_global, n_elem, node_per_element, ndof_per_node)
 
-    if model.base_shear:
-        K[-2:-2] += calculate_base_spring_stiffness(u[-2], model._Hb_spring, kind)
+    # add soil contribution
+    if model.soil is not None:
+        if model.base_shear:
+            K[-2, -2] += calculate_base_spring_stiffness(u[-2], model._Hb_spring, kind)
 
-    if model.base_moment:
-        K[-1:-1] += calculate_base_spring_stiffness(u[-1], model._Mb_spring, kind)
+        if model.base_moment:
+            K[-1, -1] += calculate_base_spring_stiffness(u[-1], model._Mb_spring, kind)
 
     return K
 
 
 def mesh_to_global_force_dof_vector(df: pd.DataFrame) -> np.ndarray:
     # extract each column (one line per node)
     force_dof_vector = df[["Px [kN]", "Py [kN]", "Mz [kNm]"]].values.reshape(-1).astype(np.float64)
@@ -671,19 +673,19 @@
         k += elem_p_delta_stiffness_matrix(model, f=f)
 
     # add soil contribution
     if model.soil is not None:
         kind = "secant"
         if model.distributed_lateral:
             k += elem_py_stiffness_matrix(model, u, kind)
-        elif model.distributed_moment:
+        if model.distributed_moment:
             k += elem_mt_stiffness_matrix(model, u, kind)
-        elif model.base_shear:
+        if model.base_shear:
             k[-1, -2, -2] += calculate_base_spring_stiffness(u[-2], model._Hb_spring, kind)
-        elif model.base_moment:
+        if model.base_moment:
             k[-1, -1, -1] += calculate_base_spring_stiffness(u[-1], model._Mb_spring, kind)
 
     # create array u of shape [n_elem x 6 x 1]
     u = global_dof_vector_to_consistent_stacked_array(u, ndof_per_node * node_per_element)
     # compute internal forces and reshape into global dof vector
     F_int = (-1) * np.matmul(k, u).reshape((-1))
```

### Comparing `openpile-0.3.1/src/openpile/core/misc.py` & `openpile-0.3.2/src/openpile/core/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,23 +128,24 @@
     x_u: float,
     n: float,
     k: float,
     y_u: float,
     output_length: int,
 ):
     # Create x vector with 10% extension
-    x = np.linspace(0, x_u, output_length - 1).astype(np.float32)
+    x = np.array([0, 0.001, 0.005, 0.01]).astype(np.float32) * x_u
+    x = np.append(x, np.linspace(0.02 * x_u, x_u, output_length - 5).astype(np.float32))
     x = np.append(x, 1.1 * x_u)
 
     a = 1 - 2 * n
 
     y = np.zeros((len(x)), dtype=np.float32)
 
     for i in range(len(x)):
-        if abs(x[i] - x_u) < 1e-4:
+        if abs(x[i] - x_u) < 1e-2:
             y[i] = y_u
         elif x[i] < x_u:
             b = 2 * n * x[i] / x_u - (1 - n) * (1 + x[i] * k / y_u)
             c = x[i] * (k / y_u) * (1 - n) - n * (x[i] ** 2 / x_u**2)
 
             y[i] = y_u * 2 * c / (-b + (b**2 - 4 * a * c) ** 0.5)
         else:
```

### Comparing `openpile-0.3.1/src/openpile/core/txt.py` & `openpile-0.3.2/src/openpile/core/txt.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/core/validation.py` & `openpile-0.3.2/src/openpile/core/validation.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/soilmodels.py` & `openpile-0.3.2/src/openpile/soilmodels.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/utils/Hb_curves.py` & `openpile-0.3.2/src/openpile/utils/Hb_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/utils/Mb_curves.py` & `openpile-0.3.2/src/openpile/utils/Mb_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/utils/graphics.py` & `openpile-0.3.2/src/openpile/utils/graphics.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/utils/mt_curves.py` & `openpile-0.3.2/src/openpile/utils/mt_curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     m_max = m_m1 + m_m2 * X / D
     psi_max = m_max / k
 
     # calculate normsalised conic function
     t, m = conic(psi_max, n, k, m_max, output_length)
 
     # return non-normalised curve
-    return m * (Su * D), t * (Su / G0)
+    return m * (Su * D**2), t * (Su / G0)
 
 
 @njit(cache=True)
 def dunkirk_sand(
     sig: float,
     X: float,
     Dr: float,
@@ -129,8 +129,8 @@
     m_max = m_u1 + m_u2 * X / L
     psi_max = m_max / k
 
     # calculate normsalised conic function
     t, m = conic(psi_max, n, k, m_max, output_length)
 
     # return non-normalised curve
-    return m * (p * D), t * (sig / G0)
+    return m * (p * D**2), t * (sig / G0)
```

### Comparing `openpile-0.3.1/src/openpile/utils/py_curves.py` & `openpile-0.3.2/src/openpile/utils/py_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/utils/qz_curves.py` & `openpile-0.3.2/src/openpile/utils/qz_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile/utils/tz_curves.py` & `openpile-0.3.2/src/openpile/utils/tz_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/src/openpile.egg-info/PKG-INFO` & `openpile-0.3.2/src/openpile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
```

### Comparing `openpile-0.3.1/src/openpile.egg-info/SOURCES.txt` & `openpile-0.3.2/src/openpile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/test/test_construct.py` & `openpile-0.3.2/test/test_construct.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/test/test_pycurves.py` & `openpile-0.3.2/test/test_pycurves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.1/test/test_utils_misc.py` & `openpile-0.3.2/test/test_utils_misc.py`

 * *Files identical despite different names*

