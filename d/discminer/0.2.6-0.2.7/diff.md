# Comparing `tmp/discminer-0.2.6.tar.gz` & `tmp/discminer-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.2.6.tar", last modified: Sun May 14 22:17:43 2023, max compression
+gzip compressed data, was "discminer-0.2.7.tar", last modified: Fri May 19 10:09:33 2023, max compression
```

## Comparing `discminer-0.2.6.tar` & `discminer-0.2.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.585278 discminer-0.2.6/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.6/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-14 22:17:43.585572 discminer-0.2.6/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.6/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.555658 discminer-0.2.6/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.6/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.6/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.6/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.6/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.6/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.6/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.6/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.6/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.6/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.6/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.6/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.6/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.569760 discminer-0.2.6/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.6/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-14 22:16:27.000000 discminer-0.2.6/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     2069 2023-05-05 17:33:30.000000 discminer-0.2.6/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.6/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.6/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.6/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.6/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.6/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.578610 discminer-0.2.6/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.6/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.6/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.6/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12955 2023-05-14 20:31:53.000000 discminer-0.2.6/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    35724 2023-05-14 22:07:59.000000 discminer-0.2.6/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    36007 2023-05-03 15:09:48.000000 discminer-0.2.6/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.6/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.580599 discminer-0.2.6/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.6/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.6/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.6/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.6/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.571711 discminer-0.2.6/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-14 22:17:43.000000 discminer-0.2.6/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.6/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-14 22:17:43.586340 discminer-0.2.6/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.6/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-14 22:17:43.584349 discminer-0.2.6/template/
--rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.6/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.6/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.6/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.6/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.255324 discminer-0.2.7/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.7/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-19 10:09:33.255594 discminer-0.2.7/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.7/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.222289 discminer-0.2.7/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     5155 2023-05-05 18:15:57.000000 discminer-0.2.7/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    11031 2023-05-17 20:12:58.000000 discminer-0.2.7/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1248 2023-05-05 08:45:28.000000 discminer-0.2.7/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     3346 2023-05-08 15:34:54.000000 discminer-0.2.7/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     3565 2023-05-18 10:58:10.000000 discminer-0.2.7/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4445 2023-05-08 15:33:38.000000 discminer-0.2.7/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4305 2023-05-08 15:25:01.000000 discminer-0.2.7/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     6604 2023-05-17 21:21:31.000000 discminer-0.2.7/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    12138 2023-05-16 12:46:47.000000 discminer-0.2.7/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5693 2023-05-10 12:27:07.000000 discminer-0.2.7/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2023-05-14 22:11:49.000000 discminer-0.2.7/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000    14004 2023-05-12 15:45:13.000000 discminer-0.2.7/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.235396 discminer-0.2.7/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.7/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-19 10:08:56.000000 discminer-0.2.7/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     2069 2023-05-05 17:33:30.000000 discminer-0.2.7/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.7/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.7/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.7/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.7/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.7/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.244412 discminer-0.2.7/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.7/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.7/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12955 2023-05-17 22:25:10.000000 discminer-0.2.7/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    35724 2023-05-14 22:07:59.000000 discminer-0.2.7/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    36001 2023-05-19 10:08:32.000000 discminer-0.2.7/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.7/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.246474 discminer-0.2.7/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.7/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.7/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.7/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.7/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.237446 discminer-0.2.7/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.7/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-19 10:09:33.256176 discminer-0.2.7/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.7/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.254451 discminer-0.2.7/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.7/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.7/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.7/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.7/template/prepare_data.py
```

### Comparing `discminer-0.2.6/LICENSE` & `discminer-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/PKG-INFO` & `discminer-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.6 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.7 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.6/README.md` & `discminer-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/_mining/make_channels.py` & `discminer-0.2.7/_mining/make_channels.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,27 +43,32 @@
 vchannels = datacube.vchannels
 
 #****************************
 #INIT MODEL AND PRESCRIPTIONS
 #****************************
 model = General2d(datacube, Rmax, Rmin=0, prototype=True)
 
-model.z_upper_func = cart.z_upper_exp_tapered
-model.z_lower_func = cart.z_lower_exp_tapered
 model.velocity_func = model.keplerian_vertical # vrot = sqrt(GM/r**3)*R
 model.line_profile = model.line_profile_bell
 model.line_uplow = model.line_uplow_mask
 
 if 'I2pwl' in meta['kind']:
     model.intensity_func = cart.intensity_powerlaw_rbreak
 elif 'I2pwlnosurf' in meta['kind']:
     model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
 else:
     model.intensity_func = cart.intensity_powerlaw_rout
 
+if 'surf2pwl' in meta['kind']:
+    model.z_upper_func = cart.z_upper_powerlaw
+    model.z_lower_func = cart.z_lower_powerlaw
+else:
+    model.z_upper_func = cart.z_upper_exp_tapered
+    model.z_lower_func = cart.z_lower_exp_tapered
+
 #Useful definitions for plots
 xmax = model.skygrid['xmax'] 
 xlim = 1.15*xmax/au_to_m
 extent= np.array([-xmax, xmax, -xmax, xmax])/au_to_m
   
 #**************
 #PROTOTYPE PARS
```

### Comparing `discminer-0.2.6/_mining/make_parfile.py` & `discminer-0.2.7/_mining/make_parfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,51 @@
 
 #**************************
 #CUSTOMISED PROPS FOR PLOTS
 #**************************
 #Put here any info you'd like to have access through the parfile.json in the analysis scripts 
 
 custom_dict = {
-    'chan_step': 2, #Plot channels every n steps
+    'chan_step': 4, #Plot channels every n steps
     'nchans': 15, #Plot n channels
     'vlim': 0.2, #Velocity max and min plot limit
     'Llim': 0.2, #Line width max and min
     'Ilim': 15, #Peak intensity max and min
 
     
 }
 
 #****************
 #DISCS BASIC INFO
 #****************
-incl_dict = { #if fixincl is found in log_pars tag take inclination from mm continuum
+discs = 'mwc480 twhyd imlup hd163296'
+vel_sign = '-1 1 1 1'
+vel_sign_dict = dict(zip(discs.split(), np.asarray(vel_sign.split()).astype(int)))
+
+incl_dict = {
     'mwc480': -37.0,
-} #sign assumes discminer convention
+    'twhyd': 5.8,
+    'imlup': -47.5,
+    'hd163296': 46.7
+}
 
 gaps_dict = {
     'mwc480': [76, 149],
+    'twhyd': [82],
+    'imlup': [116, 209],
+    'hd163296': [49, 85, 145]
 } #mm dust gaps
 
 rings_dict = {
     'mwc480': [98, 165],
+    'twhyd': [70, 160], #rings of elevated optical depth (Teague+2022)
+    'imlup': [133, 220],
+    'hd163296': [67, 101, 159]
 } #mm dust rings
 
-kinks_dict = {
-    'mwc480': [245],
-} #intensity kinks
-
 #**************************
 #GET TAGS AND PARS FROM LOG 
 #**************************
 files_dir = os.listdir()
 file_data = ''
 
 if args.log_file == '':
@@ -143,15 +152,18 @@
             argupper, arglower = np.inf, np.inf
             log_pars = np.append(log_pars, np.zeros(8))
             header += ['z0_upper', 'p_upper', 'Rb_upper', 'q_upper', 'z0_lower', 'p_lower', 'Rb_lower', 'q_lower']
 
         if 'fixincl' in kind:
             log_pars = np.append(log_pars, np.radians(incl_dict[tag_disc]))
             header += ['incl']
-                    
+            
+        log_pars = np.append(log_pars, vel_sign_dict[tag_disc])
+        header += ['vel_sign']
+        
         for i in range(len(header)):
             hdr = header[i]
             if hdr in ['p', 'q', 'Rb', 'p0', 'p1']:
                 diff_arg = np.array([i-argI0[0], i-argL0[0], i-argLs[0], i-argupper, i-arglower])                
                 diff_arg = np.where(diff_arg<=0, np.inf, diff_arg)
                 diff_min = np.argmin(diff_arg)
                 if diff_min==0: header[i]+='_I0'
@@ -265,10 +277,10 @@
     pars_dict, units_dict = get_base_pars(log_file, kind=tags_dict['kind'])
     for tk in tags_dict['kind']:
         if 'nosurf' in tk:
             pars_dict['intensity'].update({'q': 0.0})
             units_dict['intensity'].update({'q': "none"})            
             pars_dict['linewidth'].update({'q': 0.0})
             units_dict['linewidth'].update({'q': "none"})
-            
-    custom_dict.update(gaps=gaps_dict[tags_dict['disc']], rings=rings_dict[tags_dict['disc']], kinks=kinks_dict[tags_dict['disc']]) 
+
+    custom_dict.update(gaps=gaps_dict[tags_dict['disc']], rings=rings_dict[tags_dict['disc']]) 
     make_json(dicts_list = [custom_dict, tags_dict, pars_dict, units_dict], keys_list = ['custom', 'metadata', 'best_fit', 'units'])
