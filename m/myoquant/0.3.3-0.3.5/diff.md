# Comparing `tmp/myoquant-0.3.3.tar.gz` & `tmp/myoquant-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myoquant-0.3.3.tar", max compression
+gzip compressed data, was "myoquant-0.3.5.tar", max compression
```

## Comparing `myoquant-0.3.3.tar` & `myoquant-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-01-16 19:47:14.112913 myoquant-0.3.3/LICENSE
--rw-r--r--   0        0        0     6253 2023-02-11 20:09:37.818948 myoquant-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-01-16 19:47:14.112913 myoquant-0.3.3/myoquant/__init__.py
--rw-r--r--   0        0        0     1473 2023-05-10 12:40:33.520835 myoquant-0.3.3/myoquant/__main__.py
--rw-r--r--   0        0        0        0 2023-01-16 19:47:14.112913 myoquant-0.3.3/myoquant/commands/__init__.py
--rw-r--r--   0        0        0     3599 2023-01-16 19:47:14.112913 myoquant-0.3.3/myoquant/commands/docs.py
--rw-r--r--   0        0        0    11882 2023-05-10 12:40:33.564835 myoquant-0.3.3/myoquant/commands/run_atp.py
--rw-r--r--   0        0        0    13818 2023-01-16 19:47:14.112913 myoquant-0.3.3/myoquant/commands/run_he.py
--rw-r--r--   0        0        0    11258 2023-02-11 20:09:37.842948 myoquant-0.3.3/myoquant/commands/run_sdh.py
--rw-r--r--   0        0        0     6274 2023-05-10 12:40:33.584834 myoquant-0.3.3/myoquant/src/ATP_analysis.py
--rw-r--r--   0        0        0     8667 2023-02-11 20:09:37.874947 myoquant-0.3.3/myoquant/src/HE_analysis.py
--rw-r--r--   0        0        0     3865 2023-02-11 20:09:37.878947 myoquant-0.3.3/myoquant/src/SDH_analysis.py
--rw-r--r--   0        0        0        0 2023-01-16 19:47:14.116913 myoquant-0.3.3/myoquant/src/__init__.py
--rw-r--r--   0        0        0     6809 2023-05-10 12:40:33.584834 myoquant-0.3.3/myoquant/src/common_func.py
--rw-r--r--   0        0        0     2673 2023-01-16 19:47:14.116913 myoquant-0.3.3/myoquant/src/draw_line.py
--rw-r--r--   0        0        0     3319 2023-01-16 19:47:14.116913 myoquant-0.3.3/myoquant/src/gradcam.py
--rw-r--r--   0        0        0    15363 2023-01-16 19:47:14.116913 myoquant-0.3.3/myoquant/src/random_brightness.py
--rw-r--r--   0        0        0     1123 2023-05-10 12:44:13.334072 myoquant-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     7550 1970-01-01 00:00:00.000000 myoquant-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-01-16 19:47:14.112913 myoquant-0.3.5/LICENSE
+-rw-r--r--   0        0        0     6383 2023-05-19 12:06:20.470890 myoquant-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2023-01-16 19:47:14.112913 myoquant-0.3.5/myoquant/__init__.py
+-rw-r--r--   0        0        0     1473 2023-05-10 12:40:33.520835 myoquant-0.3.5/myoquant/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-16 19:47:14.112913 myoquant-0.3.5/myoquant/commands/__init__.py
+-rw-r--r--   0        0        0     3599 2023-01-16 19:47:14.112913 myoquant-0.3.5/myoquant/commands/docs.py
+-rw-r--r--   0        0        0    11882 2023-05-10 12:40:33.564835 myoquant-0.3.5/myoquant/commands/run_atp.py
+-rw-r--r--   0        0        0    13818 2023-01-16 19:47:14.112913 myoquant-0.3.5/myoquant/commands/run_he.py
+-rw-r--r--   0        0        0    11258 2023-02-11 20:09:37.842948 myoquant-0.3.5/myoquant/commands/run_sdh.py
+-rw-r--r--   0        0        0     6274 2023-05-10 12:40:33.584834 myoquant-0.3.5/myoquant/src/ATP_analysis.py
+-rw-r--r--   0        0        0     8667 2023-02-11 20:09:37.874947 myoquant-0.3.5/myoquant/src/HE_analysis.py
+-rw-r--r--   0        0        0     3865 2023-02-11 20:09:37.878947 myoquant-0.3.5/myoquant/src/SDH_analysis.py
+-rw-r--r--   0        0        0        0 2023-01-16 19:47:14.116913 myoquant-0.3.5/myoquant/src/__init__.py
+-rw-r--r--   0        0        0     6810 2023-05-19 12:06:48.166541 myoquant-0.3.5/myoquant/src/common_func.py
+-rw-r--r--   0        0        0     2673 2023-01-16 19:47:14.116913 myoquant-0.3.5/myoquant/src/draw_line.py
+-rw-r--r--   0        0        0     3319 2023-01-16 19:47:14.116913 myoquant-0.3.5/myoquant/src/gradcam.py
+-rw-r--r--   0        0        0    15363 2023-01-16 19:47:14.116913 myoquant-0.3.5/myoquant/src/random_brightness.py
+-rw-r--r--   0        0        0     1123 2023-05-19 12:09:18.564651 myoquant-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     7680 1970-01-01 00:00:00.000000 myoquant-0.3.5/PKG-INFO
```

### Comparing `myoquant-0.3.3/LICENSE` & `myoquant-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/README.md` & `myoquant-0.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 # MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images
 
 <p align="center">
   <img src="https://i.imgur.com/mzALgZL.png" alt="MyoQuant Banner" style="border-radius: 25px;" />
 </p>
 
