# Comparing `tmp/EclipsingBinaries-2.8.4a7.tar.gz` & `tmp/EclipsingBinaries-2.8.4a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-2.8.4a7.tar", last modified: Sun May 14 20:54:09 2023, max compression
+gzip compressed data, was "EclipsingBinaries-2.8.4a8.tar", last modified: Fri May 19 16:50:17 2023, max compression
```

## Comparing `EclipsingBinaries-2.8.4a7.tar` & `EclipsingBinaries-2.8.4a8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-14 20:53:49.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 20:54:09.000000 EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:54:09.436148 EclipsingBinaries-2.8.4a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-14 20:53:55.000000 EclipsingBinaries-2.8.4a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/setup.py
```

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/apass.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/apass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 Combines all APASS programs that were originally separate on GitHub for an easy editing and less to load per file.
 
 Author: Kyle Koeller
 Created: 12/26/2022
-Last Updated: 04/05/2023
+Last Updated: 05/19/2023
 """
 
 from astroquery.vizier import Vizier
 import numpy as np
 import pandas as pd
+
 import astropy.units as u
 import astropy.coordinates as coord
 from astropy.wcs import WCS
 from astropy import wcs
 from astropy.io import fits
+from astropy.visualization import ZScaleInterval
+
 from numba import jit
 import matplotlib.pyplot as plt
 import warnings
 from PyAstronomy import pyasl
 
 from .gaia import tess_mag as ga
 # from gaia import tess_mag as ga  # testing
@@ -351,20 +354,26 @@
     # convert the lists to degrees for plotting purposes
     ra_cat_new = (np.array(splitter(ra_catalog)) * 15) * u.deg
     dec_cat_new = np.array(splitter(dec_catalog)) * u.deg
 
     # text for the caption below the graph
     txt = "Number represents index value given in the final output catalog file."
 
+    # Calculate the zscale interval for the image
+    zscale = ZScaleInterval()
+
+    # Calculate vmin and vmax for the image display
+    vmin, vmax = zscale.get_limits(image)
+
     # plot the image and the overlays
     wcs = WCS(header)
     fig = plt.figure(figsize=(12, 8))
     fig.text(.5, 0.02, txt, ha='center')
     ax = plt.subplot(projection=wcs)
-    plt.imshow(image, origin='lower', cmap='cividis', aspect='equal', vmin=300, vmax=1500)
+    plt.imshow(image, origin='lower', cmap='cividis', aspect='equal', vmin=vmin, vmax=vmax)
     plt.xlabel('RA')
     plt.ylabel('Dec')
 
     overlay = ax.get_coords_overlay('icrs')
     overlay.grid(color='white', ls='dotted')
 
     ax.scatter(ra_cat_new, dec_cat_new, transform=ax.get_transform('fk5'), s=200,
```

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/find_min.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/gaia.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/menu.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 """
 Analyze images using aperture photometry within Python and not with Astro ImageJ (AIJ)
 
 Author: Kyle Koeller
 Created: 05/07/2023
-Last Updated: 05/14/2023
+Last Updated: 05/16/2023
 """
 
 # Python imports
 import numpy as np
 import pandas as pd
 from pathlib import Path
 import matplotlib.pyplot as plt
 import time
+import warnings
 
 # Astropy imports
 import ccdproc as ccdp
 from astropy.coordinates import SkyCoord
 from astropy.io import fits
+# from astropy.nddata import CCDData
 # from astropy.stats import sigma_clipped_stats
-from photutils import CircularAperture, CircularAnnulus, aperture_photometry
+from photutils.aperture import CircularAperture, CircularAnnulus, aperture_photometry
 from astropy.wcs import WCS
+import astropy.units as u
+from astropy import wcs
+
+# turn off this warning that just tells the user,
+# "The warning raised when the contents of the FITS header have been modified to be standards compliant."
+warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
 
 
 def main():
     path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the reduced images are or type "
                  "the word 'Close' to leave: ")
 
     if path.lower() == "close":
         exit()
 
     science_imagetyp = 'LIGHT'
     images_path = Path(path)
     files = ccdp.ImageFileCollection(images_path)
-    image_list = files.ccds(imagetyp=science_imagetyp, return_fname=True)
+    image_list = files.files_filtered(imagetyp=science_imagetyp)
+    print(type(image_list))
 
-    multi_aperture_photometry(image_list)
+    multi_aperture_photometry(image_list, images_path)
 
 
-def multi_aperture_photometry(image_list):
+def multi_aperture_photometry(image_list, path):
     """
     Perform aperture photometry on a list of images.
 
     Parameters
     ----------
-    image_list : list
-        List of images to perform aperture photometry on.
+    path : path
+        Path to the folder containing the images.
+    image_list : table
+        Table of images to perform aperture photometry on.
 
     Returns
     -------
     None
     """
 
     # Define the aperture parameters
@@ -56,78 +67,81 @@
     aperture_radius = 25
     annulus_radii = (40, 60)
 
     read_noise = 10.83  # * u.electron  # gathered from fits headers manually
     gain = 1.43  # * u.electron / u.adu  # gathered from fits headers manually
 
     # Magnitudes of the comparison stars (replace with your values)
-    df = pd.read_csv('254037_B.radec', skiprows=1, delim_whitespace=True)
+    df = pd.read_csv('254037_B.radec', skiprows=7, sep=",", header=None)
     magnitudes_comp = df[4]
     ra = df[0]
     dec = df[1]
     ref_star = df[2]
     # centroid = df[3]  # Not used (I don't think at least)
 