```

### Comparing `discminer-0.2.6/_mining/make_single_moments.py` & `discminer-0.2.7/_mining/make_single_moments.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from discminer.core import Data
 
 import json
 from astropy import units as u
 from argparse import ArgumentParser
 
 parser = ArgumentParser(prog='make moments', description='Make gauss or bell moments and save outputs into .fits files')
-parser.add_argument('-k', '--kind', default='gaussian', type=str, choices=['gauss', 'gaussian', 'bell'], help="1d moment kernel")
+parser.add_argument('-m', '--method', default='gaussian', type=str, choices=['gauss', 'gaussian', 'bell'], help="1d moment kernel")
+parser.add_argument('-s', '--sigma', default=4, type=float, help='Mask out pixels with peak intensities below sigma threshold')
 args = parser.parse_args()
 
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
 meta = pars['metadata']
 
@@ -21,16 +22,16 @@
 #*********
 #LOAD DATA
 #*********
 tag = meta['tag']
 file_data = 'cube_data_%s_convtb.fits'%tag
 file_model = 'cube_model_%s_convtb.fits'%tag
 
-datacube = Data(file_data, dpc) # Read data and convert to Cube object
-modelcube = Data(file_model, dpc) # Read data and convert to Cube object
+datacube = Data(file_data, dpc) # Read datacube and convert to Cube object
+modelcube = Data(file_model, dpc) # Read modelcube and convert to Cube object
 
 #**********************
 #MAKE MOMENT MAPS
 #**********************
-moments_data = datacube.make_moments(method=args.kind, tag='data')
-moments_model = modelcube.make_moments(method=args.kind, tag='model')
+moments_data = datacube.make_moments(method=args.method, tag='data', sigma_thres=args.sigma)
+moments_model = modelcube.make_moments(method=args.method, tag='model', sigma_thres=args.sigma)
```

### Comparing `discminer-0.2.6/_mining/plot_attributes_model.py` & `discminer-0.2.7/_mining/plot_attributes_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from discminer.plottools import use_discminer_style, make_up_ax
-from utils import init_data_and_model, get_noise_mask
+from utils import init_data_and_model
 
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 
 from astropy import units as u
 
@@ -28,17 +28,14 @@
 
 Rmax = 1.1*best['intensity']['Rout']*u.au #Max model radius, 10% larger than disc Rout
 
 #*******************
 #LOAD DATA AND MODEL
 #*******************
 datacube, model = init_data_and_model()
-
-noise_mean, mask = get_noise_mask(datacube, thres=2)
-vchannels = datacube.vchannels
 model.make_model()
 
 #**************
 #MAKE PLOT
 #**************
 fig = plt.figure(figsize=(14,5))
 ax0 = fig.add_axes([0.08,0.1,0.4,0.4])
```

### Comparing `discminer-0.2.6/_mining/plot_azimuthal_profiles.py` & `discminer-0.2.7/_mining/plot_azimuthal_profiles.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,87 +9,79 @@
 from astropy.io import fits
 
 import json
 import copy
 import sys
 
 from argparse import ArgumentParser
-from utils import init_data_and_model, get_noise_mask, get_1d_plot_decorators
+from utils import (add_parser_args,
+                   load_moments,
+                   init_data_and_model,
+                   get_noise_mask,
+                   get_1d_plot_decorators)
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='plot azimuthal contours', description='Plot azimuthal contours from a given moment map [velocity, linewidth, [peakintensity, peakint]?')
-parser.add_argument('-m', '--moment', default='velocity', type=str, choices=['velocity', 'linewidth', 'lineslope', 'peakint', 'peakintensity'], help="velocity, linewidth or peakintensity")
-parser.add_argument('-k', '--kind', default='residuals', type=str, choices=['data', 'model', 'residuals'], help="data, model or residuals")
+parser.add_argument('-t', '--type', default='residuals', type=str, choices=['data', 'model', 'residuals'], help="data, model or residuals")
+args = add_parser_args(parser, moment=True, kind=True, surface=True, Rinner=True, Router=True)
 args = parser.parse_args()
 
-if args.moment=='peakint':
-     args.moment = 'peakintensity'
-
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
 meta = pars['metadata']
 best = pars['best_fit']
 custom = pars['custom']
 
 vsys = best['velocity']['vsys']
 incl = best['orientation']['incl']
 Rout = best['intensity']['Rout']
 
-clabel, clabel_res, clim0, clim0_res, clim1, clim1_res, unit = get_1d_plot_decorators(args.moment, tag=args.kind)
+clabel, clabel_res, clim0, clim0_res, clim1, clim1_res, unit = get_1d_plot_decorators(args.moment, tag=args.type)
 
-if args.kind=='residuals':
+if args.type=='residuals':
     clim0 = clim0_res
     clim1 = clim1_res
     clabel = clabel_res
 
 if args.moment=='velocity':
-    if args.kind=='residuals':
-        clabel = r'Velocity %s %s'%(args.kind, unit)
+    if args.type=='residuals':
+        clabel = r'Velocity %s %s'%(args.type, unit)
     else:
-        clabel = r'Deprojected Velocity %s %s'%(args.kind, unit)        
+        clabel = r'Deprojected Velocity %s %s'%(args.type, unit)        
 
 #*******************
 #LOAD DATA AND MODEL
 #*******************
 datacube, model = init_data_and_model()
 
 noise_mean, mask = get_noise_mask(datacube, thres=2)
 vchannels = datacube.vchannels
 model.make_model()
 
 #*************************
 #LOAD MOMENT MAPS
-moment_data = fits.getdata('%s_gaussian_data.fits'%args.moment)
-moment_model = fits.getdata('%s_gaussian_model.fits'%args.moment) 
-#moment_data = fits.getdata('%s_up_doublebell_mask_data.fits'%args.moment)
-#moment_model = fits.getdata('%s_up_doublebell_mask_model.fits'%args.moment) 
+moment_data, moment_model, residuals, mtags = load_moments(args, mask=mask)
 
-#**************************
-#MASK AND COMPUTE RESIDUALS
-moment_data = np.where(mask, np.nan, moment_data)
-moment_model = np.where(mask, np.nan, moment_model)
-moment_residuals = moment_data - moment_model
-
-if args.kind=='residuals': map2d = moment_residuals
-elif args.kind=='data': map2d = moment_data
-elif args.kind=='model': map2d = moment_model
+if args.type=='residuals': map2d = residuals
+elif args.type=='data': map2d = moment_data
+elif args.type=='model': map2d = moment_model
 
-if args.kind!='residuals' and args.moment=='velocity': #deproject velocity field
-    map2d = (map2d-vsys)/(np.cos(model.projected_coords['phi']['upper'])*np.sin(incl))
+if args.type!='residuals' and args.moment=='velocity': #deproject velocity field
+    map2d = np.abs((map2d-vsys)/(np.cos(model.projected_coords['phi']['upper'])*np.sin(incl)))
     
 #**************************
 #MAKE PLOT
 
 beam_au = datacube.beam_size.to('au').value
-R_prof = np.arange(2*beam_au, 0.8*Rout, beam_au/4)
+R_prof = np.arange(args.Rinner*beam_au, args.Router*Rout, beam_au/5)
 
 color_bounds = np.array([0.5, 1.0])*Rout
 
 rail = Rail(model, map2d, R_prof)
 
 fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,6))
 ax2 = fig.add_axes([0.85,0.6,0.3*6/14,0.3])
@@ -109,10 +101,10 @@
 
 model.make_emission_surface(ax2)
 model.make_disc_axes(ax2)
 make_up_ax(ax, labeltop=False)
 make_up_ax(ax2, labelbottom=False, labelleft=False, labeltop=True)
 ax.tick_params(labelbottom=True, top=True, right=True, which='both', direction='in')
 
-plt.savefig('azimuthal_%s_%s.png'%(args.moment, args.kind), bbox_inches='tight', dpi=200)
+plt.savefig('azimuthal_%s_%s.png'%(args.moment, args.type), bbox_inches='tight', dpi=200)
 plt.show()
 plt.close()
```

### Comparing `discminer-0.2.6/_mining/plot_moment+offset.py` & `discminer-0.2.7/_mining/plot_moment+offset.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 
 meta = pars['metadata']
 best = pars['best_fit']
 custom = pars['custom']
 vsys = best['velocity']['vsys']
 Rout = best['intensity']['Rout']
 
+rings = custom['rings']
+gaps = custom['gaps']
+kinks = []
+
 ctitle, clabel, clim, cfmt, cmap_mom, cmap_res, levels_im, levels_cc, unit = get_2d_plot_decorators(args.moment)
     
 #****************
 #SOME DEFINITIONS
 #****************
 file_data = meta['file_data']
 tag = meta['tag']
@@ -63,36 +67,31 @@
 
 #*************************
 #LOAD DISC GEOMETRY
 R, phi, z = load_disc_grid()
 
 #*************************
 #LOAD MOMENT MAPS
