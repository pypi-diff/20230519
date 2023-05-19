# Comparing `tmp/energyplus_launch-3.6.7.tar.gz` & `tmp/energyplus_launch-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.6.7.tar", last modified: Wed Apr 26 21:38:00 2023, max compression
+gzip compressed data, was "energyplus_launch-3.6.8.tar", last modified: Fri May 19 19:08:18 2023, max compression
```

## Comparing `energyplus_launch-3.6.7.tar` & `energyplus_launch-3.6.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.742522 energyplus_launch-3.6.7/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.742522 energyplus_launch-3.6.7/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.742522 energyplus_launch-3.6.7/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    72348 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/widget_group_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.496853 energyplus_launch-3.6.8/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-19 19:08:18.000000 energyplus_launch-3.6.8/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.496853 energyplus_launch-3.6.8/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.496853 energyplus_launch-3.6.8/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6214 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73621 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/interface/widget_group_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-19 19:08:18.500853 energyplus_launch-3.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-05-19 19:08:10.000000 energyplus_launch-3.6.8/setup.py
```

### Comparing `energyplus_launch-3.6.7/LICENSE` & `energyplus_launch-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/PKG-INFO` & `energyplus_launch-3.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.6.7
+Version: 3.6.8
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.7/README.md` & `energyplus_launch-3.6.8/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.6.8/energyplus_launch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.6.7
+Version: 3.6.8
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.7/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.6.8/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/config.py` & `energyplus_launch-3.6.8/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.6.8/eplaunch/interface/dialog_external_viewers.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,20 @@
         super().__init__()
         self.title("Viewers")
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.suffixes = ['txt'] + list_of_suffixes
         self.extension_to_viewer = dict_of_viewer_overrides
         self._define_tk_variables()
         self._build_gui()
+        self.update_idletasks()
+        self.geometry(
+            "%dx%d+%d+%d" % (
+                self.winfo_width(), self.winfo_height(), parent_window.winfo_x() + 25, parent_window.winfo_y() + 25
+            )
+        )
         self.grab_set()
         self.transient(parent_window)
 
     def _define_tk_variables(self):
         self._tk_var_extension_list = Variable()
         self._tk_var_application_path = StringVar()
```

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.6.8/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.6.8/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.6.8/eplaunch/interface/dialog_weather.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,20 @@
         # assume cancel to allow for closing the dialog with the X
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.selected_weather_file: Optional[Path] = None
         self._epw_from_select = None
         # build the gui and call required modal methods
         self._define_tk_variables()
         self._build_gui(recent_files)
+        self.update_idletasks()
+        self.geometry(
+            "%dx%d+%d+%d" % (
+                self.winfo_width(), self.winfo_height(), parent_window.winfo_x() + 25, parent_window.winfo_y() + 25
+            )
+        )
         self.grab_set()
         self.transient(parent_window)
 
     def _define_tk_variables(self):
         self._tk_var_recent = StringVar(value="")
         self._tk_var_recent.trace('w', self._recent_changed)
         self._tk_var_select_epw_name = StringVar(value="<select_an_epw>")
```

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.6.8/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,20 @@
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.list_of_directories: List[Path] = []
         self._auto_find_dirs = auto_found_workflow_dirs
         self._tk_var_all_directories = Variable(value=current_workflow_dirs)
         self.selected_index = -1
         # build the gui and call required modal methods
         self._build_gui()
+        self.update_idletasks()
+        self.geometry(
+            "%dx%d+%d+%d" % (
+                self.winfo_width(), self.winfo_height(), parent_window.winfo_x() + 25, parent_window.winfo_y() + 25
+            )
+        )
         self.grab_set()
         self.transient(parent_window)
 
     def _update_from_traces(self, _=None):
         selected_indices = self.listbox.curselection()
         if len(selected_indices) != 1:
             self.selected_index = -1
