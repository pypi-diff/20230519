# Comparing `tmp/waveformtools-2023.5.17.tar.gz` & `tmp/waveformtools-2023.5.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveformtools-2023.5.17.tar", last modified: Wed May 17 09:12:41 2023, max compression
+gzip compressed data, was "waveformtools-2023.5.19.tar", last modified: Fri May 19 07:14:07 2023, max compression
```

## Comparing `waveformtools-2023.5.17.tar` & `waveformtools-2023.5.19.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:12:41.616490 waveformtools-2023.5.17/
--rwxrwxrwx   0 root         (0) root         (0)     1075 2023-05-17 09:11:57.000000 waveformtools-2023.5.17/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8708 2023-05-17 09:12:41.615490 waveformtools-2023.5.17/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      106 2023-05-17 09:11:57.000000 waveformtools-2023.5.17/README
--rwxrwxrwx   0 root         (0) root         (0)     8052 2023-05-17 09:11:57.000000 waveformtools-2023.5.17/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 09:12:41.616490 waveformtools-2023.5.17/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1396 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:12:41.613490 waveformtools-2023.5.17/waveformtools/
--rw-rw-rw-   0 root         (0) root         (0)     5480 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/BMS.py
--rw-rw-rw-   0 root         (0) root         (0)     9130 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/CoM.py
--rwxrwxrwx   0 root         (0) root         (0)     1284 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10875 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/compare.py
--rw-rw-rw-   0 root         (0) root         (0)    54085 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/dataIO.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/diagnostics.py
--rw-rw-rw-   0 root         (0) root         (0)    25350 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/differentiate.py
--rw-rw-rw-   0 root         (0) root         (0)     9106 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/extrapolate.py
--rw-rw-rw-   0 root         (0) root         (0)    14069 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/grids.py
--rw-rw-rw-   0 root         (0) root         (0)    10952 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     7204 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)    53835 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/simulations.py
--rw-rw-rw-   0 root         (0) root         (0)     6476 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/spherical.py
--rw-rw-rw-   0 root         (0) root         (0)    12491 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/transforms.py
--rw-rw-rw-   0 root         (0) root         (0)    60703 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/waveforms.py
--rw-rw-rw-   0 root         (0) root         (0)   110367 2023-05-17 09:11:58.000000 waveformtools-2023.5.17/waveformtools/waveformtools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:12:41.615490 waveformtools-2023.5.17/waveformtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8708 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-17 09:12:41.000000 waveformtools-2023.5.17/waveformtools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:14:07.263553 waveformtools-2023.5.19/
+-rwxrwxrwx   0 root         (0) root         (0)     1075 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-05-19 07:14:07.263553 waveformtools-2023.5.19/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      106 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/README
+-rwxrwxrwx   0 root         (0) root         (0)     8052 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 07:14:07.263553 waveformtools-2023.5.19/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1396 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:14:07.262554 waveformtools-2023.5.19/waveformtools/
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/BMS.py
+-rw-rw-rw-   0 root         (0) root         (0)     9130 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/CoM.py
+-rwxrwxrwx   0 root         (0) root         (0)     1284 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10875 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)    54107 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/dataIO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    25348 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/differentiate.py
+-rw-rw-rw-   0 root         (0) root         (0)     9106 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/extrapolate.py
+-rw-rw-rw-   0 root         (0) root         (0)    14069 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/grids.py
+-rw-rw-rw-   0 root         (0) root         (0)    10952 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     7204 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)    53835 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/simulations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/spherical.py
+-rw-rw-rw-   0 root         (0) root         (0)    12491 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)   124986 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/waveforms.py
+-rw-rw-rw-   0 root         (0) root         (0)   110367 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/waveformtools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:14:07.263553 waveformtools-2023.5.19/waveformtools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/top_level.txt
```

### Comparing `waveformtools-2023.5.17/LICENSE` & `waveformtools-2023.5.19/LICENSE`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/PKG-INFO` & `waveformtools-2023.5.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.5.17
+Version: 2023.5.19
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `waveformtools-2023.5.17/README.md` & `waveformtools-2023.5.19/README.md`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/pyproject.toml` & `waveformtools-2023.5.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/setup.py` & `waveformtools-2023.5.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # requiremnts directly from toml
 # mreq, oreq = get_requirements()
 
 
 
 setuptools.setup(
     name="waveformtools",
- 	version="2023.05.17",
+ 	version="2023.05.19",
     author="Vaishak Prasad",
     author_email="vaishakprasad@gmail.com",
     description="Functions for handling waveform and numerical relativity data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/vaishakp/waveformtools",
     packages=setuptools.find_packages(),
```

### Comparing `waveformtools-2023.5.17/waveformtools/BMS.py` & `waveformtools-2023.5.19/waveformtools/BMS.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/CoM.py` & `waveformtools-2023.5.19/waveformtools/CoM.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/__init__.py` & `waveformtools-2023.5.19/waveformtools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,8 +34,8 @@
         print("This is not a git repo! please use the version attribute instead!")
     # with open(package_directory + "/../public/date.txt", "r") as vers_file:
     # vers = vers_file.read()[:10]
 
     return vers
 
 
-__version__ = "2023.05.17"
+__version__ = "2023.05.19"
```

### Comparing `waveformtools-2023.5.17/waveformtools/compare.py` & `waveformtools-2023.5.19/waveformtools/compare.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/dataIO.py` & `waveformtools-2023.5.19/waveformtools/dataIO.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,21 +123,21 @@
 
     elif var_type == "Strain":
         # import h5py
         message("Fetching all keys from H5 file", message_verbosity=2)
         data_file = h5py.File(f"{data_dir}/{file_name}")
         all_fnames = list(data_file.keys())
         data_file.close()