-moment_data, moment_model, mtags = load_moments(args)
-
-#**************************
-#MASK MOMENTS
-moment_data = np.where(mask, np.nan, moment_data)
-moment_model = np.where(mask, np.nan, moment_model)
+moment_data, moment_model, residuals, mtags = load_moments(args, mask=mask)
 
 #**************************
 #MAKE PLOT + ZOOM-IN PANEL
-
 fig, ax = plt.subplots(ncols=2, nrows=1, figsize=(15,8))
 ax_cbar0 = fig.add_axes([0.13, 0.09, 0.77, 0.05])
 
 kwargs_im = dict(cmap=cmap_mom, extent=extent, levels=levels_im)
 kwargs_cc = dict(colors='k', linestyles='-', extent=extent, levels=levels_cc, linewidths=0.4)
 kwargs_cbar = dict(orientation='horizontal', pad=0.03, shrink=0.95, aspect=15)
 zoomcolor = '0.3'
 zoomwidth = 90
-          
+        
 def make_plot(ax, xlim=xlim, color='k', labelcolor='k'):
     im = ax.contourf(moment_data, extend='both', **kwargs_im)
-    cc = ax.contour(moment_data, **kwargs_cc)
+    if args.surface!='lower':
+        cc = ax.contour(moment_data, **kwargs_cc)
     make_up_ax(axi, xlims=(-xlim, xlim), ylims=(-xlim, xlim), labelsize=17, color=color, labelcolor=labelcolor)
     return im
 
 for i,axi in enumerate(ax):
     if i==1: im = make_plot(axi, xlim=zoomwidth, color=zoomcolor, labelcolor=zoomcolor)
     else: im = make_plot(axi, xlim=xlim)
     axi.scatter(best['orientation']['xc'], best['orientation']['yc'],
@@ -110,15 +109,15 @@
         axi.spines[side].set_color(zoomcolor)
         axi.spines[side].set_linestyle((0, (1,1.5)))
         axi.spines[side].set_capstyle('round')
     axi.grid(color='k', ls='--')
     
 for i,axi in enumerate(ax):
     Contours.emission_surface(axi, R, phi, extent=extent, R_lev=np.linspace(0.1, 1.0, 10)*Rout*u.au.to('m'), which=mtags['surf'])
-     
+        
 patch = Rectangle([-zoomwidth]*2, 2*zoomwidth, 2*zoomwidth, edgecolor=zoomcolor, facecolor='none',
                   lw=2.0, ls=(0, (1,1.5)), capstyle='round')
 ax[0].add_artist(patch)
 
 cbar0 = plt.colorbar(im, cax=ax_cbar0, format='%.1f', **kwargs_cbar)
 cbar0.ax.tick_params(labelsize=15) 
 mod_nticks_cbars([cbar0], nbins=10)
```

### Comparing `discminer-0.2.6/_mining/plot_moment+residuals.py` & `discminer-0.2.7/_mining/plot_moment+residuals.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,22 +62,18 @@
 
 #*************************
 #LOAD DISC GEOMETRY
 R, phi, z = load_disc_grid()
 
 #*************************
 #LOAD MOMENT MAPS    
-moment_data, moment_model, mtags = load_moments(args)
+moment_data, moment_model, residuals, mtags = load_moments(args, mask=mask)
         
 #**************************
 #MASK AND COMPUTE RESIDUALS
-moment_data = np.where(mask, np.nan, moment_data)
-moment_model = np.where(mask, np.nan, moment_model)
-residuals = moment_data - moment_model
-
 """
 from scipy.ndimage import gaussian_filter
 moment_data = gaussian_filter(moment_data, sigma=1.5)
 moment_model = gaussian_filter(moment_model, sigma=1.5)
 residuals = moment_data - moment_model
 """
```

### Comparing `discminer-0.2.6/_mining/plot_peak_residuals.py` & `discminer-0.2.7/_mining/plot_peak_residuals.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from discminer.plottools import (get_discminer_cmap, append_sigma_panel,
                                  make_up_ax, mod_minor_ticks, mod_major_ticks,
                                  use_discminer_style, mod_nticks_cbars,
-                                 make_substructures, make_round_map)
+                                 make_substructures, make_round_map,
+                                 get_cmap_from_color, make_clusters_1d)
 from discminer.pick import Pick
-from discminer.rail import Contours
-
-import numpy as np
-import matplotlib.pyplot as plt
-
-from astropy import units as u
-import json
-import copy
-
 from utils import (init_data_and_model,
                    get_noise_mask,
                    add_parser_args,
                    get_2d_plot_decorators,
                    load_moments)
 
+import numpy as np
+import matplotlib.pyplot as plt
+from astropy import units as u
+
+import json
 from argparse import ArgumentParser
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='Identify and show peak residuals', description='Identify peak residuals in folded maps.')
 parser.add_argument('-c', '--clean_thres', default=np.inf, type=float, help="Threshold above which peak residuals will be rejected.")
+parser.add_argument('-a', '--nphi', default=8, type=int, help="Number of azimuthal clusters.")
+parser.add_argument('-r', '--nr', default=8, type=int, help="Number of radial clusters.")
 args = add_parser_args(parser, moment=True, kind=True, surface=True, fold=True, projection=True, Rinner=True, Router=True)
 
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
@@ -65,44 +64,37 @@
 
 noise_mean, mask = get_noise_mask(datacube, thres=2)
 vchannels = datacube.vchannels
 model.make_model()
 
 #*************************
 #LOAD MOMENT MAPS
-moment_data, moment_model, mtags = load_moments(args)
-
-#**************************
-#MASK AND COMPUTE RESIDUALS
-moment_data = np.where(mask, np.nan, moment_data)
-moment_model = np.where(mask, np.nan, moment_model)
-moment_residuals = moment_data - moment_model
+moment_data, moment_model, residuals, mtags = load_moments(args, mask=mask)
     
 if args.moment=='velocity' and args.fold=='absolute':
-    moment_residuals = np.abs(moment_data-vsys) - np.abs(moment_model-vsys)
+    residuals = np.abs(moment_data-vsys) - np.abs(moment_model-vsys)
 
 #*******************
 #FIND PEAK RESIDUALS
 #*******************
 beam_au = datacube.beam_size.to('au').value
 R_prof = np.arange(args.Rinner*beam_au, args.Router*Rout, beam_au/5)
 xlim0, xlim1 = 0.5*R_prof[0], 1.05*R_prof[-1]
 
 fig, ax = plt.subplots(ncols=2, nrows=1, figsize=(11,5))    
 ax_c = fig.add_axes([0.8,0.65,0.23*5/11,0.23]) #AxesSubplot for showing contour colours 
 
-pick = Pick(model, moment_residuals, R_prof, fold=True, color_bounds = np.array([0.33, 0.66, 1.0])*Rout, ax2=ax_c)
+pick = Pick(model, residuals, R_prof, fold=True, color_bounds = np.array([0.33, 0.66, 1.0])*Rout, ax2=ax_c)
 folded_map = pick.make_2d_map() #Map where peaks will be picked from
 pick.find_peaks(clean_thres=args.clean_thres)
 
 lev = pick.lev_list
 color = pick.color_list
 peak_resid = pick.peak_resid
 peak_angle = pick.peak_angle
-peak_resid = pick.peak_resid
 
 model.make_emission_surface(ax_c)
 model.make_disc_axes(ax_c)
 ax_c.axis('off')
 
 #*******************
 #SHOW PEAK RESIDUALS
@@ -165,17 +157,28 @@
     ax.scatter(lev*cos_peak, lev*sin_peak, edgecolors='none', facecolors=color, alpha=0.2, s=100)
     ax.scatter(lev*cos_peak, lev*sin_peak, edgecolors='none', facecolors=color, alpha=1.0, s=10)
     ax.scatter(lev*cos_peak, lev*sin_peak, edgecolors='0.3', facecolors='none', alpha=1.0, s=100)
     ax.set_title('%s, folded map'%ctitle, fontsize=16, color='k')
     
 
 plt.savefig('folded_residuals_deproj_%s_%s.png'%(mtags['base'], args.projection), bbox_inches='tight', dpi=200)
+plt.show()
 plt.close()
 
 #*************
 #FIND CLUSTERS
 #*************
-pick.find_clusters(n_phi=8, n_R=8)
+try:
+    pick.find_clusters(n_phi=args.nphi, n_R=args.nr)
+except np.linalg.LinAlgError:
+    print ('Cluster finder algorithm failed due to low amount of points')
 
 #*************
 #PLOT CLUSTERS
 #*************
