# Comparing `tmp/PyShoreVolume-1.0.0.tar.gz` & `tmp/PyShoreVolume-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyShoreVolume-1.0.0.tar", last modified: Wed May  3 10:24:46 2023, max compression
+gzip compressed data, was "PyShoreVolume-1.0.1.tar", last modified: Fri May 19 18:03:56 2023, max compression
```

## Comparing `PyShoreVolume-1.0.0.tar` & `PyShoreVolume-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-03 10:24:46.945912 PyShoreVolume-1.0.0/
--rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-03 10:24:46.946017 PyShoreVolume-1.0.0/PKG-INFO
--rw-r--r--   0 owenjames   (501) staff       (20)    15186 2023-04-27 16:59:49.000000 PyShoreVolume-1.0.0/README.txt
--rw-r--r--   0 owenjames   (501) staff       (20)      117 2023-05-03 10:24:46.946720 PyShoreVolume-1.0.0/setup.cfg
--rw-r--r--   0 owenjames   (501) staff       (20)     2274 2023-05-03 10:23:39.000000 PyShoreVolume-1.0.0/setup.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-03 10:24:46.937168 PyShoreVolume-1.0.0/src/
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-03 10:24:46.939185 PyShoreVolume-1.0.0/src/PyShoreVolume/
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-03 10:24:46.940709 PyShoreVolume-1.0.0/src/PyShoreVolume/CleanandTransectLocator/
--rw-r--r--   0 owenjames   (501) staff       (20)     6705 2023-04-26 16:01:36.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5970 2023-04-26 14:58:53.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py
--rw-r--r--   0 owenjames   (501) staff       (20)      258 2023-04-26 10:05:08.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/CleanandTransectLocator/__init__.py
--rw-r--r--   0 owenjames   (501) staff       (20)     3355 2023-05-02 13:07:00.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/DOD1.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5508 2023-05-02 13:08:54.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/DataImportandTransectDefinition1.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-03 10:24:46.941550 PyShoreVolume-1.0.0/src/PyShoreVolume/Extra/
--rw-r--r--   0 owenjames   (501) staff       (20)     1322 2023-04-01 11:14:46.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/Extra/File_Organisation_Script.py
--rw-r--r--   0 owenjames   (501) staff       (20)     1739 2023-04-29 15:16:02.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/Extra/QGISMergedShoreline.py
--rw-r--r--   0 owenjames   (501) staff       (20)        0 2023-05-01 13:34:09.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/Extra/__init__.py
--rwxr--r--   0 owenjames   (501) staff       (20)     1806 2023-05-02 13:05:10.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/SCA1.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-03 10:24:46.943103 PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/
--rw-r--r--   0 owenjames   (501) staff       (20)    11033 2023-05-03 09:55:00.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/EPR.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5629 2023-04-26 16:11:01.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/LRR.py
--rw-r--r--   0 owenjames   (501) staff       (20)     7880 2023-05-03 07:49:35.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/NSM.py
--rw-r--r--   0 owenjames   (501) staff       (20)     9638 2023-05-03 10:00:49.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/NSMEandA.py
--rw-r--r--   0 owenjames   (501) staff       (20)     7935 2023-05-03 07:48:32.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/SCE.py
--rw-r--r--   0 owenjames   (501) staff       (20)      181 2023-03-22 20:35:05.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/__init__.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-03 10:24:46.945609 PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/
--rw-r--r--   0 owenjames   (501) staff       (20)    15278 2023-05-03 10:08:13.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/DEMofDifference.py
--rw-r--r--   0 owenjames   (501) staff       (20)     6106 2023-05-03 09:06:39.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/DODSubPlot.py
--rw-r--r--   0 owenjames   (501) staff       (20)     1772 2023-05-03 09:26:29.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/MaskingDEM.py
--rw-r--r--   0 owenjames   (501) staff       (20)     3219 2023-04-28 12:05:59.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py
--rw-r--r--   0 owenjames   (501) staff       (20)    11070 2023-05-03 09:27:46.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py
--rw-r--r--   0 owenjames   (501) staff       (20)    73653 2023-05-03 09:50:15.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py
--rw-r--r--   0 owenjames   (501) staff       (20)      458 2023-04-28 10:20:21.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/__init__.py
--rw-r--r--   0 owenjames   (501) staff       (20)      236 2023-05-02 14:03:43.000000 PyShoreVolume-1.0.0/src/PyShoreVolume/__init__.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-03 10:24:46.940036 PyShoreVolume-1.0.0/src/PyShoreVolume.egg-info/
--rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-03 10:24:46.000000 PyShoreVolume-1.0.0/src/PyShoreVolume.egg-info/PKG-INFO
--rw-r--r--   0 owenjames   (501) staff       (20)     1271 2023-05-03 10:24:46.000000 PyShoreVolume-1.0.0/src/PyShoreVolume.egg-info/SOURCES.txt
--rw-r--r--   0 owenjames   (501) staff       (20)        1 2023-05-03 10:24:46.000000 PyShoreVolume-1.0.0/src/PyShoreVolume.egg-info/dependency_links.txt
--rw-r--r--   0 owenjames   (501) staff       (20)      256 2023-05-03 10:24:46.000000 PyShoreVolume-1.0.0/src/PyShoreVolume.egg-info/requires.txt
--rw-r--r--   0 owenjames   (501) staff       (20)       59 2023-05-03 10:24:46.000000 PyShoreVolume-1.0.0/src/PyShoreVolume.egg-info/top_level.txt
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-19 18:03:56.295336 PyShoreVolume-1.0.1/
+-rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-19 18:03:56.295431 PyShoreVolume-1.0.1/PKG-INFO
+-rw-r--r--   0 owenjames   (501) staff       (20)    15186 2023-04-27 16:59:49.000000 PyShoreVolume-1.0.1/README.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)      117 2023-05-19 18:03:56.295758 PyShoreVolume-1.0.1/setup.cfg
+-rw-r--r--   0 owenjames   (501) staff       (20)     2274 2023-05-17 15:29:53.000000 PyShoreVolume-1.0.1/setup.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-19 18:03:56.287717 PyShoreVolume-1.0.1/src/
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-19 18:03:56.289448 PyShoreVolume-1.0.1/src/PyShoreVolume/
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-19 18:03:56.290870 PyShoreVolume-1.0.1/src/PyShoreVolume/CleanandTransectLocator/
+-rw-r--r--   0 owenjames   (501) staff       (20)     6705 2023-04-26 16:01:36.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5970 2023-04-26 14:58:53.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      258 2023-04-26 10:05:08.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/CleanandTransectLocator/__init__.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     3355 2023-05-02 13:07:00.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/DOD1.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5508 2023-05-02 13:08:54.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/DataImportandTransectDefinition1.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-19 18:03:56.291787 PyShoreVolume-1.0.1/src/PyShoreVolume/Extra/
+-rw-r--r--   0 owenjames   (501) staff       (20)     1197 2023-05-17 14:53:48.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/Extra/File_Organisation_Script.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     1587 2023-05-17 14:54:14.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/Extra/QGISMergedShoreline.py
+-rw-r--r--   0 owenjames   (501) staff       (20)        0 2023-05-01 13:34:09.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/Extra/__init__.py
+-rwxr--r--   0 owenjames   (501) staff       (20)     1806 2023-05-02 13:05:10.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/SCA1.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-19 18:03:56.293129 PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/
+-rw-r--r--   0 owenjames   (501) staff       (20)    11033 2023-05-03 09:55:00.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/EPR.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5629 2023-04-26 16:11:01.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/LRR.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     7972 2023-05-19 17:58:28.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/NSM.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     9638 2023-05-03 10:00:49.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/NSMEandA.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     7935 2023-05-03 07:48:32.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/SCE.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      181 2023-03-22 20:35:05.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/__init__.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-19 18:03:56.295108 PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/
+-rw-r--r--   0 owenjames   (501) staff       (20)    15278 2023-05-03 10:08:13.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/DEMofDifference.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     6106 2023-05-03 09:06:39.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/DODSubPlot.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     1772 2023-05-03 09:26:29.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/MaskingDEM.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     3219 2023-04-28 12:05:59.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py
+-rw-r--r--   0 owenjames   (501) staff       (20)    11070 2023-05-03 09:27:46.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py
+-rw-r--r--   0 owenjames   (501) staff       (20)    73653 2023-05-03 09:50:15.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      458 2023-04-28 10:20:21.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/__init__.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      236 2023-05-02 14:03:43.000000 PyShoreVolume-1.0.1/src/PyShoreVolume/__init__.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-19 18:03:56.290212 PyShoreVolume-1.0.1/src/PyShoreVolume.egg-info/
+-rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-19 18:03:56.000000 PyShoreVolume-1.0.1/src/PyShoreVolume.egg-info/PKG-INFO
+-rw-r--r--   0 owenjames   (501) staff       (20)     1271 2023-05-19 18:03:56.000000 PyShoreVolume-1.0.1/src/PyShoreVolume.egg-info/SOURCES.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)        1 2023-05-19 18:03:56.000000 PyShoreVolume-1.0.1/src/PyShoreVolume.egg-info/dependency_links.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)      256 2023-05-19 18:03:56.000000 PyShoreVolume-1.0.1/src/PyShoreVolume.egg-info/requires.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)       59 2023-05-19 18:03:56.000000 PyShoreVolume-1.0.1/src/PyShoreVolume.egg-info/top_level.txt
```

### Comparing `PyShoreVolume-1.0.0/PKG-INFO` & `PyShoreVolume-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShoreVolume
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Based Shoreline Change and Beach Volume Analysis Tool
 Home-page: https://github.com/owencaseyjames/PyShoreVolume
 Author: Owen Casey James
 Author-email: owen.james@kcl.ac.uk
 License: MIT
 Keywords: Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyShoreVolume-1.0.0/README.txt` & `PyShoreVolume-1.0.1/README.txt`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/setup.py` & `PyShoreVolume-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='PyShoreVolume',
-      version ='1.0.0',
+      version ='1.0.1',
       description ='Python Based Shoreline Change and Beach Volume Analysis Tool',
       author ='Owen Casey James',
       author_email = 'owen.james@kcl.ac.uk',
       licence ='MIT',
       keywords = 'Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR',
       long_description=long_description,
       long_description_content_type='text/markdown',
```

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/DOD1.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/DOD1.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/DataImportandTransectDefinition1.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/DataImportandTransectDefinition1.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/Extra/File_Organisation_Script.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/Extra/File_Organisation_Script.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 #and containing files according to dates given.
 
 import os 
 import re
 import shutil
 
 #Change directories accordingly
