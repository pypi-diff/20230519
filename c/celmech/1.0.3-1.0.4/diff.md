# Comparing `tmp/celmech-1.0.3.tar.gz` & `tmp/celmech-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celmech-1.0.3.tar", last modified: Fri Aug 19 22:59:37 2022, max compression
+gzip compressed data, was "celmech-1.0.4.tar", last modified: Fri May 19 20:38:13 2023, max compression
```

## Comparing `celmech-1.0.3.tar` & `celmech-1.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2022-08-19 22:59:37.023830 celmech-1.0.3/
--rw-r--r--   0 dtamayo    (502) staff       (20)    35149 2022-08-19 22:47:33.000000 celmech-1.0.3/LICENSE
--rw-r--r--   0 dtamayo    (502) staff       (20)       87 2022-08-19 22:57:58.000000 celmech-1.0.3/MANIFEST.in
--rw-r--r--   0 dtamayo    (502) staff       (20)      815 2022-08-19 22:59:37.023568 celmech-1.0.3/PKG-INFO
--rw-r--r--   0 dtamayo    (502) staff       (20)      665 2022-08-19 22:47:33.000000 celmech-1.0.3/README.md
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2022-08-19 22:59:37.019165 celmech-1.0.3/celmech/
--rw-r--r--   0 dtamayo    (502) staff       (20)     1676 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/__init__.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    35161 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/canonical_transformations.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    48261 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/disturbing_function.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    20688 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/hamiltonian.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    18949 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/lie_transformations.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    17261 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/maps.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    20183 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/miscellaneous.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     1525 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/multiplanet_hamiltonian.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    15198 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/nbody_simulation_utilities.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    57551 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/numerical_resonance_models.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     3491 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/numerical_resonance_utils.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    17818 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/planar_poincare.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    42697 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/poincare.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     8846 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/poisson_series.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     5049 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/resonances.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     9401 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/rk_integrator.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    49307 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/secular.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    26888 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/symplectic_evolution_operators.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     3112 2022-08-19 22:47:33.000000 celmech-1.0.3/celmech/transformations.py
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2022-08-19 22:59:37.021486 celmech-1.0.3/celmech.egg-info/
--rw-r--r--   0 dtamayo    (502) staff       (20)      815 2022-08-19 22:59:36.000000 celmech-1.0.3/celmech.egg-info/PKG-INFO
--rw-r--r--   0 dtamayo    (502) staff       (20)      858 2022-08-19 22:59:37.000000 celmech-1.0.3/celmech.egg-info/SOURCES.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)        1 2022-08-19 22:59:36.000000 celmech-1.0.3/celmech.egg-info/dependency_links.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)        1 2022-08-19 22:55:59.000000 celmech-1.0.3/celmech.egg-info/not-zip-safe
--rw-r--r--   0 dtamayo    (502) staff       (20)       85 2022-08-19 22:59:36.000000 celmech-1.0.3/celmech.egg-info/requires.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)       19 2022-08-19 22:59:36.000000 celmech-1.0.3/celmech.egg-info/top_level.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)       38 2022-08-19 22:59:37.023871 celmech-1.0.3/setup.cfg
--rw-r--r--   0 dtamayo    (502) staff       (20)     3240 2022-08-19 22:58:37.000000 celmech-1.0.3/setup.py
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2022-08-19 22:59:37.023269 celmech-1.0.3/src/
--rw-r--r--   0 dtamayo    (502) staff       (20)     4286 2022-08-19 22:58:37.000000 celmech-1.0.3/src/disturbing_function.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    18820 2022-08-19 22:47:33.000000 celmech-1.0.3/src/fmft.c
--rw-r--r--   0 dtamayo    (502) staff       (20)      971 2022-08-19 22:47:33.000000 celmech-1.0.3/src/fmftPy.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     2494 2022-08-19 22:47:33.000000 celmech-1.0.3/src/nrutil.c
--rw-r--r--   0 dtamayo    (502) staff       (20)      494 2022-08-19 22:47:33.000000 celmech-1.0.3/src/nrutil.h
--rw-r--r--   0 dtamayo    (502) staff       (20)     9536 2022-08-19 22:47:33.000000 celmech-1.0.3/src/poisson_series.c
+drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-05-19 20:38:13.641662 celmech-1.0.4/
+-rw-r--r--   0 dtamayo    (502) staff       (20)    35149 2022-08-19 22:47:33.000000 celmech-1.0.4/LICENSE
+-rw-r--r--   0 dtamayo    (502) staff       (20)       87 2022-08-19 22:57:58.000000 celmech-1.0.4/MANIFEST.in
+-rw-r--r--   0 dtamayo    (502) staff       (20)      815 2023-05-19 20:38:13.641407 celmech-1.0.4/PKG-INFO
+-rw-r--r--   0 dtamayo    (502) staff       (20)      665 2022-08-19 22:47:33.000000 celmech-1.0.4/README.md
+drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-05-19 20:38:13.635088 celmech-1.0.4/celmech/
+-rw-r--r--   0 dtamayo    (502) staff       (20)     1676 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/__init__.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    35161 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/canonical_transformations.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    48262 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/disturbing_function.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    20332 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/hamiltonian.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    18949 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/lie_transformations.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    32466 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/maps.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    24890 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/miscellaneous.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)     1525 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/multiplanet_hamiltonian.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    15198 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/nbody_simulation_utilities.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    57551 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/numerical_resonance_models.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)     3491 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/numerical_resonance_utils.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    17818 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/planar_poincare.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    42697 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/poincare.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)     8846 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/poisson_series.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)     5049 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/resonances.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)     9401 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/rk_integrator.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    49319 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/secular.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)    26888 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/symplectic_evolution_operators.py
+-rw-r--r--   0 dtamayo    (502) staff       (20)     3112 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/transformations.py
+drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-05-19 20:38:13.637843 celmech-1.0.4/celmech.egg-info/
+-rw-r--r--   0 dtamayo    (502) staff       (20)      815 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/PKG-INFO
+-rw-r--r--   0 dtamayo    (502) staff       (20)      858 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/SOURCES.txt
+-rw-r--r--   0 dtamayo    (502) staff       (20)        1 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/dependency_links.txt
+-rw-r--r--   0 dtamayo    (502) staff       (20)        1 2022-08-19 22:55:59.000000 celmech-1.0.4/celmech.egg-info/not-zip-safe
+-rw-r--r--   0 dtamayo    (502) staff       (20)       85 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/requires.txt
+-rw-r--r--   0 dtamayo    (502) staff       (20)       19 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/top_level.txt
+-rw-r--r--   0 dtamayo    (502) staff       (20)       38 2023-05-19 20:38:13.641705 celmech-1.0.4/setup.cfg
+-rw-r--r--   0 dtamayo    (502) staff       (20)     3240 2023-05-19 20:37:22.000000 celmech-1.0.4/setup.py
+drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-05-19 20:38:13.640989 celmech-1.0.4/src/
+-rw-r--r--   0 dtamayo    (502) staff       (20)     4286 2023-05-19 20:37:22.000000 celmech-1.0.4/src/disturbing_function.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)    18820 2022-08-19 22:47:33.000000 celmech-1.0.4/src/fmft.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)      971 2022-08-19 22:47:33.000000 celmech-1.0.4/src/fmftPy.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)     2494 2022-08-19 22:47:33.000000 celmech-1.0.4/src/nrutil.c
+-rw-r--r--   0 dtamayo    (502) staff       (20)      494 2022-08-19 22:47:33.000000 celmech-1.0.4/src/nrutil.h
+-rw-r--r--   0 dtamayo    (502) staff       (20)     9536 2022-08-19 22:47:33.000000 celmech-1.0.4/src/poisson_series.c
```

### Comparing `celmech-1.0.3/LICENSE` & `celmech-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/PKG-INFO` & `celmech-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celmech
-Version: 1.0.3
+Version: 1.0.4
 Summary: Open source tools for celestial mechanics
 Home-page: http://github.com/shadden/celmech
 Author: Dan Tamayo, Sam Hadden
 Author-email: tamayo.daniel@gmail.com, shadden1107@gmail.com
 License: GPL
 Keywords: astronomy astrophysics celestial-mechanics orbits orbital-mechanics
 Platform: UNKNOWN
