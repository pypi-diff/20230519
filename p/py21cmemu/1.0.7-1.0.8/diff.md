# Comparing `tmp/py21cmemu-1.0.7.tar.gz` & `tmp/py21cmemu-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py21cmemu-1.0.7.tar", max compression
+gzip compressed data, was "py21cmemu-1.0.8.tar", max compression
```

## Comparing `py21cmemu-1.0.7.tar` & `py21cmemu-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-03-03 11:01:58.918549 py21cmemu-1.0.7/LICENSE
--rw-r--r--   0        0        0     2441 2023-05-18 12:15:32.657886 py21cmemu-1.0.7/README.rst
--rw-r--r--   0        0        0     2367 2023-05-18 12:44:19.241815 py21cmemu-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      405 2023-05-18 12:44:19.241815 py21cmemu-1.0.7/src/py21cmemu/__init__.py
--rw-r--r--   0        0        0     2776 2023-05-18 12:15:32.677886 py21cmemu-1.0.7/src/py21cmemu/config.py
--rw-r--r--   0        0        0     3542 2023-05-18 12:15:32.677886 py21cmemu-1.0.7/src/py21cmemu/emulator.py
--rw-r--r--   0        0        0    14978 2023-05-18 12:15:32.677886 py21cmemu-1.0.7/src/py21cmemu/emulator_constants.npz
--rw-r--r--   0        0        0     1199 2023-05-18 12:15:32.677886 py21cmemu-1.0.7/src/py21cmemu/get_emulator.py
--rw-r--r--   0        0        0     5483 2023-05-18 12:15:32.677886 py21cmemu-1.0.7/src/py21cmemu/inputs.py
--rw-r--r--   0        0        0     7303 2023-05-18 12:15:32.677886 py21cmemu-1.0.7/src/py21cmemu/outputs.py
--rw-r--r--   0        0        0     2795 2023-05-18 12:15:32.677886 py21cmemu-1.0.7/src/py21cmemu/properties.py
--rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 py21cmemu-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-19 11:51:51.350207 py21cmemu-1.0.8/LICENSE
+-rw-r--r--   0        0        0     2441 2023-05-19 11:51:51.350207 py21cmemu-1.0.8/README.rst
+-rw-r--r--   0        0        0     2367 2023-05-19 11:52:07.070630 py21cmemu-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      405 2023-05-19 11:52:07.070630 py21cmemu-1.0.8/src/py21cmemu/__init__.py
+-rw-r--r--   0        0        0     2776 2023-05-19 11:51:51.378208 py21cmemu-1.0.8/src/py21cmemu/config.py
+-rw-r--r--   0        0        0     3517 2023-05-19 11:51:51.378208 py21cmemu-1.0.8/src/py21cmemu/emulator.py
+-rw-r--r--   0        0        0    14978 2023-05-19 11:51:51.378208 py21cmemu-1.0.8/src/py21cmemu/emulator_constants.npz
+-rw-r--r--   0        0        0     1199 2023-05-19 11:51:51.378208 py21cmemu-1.0.8/src/py21cmemu/get_emulator.py
+-rw-r--r--   0        0        0     5483 2023-05-19 11:51:51.378208 py21cmemu-1.0.8/src/py21cmemu/inputs.py
+-rw-r--r--   0        0        0     7303 2023-05-19 11:51:51.378208 py21cmemu-1.0.8/src/py21cmemu/outputs.py
+-rw-r--r--   0        0        0     2795 2023-05-19 11:51:51.378208 py21cmemu-1.0.8/src/py21cmemu/properties.py
+-rw-r--r--   0        0        0     3907 1970-01-01 00:00:00.000000 py21cmemu-1.0.8/PKG-INFO
```

### Comparing `py21cmemu-1.0.7/LICENSE` & `py21cmemu-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.7/README.rst` & `py21cmemu-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.7/pyproject.toml` & `py21cmemu-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py21cmEMU"
-version = "1.0.7"
+version = "1.0.8"
 description = "Emulator of 21cmFAST summaries."
 authors = ["Daniela Breitman <daniela.breitman@sns.it>"]
 license = "MIT"
 readme = ["README.rst"]
 homepage = "https://github.com/21cmFAST/21cmEMU"
 repository = "https://github.com/21cmFAST/21cmEMU"
 documentation = "https://21cmEMU.readthedocs.io"
```

### Comparing `py21cmemu-1.0.7/src/py21cmemu/config.py` & `py21cmemu-1.0.8/src/py21cmemu/config.py`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.7/src/py21cmemu/emulator.py` & `py21cmemu-1.0.8/src/py21cmemu/emulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,14 +90,14 @@
         The mean error on the test set (i.e. independent of theta) with all units
         restored and logs removed.
         """
         # For now, we return the mean emulator error (obtained from the test set) for
         # each summary. All errors are the median absolute difference between test set
         # and prediction AFTER units have been restored AND log has been removed.
         return {
-            "delta_err": self.PS_err,
-            "brightness_temp_err": self.Tb_err,
+            "PS_err": self.PS_err,
+            "Tb_err": self.Tb_err,
             "xHI_err": self.xHI_err,
-            "spin_temp_err": self.Ts_err,
+            "Ts_err": self.Ts_err,
             "UVLFs_err": self.UVLFs_err,
-            "tau_e_err": self.tau_err,
+            "tau_err": self.tau_err,
         }
```

### Comparing `py21cmemu-1.0.7/src/py21cmemu/emulator_constants.npz` & `py21cmemu-1.0.8/src/py21cmemu/emulator_constants.npz`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.7/src/py21cmemu/get_emulator.py` & `py21cmemu-1.0.8/src/py21cmemu/get_emulator.py`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.7/src/py21cmemu/inputs.py` & `py21cmemu-1.0.8/src/py21cmemu/inputs.py`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.7/src/py21cmemu/outputs.py` & `py21cmemu-1.0.8/src/py21cmemu/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     @property
     def UVLF_redshifts(self) -> np.ndarray:
         """The redshifts of the UVLFs."""
         return self.properties.uv_lf_zs
 
     @property
-    def ps_redshifts(self) -> np.ndarray:
+    def PS_redshifts(self) -> np.ndarray:
         """The redshifts of the power spectra."""
         return self.properties.zs_cut
 
     @property
     def redshifts(self) -> np.ndarray:
         """The redshifts of all quantities except the PS."""
         return self.properties.zs
```

### Comparing `py21cmemu-1.0.7/src/py21cmemu/properties.py` & `py21cmemu-1.0.8/src/py21cmemu/properties.py`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.0.7/PKG-INFO` & `py21cmemu-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py21cmemu
-Version: 1.0.7
+Version: 1.0.8
 Summary: Emulator of 21cmFAST summaries.
 Home-page: https://github.com/21cmFAST/21cmEMU
 License: MIT
 Keywords: Epoch of Reionization,Cosmology
 Author: Daniela Breitman
 Author-email: daniela.breitman@sns.it
 Requires-Python: >=3.8,<3.12
@@ -14,15 +14,18 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tensorflow (>=2.6.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