-dir_name = os.chdir('/Users/owenjames/Dropbox/PhD/Shoreline_Data/Porthcurno/data/lidar')
+dir_name = os.chdir('---')
 ##Make sure the below code line has ' / ' at the end to indicate this is where the files are located.
-file_names = os.listdir('/Users/owenjames/Dropbox/PhD/Shoreline_Data/Porthcurno/data/lidar/')
+file_names = os.listdir('---')
 
 #Need to look at the file names to extract the characters to be matched.
 pattern = "[0-9][0-9][0-9][0-9][0-9][0-9]"
 
 #Iterate through file names directory
 for file_name in file_names:
     #Search to match the pattern given between filenames and extract into 'dates'.
```

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/Extra/QGISMergedShoreline.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/Extra/QGISMergedShoreline.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 import processing
 from osgeo import gdal
 from qgis.core import (QgsProject, QgsRasterLayer, 
                     QgsLayerTree, QgsLayerTreeGroup,
                     QgsLayerTreeLayer)
 
 # Data Directory Path
-dir_path = '/Users/owenjames/Dropbox/PhD/Shoreline_Data/cco_data-20220526120221/data/lidar'
+dir_path = '---'
 
 #File type
 filetype = "*.asc"
 
 #Path to data directory where SCA will be perfromed from
-saved = "/Users/owenjames/Dropbox/PhD/Shoreline_Data/cco_data-20220526120221/data/lidar/"
+saved = "---"
 
 #Contour height 
-contourheight = 2.45
+contourheight = ---
 
 #CRS 
 CRSystem = 'EPSG:4326'
 
 ####Merge DEM's in Each Folder. Each folder must contain DEM's from a shared date, with the folder name
 ### the dates of the data collection in the format 'YYYYMMDD'
 for roots, subdirectory, files in os.walk(dir_path):
```

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/SCA1.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/SCA1.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/EPR.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/EPR.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/LRR.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/LRR.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/NSM.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/NSM.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from matplotlib.colors import LinearSegmentedColormap
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.lines import Line2D
+import matplotlib_scalebar
+from matplotlib_scalebar.scalebar import ScaleBar
 
 import contextily as ctx
 
 import pyproj
 
 import time
 