+fig, ax = make_clusters_1d(pick, which='phi')
+plt.savefig('clusters_phi_peak_residuals_%s_%dclust.png'%(mtags['base'], args.nphi), bbox_inches='tight', dpi=200)
+plt.show()
+
+fig, ax = make_clusters_1d(pick, which='r')
+plt.savefig('clusters_r_peak_residuals_%s_%dclust.png'%(mtags['base'], args.nr), bbox_inches='tight', dpi=200)
+plt.show()
```

### Comparing `discminer-0.2.6/_mining/plot_radial_profiles.py` & `discminer-0.2.7/_mining/plot_radial_profiles.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from discminer.plottools import (get_discminer_cmap, make_substructures,
                                  make_up_ax, mod_minor_ticks, mod_major_ticks,
                                  use_discminer_style, mod_nticks_cbars)
 from discminer.rail import Rail, Contours
 
 import numpy as np
 import matplotlib.pyplot as plt
+from matplotlib.ticker import FormatStrFormatter
 from scipy.signal import savgol_filter
 from scipy.interpolate import interp1d
 
 from astropy import units as u
 from astropy.io import fits
 import json
 import copy
@@ -65,29 +66,22 @@
 R, phi, z = load_disc_grid()
 
 R_s = R[args.surface]*u.m.to('au')
 phi_s = phi[args.surface]
 
 #*************************
 #LOAD MOMENT MAPS
-moment_data, moment_model, mtags = load_moments(args)
-if mtags['surf']=='both':
-    surf_ref = 'upper'
-else:
-    surf_ref = args.surface
+moment_data, moment_model, residuals, mtags = load_moments(args, mask=mask)
+ref_surf = mtags['ref_surf']
 tag_base = mtags['base']
 
 #**************************
-#MASK AND COMPUTE RESIDUALS
-moment_data = np.where(mask, np.nan, moment_data)
-moment_model = np.where(mask, np.nan, moment_model)
-moment_residuals = moment_data - moment_model
-    
+#ABSOLUTE RESIDUALS    
 if args.moment=='velocity':
-    moment_residuals_abs = np.abs(moment_data-vsys) - np.abs(moment_model-vsys)
+    residuals_abs = np.abs(moment_data-vsys) - np.abs(moment_model-vsys)
 
 #**************************
 #MAKE PLOTS
 beam_au = datacube.beam_size.to('au').value
 R_prof = np.arange(args.Rinner*beam_au, args.Router*Rout, beam_au/5)
 xlim0, xlim1 = 0.5*R_prof[0], 1.05*R_prof[-1]
 
@@ -107,213 +101,273 @@
         div_factor = -np.cos(np.abs(incl))        
     else: return comp
     
     return div_factor
 
 def make_savgol(prof):
     try:
-        ysav = savgol_filter(prof, 5, 3)
-        ysav_deriv = savgol_filter(prof, 5, 3, deriv=1)
+        ysav = savgol_filter(prof, 9, 3)
+        ysav_deriv = savgol_filter(prof, 9, 3, deriv=1)
     except np.linalg.LinAlgError:
         ysav = prof
         ysav_deriv = None
     return ysav, ysav_deriv 
 
+def make_basic_layout(ax):
+    ax.set_xlim(xlim0, xlim1)
+    ax.set_xlabel('Radius [au]', fontsize=MEDIUM_SIZE)
+    mod_major_ticks(ax, axis='x', nbins=10)
+    mod_minor_ticks(ax)
+    ax.axhline(0, lw=2, ls='--', color='0.7')
+
+def make_profile(ax, R_prof, ysav, y, yerr, kind='data', perr='bar', **kwargs):
+    if kind=='data':
+        label = 'Data'
+        color = 'tomato'
+        zorder = 9
+        lw = 3.5        
+    elif kind=='residuals':
+        label = 'Residuals'
+        color = '0.1'
+        zorder = 9
+        lw = 3.5
+    elif kind=='model':
+        label = 'Model'
+        color = 'dodgerblue'
+        zorder = 8
+        lw = 3.5
+    elif kind=='vphi':
+        label = r'$\Delta\upsilon_\phi$'
+        color = 'dodgerblue'
+        zorder = 9
+        lw = 3.0
+    elif kind=='vz':
+        label = r'$\upsilon_{\rm z}$'
+        color = 'k'
+        zorder = 8
+        lw = 3.0
+    elif kind=='vr':
+        label = r'$\upsilon_{\rm R}$'
+        color = '#FFB000'
+        zorder = 7
+        lw = 3.0
+    else:
+        raise ValueError(kind)
+
+    ax.plot(R_prof, ysav, c=color, lw=lw, label=label, zorder=zorder)
+
+    if kind!='model':
+        if perr=='bar':
+            ax.errorbar(R_prof, y, yerr=yerr, c=color,
+                        elinewidth=1.2, capsize=1.8, linestyle='none',
+                        marker='o', ms=6.5, markeredgewidth=1.7, markerfacecolor='0.8',
+                        alpha=0.7, zorder=zorder)
+        elif perr=='fill':
+            ax.fill_between(R_prof, y+yerr, y-yerr, color=color, alpha=0.15, zorder=zorder)
+        else:
+            raise ValueError(perr)
+        
+    if args.writetxt: writetxt([R_prof, y, yerr], tag=kind)
+
+
+    
+#*************
+#MAIN BODY
+#*************
 
 if args.moment=='velocity':
+
     mask_ang = args.mask_minor #+-mask around disc minor axis
+
     #*******************
     #VELOCITY COMPONENTS
     #*******************    
 
     #VZ
-    rail_vz = Rail(model, moment_residuals, R_prof)
-    vel_z, vel_z_error = rail_vz.get_average(mask_ang=mask_ang, surface=surf_ref)
+    rail_vz = Rail(model, residuals, R_prof)
+    vel_z, vel_z_error = rail_vz.get_average(mask_ang=mask_ang, surface=ref_surf)
     div_factor_z = get_normalisation(mask_ang, component='z')
 
     vel_z /= div_factor_z
     vel_z_error /= div_factor_z 
 
     #DVPHI
-    rail_phi = Rail(model, moment_residuals_abs, R_prof)
-    vel_phi, vel_phi_error = rail_phi.get_average(mask_ang=mask_ang, surface=surf_ref)
+    rail_phi = Rail(model, residuals_abs, R_prof)
+    vel_phi, vel_phi_error = rail_phi.get_average(mask_ang=mask_ang, surface=ref_surf)
     div_factor_phi = get_normalisation(mask_ang, component='phi')
 
     vel_phi /= div_factor_phi
     vel_phi_error /= div_factor_phi 
 
     #VPHI
     rail_phi = Rail(model, np.abs(moment_data-vsys), R_prof)
-    vel_rot, _ = rail_phi.get_average(mask_ang=mask_ang, surface=surf_ref)
+    vel_rot, _ = rail_phi.get_average(mask_ang=mask_ang, surface=ref_surf)
     vel_rot /= div_factor_phi
     vel_rot_error = vel_phi_error
 
     #VR
     mask_r = mask | (np.abs(phi_s) < np.radians(args.mask_major)) | (np.abs(phi_s) > np.radians(180-args.mask_major))
     moment_data_r = np.where(mask_r, np.nan, moment_data) 
 
     f_vp = interp1d(R_prof, vel_rot)
     f_vz = interp1d(R_prof, vel_z)
     R_interp = np.where((R_s>R_prof[0]) & (R_s<R_prof[-1]), R_s, R_prof[0])
 
     vr = -1/(np.sin(phi_s)*np.sin(incl)) * (moment_data_r - vsys - vel_sign*f_vp(R_interp)*np.cos(phi_s)*np.sin(incl) + f_vz(R_interp)*np.cos(incl))
 
     rail_vr = Rail(model, vr, R_prof)
-    vel_r, vel_r_error = rail_vr.get_average(mask_ang=0.0, surface=surf_ref, av_func=np.nanmedian)
-
-    #WRITE?
-    if args.writetxt: writetxt([R_prof, vel_z, vel_z_error], tag='vz')
-    if args.writetxt: writetxt([R_prof, vel_r, vel_r_error], tag='vr')
-    if args.writetxt: writetxt([R_prof, vel_phi, vel_phi_error], tag='vphi')
-    if args.writetxt: writetxt([R_prof, vel_rot, vel_phi_error], tag='rotationcurve')
+    vel_r, vel_r_error = rail_vr.get_average(mask_ang=0.0, surface=ref_surf, av_func=np.nanmedian)
     
     #PLOT 3D VELOCITIES
-    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(11,4))
         
     ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)
-    ax.plot(R_prof, ysav_phi, c='dodgerblue', lw=3, label=r'$\Delta\upsilon_\phi$', zorder=12)
-    ax.fill_between(R_prof, vel_phi+vel_phi_error, vel_phi-vel_phi_error, color='dodgerblue', alpha=0.15, zorder=9)
+    make_profile(ax, R_prof, ysav_phi, vel_phi, vel_phi_error, kind='vphi', perr='fill')
 
     ysav_z, ysav_z_deriv = make_savgol(vel_z)    