+<p align="center">
+  <img src="https://i.imgur.com/FxpFUT3.png" alt="MyoQuant Illustration" style="border-radius: 25px;" />
+</p>
+
 MyoQuant🔬 is a command-line tool to automatically quantify pathological features in muscle fiber histology images.  
 It is built using CellPose, Stardist, custom neural-network models and image analysis techniques to automatically analyze myopathy histology images.  
 Currently MyoQuant is capable of quantifying centralization of nuclei in muscle fiber with HE staining, anomaly in the mitochondria distribution in muscle fibers with SDH staining and the number of type 1 muscle fiber vs type 2 muscle fiber with ATP staining.
 
 An online demo with a web interface is available at [https://lbgi.fr/MyoQuant/](https://lbgi.fr/MyoQuant/). This project is free and open-source under the AGPL license, feel free to fork and contribute to the development.
 
 #### _Warning: This tool is still in early phases and active development._
```

### Comparing `myoquant-0.3.3/myoquant/__main__.py` & `myoquant-0.3.5/myoquant/__main__.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/commands/docs.py` & `myoquant-0.3.5/myoquant/commands/docs.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/commands/run_atp.py` & `myoquant-0.3.5/myoquant/commands/run_atp.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/commands/run_he.py` & `myoquant-0.3.5/myoquant/commands/run_he.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/commands/run_sdh.py` & `myoquant-0.3.5/myoquant/commands/run_sdh.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/src/ATP_analysis.py` & `myoquant-0.3.5/myoquant/src/ATP_analysis.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/src/HE_analysis.py` & `myoquant-0.3.5/myoquant/src/HE_analysis.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/src/SDH_analysis.py` & `myoquant-0.3.5/myoquant/src/SDH_analysis.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/src/common_func.py` & `myoquant-0.3.5/myoquant/src/common_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 """
 import os
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 import sys
 import math
 
-import tensorflow as tf
 import torch
+import tensorflow as tf
+
 from cellpose.models import Cellpose
 from csbdeep.utils import normalize
 from stardist.models import StarDist2D
 from tensorflow import keras
 import numpy as np
 from PIL import Image
 from skimage.measure import regionprops_table
```

### Comparing `myoquant-0.3.3/myoquant/src/draw_line.py` & `myoquant-0.3.5/myoquant/src/draw_line.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/src/gradcam.py` & `myoquant-0.3.5/myoquant/src/gradcam.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/myoquant/src/random_brightness.py` & `myoquant-0.3.5/myoquant/src/random_brightness.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.3/pyproject.toml` & `myoquant-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "myoquant"
-version = "0.3.3"
+version = "0.3.5"
 description = "MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images."
 authors = ["Corentin Meyer <corentin.meyer@etu.unistra.fr>"]
 maintainers = ["Corentin Meyer <corentin.meyer@etu.unistra.fr>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://lbgi.fr/MyoQuant/"
 repository = "https://github.com/lambda-science/MyoQuant"
```

### Comparing `myoquant-0.3.3/PKG-INFO` & `myoquant-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myoquant
-Version: 0.3.3
+Version: 0.3.5
 Summary: MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images.
 Home-page: https://lbgi.fr/MyoQuant/
 License: AGPL-3.0-or-later
 Keywords: histology,quantification,biology,deep-learning
 Author: Corentin Meyer
 Author-email: corentin.meyer@etu.unistra.fr
 Maintainer: Corentin Meyer
@@ -33,14 +33,18 @@
 
 # MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images
 
 <p align="center">
   <img src="https://i.imgur.com/mzALgZL.png" alt="MyoQuant Banner" style="border-radius: 25px;" />
 </p>
 
+<p align="center">
+  <img src="https://i.imgur.com/FxpFUT3.png" alt="MyoQuant Illustration" style="border-radius: 25px;" />
+</p>
+
 MyoQuant🔬 is a command-line tool to automatically quantify pathological features in muscle fiber histology images.  
 It is built using CellPose, Stardist, custom neural-network models and image analysis techniques to automatically analyze myopathy histology images.  
 Currently MyoQuant is capable of quantifying centralization of nuclei in muscle fiber with HE staining, anomaly in the mitochondria distribution in muscle fibers with SDH staining and the number of type 1 muscle fiber vs type 2 muscle fiber with ATP staining.
 
 An online demo with a web interface is available at [https://lbgi.fr/MyoQuant/](https://lbgi.fr/MyoQuant/). This project is free and open-source under the AGPL license, feel free to fork and contribute to the development.
 
 #### _Warning: This tool is still in early phases and active development._
```