-    # Convert RA and DEC to pixel positions
-    sky_coords = SkyCoord(ra, dec, unit='deg', frame='icrs')
-    pixel_coords = WCS.all_world2pix(sky_coords.ra, sky_coords.dec, 1)
-
-    target_position = pixel_coords[0]
-    comparison_positions = pixel_coords[1:]
-
     magnitudes = []
     mag_err = []
     hjd = []
     bjd = []
 
     # Start interactive mode
     plt.ion()
 
     # Create a figure and axis
     fig, ax = plt.subplots()
 
     for _, image_file in enumerate(image_list):
-        image_data, header = fits.getdata(image_file, header=True)
+        image_data, header = fits.getdata(path / image_file, header=True)
+        wcs = WCS(header)
+
+        # ccd = CCDData(image_data, wcs=wcs, unit='adu')
+
+        # Convert RA and DEC to pixel positions
+        sky_coords = SkyCoord(ra, dec, unit=(u.h, u.deg), frame='icrs')
+        pixel_coords = wcs.world_to_pixel(sky_coords)
+
+        target_position = pixel_coords[0]
+        comparison_positions = pixel_coords[1:]
 
-        hjd.append(header['HJD'])
-        bjd.append(header['BJD'])
+        hjd.append(header['HJD-OBS'])
+        bjd.append(header['BJD-OBS'])
 
         # Create the apertures and annuli
         target_aperture = CircularAperture(target_position, r=aperture_radius)
         comparison_apertures = CircularAperture(comparison_positions, r=aperture_radius)
         target_annulus = CircularAnnulus(target_position, *annulus_radii)
         comparison_annuli = CircularAnnulus(comparison_positions, *annulus_radii)
 
         # Perform aperture photometry
         target_phot_table = aperture_photometry(image_data, target_aperture)
-        comparison_phot_tables = aperture_photometry(image_data, comparison_apertures)
+        comparison_phot_tables = [aperture_photometry(image_data, aperture) for aperture in comparison_apertures]
 
         # Perform annulus photometry to estimate the background
         target_annulus_table = aperture_photometry(image_data, target_annulus)
-        comparison_annuli_tables = aperture_photometry(image_data, comparison_annuli)
+        comparison_annuli_tables = [aperture_photometry(image_data, annulus) for annulus in comparison_annuli]
 
         # Calculate the background mean and standard deviation
-        target_background_mean = target_annulus_table['aperture_sum'][0] / target_annulus.area()
+        target_background_mean = target_annulus_table['aperture_sum'][0] / target_annulus.area
         target_background_stddev = np.sqrt(target_background_mean)
 
-        comparison_background_means = [table['aperture_sum'][0] / annulus.area()
+        comparison_background_means = [table['aperture_sum'][0] / annulus.area
                                        for table, annulus in zip(comparison_annuli_tables, comparison_annuli)]
         comparison_background_stddevs = [np.sqrt(mean) for mean in comparison_background_means]
 
         # Subtract the background: Calculate net integrated counts
-        target_sum = target_phot_table['aperture_sum'][0] - target_aperture.area() * target_background_mean
-        comparison_sums = [table['aperture_sum'][0] - aperture.area() * mean
+        target_sum = target_phot_table['aperture_sum'][0] - target_aperture.area * target_background_mean
+        comparison_sums = [table['aperture_sum'][0] - aperture.area * mean
                            for table, aperture, mean in
                            zip(comparison_phot_tables, comparison_apertures, comparison_background_means)]
 
         # Calculate the errors
         target_error = np.sqrt(
-            target_sum / gain + target_aperture.area() * target_background_stddev ** 2 + target_aperture.area() ** 2 * read_noise ** 2)
+            target_sum / gain + target_aperture.area * target_background_stddev ** 2 + target_aperture.area ** 2 * read_noise ** 2)
         comparison_errors = [
-            np.sqrt(comp_sums / gain + aperture.area() * stddev ** 2 + aperture.area() ** 2 * read_noise ** 2)
+            np.sqrt(comp_sums / gain + aperture.area * stddev ** 2 + aperture.area ** 2 * read_noise ** 2)
             for comp_sums, aperture, stddev in zip(comparison_sums, comparison_apertures, comparison_background_stddevs)]
 
         # Calculate the magnitude and error of the target star
         target_magnitude = -2.5 * np.log10(target_sum / np.mean(comparison_sums))
 
         # Calculate the error in the magnitude
         target_magnitude_error = (2.5 / np.log(10)) * np.sqrt((target_error / target_sum) ** 2 + np.mean(
```

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a7
+Version: 2.8.4a8
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 [![Python 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml)
+[![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # Binary Star Research Package
```

### Comparing `EclipsingBinaries-2.8.4a7/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/LICENSE` & `EclipsingBinaries-2.8.4a8/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a7/PKG-INFO` & `EclipsingBinaries-2.8.4a8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a7
+Version: 2.8.4a8
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 [![Python 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml)
+[![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # Binary Star Research Package
```

### Comparing `EclipsingBinaries-2.8.4a7/README.md` & `EclipsingBinaries-2.8.4a8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [![Python 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml)
+[![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
 # Binary Star Research Package
```

### Comparing `EclipsingBinaries-2.8.4a7/setup.py` & `EclipsingBinaries-2.8.4a8/setup.py`

 * *Files identical despite different names*