-    ax.plot(R_prof, ysav_z, c='k', lw=3, label=r'$\upsilon_{\rm z}$', zorder=8)
-    ax.fill_between(R_prof, vel_z+vel_z_error, vel_z-vel_z_error, color='k', alpha=0.15, zorder=8)
-        
+    make_profile(ax, R_prof, ysav_z, vel_z, vel_z_error, kind='vz', perr='fill')
+    
     ysav_r, ysav_r_deriv = make_savgol(vel_r)
-    ax.plot(R_prof, ysav_r, c='#FFB000', lw=3, label=r'$\upsilon_{\rm R}$', zorder=7)
-    ax.fill_between(R_prof, vel_r+vel_r_error, vel_r-vel_r_error, color='#FFB000', alpha=0.15, zorder=7)
+    make_profile(ax, R_prof, ysav_r, vel_r, vel_r_error, kind='vr', perr='fill')    
 
-    ax.axhline(0, lw=2, ls='--', color='0.7')
-    
-    ax.set_xlabel('Radius [au]')
-    ax.set_xlim(xlim0, xlim1)
-    ax.set_ylabel(r'$\delta\upsilon$ [km/s]')
+    #DECORATIONS
+    make_basic_layout(ax)
+    ax.set_ylabel(r'$\delta\upsilon$ [km/s]', fontsize=MEDIUM_SIZE)
     ax.set_ylim(clim0_res, clim1_res)
-    mod_major_ticks(ax, axis='x', nbins=10)
-    mod_minor_ticks(ax)
-    make_1d_legend(ax, fontsize=MEDIUM_SIZE+1)
-    
+    make_1d_legend(ax, fontsize=MEDIUM_SIZE+1)    
     make_substructures(ax, gaps=gaps, rings=rings, label_gaps=True, label_rings=True)
     
     plt.savefig('velocity_components_%s.png'%tag_base, bbox_inches='tight', dpi=200)
     plt.show()
 
     #*******************
     #ROTATION CURVE
     #*******************
-    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))        
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(11,4))        
 
     #DATA CURVE
     ysav_rot, ysav_rot_deriv = make_savgol(vel_rot)
-    ax.plot(R_prof, ysav_rot, c='tomato', lw=3.5, label=r'Data', zorder=12)
-    ax.fill_between(R_prof, vel_rot+vel_rot_error, vel_rot-vel_rot_error, color='tomato', alpha=0.15, zorder=9)
-    
-    #r"""
+    make_profile(ax, R_prof, ysav_rot, vel_rot, vel_rot_error, kind='data')
+
     #MODEL CURVE
     rail_phi = Rail(model, np.abs(moment_model-vsys), R_prof)
-    vel_phi, _ = rail_phi.get_average(mask_ang=mask_ang, surface=surf_ref)
+    vel_phi, _ = rail_phi.get_average(mask_ang=mask_ang, surface=ref_surf)
     vel_phi /= div_factor_phi
-    ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)
-    ax.plot(R_prof, ysav_phi, c='0.7', lw=4.0, label=r'Model', zorder=11)
-    #"""
+    ysav_phi, ysav_phi_deriv_mod = make_savgol(vel_phi)
+    make_profile(ax, R_prof, ysav_phi, vel_phi, _, kind='model')
     
     #PERFECT KEPLERIAN
     coords = {'R': R_prof*u.au.to('m')}
-    velocity_upper = model.get_attribute_map(coords, 'velocity', surface=surf_ref) * vel_sign
+    velocity_upper = model.get_attribute_map(coords, 'velocity', surface=ref_surf) * vel_sign
     ax.plot(R_prof, velocity_upper, c='k', lw=2.5, ls='--', label=r'Keplerian (%.2f Msun)'%Mstar, zorder=13)
 
     #DECORATIONS
-    ax.axhline(0, lw=2, ls='--', color='0.7')
-
-    ax.set_xlabel('Radius [au]')
-    ax.set_xlim(xlim0, xlim1)    
-    ax.set_ylabel(r'Rotation velocity [km/s]')
+    make_basic_layout(ax)
+    ax.set_ylabel(r'Rotation velocity [km/s]', fontsize=MEDIUM_SIZE)
     ax.set_ylim(clim0, 1.2*np.nanmax(vel_phi))
-    mod_major_ticks(ax, axis='x', nbins=10)
-    mod_minor_ticks(ax)    
-    make_1d_legend(ax)
-
+    make_1d_legend(ax, fontsize=MEDIUM_SIZE-3)
     make_substructures(ax, gaps=gaps, rings=rings, label_gaps=True, label_rings=True)  
     
     plt.savefig('rotation_curve_%s.png'%tag_base, bbox_inches='tight', dpi=200)
     plt.show()
 
     """
     #Data rotation curve - perfect_Keplerian
     fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4)) 
     ax.plot(R_prof, vel_rot-velocity_upper, c='k', lw=2.5, ls='--', label=r'Keplerian (%.2f Msun)'%Mstar, zorder=13)
     plt.show()
     """
     
 else:
-    mask_ang = 0.0
+
+    mask_ang = args.mask_minor
+
+    if args.surface in ['low', 'lower']:
+        mask_r = mask | (np.abs(phi_s) < np.radians(args.mask_major)) | (np.abs(phi_s) > np.radians(180-args.mask_major))
+        moment_data = np.where(mask_r, np.nan, moment_data) 
+    
     #*****************
     #ABSOLUTE PROFILES
     #*****************
-    kw_avg = dict(surface=surf_ref, av_func=np.nanmedian, mask_ang=mask_ang)
+    kw_avg = dict(surface=ref_surf, av_func=np.nanmedian, mask_ang=mask_ang)
     
-    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))
+    fig, ax = plt.subplots(ncols=1, nrows=2, figsize=(11,7))
 
     #DATA CURVE
     rail_phi = Rail(model, moment_data, R_prof)
     vel_phi, vel_phi_error = rail_phi.get_average(**kw_avg)
 
     ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)    
-    ax.plot(R_prof, ysav_phi, c='tomato', lw=4.0, label=r'Data', zorder=12)
-    ax.fill_between(R_prof, vel_phi+vel_phi_error, vel_phi-vel_phi_error, color='tomato', alpha=0.15, zorder=9)
-
-    if args.writetxt: writetxt([R_prof, vel_phi, vel_phi_error], tag='data')
+    make_profile(ax[0], R_prof, ysav_phi, vel_phi, vel_phi_error, kind='data')    
 
     #MODEL CURVE
     rail_phi = Rail(model, moment_model, R_prof)
     vel_phi, vel_phi_error = rail_phi.get_average(**kw_avg)
 
-    ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)    
-    ax.plot(R_prof, ysav_phi, c='dodgerblue', lw=3.5, label=r'Model', zorder=11)
-
-    if args.writetxt: writetxt([R_prof, vel_phi, vel_phi_error], tag='model')
-    
-    #DECORATIONS
-    ax.axhline(0, lw=2, ls='--', color='0.7')
-
-    ax.set_xlabel('Radius [au]')
-    ax.set_xlim(xlim0, xlim1)    
-    ax.set_ylabel(clabel)
-    ax.set_ylim(clim0, clim1)
-    mod_major_ticks(ax, axis='x', nbins=10)
-    mod_minor_ticks(ax)
-    make_1d_legend(ax)
-
-    make_substructures(ax, gaps=gaps, rings=rings, label_gaps=True, label_rings=True)  
-    
-    plt.savefig('radial_profile_%s.png'%tag_base, bbox_inches='tight', dpi=200)
-    plt.show()
+    ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)
+    make_profile(ax[0], R_prof, ysav_phi, vel_phi, vel_phi_error, kind='model')        
 
-    #****************
     #RESIDUALS
-    #****************    
-    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))
-
-    rail_phi = Rail(model, moment_residuals, R_prof)
+    rail_phi = Rail(model, residuals, R_prof)
     vel_phi, vel_phi_error = rail_phi.get_average(**kw_avg)
 
-    ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)    
-    ax.plot(R_prof, ysav_phi, c='tomato', lw=4.0, label=r'Residuals', zorder=12)
-    ax.fill_between(R_prof, vel_phi+vel_phi_error, vel_phi-vel_phi_error, color='tomato', alpha=0.15, zorder=9)
-
-    if args.writetxt: writetxt([R_prof, vel_phi, vel_phi_error], tag='residuals')    
+    ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)
+    make_profile(ax[1], R_prof, ysav_phi, vel_phi, vel_phi_error, kind='residuals')
 
+    #***********
     #DECORATIONS
-    ax.axhline(0, lw=2, ls='--', color='0.7')
-
-    ax.set_xlabel('Radius [au]')
-    ax.set_xlim(xlim0, xlim1)    
-    ax.set_ylabel(clabel_res)
-    ax.set_ylim(clim0_res, clim1_res)
-    mod_major_ticks(ax, axis='x', nbins=10)
-    mod_minor_ticks(ax)
+    #***********
+    ax[0].set_ylim(clim0, clim1)
+    ax[1].set_ylim(clim0_res, clim1_res)
+
+    #fmt
+    #******    
+    ticks = ax[1].get_yticks()
+
+    makeint = False
+    for tick in ticks:
+        if str(tick)[-2:] != '.0':
+            break
+        else:
+            makeint = True
+
+    ftick = round(ticks[0], 2)
+    ftick = int(ftick) if makeint else ftick
+    
+    isfloat = isinstance(ftick, float)
+    lfmt = len(str(ftick))
+    
+    if isfloat:
+        if ftick<0.2:
+            ftick_res = str(ftick)+'0'
+            lfmt+=1
 