```

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/frame_main.py` & `energyplus_launch-3.6.8/eplaunch/interface/frame_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime
 from fnmatch import fnmatch
 
 from json import dumps
 from mimetypes import guess_type
+from os import getenv
 from pathlib import Path
 from platform import system
 from queue import Queue
 from sys import version_info
 
 from subprocess import Popen
 from tkinter import Tk, PhotoImage, StringVar, Menu, DISABLED, Frame, Label, NSEW, E, VERTICAL, \
@@ -118,15 +119,15 @@
         self._repopulate_recent_weather_list()
         self._rebuild_recent_folder_menu()
         self._rebuild_favorite_folder_menu()
         self._rebuild_group_menu()
         self._init = False
 
         # finally set the initial directory and update the file listing
-        self.dir_tree.dir_list.refresh_listing(self.conf.directory)
+        self.dir_tree.dir_list.try_to_select_directory(self.conf.directory)
         self._update_file_list()
 
         # set the minimum size and redraw the app
         self.minsize(1050, 400)
         self.update()  # one quick redraw should be fine here to get updated geometry
         self.dir_files_pw.sashpos(0, self.conf.dir_file_paned_window_sash_position)
         self.conf.list_group_paned_window_sash_position = min(
@@ -345,17 +346,15 @@
 
     def _build_listings(self, container: Frame):
         # use vertical for the primary paned window
         self.list_group_pw = ttkPanedWindow(container, orient=VERTICAL)
         # create a sub paned window that is vertical to split the directory from the group box
         self.dir_files_pw = ttkPanedWindow(container, orient=HORIZONTAL)
         # the top part of this pane is simply the directory tree, add it with a heavier weight
-        self.dir_tree = DirListScrollableFrame(
-            self.dir_files_pw, on_select=self._new_dir_selected, on_root_changed=self._new_root_dir
-        )
+        self.dir_tree = DirListScrollableFrame(self.dir_files_pw, on_select=self._new_dir_selected)
         self.dir_files_pw.add(self.dir_tree, weight=1)
         self.file_list = FileListScrollableFrame(
             self.dir_files_pw, on_selection_changed=self._callback_file_selection_changed
         )
         self.dir_files_pw.add(self.file_list, weight=1)
         self.list_group_pw.add(self.dir_files_pw, weight=5)
         # the bottom part of the primary pane will be a label frame containing a group listbox, add it with lower weight
@@ -566,15 +565,15 @@
         except IndexError:
             messagebox.showerror("Error", f"Could not navigate to group entry at index {idx}")
             return
         if not entry.exists():
             messagebox.showerror("Error", f"Could not navigate to group entry, it doesn't exist: {entry}")
             return
         self.conf.directory = entry.parent
-        self.dir_tree.dir_list.refresh_listing(self.conf.directory)
+        self.dir_tree.dir_list.try_to_select_directory(self.conf.directory)
         self._update_file_list()
         self.file_list.tree.try_to_reselect([entry.name])
 
     # endregion
 
     # region handling file/folder navigation
 
@@ -611,15 +610,15 @@
         for index, folder in enumerate(self.conf.folders_favorite):
             self.menu_nav_favorites.add_command(
                 label=str(folder), command=lambda i=index: self._handle_favorite_folder_selection(i)
             )
 
     def _handle_favorite_folder_selection(self, folder_index: int):
         self.conf.directory = self.conf.folders_favorite[folder_index]
-        self.dir_tree.dir_list.refresh_listing(self.conf.directory)
+        self.dir_tree.dir_list.try_to_select_directory(self.conf.directory)
         self._update_file_list()
 
     def _rebuild_recent_folder_menu(self):
         self.menu_nav_recent.delete(0, END)
         for index, folder in enumerate(self.conf.folders_recent):
             self.menu_nav_recent.add_command(
                 label=str(folder), command=lambda i=index: self._handle_recent_folder_selection(i)
@@ -627,15 +626,15 @@
 
     def _navigate_to_previous_folder(self):
         if len(self.conf.folders_recent) > 1:
             self._handle_recent_folder_selection(1)
 
     def _handle_recent_folder_selection(self, folder_index: int):
         self.conf.directory = self.conf.folders_recent[folder_index]
-        self.dir_tree.dir_list.refresh_listing(self.conf.directory)
+        self.dir_tree.dir_list.try_to_select_directory(self.conf.directory)
         self._update_file_list()
 
     def _get_files_in_current_directory(self, workflow_file_patterns: List[str]) -> List[Tuple[str, str, str, str]]:
         """
         Returns a list of file information for each file in the currently selected directory
         :param workflow_file_patterns: List of file patterns that this workflow supports, for filtering
         :return: A list of tuples which each contain (file name, file type, file size, modified time) for each file
@@ -658,29 +657,28 @@
                 guessed_type = guess_type(base_name)[0]
                 file_type_string = "(unknown)" if guessed_type is None else guessed_type
                 file_list.append((base_name, file_type_string, file_size_string, modified_time_string))
         # sort the list and return it
         file_list.sort(key=lambda x: x[0])
         return file_list
 
-    def _new_dir_selected(self, _: bool, selected_path: Path):
+    def _new_dir_selected(self, selected_path: Path):
         self.previous_selected_directory = self.conf.directory
         self.conf.directory = selected_path
-        if len(self.conf.folders_recent) > 0 and self.conf.folders_recent[0] != selected_path:
+        if len(self.conf.folders_recent) == 0:
+            self.conf.folders_recent.appendleft(selected_path)
+        elif len(self.conf.folders_recent) > 0 and self.conf.folders_recent[0] != selected_path:
             self.conf.folders_recent.appendleft(selected_path)
         self._rebuild_recent_folder_menu()
         try:
             self._update_status_bar(f"Selected directory: {self.conf.directory}")
             self._update_file_list()
         except Exception as e:  # noqa -- status_bar and things may not exist during initialization, just ignore
             print(str(e))  # log it to the console for fun
 
-    def _new_root_dir(self, new_root_path: Path):
-        self._new_dir_selected(True, new_root_path)
-
     def _update_file_list(self):
         """Update the file listing widget by querying the directory and cache contents, try to reselect current files"""
         # If selected directory hasn't been set up yet then just carry on, this is only happening during app init
         if self._init or not self.conf.directory:
             return
 
         # If we aren't in a directory, just warn and abort, should not really be possible to get him after init
@@ -744,15 +742,15 @@
             # always add the row to the main list
             control_list_rows.append(row)
 
         # clear all items from the listview and then add them back in
         self.file_list.tree.set_files(control_list_rows)
         if previous_selected_files:
             self.file_list.tree.try_to_reselect(previous_selected_files)
-        self._rebuild_group_menu()
+        # self._rebuild_group_menu()
 
     def _is_file_stale(self, input_file_name: str) -> Optional[bool]:
         """
         Returns a tri-state value trying to characterize whether the current file is "stale."
         It tries to determine this based on the output suffixes of the current workflow.
         If the current workflow does not include any output suffixes, "stale" cannot be determined.
         If '.err' is in the output suffixes, this is the only suffix checked.
@@ -765,15 +763,17 @@
         if full_file_path.exists():
             input_file_date = full_file_path.lstat().st_mtime
             suffixes = self.workflow_manager.current_workflow.output_suffixes
             if '.err' in suffixes:  # for energyplus workflows just use the err file
                 suffixes = ['.err']
             file_name_no_ext = full_file_path.with_suffix('').name
             for suffix in suffixes:
-                tentative_output_file_path = self.conf.directory / (file_name_no_ext + suffix)
+                output_sub_dir = f"EPLaunchRun_{file_name_no_ext}"
+                output_file_name = file_name_no_ext + suffix
+                tentative_output_file_path = self.conf.directory / output_sub_dir / output_file_name
                 if tentative_output_file_path.exists():
                     output_file_date = tentative_output_file_path.lstat().st_mtime
                     if output_file_date < input_file_date:
                         return True
         return False
 
     def _callback_file_selection_changed(self, selected_file_names: List[str]) -> None:
@@ -1307,21 +1307,23 @@
             eplus_specific_output_path = self.conf.directory / eplus_sub_dir / f"{filename_no_ext}{suffix_to_open}"
             eplus_specific_output_file = str(eplus_specific_output_path)
             if new_path.exists():
                 if suffix_to_open in self.conf.viewer_overrides:
                     if self.conf.viewer_overrides[suffix_to_open] is not None:
                         # then the viewer override was found, and not None, so use it
                         Popen([str(self.conf.viewer_overrides[suffix_to_open]), new_path_str])
+                        continue
                 # if we make it this far, we didn't open it with a custom viewer, try to use the default
                 self._open_file_or_dir_with_default(new_path)
             elif eplus_specific_output_path.exists():
                 if suffix_to_open in self.conf.viewer_overrides:
                     if self.conf.viewer_overrides[suffix_to_open] is not None:
                         # then the viewer override was found, and not None, so use it
                         Popen([str(self.conf.viewer_overrides[suffix_to_open]), eplus_specific_output_file])
+                        continue
                 # if we make it this far, we didn't open it with a custom viewer, try to use the default
                 self._open_file_or_dir_with_default(eplus_specific_output_path)
             else:
                 message = """At least some of the output files were not found.
 Make sure that the workflow has run on the selected input file(s), and that the runs
 actually generated the requested outputs.  Any found output files are being opened now."""
                 messagebox.showwarning("Missing Output Files", message)
@@ -1369,16 +1371,42 @@
 
     def _open_text_editor(self) -> None:
         for file_name in self.conf.file_selection:
             full_path_str = self.conf.directory / file_name
             if 'txt' in self.conf.viewer_overrides and self.conf.viewer_overrides['txt']:
                 text_editor_binary = str(self.conf.viewer_overrides['txt'])
                 Popen([text_editor_binary, full_path_str])
-            else:
-                self._open_file_or_dir_with_default(full_path_str)
+                return
+            if system() == 'Windows':
+                potential_program = self._find_default_text_editor_on_windows()
+                if potential_program != '':
+                    Popen([potential_program, full_path_str])
+                    return
+            # if neither of those work, just open with the default editor
+            self._open_file_or_dir_with_default(full_path_str)
+
+    @staticmethod
+    def _find_default_text_editor_on_windows() -> str:
+        from winreg import OpenKey, QueryValueEx, HKEY_CLASSES_ROOT
+        try:
+            key = OpenKey(HKEY_CLASSES_ROOT, '.txt')
+            default_value, _ = QueryValueEx(key, '')
+            key.Close()
+
+            key = OpenKey(HKEY_CLASSES_ROOT, default_value + r'\shell\open\command')
+            command, _ = QueryValueEx(key, '')
+            key.Close()
+
+            # resolve the SystemRoot item
+            command = command.replace('%SystemRoot%', getenv('SystemRoot'))
+
+            # then just take the program name by splitting any trailing % placeholders
+            return command.split('%')[0].strip()
+        except WindowsError:
+            return ''
 
     def _open_file_browser(self) -> None:
         self._open_file_or_dir_with_default(self.conf.directory)
 
     @staticmethod
     def _open_documentation() -> None:
         open_web(DOCS_URL)
```

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.6.8/eplaunch/interface/widget_dir_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,117 +1,134 @@
 from pathlib import Path
