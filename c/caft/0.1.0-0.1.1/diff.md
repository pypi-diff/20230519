# Comparing `tmp/caft-0.1.0.tar.gz` & `tmp/caft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caft-0.1.0.tar", last modified: Thu May 18 17:51:00 2023, max compression
+gzip compressed data, was "caft-0.1.1.tar", last modified: Thu May 18 19:38:29 2023, max compression
```

## Comparing `caft-0.1.0.tar` & `caft-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 17:51:00.544050 caft-0.1.0/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1068 2023-05-05 11:28:23.000000 caft-0.1.0/LICENSE
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)      100 2023-05-17 23:40:59.000000 caft-0.1.0/MANIFEST.in
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)    11719 2023-05-18 17:51:00.544153 caft-0.1.0/PKG-INFO
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)    10659 2023-05-18 17:49:25.000000 caft-0.1.0/README.md
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 17:51:00.540488 caft-0.1.0/caft/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)       22 2023-05-05 11:28:23.000000 caft-0.1.0/caft/__init__.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1609 2023-05-17 21:50:03.000000 caft-0.1.0/caft/affine.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     7340 2023-05-17 09:20:27.000000 caft-0.1.0/caft/equation.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     3885 2023-05-17 20:49:12.000000 caft-0.1.0/caft/npoc.py
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 17:51:00.542088 caft-0.1.0/caft.egg-info/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)    11719 2023-05-18 17:51:00.000000 caft-0.1.0/caft.egg-info/PKG-INFO
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)      407 2023-05-18 17:51:00.000000 caft-0.1.0/caft.egg-info/SOURCES.txt
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)        1 2023-05-18 17:51:00.000000 caft-0.1.0/caft.egg-info/dependency_links.txt
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)       70 2023-05-18 17:51:00.000000 caft-0.1.0/caft.egg-info/requires.txt
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)       11 2023-05-18 17:51:00.000000 caft-0.1.0/caft.egg-info/top_level.txt
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)       98 2023-05-05 11:28:23.000000 caft-0.1.0/pyproject.toml
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)      107 2023-05-18 17:51:00.544476 caft-0.1.0/setup.cfg
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1941 2023-05-17 22:31:58.000000 caft-0.1.0/setup.py
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 17:51:00.542295 caft-0.1.0/tests/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)        0 2023-05-05 11:28:23.000000 caft-0.1.0/tests/__init__.py
-drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 17:51:00.543755 caft-0.1.0/tests/tests_caft/
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)        0 2023-05-16 22:01:44.000000 caft-0.1.0/tests/tests_caft/__init__.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)      912 2023-05-17 21:37:54.000000 caft-0.1.0/tests/tests_caft/test_affine.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1539 2023-05-17 23:51:25.000000 caft-0.1.0/tests/tests_caft/test_equation.py
--rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1528 2023-05-17 20:25:03.000000 caft-0.1.0/tests/tests_caft/test_npoc.py
+drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.633545 caft-0.1.1/
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1068 2023-05-05 11:28:23.000000 caft-0.1.1/LICENSE
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)      129 2023-05-18 19:27:10.000000 caft-0.1.1/MANIFEST.in
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     4313 2023-05-18 19:38:29.633653 caft-0.1.1/PKG-INFO
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     3253 2023-05-18 18:47:12.000000 caft-0.1.1/README.md
+drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.629586 caft-0.1.1/caft/
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)       22 2023-05-18 19:31:17.000000 caft-0.1.1/caft/__init__.py
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1609 2023-05-17 21:50:03.000000 caft-0.1.1/caft/affine.py
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     7340 2023-05-17 09:20:27.000000 caft-0.1.1/caft/equation.py
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     3885 2023-05-17 20:49:12.000000 caft-0.1.1/caft/npoc.py
+drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.631045 caft-0.1.1/caft.egg-info/
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     4313 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/PKG-INFO
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)      466 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/SOURCES.txt
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)        1 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/dependency_links.txt
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)       70 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/requires.txt
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)       11 2023-05-18 19:38:29.000000 caft-0.1.1/caft.egg-info/top_level.txt
+drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.631460 caft-0.1.1/img/
+-rw-------   0 Josh.Dunn   (504) staff       (20)    42606 2023-05-18 18:39:36.000000 caft-0.1.1/img/affine_transformed_scatter.png
+-rw-------   0 Josh.Dunn   (504) staff       (20)    22050 2023-05-18 18:34:12.000000 caft-0.1.1/img/fx_scatter_plot.png
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)       98 2023-05-05 11:28:23.000000 caft-0.1.1/pyproject.toml
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)      107 2023-05-18 19:38:29.633954 caft-0.1.1/setup.cfg
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1941 2023-05-17 22:31:58.000000 caft-0.1.1/setup.py
+drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.632084 caft-0.1.1/tests/
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)        0 2023-05-05 11:28:23.000000 caft-0.1.1/tests/__init__.py
+drwxr-xr-x   0 Josh.Dunn   (504) staff       (20)        0 2023-05-18 19:38:29.633189 caft-0.1.1/tests/tests_caft/
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)        0 2023-05-16 22:01:44.000000 caft-0.1.1/tests/tests_caft/__init__.py
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)      912 2023-05-17 21:37:54.000000 caft-0.1.1/tests/tests_caft/test_affine.py
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1627 2023-05-18 18:27:26.000000 caft-0.1.1/tests/tests_caft/test_equation.py
+-rw-r--r--   0 Josh.Dunn   (504) staff       (20)     1528 2023-05-17 20:25:03.000000 caft-0.1.1/tests/tests_caft/test_npoc.py
```

### Comparing `caft-0.1.0/LICENSE` & `caft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caft-0.1.0/caft/affine.py` & `caft-0.1.1/caft/affine.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.0/caft/equation.py` & `caft-0.1.1/caft/equation.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.0/caft/npoc.py` & `caft-0.1.1/caft/npoc.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.0/setup.py` & `caft-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.0/tests/tests_caft/test_affine.py` & `caft-0.1.1/tests/tests_caft/test_affine.py`

 * *Files identical despite different names*

### Comparing `caft-0.1.0/tests/tests_caft/test_equation.py` & `caft-0.1.1/tests/tests_caft/test_equation.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,29 +23,36 @@
 def test_sympy_function_regressor():
     """Test sympy function regressor."""
     sodr = SympyODRegressor("a*x**2 + b", beta0={"a": 3, "b": 5})
     X = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]).reshape(-1, 1)
     y = 5 * X ** 2 + 10
     sodr.fit(X, y)
     y_pred = sodr.predict(X)