-    make_substructures(ax, gaps=gaps, rings=rings, label_gaps=True, label_rings=True)
+        ndec = len(str(ftick).split('.')[-1])
+        ndec_res = len(str(ftick_res).split('.')[-1])
         
-    plt.savefig('radial_profile_residuals_%s.png'%tag_base, bbox_inches='tight', dpi=200)
-    plt.show()
+        cfmt = '%'+'%d.%df'%(lfmt, ndec)
+        cfmt_res = '%'+'%d.%df'%(lfmt, ndec_res)
+        
+    else:
+        cfmt = cfmt_res = '%'+'%dd'%lfmt
     
+    #******
+    #Axes
+    #****
+    for axi in ax:
+        make_basic_layout(axi)
+        axi.tick_params(which='both', labelsize=MEDIUM_SIZE-2)
+
+    ax[0].yaxis.set_major_formatter(FormatStrFormatter(cfmt))
+    ax[1].yaxis.set_major_formatter(FormatStrFormatter(cfmt_res))            
+    ax[0].set_xlabel(None)
+    ax[1].set_xlabel('Radius [au]', fontsize=MEDIUM_SIZE)
+    ax[0].set_ylabel(clabel, fontsize=MEDIUM_SIZE)
+    ax[1].set_ylabel('Residuals'+clabel_res.split('residuals')[-1], fontsize=MEDIUM_SIZE)
 
+    make_1d_legend(ax[0], ncol=2)
+
+    make_substructures(ax[0], gaps=gaps, rings=rings, label_gaps=True, label_rings=True)  
+    make_substructures(ax[1], gaps=gaps, rings=rings)
+    
+    plt.savefig('radial_profile_%s.png'%tag_base, bbox_inches='tight', dpi=200)
+    plt.show()
```

### Comparing `discminer-0.2.6/_mining/plot_residuals+all.py` & `discminer-0.2.7/_mining/plot_residuals+all.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import copy
 from argparse import ArgumentParser
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='plot moment maps', description='Plot moment map [velocity, linewidth, [peakintensity, peakint]?')
 parser.add_argument('-c', '--coords', default='sky', type=str, choices=['disc', 'sky'], help="reference frame")
-args = add_parser_args(parser, kind=True, surface=True)
+args = add_parser_args(parser, kind=True, surface=True, Rinner=True, Router=True)
      
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
@@ -87,28 +87,33 @@
 moments_data = {}
 moments_model = {}
 residuals = {}
 mtags = {}
 mtypes = ['linewidth', 'velocity', 'peakintensity']
 
 for moment in mtypes:
-    md, mm, mt = load_moments(args, moment=moment)
-    md = np.where(mask, np.nan, md)
-    mm = np.where(mask, np.nan, mm)     
+    if args.coords=='sky':
+        md, mm, rr, mt = load_moments(args, moment=moment, mask=mask)
+    elif args.coords=='disc':
+        md, mm, rr, mt = load_moments(
+            args,
+            moment=moment,
+            mask=mask,
+            clip_Rmin=args.Rinner*datacube.beam_size,
+            clip_Rmax=args.Router*Rout*u.au,
+            clip_Rgrid=R[args.surface]*u.m
+        )        
     mtags[moment] = mt
     moments_data[moment] = md 
     moments_model[moment] = mm 
-    residuals[moment] = md - mm
+    residuals[moment] = rr
          
 #****************
 #USEFUL FUNCTIONS
 #****************
-def clip_prop_radially(prop2d, Rmin=datacube.beam_size.to('au').value, Rmax=np.inf, Rgrid=R_nonan_au):
-    return np.where((Rgrid<Rmin) | (Rgrid>Rmax), np.nan, prop2d)
-
 def decorate_ax_res_2D(ax, cbar, lim=xlim):
     ax.set_aspect(1)
     make_up_ax(ax, xlims=(-lim,lim), ylims=(-lim,lim), labelsize=13)
     ax.set_xlabel('Offset [au]')
     ax.xaxis.set_label_position('top')    
     cbar.ax.tick_params(which='major', direction='in', width=2.7, size=4.8, pad=4, labelsize=12)
     cbar.ax.tick_params(which='minor', direction='in', width=2.3, size=3.3)
@@ -132,29 +137,30 @@
     levels_resid = np.linspace(-clim, clim, 32)
     levels_cbar = np.linspace(-clim, clim, 5)
 
     kwargs_im = dict(cmap=cmap_res, levels=levels_resid, extend='both', origin='lower')
     kwargs_cbar = dict(orientation='horizontal', format=cfmt, ticks=levels_cbar, pad=0.03, shrink=0.95, aspect=15)    
     
     if args.coords=='sky':
-        #clip_prop_radially(residuals[moment])
         im = axi.contourf(residuals[moment], extent=extent, **kwargs_im)
         Contours.emission_surface(axi, R, phi, extent=extent,
                                   R_lev=np.linspace(0.1, 1.0, 10)*Rout*au_to_m,
                                   which=mtags['velocity']['surf']
         )
         Contours.disc_axes(axi,
                            R[args.surface][nh]/au_to_m,
                            z[args.surface][nh]/au_to_m,
                            incl, PA, xc=xc, yc=yc)
         
     elif args.coords=='disc':
-        im = axi.contourf(Xproj, Yproj, clip_prop_radially(residuals[moment], Rmax=Rout), **kwargs_im)                         
-        make_substructures(axi, gaps=gaps, rings=rings, twodim=True)
-        _make_radial_grid_2D(axi, Rout, gaps=gaps, rings=rings, make_labels=True, label_freq=2)
+        im = axi.contourf(Xproj, Yproj, residuals[moment], **kwargs_im)
+        #make_substructures(axi, gaps=gaps, rings=rings, twodim=True)
+        if Rout>700: lf = 4
+        else: lf = 2
+        _make_radial_grid_2D(axi, args.Router*Rout, gaps=gaps, make_labels=True, label_freq=lf)
         
     cbar = plt.colorbar(im, cax=cbar_axes[i], **kwargs_cbar)
     cbar.set_label(clabels[moment], fontsize=14)
 
     decorate_ax_res_2D(axi, cbar)
     datacube.plot_beam(axi, fc='lime')
```

### Comparing `discminer-0.2.6/_mining/plot_residuals+deproj.py` & `discminer-0.2.7/_mining/plot_residuals+deproj.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from discminer.core import Data
-from discminer.rail import Contours
 import discminer.cart as cart
 from discminer.plottools import (make_round_map,
                                  make_polar_map,
                                  make_substructures,
                                  make_up_ax,
                                  mod_major_ticks,
                                  mod_nticks_cbars,
                                  use_discminer_style)
 
-from utils import (get_2d_plot_decorators,
+from utils import (make_and_save_filaments,
+                   init_data_and_model,
+                   get_2d_plot_decorators,
                    get_noise_mask,
                    load_moments,
                    load_disc_grid,
                    add_parser_args)
 
 import numpy as np
 import matplotlib.pyplot as plt
@@ -21,15 +22,16 @@
 
 import json
 from argparse import ArgumentParser
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='plot residual maps', description='Plot residual maps')
-args = add_parser_args(parser, moment=True, kind=True, surface=True, projection=True)
+parser.add_argument('-f', '--filaments', default=0, type=int, choices=[0, 1], help="Make filaments")
+args = add_parser_args(parser, moment=True, kind=True, surface=True, projection=True, Rinner=True, Router=True)
 
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
@@ -77,67 +79,69 @@
 #LOAD DISC GEOMETRY
 R, phi, z = load_disc_grid()
 
 Xproj = R[args.surface]*np.cos(phi[args.surface])
 Yproj = R[args.surface]*np.sin(phi[args.surface])
 
 #*************************
-#LOAD MOMENT MAPS    
-moment_data, moment_model, mtags = load_moments(args)
-
-#****************
-#USEFUL FUNCTIONS
-#****************
-def clip_prop_radially(prop2d, Rmin=datacube.beam_size, Rmax=np.inf, Rgrid=R[args.surface]*u.m):
-    Rmin = Rmin.to('au').value
-    Rgrid = np.nan_to_num(Rgrid).to('au').value
-    try:
-        Rmax = Rmax.to('au').value
-    except AttributeError:
-        Rmax = Rmax
-    return np.where((Rgrid<Rmin) | (Rgrid>Rmax), np.nan, prop2d)
-
-#**************************
-#MASK AND COMPUTE RESIDUALS
-moment_data = np.where(mask, np.nan, moment_data)
-moment_model = np.where(mask, np.nan, moment_model)
-residuals = clip_prop_radially(moment_data - moment_model, Rmax=Rout)
+#LOAD AND CLIP MOMENT MAPS    
+moment_data, moment_model, residuals, mtags = load_moments(
+    args,
+    mask=mask,
+    clip_Rmin=0.0*u.au,
+    clip_Rmax=args.Router*Rout*u.au,
+    clip_Rgrid=R[args.surface]*u.m
+)
+#residuals = moment_data
+#cmap_res = cmap_mom
 