```

### Comparing `celmech-1.0.3/README.md` & `celmech-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/__init__.py` & `celmech-1.0.4/celmech/__init__.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/canonical_transformations.py` & `celmech-1.0.4/celmech/canonical_transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/disturbing_function.py` & `celmech-1.0.4/celmech/disturbing_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
                     if eccentricities == False and k_nu_depend_on_eccentricities(k_vec, nu_vec) == True:
                         continue
                     args.append((k_vec,nu_vec))
     return args
 
 def laplace_b(s,j,n,alpha):
     r"""
-    Calculates :math:`n`th derivative with respect to :math:`\alpha` of Laplace coefficient :math:`b_s^j(\alpha)`.
+    Calculates :math:`n`-th derivative with respect to :math:`\alpha` of Laplace coefficient :math:`b_s^j(\alpha)`.
     Uses recursion and scipy special functions. 
 
     Arguments
     ---------
     s : float 
         half-integer parameter of Laplace coefficient. 
     j : int
```

### Comparing `celmech-1.0.3/celmech/hamiltonian.py` & `celmech-1.0.4/celmech/hamiltonian.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,25 +445,16 @@
         self.state.t = self.integrator.t
         self.state.values = self.integrator.y
 
     def _update(self):
         self._needs_update=False # reset flag up top to avoid infinite recursion
         self._N_H = self._H # reset to Hamiltonian with all parameters unset
         # 
-        # Update raw numerical constants first then update functions
-        # Less hacky way to do this?
-        function_keyval_pairs = []
-        for key, val in self._H_params.items(): 
-            if isinstance(val,float):
-                self._N_H = self._N_H.subs(key, val)
-            else:
-                function_keyval_pairs.append((key,val)) 
-        for keyval in function_keyval_pairs:
-            self._N_H = self._N_H.subs(keyval[0],keyval[1])
-
+        # Change subs to xreplace here, Dec 7 2022
+        self._N_H = self._N_H.xreplace(self._H_params)
         qp_vars = self.qp_vars
         flow = []
         Nflow = []
         for v in self.qp_vars:
             deriv = self.Lie_deriv(v)
             Nderiv = self.N_Lie_deriv(v)
             flow.append(deriv)
```

### Comparing `celmech-1.0.3/celmech/lie_transformations.py` & `celmech-1.0.4/celmech/lie_transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/maps.py` & `celmech-1.0.4/celmech/maps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from .miscellaneous import sk,Dsk
+from sympy import totient
 
 class StandardMap():
     r"""
     A class representing the `Chirikov standard map`_.
     The map depends on a single parameter, :math:`K` 
     and is defind by
 
@@ -77,14 +78,71 @@
     def __call__(self,x):
         theta,p = x
         p1 = p + self.K * np.sin(theta)
         theta1 = theta + p1
         x1 = np.array([theta1,p1])
         x1 = self._modfn(x1)
         return x1