-from tkinter import Tk, NSEW, VERTICAL, HORIZONTAL, Frame, END, NS, TOP, BOTH, EW, PhotoImage, BROWSE, filedialog
+from platform import system
+from string import ascii_uppercase
+from tkinter import Tk, NSEW, VERTICAL, HORIZONTAL, Frame, END, NS, TOP, BOTH, EW, PhotoImage, BROWSE
 from tkinter.ttk import Treeview, Scrollbar
-from typing import Callable, Optional
+from typing import Callable, List, Optional
 
 
 class DirListWidget(Treeview):
     def __init__(
             self, parent_frame: Frame,
-            on_select: Optional[Callable[[bool, Path], None]] = None,
-            on_root_changed: Optional[Callable[[Path], None]] = None
+            on_select: Optional[Callable[[Path], None]] = None
     ):
         super().__init__(parent_frame, selectmode=BROWSE)
-        # member variables
-        self.directory_node_ids = []
-        self.root_path = None  # Path
+        self.heading('#0', text='Directory Selection Tree')
         # disable callbacks while widget is initializing
         self.callback_on_new_selection = None
-        self.callback_on_root_changed = None
-        # set up the initial directory listing
+        # set some paths to icons
         this_file_dir = Path(__file__).parent.resolve()
-        initial_root_path = Path(this_file_dir)
         folder_icon_path = this_file_dir / 'resources' / 'folder_opened.png'
         self.root_folder_image = PhotoImage(file=folder_icon_path)
         folder_closed_icon_path = this_file_dir / 'resources' / 'folder_closed.png'
         self.non_root_folder_image = PhotoImage(file=folder_closed_icon_path)