-        message(all_fnames)
+        # message(all_fnames)
 
     # Parse ell values
     # Filter the keys.
     all_fnames = [item for item in all_fnames if "_l" in item]
 
-    message("All files found", all_fnames, message_verbosity=2)
+    message("All files found", all_fnames, message_verbosity=3)
 
     ell_max = get_ell_max_from_keys(all_fnames)
 
     return ell_max, all_fnames
 
 
 def _get_modes_list_from_keys(keys_list, r_ext):
@@ -379,15 +379,14 @@
     message("Loading RIT Psi4 type data.", message_verbosity=1)
     from waveformtools.waveforms import modes_array
 
     if not wfa:
         wfa = modes_array(label=label, data_dir=data_dir, modes_list=wf_modes_list)
 
     if modes_list is None:
-
         # Max available mode l.
         if ell_max is None:
             ell_max, _ = get_ell_max_from_file(data_dir)
 
         # Construct a modes list
         wf_modes_list = construct_mode_list(ell_max=ell_max, spin_weight=spin_weight)
 
@@ -679,15 +678,15 @@
 
     message("Reading in modes...")
     for ell, emm_list in modes_list:
         for emm in emm_list:
             this_amp_key = f"amp_l{ell}_m{emm}"
             this_phase_key = f"phase_l{ell}_m{emm}"
 
-            message("Loading", ell, emm)
+            message("Loading", ell, emm, message_verbosity=3)
             # Construct file path
 
             # Create modes_array on first run
 
             ###############################
             # Load the phase data
             ##############################
```

### Comparing `waveformtools-2023.5.17/waveformtools/diagnostics.py` & `waveformtools-2023.5.19/waveformtools/diagnostics.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/differentiate.py` & `waveformtools-2023.5.19/waveformtools/differentiate.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     dydx : 1d array
            The first order derivative of y w.r.t. x.
     """
 
     if method == "CS":
         dydx = Chebyshev_differential(x_data, y_data, order=1, degree=degree)
     else:
-
         delta_x_all = np.diff(x_data)
 
         if (delta_x_all - delta_x_all[0] < 1e-14).all():
             message("No interpolation required.")
             interp = False
             x_uniform = x_data
             y_uniform = y_data
@@ -66,15 +65,14 @@
 
         if method == "FS":
             dydx_new, _, x_new, _ = Fourier_differential(
                 delta_x=delta_x, udata_x=y_uniform, order=1, zero_mode=0, taper=False
             )
 
         elif method == "FD":
-
             if degree == 1:
                 dydx_new = differentiate(y_uniform, delta_x)
             elif degree == 2:
                 dydx_new = differentiate2(y_uniform, delta_x)
             elif degree == 3:
                 dydx_new = differentiate3(y_uniform, delta_x)
             elif degree == 4:
```

### Comparing `waveformtools-2023.5.17/waveformtools/extrapolate.py` & `waveformtools-2023.5.19/waveformtools/extrapolate.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/grids.py` & `waveformtools-2023.5.19/waveformtools/grids.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/integrate.py` & `waveformtools-2023.5.19/waveformtools/integrate.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/legacy.py` & `waveformtools-2023.5.19/waveformtools/legacy.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/simulations.py` & `waveformtools-2023.5.19/waveformtools/simulations.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/spherical.py` & `waveformtools-2023.5.19/waveformtools/spherical.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools/transforms.py` & `waveformtools-2023.5.19/waveformtools/transforms.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """ Methods to transform the waveform """
 
 import numpy as np
+
 from waveformtools.waveformtools import message
+
 # from numba import jit, njit
 
 
 # @njit(parallel=True)
 def compute_fft(udata_x, delta_x):
     """Find the FFT of the samples in time-space, and return with the frequencies.
 
@@ -276,15 +278,14 @@
     for aar in range(0, ell - abs_spin_weight + 1):
         subterm = 0
 
         if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
             message(f"Skipping r {aar}", message_verbosity=3)
             continue
         else:
-
             term1 = comb(ell - abs_spin_weight, aar)
             term2 = comb(ell + abs_spin_weight, aar + abs_spin_weight - emm)
             term3 = np.power(float(-1), (ell - aar - abs_spin_weight))
             term4 = np.exp(1j * emm * phi_grid)
             term5 = np.power(np.tan(theta_grid / 2), (-2 * aar - abs_spin_weight + emm))
             subterm = term1 * term2 * term3 * term4 * term5
 
@@ -381,15 +382,14 @@
     # To get negative spin weight SWSH
     # in terms of positive spin weight
     factor = 1
     if spin_weight < 0:
         factor = sp.Pow(-1, ell)
 
     for aar in range(ell - abs_spin_weight + 1):
-
         if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
             # message('Continuing')
             continue
         else:
             # message('r, l, s, m', r, l, s, m)
             # a1 = sp.binomial(ell - spin_weight, aar)
             # message(a1)
```

### Comparing `waveformtools-2023.5.17/waveformtools/waveformtools.py` & `waveformtools-2023.5.19/waveformtools/waveformtools.py`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.17/waveformtools.egg-info/PKG-INFO` & `waveformtools-2023.5.19/waveformtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.5.17
+Version: 2023.5.19
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `waveformtools-2023.5.17/waveformtools.egg-info/SOURCES.txt` & `waveformtools-2023.5.19/waveformtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