+    wrt = sp.Symbol('x')
+
+    check_sp_equation = sodr.beta[0] * wrt ** 2 + sodr.beta[1]
 
     assert sodr.beta == pytest.approx([5, 10], rel=1e-3)
-    # assert sympy_approx_equals(sodr.sp_equation, 5 * sodr.wrt_symbol ** 2 + 10)
+    assert sodr.sp_equation == check_sp_equation
     assert sodr.wrt_symbol == sp.Symbol("x")
     assert y_pred == pytest.approx(y.reshape(-1), rel=1e-3)
 
 
 def test_odregressor():
     """Test odr regressor."""
     odr = ODRegressor(degree=2, wrt='s')
     X = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]).reshape(-1, 1)
     y = (5 * X ** 2) + (2 * X) + 10
     odr.fit(X, y)
     y_pred = odr.predict(X)
     wrt = sp.Symbol('s')
 
-    check_sp_equation = (5.0 * wrt ** 2) + (2.0 * wrt) + 10.0
+    check_sp_equation = (
+        odr.beta[2] * wrt ** 2
+        + (odr.beta[1] * wrt)
+        + odr.beta[0]
+    )
 
     assert odr.beta == pytest.approx([10, 2, 5], rel=1e-3)
-    # assert sympy_approx_equals(odr.sp_equation, check_sp_equation)
+    assert odr.sp_equation == check_sp_equation
     assert odr.wrt_symbol == sp.Symbol("s")
     assert y_pred == pytest.approx(y.reshape(-1), rel=1e-3)
```

### Comparing `caft-0.1.0/tests/tests_caft/test_npoc.py` & `caft-0.1.1/tests/tests_caft/test_npoc.py`

 * *Files identical despite different names*