@@ -160,14 +162,15 @@
                     ax.annotate(trid[ins], (coordx[ins], coordy[ins]))  
                     
                divider = make_axes_locatable(ax)
                cax = divider.append_axes("right", size="5%", pad=0.05)           
                cbar = fig.colorbar(cm.ScalarMappable(norm=norm, cmap = cmaps), ax = ax, cax = cax)
                cbar.set_label('Change in Meters', rotation=270,fontsize = 13, labelpad = 12)
                ctx.add_basemap(ax, source=ctx.providers.Esri.WorldImagery, zoom=15)
+              
                ax.set_title('Net Shoreline Change', fontsize=15)
                ax.set_ylabel('Latitude', fontsize = 12)
                ax.set_xlabel('Longitude', fontsize=12)
                plt.show()         
                fig.savefig(save_to_path+'/netshorelinemovement.png',bbox_inches='tight')
```

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/NSMEandA.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/NSMEandA.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/ShorelineChange/SCE.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/ShorelineChange/SCE.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/DEMofDifference.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/DEMofDifference.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/DODSubPlot.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/DODSubPlot.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/MaskingDEM.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/MaskingDEM.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py` & `PyShoreVolume-1.0.1/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume.egg-info/PKG-INFO` & `PyShoreVolume-1.0.1/src/PyShoreVolume.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShoreVolume
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Based Shoreline Change and Beach Volume Analysis Tool
 Home-page: https://github.com/owencaseyjames/PyShoreVolume
 Author: Owen Casey James
 Author-email: owen.james@kcl.ac.uk
 License: MIT
 Keywords: Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyShoreVolume-1.0.0/src/PyShoreVolume.egg-info/SOURCES.txt` & `PyShoreVolume-1.0.1/src/PyShoreVolume.egg-info/SOURCES.txt`

 * *Files identical despite different names*