-        self.root_node = self.insert('', END, text=this_file_dir.anchor, open=True, image=self.root_folder_image)
-        self.refresh_listing(initial_root_path)
-        # bind some events, we may just forward them to callbacks
+        # load the drive root(s), initially closed, with a single dummy item inside, so it allows expanding
+        self.root_node_ids = []
+        for r in DirListWidget.get_roots_by_platform():
+            drive_root = self.insert('', END, text=r.anchor, open=False, tags=r.parts)
+            self.root_node_ids.append(drive_root)
+            self.insert(drive_root, END, text='{loading}', open=False, image=self.non_root_folder_image)
+        # bind the click event
         self.bind('<<TreeviewSelect>>', self._item_selected)
-        self.bind('<Double-1>', self._item_double_clicked)
+        self.bind('<<TreeviewOpen>>', self._item_expanded)
         # connect bindings
         self.callback_on_new_selection = on_select
-        self.callback_on_root_changed = on_root_changed
+
+    def _item_expanded(self, *_):
+        item_id = self.focus()
+        self._rebuild_single_node(item_id)
+
+    def _rebuild_single_node(self, item_id: str):
+        item_details = self.item(item_id)
+        item_path = Path(*item_details['tags'])
+        # first delete any items from this node
+        for item in self.get_children(item_id):
+            self.delete(item)
+        # now rebuild it
+        raw_child_paths = []
+        try:
+            for f in item_path.iterdir():
+                if f.is_dir():
+                    raw_child_paths.append(f)
+        except PermissionError:
+            self.insert(item_id, END, text="{access_denied}", open=False, image=self.non_root_folder_image)
+            return
+        if len(raw_child_paths) == 0:
+            self.insert(item_id, END, text="{empty}", open=False, image=self.non_root_folder_image)
+        else:
+            new_child_file_paths = sorted(raw_child_paths)
+            for path in new_child_file_paths:
+                new_child_id = self.insert(
+                    item_id, END, text=path.name, open=False, image=self.non_root_folder_image, tags=path.parts
+                )
+                self.insert(new_child_id, END, text="{loading}", open=False, image=self.non_root_folder_image)
+
+    @staticmethod
+    def get_roots_by_platform() -> List[Path]:
+        platform_name = system()
+        if platform_name == 'Windows':
+            from ctypes import windll
+            bitmask = windll.kernel32.GetLogicalDrives()
+            roots: List[Path] = []
+            for letter in ascii_uppercase:
+                if bitmask & 1:
+                    roots.append(Path(f"{letter}:\\"))
+                bitmask >>= 1
+        else:  # Linux/Mac
+            roots = [Path('/')]
+        return roots
 
     def _item_selected(self, *_):
         if len(self.selection()) != 1:
             return  # must not have selected anything
         single_selected_item_id = self.selection()[0]
         item_contents = self.item(single_selected_item_id)
         if self.callback_on_new_selection:
-            is_root = single_selected_item_id == self.root_node
-            if is_root:
-                selected_path = self.root_path
-            else:
-                selected_path = Path(item_contents['values'][0])
-            self.callback_on_new_selection(is_root, selected_path)
-
-    def _item_double_clicked(self, *_):
-        if len(self.selection()) != 1:
-            return  # must not have selected anything
-        # with select-mode set to browse there should only be one selected item at a time
-        single_selected_item_id = self.selection()[0]
-        item_contents = self.item(single_selected_item_id)
-        # default double click behavior is to reset the root to the double-clicked folder
-        if single_selected_item_id == self.root_node:
-            return
-        # values will only hold one extra item, the absolute path for that node
-        clicked_node_path = item_contents['values'][0]
-        self.refresh_listing(Path(clicked_node_path))
-
-    def reset_tree(self):
-        self.heading('#0', text="(Dir Path)", anchor='w', command=self.select_new_root)
-        for item in self.directory_node_ids:
-            self.delete(item)
-        self.directory_node_ids.clear()
+            selected_path = Path(*item_contents['tags'])
+            self.callback_on_new_selection(selected_path)
 
-    def select_new_root(self):
-        response = filedialog.askdirectory()
-        if not response:
-            return
-        p = Path(response)
-        if p.exists():
-            self.refresh_listing(p)
-
-    def refresh_listing(self, new_path: Optional[Path] = None):
-        self.reset_tree()
-        if new_path is not None:
-            string_root = str(new_path)
-            self.heading('#0', text="Click here to select root...")
-            self.root_path = new_path
-            self.item(self.root_node, text=string_root, image=self.root_folder_image)
-        new_id = self.insert(
-            self.root_node, 'end', text=".. (parent dir)", values=(str(self.root_path.parent),),
-            image=self.non_root_folder_image
-        )
-        self.directory_node_ids.append(new_id)
-        for p in sorted(self.root_path.glob('*')):
-            if p.is_dir() and not p.name.startswith('.') and not p.name.startswith('__py'):
-                new_id = self.insert(
-                    self.root_node, 'end', text=str(p.name), open=False, values=(str(p),),
-                    image=self.non_root_folder_image
-                )
-                self.directory_node_ids.append(new_id)
-            # elif p.is_file() and not p.name.startswith('.') and not p.name.startswith('__'):
-            #     print(f"Filename \"{p.name}\"; File path \"{str(p)}\"")
-        # self.update()
-        if new_path and self.callback_on_root_changed:
-            self.callback_on_root_changed(new_path)
-        self.selection_set(self.root_node)
+    def try_to_select_directory(self, target_path: Path):
+        path_parts = target_path.parts
+        # loop over each root, looking for the root node that matches the root of the target path
+        # this is treated a little different because root paths could look weird on Windows, so
+        # instead of a string match, I'm doing a pathlib.Path() equality check
+        for found_root in self.root_node_ids:
+            root_item = self.item(found_root)
+            root_name = root_item['tags'][0]
+            if Path(root_name) == Path(target_path.anchor):
+                break
+        else:
+            # Could not find the root directory, just select the root
+            raise Exception("Not an exception eventually")
+        latest_parent_id = found_root
+        items_to_expand = [latest_parent_id]
+        self._rebuild_single_node(latest_parent_id)
+        for ind, part in enumerate(path_parts):
+            if ind == 0:
+                continue  # we already got the root
+            for child_node_id in self.get_children(latest_parent_id):
+                this_child_node = self.item(child_node_id)
+                if this_child_node['text'] == part:
+                    latest_parent_id = child_node_id
+                    items_to_expand.append(latest_parent_id)
+                    self._rebuild_single_node(latest_parent_id)
+                    break
+        for i in items_to_expand:
+            self.item(i, open=True)
+        self.selection_set(latest_parent_id)
+        self.see(latest_parent_id)
 
 
 class DirListScrollableFrame(Frame):
     def __init__(
             self, parent,
-            on_select: Optional[Callable[[bool, Path], None]] = None,
-            on_root_changed: Optional[Callable[[Path], None]] = None
+            on_select: Optional[Callable[[Path], None]] = None
     ):
         super().__init__(parent)