+    
+    def with_variational(self,X,dX):
+        r"""
+        Apply the map along with the tangent map to point plus variationals.
+        In particular, 
+
+        .. math::
+            \begin{align}
+            (\theta', w') &=& T(\theta, w) 
+            \\
+            (\delta \theta',\delta  w') &=& DT(\theta, w) \cdot (\delta \theta,\delta  w) 
+        
+        where :math:`T` is the usual map and :math:`DT` is the Jacobian of the map.
+
+        Parameters
+        ----------
+        X : array-like
+            The point :math:`X = (\theta,w)`
+        dX : array-like
+            The variational vector :math:`(\delta\theta,\delta w)`
+        
+        Returns
+        -------
+        X' : array-like
+            The new point
+        dX' : array-lke
+            The new variationl vector
+        """
+        jac = self.jac(X)
+        X1 = self.__call__(X)
+        dX1 = jac @ dX
+        return X1,dX1
+
+    def action(self,pt):
+        r"""
+        Evaluate The action zero-form,
+
+        .. math::
+        \lambda(\theta,w) = 2\pi\left(\frac{w'^2}{2}- \frac{\epsilon}{2\pi}  F_\beta(\theta)\right)~,
+
+        where :math:`w' = w - \epsilon \partial_\theta F_\beta(\theta)`. The action zero-form satisfies
+        :math:`T^*(w d\theta) - w d\theta = d\lambda` where :math:`T^*` is the pullback of the map.
+
+        Parameters
+        ----------
+        pt : array-like
+            the point :math:`(\theta,w)` at which to evlauate the action.
+
+        Returns
+        -------
+        float
+            The value of the action zero-form, :math:`\lambda(\theta,w)`
+        """
+        theta,p = pt
+        K = self.K
+        p1 = p + K * np.sin(theta)
+        return 0.5 * p1 * p1 - K * np.cos(theta)
 
     def inv(self,x):
         r"""
         The inverse mapping
 
         .. math::
             \begin{align}
@@ -211,14 +269,27 @@
         K = self.K
         Kcos = K*np.cos(theta)
         jac = np.array([
             [1 + Kcos, 1],
             [Kcos,1]
         ])
         return jac
+    def symmetry_lines(self):
+        """
+        Return the symmetry lines of the map.
+
+        Returns
+        -------
+        tuple
+            Tuple containing three functions that parameterize the symmetry lines of the map.
+        """
+        sline1 = lambda x: np.array((0,x))
+        sline2 = lambda x: np.array((np.pi,x))
+        sline3 = lambda x: np.array((0.5 * x,x))
+        return (sline1,sline2,sline3)
 
 class EncounterMap():
     r"""
     A class representing the encounter map.
     The map depends on three parameters,
     :math:`\epsilon,y`, and :math:`J`.
     The map is defined by the equations
@@ -235,16 +306,22 @@
     The parameter `mod_p=True` can be set to take the 
     :math:`p` coordinate modulo :math:`2\pi` as well.
 
     .. _Chirikov standard map: https://en.wikipedia.org/wiki/Standard_map
 
     Parameters
     ----------
-    K : float
-        Map non-linearity parameter.
+    m : float
+        Planet-star mass ratio
+    y : float
+        The eccentricity divided by the orbit-crossing eccentricity.
+    J : float
+        Center the map on the :math:`J`::math:`J-1` MMR. For integer J, the map
+        is centered on a first order MMR. For rational :math:`J=p/q`, the map is
+        centered on a :math:`q`th order MMR
     mod_theta : bool, optional
         If True, the :math:`\theta` coordinate
         is taken modulo :math:`2\pi`.
         Default is `True`
     mod_p : bool, optional
         If True, the :math:`p` coordinate
         is taken modulo :math:`2\pi`.
@@ -511,38 +588,43 @@
             if coeff==0:
                 continue
             npows = pows.shape[0]
             sub_tot += coeff * np.product(farr[:npows]**pows)
         tot+= Tprime_ij * sub_tot
     return tot
 
-def func_from_series(coeffs,x):
+from scipy.interpolate import pade as pade_approx
+def func_from_series(coeffs,x,pade=False):
     """
     Given a set of Taylor series coefficients, (c_0,....,c_N), evalute
     the sum
 
     .. math::
         \sum_{n=0}^{N} c_n x^n / n!
 
     Arguments
     ---------
     coeffs : numpy array
-        Values of Taylor series coeffieciens
+        Values of Taylor series coefficients
     x : float
         Argument of function
 
     Returns
     -------
     float
     """
