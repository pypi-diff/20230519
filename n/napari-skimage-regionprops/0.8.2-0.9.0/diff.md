# Comparing `tmp/napari-skimage-regionprops-0.8.2.tar.gz` & `tmp/napari-skimage-regionprops-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-skimage-regionprops-0.8.2.tar", last modified: Tue Mar  7 10:30:35 2023, max compression
+gzip compressed data, was "napari-skimage-regionprops-0.9.0.tar", last modified: Sat Mar 11 08:15:36 2023, max compression
```

## Comparing `napari-skimage-regionprops-0.8.2.tar` & `napari-skimage-regionprops-0.9.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 10:30:35.480942 napari-skimage-regionprops-0.8.2/
-drwxrwxrwx   0        0        0        0 2023-03-07 10:30:35.398224 napari-skimage-regionprops-0.8.2/.github/
-drwxrwxrwx   0        0        0        0 2023-03-07 10:30:35.406302 napari-skimage-regionprops-0.8.2/.github/workflows/
--rw-rw-rw-   0        0        0      603 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/.github/workflows/plugin_preview.yml
--rw-rw-rw-   0        0        0     2661 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1053 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-07 10:30:35.406302 napari-skimage-regionprops-0.8.2/.napari/
--rw-rw-rw-   0        0        0      303 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/.napari/config.yml
--rw-rw-rw-   0        0        0     1554 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/LICENSE
--rw-rw-rw-   0        0        0      181 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9893 2023-03-07 10:30:35.480942 napari-skimage-regionprops-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     8726 2023-03-07 10:28:21.000000 napari-skimage-regionprops-0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-07 10:30:35.437552 napari-skimage-regionprops-0.8.2/data/
--rw-rw-rw-   0        0        0      435 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.8.2/data/BBBC007_reference.txt
--rw-rw-rw-   0        0        0    53130 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.8.2/data/actin.tif
--rw-rw-rw-   0        0        0   105872 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.8.2/data/cell_labels.tif
--rw-rw-rw-   0        0        0    53130 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.8.2/data/dna.tif
--rw-rw-rw-   0        0        0   105872 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.8.2/data/dna_labels.tif
--rwxrwxrwx   0        0        0      201 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/deploy.bat
--rw-rw-rw-   0        0        0   199095 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/measure_point_coordinate.png
--rw-rw-rw-   0        0        0   192170 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/measure_point_intensity.png
-drwxrwxrwx   0        0        0        0 2023-03-07 10:30:35.454340 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/
--rw-rw-rw-   0        0        0      959 2023-03-07 10:26:42.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/__init__.py
--rw-rw-rw-   0        0        0     5425 2023-02-02 19:27:24.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_all_frames.py
--rw-rw-rw-   0        0        0     1241 2023-02-02 19:27:24.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_load_csv.py
--rw-rw-rw-   0        0        0     2058 2023-01-15 16:56:44.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_measure_points.py
--rw-rw-rw-   0        0        0    37787 2023-03-07 10:23:38.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_multichannel.py
--rw-rw-rw-   0        0        0     3337 2023-01-29 10:45:07.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_parametric_images.py
--rw-rw-rw-   0        0        0    10055 2023-03-04 19:23:18.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_process_tables.py
--rw-rw-rw-   0        0        0    10703 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_regionprops.py
--rw-rw-rw-   0        0        0    12766 2023-02-27 15:57:38.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_table.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:30:35.480942 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_tests/
--rw-rw-rw-   0        0        0        2 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_tests/__init__.py
--rw-rw-rw-   0        0        0    13090 2023-01-29 08:51:40.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_tests/test_function.py
--rw-rw-rw-   0        0        0     7558 2023-03-07 10:23:26.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_tests/test_things_inside_things.py
--rw-rw-rw-   0        0        0     3256 2022-12-20 23:05:22.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_tests/test_timelapse.py
--rw-rw-rw-   0        0        0     1481 2023-02-02 19:27:24.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:30:35.470437 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/
--rw-rw-rw-   0        0        0     9893 2023-03-07 10:30:34.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1273 2023-03-07 10:30:35.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 10:30:34.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2023-03-07 10:30:34.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      120 2023-03-07 10:30:34.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-03-07 10:30:34.000000 napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2023-02-02 19:27:24.000000 napari-skimage-regionprops-0.8.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-07 10:30:35.480942 napari-skimage-regionprops-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     2135 2023-03-07 10:26:42.000000 napari-skimage-regionprops-0.8.2/setup.py
--rw-rw-rw-   0        0        0      877 2023-01-15 16:56:44.000000 napari-skimage-regionprops-0.8.2/tox.ini
+drwxrwxrwx   0        0        0        0 2023-03-11 08:15:36.245859 napari-skimage-regionprops-0.9.0/
+drwxrwxrwx   0        0        0        0 2023-03-11 08:15:36.125553 napari-skimage-regionprops-0.9.0/.github/
+drwxrwxrwx   0        0        0        0 2023-03-11 08:15:36.153883 napari-skimage-regionprops-0.9.0/.github/workflows/
+-rw-rw-rw-   0        0        0      603 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/.github/workflows/plugin_preview.yml
+-rw-rw-rw-   0        0        0     2661 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1053 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/.gitignore
+drwxrwxrwx   0        0        0        0 2023-03-11 08:15:36.158936 napari-skimage-regionprops-0.9.0/.napari/
+-rw-rw-rw-   0        0        0      303 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/.napari/config.yml
+-rw-rw-rw-   0        0        0     1554 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      181 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10051 2023-03-11 08:15:36.244862 napari-skimage-regionprops-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8884 2023-03-11 08:11:15.000000 napari-skimage-regionprops-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-03-11 08:15:36.190283 napari-skimage-regionprops-0.9.0/data/
+-rw-rw-rw-   0        0        0      435 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.9.0/data/BBBC007_reference.txt
+-rw-rw-rw-   0        0        0    53130 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.9.0/data/actin.tif
+-rw-rw-rw-   0        0        0   105872 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.9.0/data/cell_labels.tif
+-rw-rw-rw-   0        0        0    53130 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.9.0/data/dna.tif
+-rw-rw-rw-   0        0        0   105872 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.9.0/data/dna_labels.tif
+-rwxrwxrwx   0        0        0      201 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/deploy.bat
+-rw-rw-rw-   0        0        0   199095 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/measure_point_coordinate.png
+-rw-rw-rw-   0        0        0   192170 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/measure_point_intensity.png
+drwxrwxrwx   0        0        0        0 2023-03-11 08:15:36.220579 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/
+-rw-rw-rw-   0        0        0      987 2023-03-11 07:45:02.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/__init__.py
+-rw-rw-rw-   0        0        0     5425 2023-02-02 19:27:24.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_all_frames.py
+-rw-rw-rw-   0        0        0     1281 2023-03-11 08:11:19.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_load_csv.py
+-rw-rw-rw-   0        0        0     2058 2023-01-15 16:56:44.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_measure_points.py
+-rw-rw-rw-   0        0        0    37787 2023-03-07 10:23:38.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_multichannel.py
+-rw-rw-rw-   0        0        0     7384 2023-03-11 08:11:15.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_parametric_images.py
+-rw-rw-rw-   0        0        0    10055 2023-03-04 19:23:18.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_process_tables.py
+-rw-rw-rw-   0        0        0    10703 2023-02-23 17:02:30.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_regionprops.py
+-rw-rw-rw-   0        0        0    12789 2023-03-11 07:05:06.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_table.py
+drwxrwxrwx   0        0        0        0 2023-03-11 08:15:36.243824 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_tests/
+-rw-rw-rw-   0        0        0        2 2022-12-08 11:00:14.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_tests/__init__.py
+-rw-rw-rw-   0        0        0    18484 2023-03-11 08:11:15.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_tests/test_function.py
+-rw-rw-rw-   0        0        0     7558 2023-03-07 10:23:26.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_tests/test_things_inside_things.py
+-rw-rw-rw-   0        0        0     3372 2023-03-11 07:05:06.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_tests/test_timelapse.py
+-rw-rw-rw-   0        0        0     1481 2023-02-02 19:27:24.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-03-11 08:15:36.239818 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/
+-rw-rw-rw-   0        0        0    10051 2023-03-11 08:15:35.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1273 2023-03-11 08:15:36.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-11 08:15:35.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-03-11 08:15:35.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      120 2023-03-11 08:15:35.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-03-11 08:15:35.000000 napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      128 2023-02-02 19:27:24.000000 napari-skimage-regionprops-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-03-11 08:15:36.245859 napari-skimage-regionprops-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2135 2023-03-11 07:45:02.000000 napari-skimage-regionprops-0.9.0/setup.py
+-rw-rw-rw-   0        0        0      893 2023-03-11 07:05:06.000000 napari-skimage-regionprops-0.9.0/tox.ini
```

### Comparing `napari-skimage-regionprops-0.8.2/.github/workflows/plugin_preview.yml` & `napari-skimage-regionprops-0.9.0/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/.github/workflows/test_and_deploy.yml` & `napari-skimage-regionprops-0.9.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/.gitignore` & `napari-skimage-regionprops-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/LICENSE` & `napari-skimage-regionprops-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/PKG-INFO` & `napari-skimage-regionprops-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-skimage-regionprops
-Version: 0.8.2
+Version: 0.9.0
 Summary: A regionprops table widget plugin for napari
 Home-page: https://github.com/haesleinhuepf/napari-skimage-regionprops
 Author: Marcelo Zoccoler, Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -90,15 +90,15 @@
  
  ![](https://github.com/haesleinhuepf/napari-skimage-regionprops/raw/master/images/things_inside_things_demo.gif)
 
 ## Usage, programmatically
 
 You can also control the tables programmatically. See this 
 [example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/tables.ipynb) for details on regionprops and
-[this example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/measure_points.ipynb) for details on measuring intensity at point coordinates.
+[this example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/measure_points.ipynb) for details on measuring intensity at point coordinates. For creating parametric map images, see [this notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/map_measurements.ipynb).
 
 
 ## Features
 The user can select categories of features for feature extraction in the user interface. These categories contain measurements from the scikit-image [regionprops list of measurements](https://scikit-image.org/docs/dev/api/skimage.measure.html#skimage.measure.regionprops) library:
 * size:
   * area
   * bbox_area
```

### Comparing `napari-skimage-regionprops-0.8.2/README.md` & `napari-skimage-regionprops-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
  
  ![](https://github.com/haesleinhuepf/napari-skimage-regionprops/raw/master/images/things_inside_things_demo.gif)
 
 ## Usage, programmatically
 
 You can also control the tables programmatically. See this 
 [example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/tables.ipynb) for details on regionprops and
-[this example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/measure_points.ipynb) for details on measuring intensity at point coordinates.
+[this example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/measure_points.ipynb) for details on measuring intensity at point coordinates. For creating parametric map images, see [this notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/map_measurements.ipynb).
 
 
 ## Features
 The user can select categories of features for feature extraction in the user interface. These categories contain measurements from the scikit-image [regionprops list of measurements](https://scikit-image.org/docs/dev/api/skimage.measure.html#skimage.measure.regionprops) library:
 * size:
   * area
   * bbox_area
```

### Comparing `napari-skimage-regionprops-0.8.2/data/actin.tif` & `napari-skimage-regionprops-0.9.0/data/actin.tif`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/data/cell_labels.tif` & `napari-skimage-regionprops-0.9.0/data/cell_labels.tif`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/data/dna.tif` & `napari-skimage-regionprops-0.9.0/data/dna.tif`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/data/dna_labels.tif` & `napari-skimage-regionprops-0.9.0/data/dna_labels.tif`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/measure_point_coordinate.png` & `napari-skimage-regionprops-0.9.0/measure_point_coordinate.png`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/measure_point_intensity.png` & `napari-skimage-regionprops-0.9.0/measure_point_intensity.png`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/__init__.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from ._table import add_table, get_table, TableWidget
 from ._regionprops import regionprops, regionprops_table, regionprops_table_all_frames
 from ._multichannel import link_two_label_images, measure_labels, measure_labels_with_intensity
 from ._multichannel import measure_labels_in_labels_with_intensity, measure_labels_in_labels
 from ._multichannel import regionprops_measure_things_inside_things
 from ._process_tables import merge_measurements_to_reference, make_summary_table
-from ._parametric_images import visualize_measurement_on_labels, relabel
+from ._parametric_images import visualize_measurement_on_labels, relabel, map_measurements_on_labels
 from ._measure_points import measure_points
 from napari_plugin_engine import napari_hook_implementation
 from ._load_csv import load_csv
 
 try:
     from ._version import version as __version__
 except ImportError:
-    __version__ = "0.8.2"
+    __version__ = "0.9.0"
 
 
 @napari_hook_implementation
 def napari_experimental_provide_function():
     return [regionprops_table, visualize_measurement_on_labels, load_csv]
```

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_all_frames.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_all_frames.py`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_load_csv.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_load_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     import napari
 except Exception as e:
     import warnings
     warnings.warn(str(e))
 
 
 @register_function(menu="Measurement > Load from CSV (nsr)")
-def load_csv(csv_filename:"magicgui.types.PathLike", labels_layer: "napari.layers.Labels", viewer: "napari.Viewer" = None):
+def load_csv(csv_filename:"magicgui.types.PathLike", labels_layer: "napari.layers.Labels", show_table: bool = True, viewer: "napari.Viewer" = None):
     """Save contents of a CSV file into a given layer's properties"""
     import pandas as pd
     # load region properties from csv file
     reg_props = pd.read_csv(csv_filename)
     try:
         edited_reg_props = reg_props.drop(["Unnamed: 0"], axis=1)
     except KeyError:
@@ -26,10 +26,10 @@
         edited_reg_props = pd.concat([label_column, edited_reg_props], axis=1)
 
     if hasattr(labels_layer, "properties"):
         labels_layer.properties = edited_reg_props
     if hasattr(labels_layer, "features"):
         labels_layer.features = edited_reg_props
 
-    if viewer is not None:
+    if viewer is not None and show_table:
         from ._table import add_table
         add_table(labels_layer, viewer)
```

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_measure_points.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_measure_points.py`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_multichannel.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_multichannel.py`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_process_tables.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_process_tables.py`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_regionprops.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_regionprops.py`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_table.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
 
     def _double_clicked_table(self):
         if "label" in self._table.keys():
             selected_column = list(self._table.keys())[self._view.currentColumn()]
             print("Selected column", selected_column)
             if selected_column is not None:
                 if isinstance(self._layer, napari.layers.Labels):
-                    from ._parametric_images import visualize_measurement_on_labels
-                    new_layer = self._viewer.add_image( visualize_measurement_on_labels(self._layer, selected_column, self._viewer) ,
+                    from ._parametric_images import visualize_measurement_on_labels, map_measurements_on_labels
+                    new_layer = self._viewer.add_image( map_measurements_on_labels(self._layer, selected_column, self._viewer) ,
                                                         name=selected_column + " in " + self._layer.name ,
                                                         affine=self._layer.affine ,
                                                         scale=self._layer.scale,
                                                         rotate=self._layer.rotate
                                                         )
                     new_layer.contrast_limits = [np.min(self._table[selected_column]), np.max(self._table[selected_column])]
                     new_layer.colormap = "jet"
```

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_tests/test_function.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_tests/test_function.py`

 * *Files 23% similar despite different names*

```diff
@@ -50,17 +50,19 @@
 
     # check table results
     area_measurements = table_widget.get_content()['area']
     print(area_measurements)
     assert np.array_equal([9, 6, 6, 1], area_measurements)
 
     # generate a parametric image
-    from napari_skimage_regionprops import visualize_measurement_on_labels
+    from napari_skimage_regionprops import visualize_measurement_on_labels, map_measurements_on_labels
     result = visualize_measurement_on_labels(labels_layer, "area", viewer)
     assert result is not None
+    result = map_measurements_on_labels(labels_layer, "area", viewer)
+    assert result is not None
 
     reference = np.asarray([
         [0, 0, 0, 0, 0, 0, 0],
         [9, 9, 9, 0, 0, 6, 6],
         [9, 9, 9, 0, 0, 6, 6],
         [9, 9, 9, 0, 0, 6, 6],
         [0, 0, 0, 0, 0, 0, 0],
@@ -411,7 +413,177 @@
     # check one measurement
     assert np.array_equal(table['area'], [27, 9])
 
     # check that measurements that depend on convex_area are absent in this case
     assert "convex_area" not in table.keys()
     assert "feret_max_diameter" not in table.keys()
     assert "solidity" not in table.keys()
+
+def test_map_measurements_WITHOUT_BG_on_sequential_labels_WITHOUT_BG(make_napari_viewer):
+    import numpy as np
+    from pandas import DataFrame
+    from napari_skimage_regionprops._parametric_images import map_measurements_on_labels
+    
+    measurements = [6, 9, 12, 15]
+    labels = np.array(
+        [[1, 2],
+         [3, 4]]
+         )
+    output = np.array(
+        [[6, 9],
+         [12, 15]]
+    )
+
+    table = DataFrame({
+        'label': np.unique(labels[labels != 0]),
+        'measurements': measurements})
+
+    viewer = make_napari_viewer()
+    labels_layer = viewer.add_labels(labels, features=table)
+    result = map_measurements_on_labels(labels_layer, column='measurements')
+    assert np.array_equal(output, result)
+
+def test_map_measurements_WITHOUT_BG_on_NON_sequential_labels_WITHOUT_BG(make_napari_viewer):
+    import numpy as np
+    from pandas import DataFrame
+    from napari_skimage_regionprops._parametric_images import map_measurements_on_labels
+    
+    measurements = [6, 9, 12, 15]
+    labels = np.array(
+        [[2, 4],
+         [6, 8]]
+         )
+    output = np.array(
+        [[6, 9],
+         [12, 15]]
+    )
+
+    table = DataFrame({
+        'label': np.unique(labels[labels != 0]),
+        'measurements': measurements})
+
+    viewer = make_napari_viewer()
+    labels_layer = viewer.add_labels(labels, features=table)
+    result = map_measurements_on_labels(labels_layer, column='measurements')
+    assert np.array_equal(output, result)
+
+
+def test_map_measurements_WITHOUT_BG_on_NON_sequential_labels_WITHOUT_BG_unsorted(make_napari_viewer):
+    import numpy as np
+    from pandas import DataFrame
+    from napari_skimage_regionprops._parametric_images import map_measurements_on_labels
+
+    measurements = [6, 9, 12, 15]
+    labels = np.array(
+        [[2, 4],
+         [6, 8]]
+    )
+    output = np.array(
+        [[9, 6],
+         [12, 15]]
+    )
+
+    table = DataFrame({
+        'label': [4, 2, 6, 8],
+        'measurements': measurements})
+
+    viewer = make_napari_viewer()
+    labels_layer = viewer.add_labels(labels, features=table)
+    result = map_measurements_on_labels(labels_layer, column='measurements')
+    assert np.array_equal(output, result)
+
+
+def test_map_measurements_WITHOUT_BG_on_sequential_labels_WITH_BG(make_napari_viewer):
+    import numpy as np
+    from pandas import DataFrame
+    from napari_skimage_regionprops._parametric_images import map_measurements_on_labels
+    
+    measurements = [6, 9, 12]
+    labels = np.array(
+        [[0, 1],
+         [2, 3]]
+         )
+    output = np.array(
+        [[0, 6],
+         [9, 12]]
+    )
+
+    table = DataFrame({
+        'label': np.unique(labels[labels != 0]),
+        'measurements': measurements})
+
+    viewer = make_napari_viewer()
+    labels_layer = viewer.add_labels(labels, features=table)
+    result = map_measurements_on_labels(labels_layer, column='measurements')
+    assert np.array_equal(output, result)
+
+def test_map_measurements_WITHOUT_BG_on_NON_sequential_labels_WITH_BG(make_napari_viewer):
+    import numpy as np
+    from pandas import DataFrame
+    from napari_skimage_regionprops._parametric_images import map_measurements_on_labels
+    
+    measurements = [6, 9, 12]
+    labels = np.array(
+        [[0, 2],
+         [4, 6]]
+         )
+    output = np.array(
+        [[0, 6],
+         [9, 12]]
+    )
+
+    table = DataFrame({
+        'label': np.unique(labels[labels != 0]),
+        'measurements': measurements})
+
+    viewer = make_napari_viewer()
+    labels_layer = viewer.add_labels(labels, features=table)
+    result = map_measurements_on_labels(labels_layer, column='measurements')
+    assert np.array_equal(output, result)
+
+def test_map_measurements_WITH_BG_on_sequential_labels_WITH_BG(make_napari_viewer):
+    import numpy as np
+    from pandas import DataFrame
+    from napari_skimage_regionprops._parametric_images import map_measurements_on_labels
+    
+    measurements = [3, 6, 9, 12]
+    labels = np.array(
+        [[0, 1],
+         [2, 3]]
+         )
+    output = np.array(
+        [[3, 6],
+         [9, 12]]
+    )
+
+    table = DataFrame({
+        'label': np.unique(labels),
+        'measurements': measurements})
+
+    viewer = make_napari_viewer()
+    labels_layer = viewer.add_labels(labels, features=table)
+    result = map_measurements_on_labels(labels_layer, column='measurements')
+    assert np.array_equal(output, result)
+
+def test_map_measurements_WITH_BG_on_NON_sequential_labels_WITH_BG(make_napari_viewer):
+    import numpy as np
+    from pandas import DataFrame
+    from napari_skimage_regionprops._parametric_images import map_measurements_on_labels
+    
+    measurements = [3, 6, 9, 12]
+    labels = np.array(
+        [[0, 2],
+         [4, 6]]
+         )
+    output = np.array(
+        [[3, 6],
+         [9, 12]]
+    )
+
+    table = DataFrame({
+        'label': np.unique(labels),
+        'measurements': measurements})
+
+    viewer = make_napari_viewer()
+    labels_layer = viewer.add_labels(labels, features=table)
+    result = map_measurements_on_labels(labels_layer, column='measurements')
+    assert np.array_equal(output, result)
```

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_tests/test_things_inside_things.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_tests/test_things_inside_things.py`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_tests/test_timelapse.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_tests/test_timelapse.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,18 +78,20 @@
 
     regionprops_table_all_frames(image, labels, size=False, napari_viewer=viewer)
 
     df = pd.DataFrame(labels_layer.properties)
 
     assert df.shape[0] == 8
 
-    from napari_skimage_regionprops import visualize_measurement_on_labels
+    from napari_skimage_regionprops import visualize_measurement_on_labels, map_measurements_on_labels
 
     visualize_measurement_on_labels(labels_layer, column="mean_intensity", viewer=viewer)
 
+    map_measurements_on_labels(labels_layer, column="mean_intensity", viewer=viewer)
+
 def test_frame_variable_in_timelapse(make_napari_viewer):
     viewer = make_napari_viewer()
 
     import numpy as np
     import pandas as pd
     from skimage.data import binary_blobs
     from skimage.measure import regionprops_table, label
```

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops/_utilities.py` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops/_utilities.py`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/PKG-INFO` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-skimage-regionprops
-Version: 0.8.2
+Version: 0.9.0
 Summary: A regionprops table widget plugin for napari
 Home-page: https://github.com/haesleinhuepf/napari-skimage-regionprops
 Author: Marcelo Zoccoler, Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -90,15 +90,15 @@
  
  ![](https://github.com/haesleinhuepf/napari-skimage-regionprops/raw/master/images/things_inside_things_demo.gif)
 
 ## Usage, programmatically
 
 You can also control the tables programmatically. See this 
 [example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/tables.ipynb) for details on regionprops and
-[this example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/measure_points.ipynb) for details on measuring intensity at point coordinates.
+[this example notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/measure_points.ipynb) for details on measuring intensity at point coordinates. For creating parametric map images, see [this notebook](https://github.com/haesleinhuepf/napari-skimage-regionprops/blob/master/demo/map_measurements.ipynb).
 
 
 ## Features
 The user can select categories of features for feature extraction in the user interface. These categories contain measurements from the scikit-image [regionprops list of measurements](https://scikit-image.org/docs/dev/api/skimage.measure.html#skimage.measure.regionprops) library:
 * size:
   * area
   * bbox_area
```

### Comparing `napari-skimage-regionprops-0.8.2/napari_skimage_regionprops.egg-info/SOURCES.txt` & `napari-skimage-regionprops-0.9.0/napari_skimage_regionprops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-skimage-regionprops-0.8.2/setup.py` & `napari-skimage-regionprops-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     url='https://github.com/haesleinhuepf/napari-skimage-regionprops',
     description='A regionprops table widget plugin for napari',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     python_requires='>=3.8',
     install_requires=requirements,
-    version='0.8.2',
+    version='0.9.0',
     #use_scm_version=use_scm,
     setup_requires=['setuptools_scm'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Framework :: napari',
         'Topic :: Scientific/Engineering :: Image Processing',
```

### Comparing `napari-skimage-regionprops-0.8.2/tox.ini` & `napari-skimage-regionprops-0.9.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -30,8 +30,9 @@
     pytest-xvfb ; sys_platform == 'linux'
     # you can remove these if you don't use them
     napari
     magicgui
     pytest-qt
     qtpy
     pyqt5
+    deprecated
 commands = pytest -v --color=yes --cov=napari_skimage_regionprops --cov-report=xml
```