-        self.dir_list = DirListWidget(self, on_select, on_root_changed)
+        self.dir_list = DirListWidget(self, on_select)
         self.dir_list.grid(row=0, column=0, sticky=NSEW)
         ysb = Scrollbar(self, orient=VERTICAL, command=self.dir_list.yview)
         xsb = Scrollbar(self, orient=HORIZONTAL, command=self.dir_list.xview)
         self.dir_list.configure(yscrollcommand=ysb.set, xscrollcommand=xsb.set)
         ysb.grid(row=0, column=1, sticky=NS)
         xsb.grid(row=1, column=0, sticky=EW)
         self.grid_rowconfigure(0, weight=1)
@@ -119,8 +136,9 @@
 
 
 if __name__ == "__main__":
     root = Tk()
     root.title('Directory Listing Widget Demo')
     file_listing = DirListScrollableFrame(root)
     file_listing.pack(side=TOP, expand=True, fill=BOTH)
+    file_listing.dir_list.try_to_select_directory(Path('/eplus/repos/1eplus'))
     root.mainloop()
```

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.6.8/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/interface/widget_group_list.py` & `energyplus_launch-3.6.8/eplaunch/interface/widget_group_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/utilities/cache.py` & `energyplus_launch-3.6.8/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.6.8/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/utilities/version.py` & `energyplus_launch-3.6.8/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/workflows/base.py` & `energyplus_launch-3.6.8/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.6.8/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.6.8/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.6.8/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/workflows/manager.py` & `energyplus_launch-3.6.8/eplaunch/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/workflows/workflow.py` & `energyplus_launch-3.6.8/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.6.8/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.6.8/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.7/setup.py` & `energyplus_launch-3.6.8/setup.py`

 * *Files identical despite different names*