-    return coeffs @ np.array([x**n/np.math.factorial(n) for n in range(coeffs.shape[0])])
+    if not pade:
+        return coeffs @ np.array([x**n/np.math.factorial(n) for n in range(coeffs.shape[0])])
+    else:
+        p,q = pade_approx(coeffs,len(coeffs)//2)
+        return p(x)/q(x)
 
-def manifold_approx(u,n,farr,garr):
-    f = lambda x: func_from_series(farr[:n+1],x)
-    g = lambda x: func_from_series(garr[:n+1],x)
+def manifold_approx(u,n,farr,garr,pade=False):
+    f = lambda x: func_from_series(farr[:n+1],x,pade)
+    g = lambda x: func_from_series(garr[:n+1],x,pade)
     p0 = np.array([u,f(u)])
     p1 = np.array([g(u),f(g(u))])
     return p0,p1
 
 def solve_manifold_f_and_g(xunst,mapobj,Nmax,unstable=True):
     r"""
     Solve for Taylor series approximations of functions
@@ -566,14 +648,19 @@
         If true, solve for the unstable manifold f and
         g functions, otherwise solve for the stable manifold
         functions.
     Returns
     -------
     R : ndarray, shape (2,2)
         Rotation matrix
+    f_arr : ndarray, shame (Nmax,)
+        Coefficients of taylor expansion for :math:`f`
+    g_arr : ndarray, shame (Nmax,)
+        Coefficients of taylor expansion for :math:`g`
+
     """
     # Array of partial derivatives up to order Nmax
     if unstable:
         T = mapobj.partial_derivs(xunst,Nmax)
     else:
         T = mapobj.inv_partial_derivs(xunst,Nmax)
     # jacobian evaluated at xunst
@@ -609,7 +696,415 @@
         PsiPerp = evaluate_Psi(Psi_dict,Tprime[1],farr)
         PsiU = evaluate_Psi(Psi_dict,Tprime[0],farr)
         denom = Tperp_01-lambdaU**n
         Bsum = _evaluate_chain_rule(n,farr,garr)
         farr[n] = (Bsum-PsiPerp)/denom
         garr[n] = TU_01 * farr[n] + PsiU
     return R, farr, garr
+
+############################################### 
+############# Comet Map Utilities ############# 
+############################################### 
+from .miscellaneous import levin_method_integrate_adaptive
+from .disturbing_function import laplace_b
+from warnings import warn
+
+from scipy.special import eval_chebyt,eval_chebyu
+def _comet_map_coeff_ck(tau,k,q):
+    alpha = 1/q
+    op_tausq = 1+tau*tau
+    om_tausq = 2-op_tausq
+    T = eval_chebyt(k,om_tausq/op_tausq)
+    lb = laplace_b(0.5,k,0,alpha/op_tausq)
+    if k==1:
+        lb -=alpha/op_tausq
+    return np.sqrt(2 * q) * lb * T
+def _comet_map_coeff_sk(tau,k,q):
+    alpha = 1/q
+    op_tausq = 1+tau*tau
+    om_tausq = 2-op_tausq
+    U = eval_chebyu(k-1,om_tausq/op_tausq) * (2*tau/op_tausq)
+    lb = laplace_b(0.5,k,0,alpha/op_tausq)
+    if k==1:
+        lb -=alpha/op_tausq
+    return np.sqrt(2 * q) * lb * U
+def _comet_map_get_osc_root(k,q,N,phase_offset = 0):
+    p=np.zeros(4)
+    p[0] = np.sqrt(2*q*q*q) * k / 3
+    p[2] = 3 * p[0]
+    p[3] = -2 * np.pi * N - phase_offset
+    root = np.real(np.roots(p)[-1])
+    return root
+
+def _comet_map_get_levin_integration_funcs(k,q):
+    sk = _comet_map_coeff_sk
+    ck = _comet_map_coeff_ck
+    fvec_fn = lambda x: [np.vectorize(sk)(x,k,q),np.vectorize(ck)(x,k,q)]
+    g = lambda x: np.sqrt(2*q*q*q) * k * (1 + x*x)
+    zerofn = np.vectorize(lambda x: 0)
+    Amtrx_fns = [[ zerofn, np.vectorize(g)],[np.vectorize(lambda x: -1*g(x)),zerofn]]
+    wvec_fn = lambda x: [np.sin(k*np.sqrt(2*q*q*q)*(x+x*x*x/3)),np.cos(k*np.sqrt(2*q*q*q)*(x+x*x*x/3))]
+    return fvec_fn,wvec_fn,Amtrx_fns
+
+def comet_map_ck(k,q,atol=1.49e-8,Nmax=10,**kwargs):
+    max_intervals = kwargs.get('max_intervals',10)
+    max_quad_pts = kwargs.get('max_quad_pts',128)
+    interval_size =kwargs.get(
+        'interval_size',
+        _comet_map_get_osc_root(k,q,5,np.pi/4)
+    )
+    fvec_fn,wvec_fn,Amtrx_fns = _comet_map_get_levin_integration_funcs(k,q)
+    i=0
+    tot = 0
+    while i<=max_intervals:
+        last = levin_method_integrate_adaptive(
+            fvec_fn,wvec_fn,Amtrx_fns,
+            i*interval_size,(i+1)*interval_size,
+            Nmax=max_quad_pts,
+            rtol=0,atol=atol
+        )
+        tot += last
+        i+=1
+        if np.abs(last)<atol:
+            break
+    else:
+        warn("Exceeded maximum number of iteractions")
+    return 2*tot
+
+class CometMap():
+    r"""
+    A class representing the comet map. The map depends on the pericenter
+    distance to perturber semi-major axis ratio, :math:`q/a_p`, the
+    comet-perturber semi-major axis ratio, :math:`a/a_p`, and the
+    perturber-star mass ratio, :math:`mu`. The map is defined by the equations 
+
+    .. math::
+        \begin{align}
+        w' &= w + \epsilon f(\theta; q/a_p) \\
+        \theta' &= \theta + 2\pi\left(N + w'\right)
+        \end{align}
+
+    By default, the map is defined on the cylinder with
+    the :math:`\theta` coordinate taken mod :math:`2\pi`.
+    The parameter `mod_p=True` can be set to take the 
+    :math:`p` coordinate modulo :math:`2\pi` as well.
+
+    Parameters
+    ----------
+    m : float
+        Planet-star mass ratio.
+    q : float
+        Pericenter distance of comet, measured in units of the perturber
+        semi-major axis.
+    N : int
+        Center the map on an an  :math:`N:1` MMR.
+    kmax : int
+        Maximum order of Fourier amplitude to compute.
+    mod_theta : bool, optional
+        If True, the :math:`\theta` coordinate
+        is taken modulo :math:`2\pi`.
+        Default is `True`
+    mod_p : bool, optional
+        If True, the :math:`p` coordinate
+        is taken modulo :math:`2\pi`.
+        Default is `False`.
+    """
+    def __init__(self,m,N,q,kmax=32,mod=True):
+        self.m = m
+        self.N = N
+        assert type(N)==int, "Only integer N allowed"
+        self._kmax = kmax
+        self._q = q
+        self._update_amplitudes()
+        self.mod = mod
+    @property 
+    def q(self):
+        return self._q
+    @q.setter
+    def q(self,val):
+        self._q = val
+        self._update_amplitudes()
+
+    @property
+    def mod(self):
+        return self._mod
+
+    @mod.setter
+    def mod(self,val):
+        self._mod = val
+        if val:
+            self._modfn = lambda x: np.mod(x,2*np.pi)
+        else:
+            self._modfn = lambda x: x
+    @property
+    def kmax(self):
+        return self._kmax
+    @kmax.setter
+    def kmax(self,val):
+        self._kmax = val
+        self._update_amplitudes()
+    @property
+    def a0(self):
+        N = self.N
+        return N**(2/3)
+    @a0.setter
+    def a0(self,val):
+        self.N = a0**(1.5)
+    @property
+    def x0(self):
+        return 1/self.a0
+    @property
+    def eps(self):
+        a0 = self.a0
+        m = self.m
+        return 3*a0**(2.5) * m
+
+    def _update_amplitudes(self,atol=1.49e-8):
+        q = self._q
+        kmax = self._kmax
+        self.amps = np.array([ 
+            k*comet_map_ck(k,q,atol=atol) for k in range(1,kmax+1)
+        ])
+    def f(self,theta):
+        r"""
+        The kick function of the map, :math:`-\partial_\theta F_\beta(\theta)`.
+
+        Parameters
+        ----------
+        theta : float
+            Angle varaible at which to evaluate the kick function
+
+        Returns
+        -------
+        float
+            Value of the kick function
+        """
+        sin_ktheta = np.array([np.sin(k*theta) for k in range(1,self.kmax+1)])
+        return self.amps @ sin_ktheta
+    def F(self, theta):
+        r"""
+        The `potential function', :math:`F_\beta(\theta)` from which the map's kick function is derived.
+
+        Parameters
+        ----------
+        theta : float
+            Angle varaible at which to evaluate the potential function
+
+        Returns
+        -------
+        float
+            Value of the potential function
+        """
+        return np.sum([amp * np.cos((k_minus_1 + 1)*theta) / (k_minus_1 + 1) for k_minus_1,amp in enumerate(self.amps)])
+    def dfdtheta_n(self,theta,n):
+        trig = np.array([k**(n) * np.sin(k*theta + 0.5 * n * np.pi) for k in range(1,self.kmax+1)])
+        return self.amps @ trig
+    
+    def __call__(self,X):
+        theta,w = X
+        eps = self.eps
+        w1 = w + eps * self.f(theta)
+        theta1 = theta + 2 * np.pi * w1
+        theta1 = self._modfn(theta1)
+        return np.array([theta1,w1])
+    
+    def action(self,pt):
+        r"""
+        Evaluate The action zero-form,
+
+        .. math::
+        \lambda(\theta,w) = 2\pi\left(\frac{w'^2}{2}- \frac{\epsilon}{2\pi}  F_\beta(\theta)\right)~,
+
+        where :math:`w' = w - \epsilon \partial_\theta F_\beta(\theta)`. The action zero-form satisfies
+        :math:`T^*(w d\theta) - w d\theta = d\lambda` where :math:`T^*` is the pullback of the map.
+
+        Parameters
+        ----------
+        pt : array-like
+            the point :math:`(\theta,w)` at which to evlauate the action.
+
+        Returns
+        -------
+        float
+            The value of the action zero-form, :math:`\lambda(\theta,w)`
+        """
+        theta,w = pt
+        eps = self.eps
+        w1 = w + eps * self.f(theta)
+        Fval = self.F(theta)
+        return np.pi * w1 * w1 - eps * Fval
+    
+    def with_variational(self,X,dX):
+        r"""
+        Apply the map along with the tangent map to point plus variationals.
+        In particular, 
+
+        .. math::
+            \begin{align}
+            (\theta', w') &=& T(\theta, w) 
+            \\
+            (\delta \theta',\delta  w') &=& DT(\theta, w) \cdot (\delta \theta,\delta  w) 
+        
+        where :math:`T` is the usual map and :math:`DT` is the Jacobian of the map.
+
+        Parameters
+        ----------
+        X : array-like
+            The point :math:`X = (\theta,w)`
+        dX : array-like
+            The variational vector :math:`(\delta\theta,\delta w)`
+        
+        Returns
+        -------
+        X' : array-like
+            The new point
+        dX' : array-lke
+            The new variationl vector
+        """
+        jac = self.jac(X)
+        X1 = self.__call__(X)
+        dX1 = jac @ dX
+        return X1,dX1
+
+    def full_map(self,pt):
+        r"""
+        Use version of map, defined as
+        .. math::
+            \begin{align}
+                x' &=& x - 2\mu \pd{F_\beta(\theta)}{\theta} 
+                \\
+                \theta' &=& \theta + \frac{2\pi}{x'^{3/2}}~.
+            \end{eqnarray}
+
+        where :math:`x` represents the test particle's inverse semi-major axis.
+
+        Arguments
+        ---------
+        pt : array-like 
+            The point :math:`(\theta,x)` to map
+        
+        Returns
+        -------
+        pt1 : array
+            Resulting point :math:`(\theta',x')`
+        """
+        theta,x = pt
+        x1 = x - 2 * self.m * self.f(theta)
+        theta1 = theta + 2 * np.pi / x1**(1.5)
+        theta1 = self._modfn(theta1)
+        return np.array([theta1,x1])
+    
+    def jac(self,X):
+        theta,x = X
+        dx1_dx = 1
+        dx1_dtheta = self.eps * self.dfdtheta_n(theta,1)
+        dtheta1_dx =2*np.pi * dx1_dx
+        dtheta1_dtheta = 1 + 2 * np.pi * dx1_dtheta
+        return np.array([[dtheta1_dtheta,dtheta1_dx],[dx1_dtheta,dx1_dx]])
+    def inv(self,X):
+        theta1,x1 = X
+        eps = self.eps
+        theta = theta1 - 2 * np.pi * x1 
+        x = x1 - eps * self.f(theta)
+        return (theta,x)
+
+    def partial_derivs(self,x0,Nmax):
+        """
+        Get the partial derivatives of the map up 
+        to order `Nmax` evaluated at point `x0`.
+        """
+        theta,x = x0
+        T = np.zeros((2,Nmax+1,Nmax+1))
+        eps = self.eps
+        T[:,0,0] = self.__call__(x0)
+        T[0][0,1] = +2 * np.pi
+        T[1][0,1] = 1
+        n=1
+        eps_fn = eps * self.dfdtheta_n(theta,n)
+        T[0][1,0] = 1 + 2 * np.pi * eps_fn
+        T[1][1,0] = eps_fn
+        for n in range(2,Nmax+1):
+            eps_fn = eps * self.dfdtheta_n(theta,n)
+            T[0][n,0] = +2 * np.pi * eps_fn
+            T[1][n,0] = eps_fn
+        return T
+
+    def inv_partial_derivs(self,x0,Nmax):
+        """
+        Get the partial derivatives of the map up 
+        to order `Nmax` evaluated at point `x0`.
+        """
+        theta1,x1 = x0
+        T = np.zeros((2,Nmax+1,Nmax+1))
+        eps = self.eps
+        T[:,0,0] = self.inv(x0)
+        T[0][1,0] = 1
+        T[0][0,1] = -2 * np.pi
+        theta,x = T[:,0,0]
+        for n in range(1,Nmax+1):
+            eps_fn = eps * self.dfdtheta_n(theta,n)
+            for l in range(n+1):
+                T[1][l,n-l] = -1 * (-2*np.pi)**(n-l) * eps_fn
+        T[1][0,1] += 1
+        return T
+    
+    def get_eps_crit(self,tau=1,kmax=None):
+        r"""
+        Calculate the critical :math:`\epsilon` parameter at which the onset of chaos is predicted based on the resonant optical depth.
+
+        Arguments
+        ---------
+        tau : float, optional
+            Sets the resonant optical depth for the onset of chaos.
+            The default value is 1.
+        
+        Returns
+        -------
+        float : 
+            Critical value of epsilon.
+        """
+        if kmax is None:
+            kmax = self.kmax
+        tot = 0
+
+        first_order_half_width_sq = 0
+        for k_minus_one,amp in enumerate(self.amps):
+            k=k_minus_one+1
+            ck = amp/k
+            if k>1 and k<=kmax:
+                half_width = np.sqrt(2 * ck / np.pi)
+                tot+=2*totient(k)*half_width
+            if k%2:
+                # odd orders contribute to first-order width at pi
+                first_order_half_width_sq += (2/np.pi) * ck
+        tot += 2*np.sqrt(first_order_half_width_sq)
+        return tau*tau/tot/tot
+    
+    def D_QL(self):
+        r"""
+        Compute the quasi-linear estimate for the local
+        diffusion coefficient given by 
+
+        .. math::
+            D_mathrm{QL} = \frac{1}{2}\epsilon^2\sum_{k}k^2C_{k}(\beta)^2
+
+        Returns
+        -------
+        D_QL : float
+        """
+        eps = self.eps
+        amps = self.amps
+        amps_sq = amps @ amps
+        return 0.5 * eps * eps * amps_sq
+    def symmetry_lines(self):
+        """
+        Return the symmetry lines of the map.
+
+        Returns
+        -------
+        tuple
+            Tuple containing three functions that parameterize the symmetry lines of the map.
+        """
+        sline1 = lambda x: np.array((0,x))
+        sline2 = lambda x: np.array((np.pi,x))
+        sline3 = lambda x: np.array((np.pi * x,x))
+        return (sline1,sline2,sline3)
```

### Comparing `celmech-1.0.3/celmech/miscellaneous.py` & `celmech-1.0.4/celmech/miscellaneous.py`

 * *Files 13% similar despite different names*

```diff
@@ -283,15 +283,17 @@
 
     Returns
     -------
     AMD : float
         The value of the systems angular momentum 
         deficit.
     """
-
+    # copy sim and move to center of mass
+    sim = sim.copy()
+    sim.move_to_com()
     pstar = sim.particles[0]
     Mstar = pstar.m
     Ltot = pstar.m * np.cross(pstar.xyz,pstar.vxyz)
     ps = sim.particles[1:]
     Lmbda=np.zeros(len(ps))
     G = np.zeros(len(ps))
     Lhat = np.zeros((len(ps),3))
@@ -391,15 +393,15 @@
         C = AMD / LmbdaOut
         coeffs[i] = C / Ccrit
     return coeffs
 
 ######################################################
 ######################## FMFT ########################
 ######################################################
-p2d = np.ctypeslib.ndpointer(dtype = np.float,ndim = 2,flags = 'C')
+p2d = np.ctypeslib.ndpointer(dtype = np.float64,ndim = 2,flags = 'C')
 _fmft = clibcelmech.fmft_wrapper
 _fmft.argtypes =[p2d, c_int, c_double, c_double, c_int, p2d, c_long]
 _fmft.restype = c_int
 def _check_errors(ret, func, args):
     if ret<=0:
         raise RuntimeError("FMFT returned error code %d for the given arguments"%ret)
     return ret
@@ -592,7 +594,139 @@
     assert eps not in exprn.free_symbols, "Epsilon appears as a free symbols in 'exprn'."
     rule = dict()
     for n,variables in order_rules.items():
         rule.update({v:eps**n * v for v in variables})
     sexprn = series(exprn.subs(rule),eps,0,max_order+1)
     result = sexprn.removeO().subs({eps:1})
     return result
+
+################################################
+########### Levin Method Integration ###########
+################################################
+
+from scipy.linalg import lu_factor, lu_solve
+def linsolve(A,y):
+    """
+    Solve linear system of equations
+    
+    .. math::
+        A \cdot x = y
+    
+    for y.
+    """
+    return lu_solve(lu_factor(A),y)
+def _chebyshev_gauss_lobatto_points(n,a,b):
+    """Get Gauss-Lobatto quadrature points for Chebyshev polynomials"""
+    return 0.5 * (a+b) + 0.5 * (a-b) * np.cos(np.pi*np.arange(n)/(n-1))
+def _chebyshev_Dmatrix(n):
+    """Chebyshev derivative matrix for pseudo-spectral method"""
+    x = np.cos(np.pi*np.arange(n)/(n-1))
+    c = lambda j: 2 if j==0 or j==n-1 else 1
+    Dkj = lambda k,j: (c(k)/c(j))*(-1)**(k+j+1) / (x[k]-x[j]) if k!=j else 0
+    Dmtrx = np.array([[Dkj(k,j) for j in range(n)]for k in range(n)])
+    Dmtrx -= np.diag(np.sum(Dmtrx,axis=1))
+    return Dmtrx
+def levin_method_integrate(fvec_fn,wvec_fn,Amtrx_fns,a,b,N=32):
+    r"""Evlauate integrals of the form
+
+    .. math::
+        I(a,b) = \int_{a}^{b} \vec{f}(x)\cdot\vec{w}(x) dx
+
+    where the functions :math:`\vec{w}(x)` satisfy a linear differential
+    equation of the form :math:`\frac{d}{dx}\vec{w}(x) = A(x) \cdot
+    \vec{w}(x)`. Evaluation is done using `Levin's method`_.
+
+
+    .. _Levin's method: https://www.sciencedirect.com/science/article/pii/0377042794001189
+
+    Parameters
+    ----------
+    fvec_fn : function
+        A function that returns the vector :math:`\vec{f}(x)`.
+    wvec_fn : function
+        A function that returns the vector :math:`\vec{w}(x)`.
+    Amtrx_fns : list of functions
+        A list of functions giving the entries of matrix :math:`A(x)` appearing
+        in the differential equation obeyed by :math:`\vec{w}(x)`. Input should
+        use nested lists to match the structure of the matrix.
+    a : float
+        Lower integration limit
+    b : float
+        Upper integration limit
+    N : int
+        Number of quadrature points to use
+
+    Returns
+    -------
+    float
+    """
+    chebD = _chebyshev_Dmatrix(N)
+    wa = wvec_fn(a)
+    wb = wvec_fn(b)
+    f = 0.5 * (b-a)
+    xj = _chebyshev_gauss_lobatto_points(N,a,b)
+    zeroN = np.zeros((N,N))
+    M = len(wa)
+    D = np.block([[chebD if j==i else zeroN for j in range(M)] for i in range(M)])    
+    A_tr_mtrx = np.block([[np.diag(Amtrx_fns[i][j](xj)) for i in range(M)] for j in range(M)])
+    Fsoln = linsolve(D + f*A_tr_mtrx,f*np.reshape(fvec_fn(xj),-1))
+    Fa,Fb = Fsoln[::N],Fsoln[N-1::N]
+    ans=Fb@wb - Fa@wa
+    return ans
+def levin_method_integrate_adaptive(fvec_fn,wvec_fn,Amtrx_fns,a,b,N0=32,Nmax=128,rtol = 1.49e-08,atol = 1.49e-08 ):
+    r"""Evlauate integrals of the form
+
+    .. math::
+        I(a,b) = \int_{a}^{b} \vec{f}(x)\cdot\vec{w}(x) dx
+
+    where the functions :math:`\vec{w}(x)` satisfy a linear differential
+    equation of the form :math:`\frac{d}{dx}\vec{w}(x) = A(x) \cdot
+    \vec{w}(x)`. Evaluation is done using `Levin's method`_.
+
+    Method is applied adaptively with increasing number of quadrature points
+    until the estimated error, :math:`\delta` satisfies :math:`\delta <
+    \epsilon_\mathrm{rel}|I(a,b)| + \epsilon_\mathrm{abs}`.
+
+    .. _Levin's method: https://www.sciencedirect.com/science/article/pii/0377042794001189
+
+    Parameters
+    ----------
+    fvec_fn : function
+        A function that returns the vector :math:`\vec{f}(x)`.
+    wvec_fn : function
+        A function that returns the vector :math:`\vec{w}(x)`.
+    Amtrx_fns : list of functions
+        A list of functions giving the entries of matrix :math:`A(x)` appearing
+        in the differential equation obeyed by :math:`\vec{w}(x)`. Input should
+        use nested lists to match the structure of the matrix.
+    a : float
+        Lower integration limit
+    b : float
+        Upper integration limit
+    N0 : int
+        Initial number of Gauss-Lobatto quadrature points to use.
+    Nmax : int
+        Maximum number of quadrature points to use.
+    rtol : float
+        Relative tolerance
+    atol : float
+        Absolute tolerance
+
+    Returns
+    -------
+    float
+    """
+    delta = np.inf
+    ans_old = np.inf
+    N=N0
+    while N<=Nmax:
+        ans = levin_method_integrate(fvec_fn,wvec_fn,Amtrx_fns,a,b,N)
+        delta = np.abs(ans-ans_old)
+        ans_old = ans
+        N*=2
+        if delta < rtol * np.abs(ans) + atol:
+            break
+    else:
+        msg="Exceeded maximum number of quadruature points without converging.\n"
+        msg+="N={}, delta = {}, target = {}".format(N,delta,rtol * np.abs(ans) + atol)
+        warnings.warn(msg)
+    return ans
```

### Comparing `celmech-1.0.3/celmech/multiplanet_hamiltonian.py` & `celmech-1.0.4/celmech/multiplanet_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/nbody_simulation_utilities.py` & `celmech-1.0.4/celmech/nbody_simulation_utilities.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/numerical_resonance_models.py` & `celmech-1.0.4/celmech/numerical_resonance_models.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/numerical_resonance_utils.py` & `celmech-1.0.4/celmech/numerical_resonance_utils.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/planar_poincare.py` & `celmech-1.0.4/celmech/planar_poincare.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/poincare.py` & `celmech-1.0.4/celmech/poincare.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/poisson_series.py` & `celmech-1.0.4/celmech/poisson_series.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/resonances.py` & `celmech-1.0.4/celmech/resonances.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/rk_integrator.py` & `celmech-1.0.4/celmech/rk_integrator.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/secular.py` & `celmech-1.0.4/celmech/secular.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,18 +128,18 @@
     def inclination_matrix(self):
         return Matrix([
             [self.inc_entries[max(i,j),min(i,j)] for i in xrange(1,self.N)]
             for j in xrange(1,self.N) 
             ])
     @property 
     def Neccentricity_matrix(self):
-        return np.array(self.eccentricity_matrix.subs(self.params)).astype(np.float64)
+        return np.array(self.eccentricity_matrix.xreplace(self.params)).astype(np.float64)
     @property 
     def Ninclination_matrix(self):
-        return np.array(self.inclination_matrix.subs(self.params)).astype(np.float64)
+        return np.array(self.inclination_matrix.xreplace(self.params)).astype(np.float64)
     @property
     def Tsec(self):
         Omega_e = np.max( np.abs(self.eccentricity_eigenvalues()) )
         Omega_i = np.max( np.abs(self.inclination_eigenvalues()) )
         return 2 * np.pi / max(Omega_e,Omega_i)
     def _chop(self,arr):
         arr[np.abs(arr)<self.tol] = 0
@@ -1206,15 +1206,15 @@
             ubar=get_symbol_vec(r"\bar{u}")
             v=get_symbol_vec("v")
             vbar=get_symbol_vec(r"\bar{v}")
             Te,TI,De,DI = self.diagonalizing_tranformations()
             cvars = H.gens
             transformed_vars = np.concatenate((Te.dot(u),TI.dot(v),Te.dot(ubar),TI.dot(vbar)))
             rule={a:b for a,b in zip(cvars,transformed_vars)}
-            H = H.as_expr().subs(rule)
+            H = H.as_expr().xreplace(rule)
             H += De.dot(u).dot(ubar) + DI.dot(v).dot(vbar)
             H = H.as_poly(u+v+ubar+vbar)
         return H
 
     def _hamiltonian_to_poly(self,include_linear_terms):
         get_symbol_vec = self._get_symbol_vec
         Npl = self.Npl
```

### Comparing `celmech-1.0.3/celmech/symplectic_evolution_operators.py` & `celmech-1.0.4/celmech/symplectic_evolution_operators.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech/transformations.py` & `celmech-1.0.4/celmech/transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/celmech.egg-info/PKG-INFO` & `celmech-1.0.4/celmech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celmech
-Version: 1.0.3
+Version: 1.0.4
 Summary: Open source tools for celestial mechanics
 Home-page: http://github.com/shadden/celmech
 Author: Dan Tamayo, Sam Hadden
 Author-email: tamayo.daniel@gmail.com, shadden1107@gmail.com
 License: GPL
 Keywords: astronomy astrophysics celestial-mechanics orbits orbital-mechanics
 Platform: UNKNOWN
```

### Comparing `celmech-1.0.3/celmech.egg-info/SOURCES.txt` & `celmech-1.0.4/celmech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/setup.py` & `celmech-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Try to get git hash
 try:
     import subprocess
     ghash = subprocess.check_output(["git", "rev-parse", "HEAD"]).decode("ascii")
     ghash_arg = "-DCELMECHGITHASH="+ghash.strip()
 except:
-    ghash_arg = "-DCELMECHGITHASH=0b07b5a7cab5243fc616c0d2dcbdb20ce47397e0" #GITHASHAUTOUPDATE
+    ghash_arg = "-DCELMECHGITHASH=255ba6181dbc18d75b9a177ea5ab1505c2487ff6" #GITHASHAUTOUPDATE
 
 extra_link_args=[]
 if sys.platform == 'darwin':
     from distutils import sysconfig
     vars = sysconfig.get_config_vars()
     vars['LDSHARED'] = vars['LDSHARED'].replace('-bundle', '-shared')
     extra_link_args=['-Wl,-install_name,@rpath/libcelmech'+suffix]
@@ -45,15 +45,15 @@
     packages = ['theano', 'sympy>=1.1.1', 'numpy', 'scipy>=1.2.0', 'reboundx>=3.1.0', 'rebound>=3.5.11', 'mpmath>=1.0.0']
     try:
         install_requires += packages
     except:
         install_requires = packages
 
 setup(name='celmech',
-    version='1.0.3',
+    version='1.0.4',
     description='Open source tools for celestial mechanics',
     url='http://github.com/shadden/celmech',
     author='Dan Tamayo, Sam Hadden',
     author_email='tamayo.daniel@gmail.com, shadden1107@gmail.com',
     license='GPL',
     classifiers=[
         # How mature is this project? Common values are
```

### Comparing `celmech-1.0.3/src/disturbing_function.c` & `celmech-1.0.4/src/disturbing_function.c`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #include <stdio.h>
 #include <assert.h>
 
 #define STRINGIFY(s) str(s)
 #define str(s) #s
 
 const char* celmech_build_str = __DATE__ " " __TIME__; // Date and time build string. 
-const char* celmech_version_str = "1.0.3";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
+const char* celmech_version_str = "1.0.4";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
 const char* celmech_githash_str = STRINGIFY(CELMECHGITHASH);             // This line gets updated automatically. Do not edit manually.
 
 double laplace(double s, int i, int j, double a);
 double GeneralOrderCoefficient(int res_j, int order, int epower,double a);
 
 int binomialCoeff(int n, int k)
 {
```

### Comparing `celmech-1.0.3/src/fmft.c` & `celmech-1.0.4/src/fmft.c`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/src/fmftPy.c` & `celmech-1.0.4/src/fmftPy.c`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/src/nrutil.c` & `celmech-1.0.4/src/nrutil.c`

 * *Files identical despite different names*

### Comparing `celmech-1.0.3/src/poisson_series.c` & `celmech-1.0.4/src/poisson_series.c`

 * *Files identical despite different names*