+#***********
+#MAKE PLOTS
 clabels = {
     'linewidth': r'$\Delta$ Line width [km s$^{-1}$]',
     'lineslope': r'$\Delta$ Line slope',
     'velocity': r'$\Delta$ Centroid [km s$^{-1}$]',
     'peakintensity': r'$\Delta$ Peak Int. [K]'
 }
 
+   
 if args.projection=='cartesian':
     levels_resid = np.linspace(-clim, clim, 32)
     
     if args.surface in ['up', 'upper']:
         z_func = cart.z_upper_exp_tapered
         z_pars = best['height_upper']
 
     elif args.surface in ['low', 'lower']:
         z_func = cart.z_lower_exp_tapered
         z_pars = best['height_lower']
     
-    fig, ax = make_round_map(residuals, levels_resid, Xproj*u.m, Yproj*u.m, Rout*u.au,
+    fig, ax = make_round_map(residuals, levels_resid, Xproj*u.m, Yproj*u.m, args.Router*Rout*u.au,
                              z_func=z_func, z_pars=z_pars, incl=incl, PA=PA, xc=xc, yc=yc,
                              cmap=cmap_res, clabel=unit, fmt=cfmt, 
-                             gaps=gaps, rings=rings)
+                             gaps=gaps, rings=rings,
+                             mask_inner=args.Rinner*datacube.beam_size)
     
     make_substructures(ax, gaps=gaps, rings=rings, twodim=True, label_rings=True)
 
+    if args.filaments:
+        _, model = init_data_and_model()
+        model.make_model()
+        fil_pos, fil_neg = make_and_save_filaments(model, residuals, tag=mtags['base']+'_'+args.projection, return_all=False)        
+
+        ax.contour(Xproj/au_to_m, Yproj/au_to_m, fil_pos.skeleton, linewidths=0.2, colors='darkred', alpha=1, zorder=11)
+        ax.contour(Xproj/au_to_m, Yproj/au_to_m, fil_neg.skeleton, linewidths=0.2, colors='navy', alpha=1, zorder=11)
+    
 elif args.projection=='polar':
-    levels_resid = np.linspace(-clim, clim, 48)    
+    levels_resid = np.linspace(-clim, clim, 48)    #levels_im #
     fig, ax, cbar = make_polar_map(residuals, levels_resid,
-                                   R[args.surface]*u.m, phi[args.surface]*u.rad, Rout*u.au,
-                                   Rin = datacube.beam_size,
+                                   R[args.surface]*u.m, phi[args.surface]*u.rad, args.Router*Rout*u.au,
+                                   Rin=args.Rinner*datacube.beam_size,
                                    cmap=cmap_res, fmt=cfmt, clabel=clabels[args.moment])
                                    
     make_substructures(ax, gaps=gaps, rings=rings, twodim=True, polar=True, label_rings=True)
     
 ax.set_title(ctitle, fontsize=16, color='k')
 
-plt.savefig('residuals_deproj_%s_%s.png'%(mtags['base'], args.projection), bbox_inches='tight', dpi=200)
+plt.savefig('residuals_deproj_%s_%s_.png'%(mtags['base'], args.projection), bbox_inches='tight', dpi=200)
 plt.show()
 plt.close()
```

### Comparing `discminer-0.2.6/_mining/utils.py` & `discminer-0.2.7/_mining/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 import json
 import decimal
 import warnings
 import copy
 
 from discminer.plottools import get_discminer_cmap
 from discminer.core import Data
+from discminer.rail import Rail
 from discminer.disc2d import Model
 import discminer.cart as cart
 
 from astropy.io import fits
 import astropy.units as u
 
 import numpy as np
+import matplotlib
 
 molplot = {
     '12co': r'$^{\rm 12}$CO',
     '13co': r'$^{\rm 13}$CO',
     'cs': r'CS'
 }
 
@@ -35,31 +37,31 @@
                     fold=False, writetxt=False, 
 ):
 
     if moment:
         parser.add_argument('-m', '--moment', default='velocity', type=str, choices=['velocity', 'linewidth', 'lineslope', 'peakint', 'peakintensity'], help="velocity, linewidth or peakintensity")
 
     if mask_minor:
-        parser.add_argument('-b', '--mask_minor', default=60.0, type=float, help="+- azimuthal mask around disc minor axis for computation of vphi and vz velocity components")
+        parser.add_argument('-b', '--mask_minor', default=30.0, type=float, help="+- azimuthal mask around disc minor axis for computation of vphi and vz velocity components")
     if mask_major:
         parser.add_argument('-a', '--mask_major', default=30.0, type=float, help="+- azimuthal mask around disc major axis for computation of vR velocity component")
     if kind:
         parser.add_argument('-k', '--kind', default='gaussian', type=str, choices=['gauss', 'gaussian', 'bell', 'dgauss', 'doublegaussian', 'dbell', 'doublebell'], help="gauss(or gaussian), dbell(or doublebell)")
     if surface:
         parser.add_argument('-s', '--surface', default='upper', type=str, choices=['up', 'upper', 'low', 'lower'], help="upper or lower surface moment map")
     if fold:
         parser.add_argument('-f', '--fold', default='absolute', type=str, choices=['absolute', 'standard'], help="if moment=velocity, fold absolute or standard velocity residuals")
     if projection:
         parser.add_argument('-p', '--projection', default='cartesian', type=str, choices=['cartesian', 'polar'], help="Project residuals onto a cartesian or a polar map")
     if writetxt:
-        parser.add_argument('-w', '--writetxt', default=False, type=bool, help="write txt files")
+        parser.add_argument('-w', '--writetxt', default=1, type=int, choices=[0, 1], help="write txt files")
     if Rinner:
         parser.add_argument('-i', '--Rinner', default=1.0, type=float, help="Number of beams to mask out from inner region")
     if Router:
-        parser.add_argument('-o', '--Router', default=0.9, type=float, help="Fraction of Rout to consider as the outer radius for the analysis")
+        parser.add_argument('-o', '--Router', default=0.98, type=float, help="Fraction of Rout to consider as the outer radius for the analysis")
 
     args = parser.parse_args()
 
     try:
         if args.moment=='peakint':
             args.moment = 'peakintensity'
     except AttributeError:
@@ -84,27 +86,33 @@
 
     datacube = Data(file_data, dpc) # Read data and convert to Cube object
 
     if init_model:
         Rmax = Rmax*Rout*u.au
         model = Model(datacube, Rmax=Rmax, Rmin=Rmin, prototype=True)
         
-        model.z_upper_func = cart.z_upper_exp_tapered
-        model.z_lower_func = cart.z_lower_exp_tapered
         model.velocity_func = model.keplerian_vertical # vrot = sqrt(GM/r**3)*R
         model.line_profile = model.line_profile_bell
         model.line_uplow = model.line_uplow_mask
-    
+
         if 'I2pwl' in meta['kind']:
             model.intensity_func = cart.intensity_powerlaw_rbreak
         elif 'I2pwlnosurf' in meta['kind']:
             model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
         else:
             model.intensity_func = cart.intensity_powerlaw_rout
 
+        if 'surf2pwl' in meta['kind']:
+            model.z_upper_func = cart.z_upper_powerlaw
+            model.z_lower_func = cart.z_lower_powerlaw
+        else:
+            model.z_upper_func = cart.z_upper_exp_tapered
+            model.z_lower_func = cart.z_lower_exp_tapered
+
+            
         #****************
         #PROTOTYPE PARAMS
         #****************
         model.params = copy.copy(best)
         model.params['intensity']['I0'] /= meta['downsamp_factor']
 
         return datacube, model
@@ -245,41 +253,70 @@
     if return_mean:
         noise_mean = np.mean(noise)
         mask = np.nanmax(data, axis=0) < thres*noise_mean
         return noise_mean, mask
     else:
         mask = np.nanmax(data, axis=0) < thres*noise
         return noise, mask
-    
-def load_moments(args, moment=None):
-    if moment is None: moment = args.moment
-    if moment=='peakint': moment='peakintensity'
+
+def load_moments(
+        args, moment=None, mask=[],
+        clip_Rgrid=None, clip_Rmin=0*u.au, clip_Rmax=np.inf*u.au
+):    
+    if moment is None:
+        moment = args.moment
     
     if args.kind in ['gauss', 'gaussian', 'bell']:
-        tag_surf = 'both' 
+        tag_surf = 'both'
+        ref_surf = 'upper' #For contour plots
     else:
         if args.surface in ['up', 'upper']:
-            tag_surf = 'up' 
+            tag_surf = 'up'
+            ref_surf = 'upper'
         elif args.surface in ['low', 'lower']:
             tag_surf = 'low'
-
+            ref_surf = 'lower'
+            
     if args.kind in ['gauss', 'gaussian']:
         tag_base = f'{moment}_gaussian'
     elif args.kind in ['bell']:
         tag_base = f'{moment}_bell'
     elif args.kind in ['dgauss', 'doublegaussian']:
         tag_base = f'{moment}_{tag_surf}_doublegaussian_mask'
     elif args.kind in ['dbell', 'doublebell']:
         tag_base = f'{moment}_{tag_surf}_doublebell_mask'
 
+    #Read and mask moment maps, and compute residuals
     moment_data = fits.getdata(tag_base+'_data.fits')
     moment_model = fits.getdata(tag_base+'_model.fits')
-    
-    return moment_data, moment_model, dict(surf=tag_surf, base=tag_base)
 
+    moment_data[mask] = np.nan
+    moment_model[mask] = np.nan
+    
+    def clip_radially(prop2d): #should be within masking function in discminer         
+        Rmin = clip_Rmin.to('au').value
+        Rgrid = np.nan_to_num(clip_Rgrid).to('au').value
+        Rmax = clip_Rmax.to('au').value
+        return np.where((Rgrid<Rmin) | (Rgrid>Rmax), np.nan, prop2d)    
+
+    if isinstance(clip_Rgrid, np.ndarray):        
+        moment_data = clip_radially(moment_data)
+        moment_model = clip_radially(moment_model)
+        
+    residuals = moment_data - moment_model
+        
+    if args.surface in ['low', 'lower']:
+        pass
+        #from scipy.ndimage import gaussian_filter
+        #moment_data = gaussian_filter(moment_data, 0.5)
+        #moment_data[moment_data > 50.0] = np.nan
+        
+    return moment_data, moment_model, residuals, dict(surf=tag_surf, ref_surf=ref_surf, base=tag_base)
+    
+    
 def load_disc_grid():
     R = dict(
         upper=np.load('upper_R.npy'),
         lower=np.load('lower_R.npy')
     )
 
     phi = dict(
@@ -290,10 +327,72 @@
     z = dict(
         upper=np.load('upper_z.npy'),
         lower=np.load('lower_z.npy')
     )
     return R, phi, z
 
 def make_1d_legend(ax, **kwargs):
-    kwargs_def = dict(frameon=False, fontsize=MEDIUM_SIZE-2, ncol=3, loc='lower right', bbox_to_anchor=(1.0, 1.0))
+    kwargs_def = dict(
+        frameon=False,
+        fontsize=MEDIUM_SIZE,
+        ncol=3,
+        handlelength=2.0,
+        handletextpad=0.5,
+        borderpad=0.0,
+        columnspacing=1.5,
+        loc='lower right',
+        bbox_to_anchor=(1.0, 1.0)
+    )
     kwargs_def.update(kwargs)
     return ax.legend(**kwargs_def)
+
+def make_and_save_filaments(model, map2d,
+                            writefits=True, tag='',
+                            return_all=True, cmap='jet'
+):
+    mrail = Rail(model, map2d)
+    fil_pos, fil_neg = mrail.make_filaments(
+        smooth_size=0.1*model.beam_size,
+        adapt_thresh=model.beam_size,
+        size_thresh=100*u.pix**2
+    )
+    masked_pos = np.ma.masked_where(fil_pos.skeleton!=1, fil_pos.skeleton)
+    masked_neg = np.ma.masked_where(fil_neg.skeleton!=1, fil_neg.skeleton)
+
+    #ax.imshow(masked_pos, cmap='Reds_r', alpha=1, zorder=3, extent = [mm.X.min(),mm.X.max(), mm.Y.min(),mm.Y.max()], origin='lower')
+    #ax.imshow(masked_neg, cmap='Blues_r', alpha=1, zorder=3, extent = [mm.X.min(),mm.X.max(), mm.Y.min(),mm.Y.max()], origin='lower')
+    
+    fil_pos_list = [fil_pos.skeleton, fil_pos.skeleton_longpath]
+    fil_neg_list = [fil_neg.skeleton, fil_neg.skeleton_longpath]
+        
+    for fil in fil_pos.filaments:
+        fil_i = np.zeros_like(fil_pos.skeleton)
+        fil_i[fil.pixel_coords] = 1 
+        fil_pos_list.append(fil_i)
+            
+    for fil in fil_neg.filaments:
+        fil_i = np.zeros_like(fil_neg.skeleton)
+        fil_i[fil.pixel_coords] = 1 
+        fil_neg_list.append(fil_i)
+
+    if writefits:
+        if len(tag)>0:
+            if tag[0]!='_':
+                tag='_'+tag
+                
+        fits.writeto('filaments_pos%s.fits'%tag, np.asarray(fil_pos_list), header=model.header, overwrite=True)
+        fits.writeto('filaments_neg%s.fits'%tag, np.asarray(fil_neg_list), overwrite=True)
+
+    if return_all:
+        cmap = matplotlib.cm.get_cmap(cmap)
+        npos = len(fil_pos.filaments)
+        nneg = len(fil_neg.filaments)
+        cpos = np.linspace(0.6, 1.0, npos)        
+        cneg = np.linspace(0.4, 0.0, nneg)
+        colors_dict = {}
+        colors_dict.update({i+1: matplotlib.colors.to_hex(cmap(cpos[i])) for i in range(npos)})
+        colors_dict.update({-i-1: matplotlib.colors.to_hex(cmap(cneg[i])) for i in range(nneg)})
+
+        return fil_pos_list, fil_neg_list, colors_dict
+
+    else:
+        return fil_pos, fil_neg
```

### Comparing `discminer-0.2.6/discminer/cart.py` & `discminer-0.2.7/discminer/cart.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/core.py` & `discminer-0.2.7/discminer/core.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/cube.py` & `discminer-0.2.7/discminer/cube.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/disc2d.py` & `discminer-0.2.7/discminer/disc2d.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/grid.py` & `discminer-0.2.7/discminer/grid.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/icons/button_box.png` & `discminer-0.2.7/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/icons/button_cursor.jpeg` & `discminer-0.2.7/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/icons/button_path.png` & `discminer-0.2.7/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/icons/button_return.png` & `discminer-0.2.7/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/icons/button_surface.png` & `discminer-0.2.7/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/icons/button_trash.jpg` & `discminer-0.2.7/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/pick.py` & `discminer-0.2.7/discminer/pick.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/plottools.py` & `discminer-0.2.7/discminer/plottools.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/rail.py` & `discminer-0.2.7/discminer/rail.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,16 +173,16 @@
         coord_list, lev_list, resid_list, color_list = [], [], [], []
         if np.sum(coord_levels==coord_ref)==0 and coord_ref is not None: coord_levels = np.append(coord_levels, coord_ref)
         for lev in coord_levels:
             contour = measure.find_contours(coords[0], lev) #, fully_connected='high', positive_orientation='high')
             if len(contour)==0:
                 print ('no contours found for phi =', lev)
                 continue
-            ind_good = np.argmin([np.abs(lev-coords[0][tuple(np.round(contour[i][0]).astype(np.int))]) for i in range(len(contour))]) #get contour id closest to lev
-            inds_cont = np.round(contour[ind_good]).astype(np.int)
+            ind_good = np.argmin([np.abs(lev-coords[0][tuple(np.round(contour[i][0]).astype(int))]) for i in range(len(contour))]) #get contour id closest to lev
+            inds_cont = np.round(contour[ind_good]).astype(int)
             inds_cont = [tuple(f) for f in inds_cont]
             first_cont = np.array([coords[0][i] for i in inds_cont])
             second_cont = np.array([coords[1][i] for i in inds_cont])
             prop_cont = np.array([prop[i] for i in inds_cont])
 
             corr_inds = np.abs(first_cont-lev) < acc_threshold #clean based on acc_threshold
```

### Comparing `discminer-0.2.6/discminer/testyapf.py` & `discminer-0.2.7/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/tools/discminer.mplstyle` & `discminer-0.2.7/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/tools/fit_kernel.py` & `discminer-0.2.7/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer/tools/utils.py` & `discminer-0.2.7/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/discminer.egg-info/PKG-INFO` & `discminer-0.2.7/discminer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.6 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.7 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.6/discminer.egg-info/SOURCES.txt` & `discminer-0.2.7/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/setup.py` & `discminer-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/template/README.rst` & `discminer-0.2.7/template/README.rst`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/template/download_MAPS.sh` & `discminer-0.2.7/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.2.7/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.6/template/prepare_data.py` & `discminer-0.2.7/template/prepare_data.py`

 * *Files identical despite different names*

