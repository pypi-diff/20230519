# Comparing `tmp/gp2-0.5.22.23.tar.gz` & `tmp/gp2-0.5.23.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2-0.5.22.23.tar", last modified: Thu May 18 21:52:59 2023, max compression
+gzip compressed data, was "gp2-0.5.23.23.tar", last modified: Thu May 18 22:07:12 2023, max compression
```

## Comparing `gp2-0.5.22.23.tar` & `gp2-0.5.23.23.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:45:48.000000 gp2-0.5.22.23/
--rw-rw-r--   0  1981811  1981811     1068 2023-05-03 06:05:46.000000 gp2-0.5.22.23/LICENSE
--rw-r--r--   0  1981811  1981811      630 2023-05-18 21:45:48.000000 gp2-0.5.22.23/PKG-INFO
--rw-rw-r--   0  1981811  1981811     3677 2023-05-03 06:16:48.000000 gp2-0.5.22.23/README.md
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:45:29.000000 gp2-0.5.22.23/gp2/
--rw-rw-r--   0  1981811  1981811       91 2023-05-18 21:13:26.000000 gp2-0.5.22.23/gp2/__init__.py
--rw-r--r--   0  1981811  1981811       53 2023-05-18 21:36:06.000000 gp2-0.5.22.23/gp2/__version__.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:45:36.000000 gp2-0.5.22.23/gp2/data/
--rw-rw-r--   0  1981811  1981811       89 2023-05-18 21:21:25.000000 gp2-0.5.22.23/gp2/data/__init__.py
--rw-rw-r--   0  1981811  1981811     2970 2023-05-03 06:40:53.000000 gp2-0.5.22.23/gp2/data/collection.py
--rw-rw-r--   0  1981811  1981811     5051 2023-05-03 06:31:35.000000 gp2-0.5.22.23/gp2/data/manager.py
--rw-rw-r--   0  1981811  1981811      296 2023-05-03 06:25:06.000000 gp2-0.5.22.23/gp2/data/point.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:45:37.000000 gp2-0.5.22.23/gp2/gp2/
--rw-rw-r--   0  1981811  1981811      118 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/__init__.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:45:45.000000 gp2-0.5.22.23/gp2/gp2/classifiers/
--rw-rw-r--   0  1981811  1981811      458 2023-05-18 21:21:50.000000 gp2-0.5.22.23/gp2/gp2/classifiers/__init__.py
--rw-rw-r--   0  1981811  1981811     3918 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py
--rw-rw-r--   0  1981811  1981811      829 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/classifier.py
--rw-rw-r--   0  1981811  1981811     7114 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/k_att_unet2d.py
--rw-rw-r--   0  1981811  1981811     5010 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/k_r2_unet2d.py
--rw-rw-r--   0  1981811  1981811     5786 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/k_res_unet2d.py
--rw-rw-r--   0  1981811  1981811     5564 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/k_unet.py
--rw-rw-r--   0  1981811  1981811     6349 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/k_unet2d.py
--rw-rw-r--   0  1981811  1981811     8242 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/k_unet3_plus2d.py
--rw-rw-r--   0  1981811  1981811     6692 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/k_unet_plus2d.py
--rw-rw-r--   0  1981811  1981811     5124 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/k_vnet2d.py
--rw-rw-r--   0  1981811  1981811    10246 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/unet.py
--rw-rw-r--   0  1981811  1981811     6248 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/classifiers/unet_plus.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:45:48.000000 gp2-0.5.22.23/gp2/gp2/discriminators/
--rw-rw-r--   0  1981811  1981811      206 2023-05-18 21:22:00.000000 gp2-0.5.22.23/gp2/gp2/discriminators/__init__.py
--rw-rw-r--   0  1981811  1981811     4430 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/discriminators/base_cnn_discriminator.py
--rw-rw-r--   0  1981811  1981811     3660 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/discriminators/cnn_discriminator_plus.py
--rw-rw-r--   0  1981811  1981811     5157 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/discriminators/cnndiscriminator.py
--rw-rw-r--   0  1981811  1981811      505 2023-05-03 03:30:40.000000 gp2-0.5.22.23/gp2/gp2/discriminators/discriminator.py
--rw-rw-r--   0  1981811  1981811     8123 2023-05-18 21:23:11.000000 gp2-0.5.22.23/gp2/gp2/util.py
--rw-rw-r--   0  1981811  1981811    29021 2023-05-18 21:21:26.000000 gp2-0.5.22.23/gp2/runner.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:45:32.000000 gp2-0.5.22.23/gp2.egg-info/
--rw-r--r--   0  1981811  1981811      630 2023-05-18 21:45:18.000000 gp2-0.5.22.23/gp2.egg-info/PKG-INFO
--rw-r--r--   0  1981811  1981811     1004 2023-05-18 21:45:21.000000 gp2-0.5.22.23/gp2.egg-info/SOURCES.txt
--rw-r--r--   0  1981811  1981811        1 2023-05-18 21:45:18.000000 gp2-0.5.22.23/gp2.egg-info/dependency_links.txt
--rw-r--r--   0  1981811  1981811       97 2023-05-18 21:45:18.000000 gp2-0.5.22.23/gp2.egg-info/requires.txt
--rw-r--r--   0  1981811  1981811        4 2023-05-18 21:45:19.000000 gp2-0.5.22.23/gp2.egg-info/top_level.txt
--rw-r--r--   0  1981811  1981811       38 2023-05-18 21:45:48.000000 gp2-0.5.22.23/setup.cfg
--rw-r--r--   0  1981811  1981811      993 2023-05-18 21:44:28.000000 gp2-0.5.22.23/setup.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 22:00:01.000000 gp2-0.5.23.23/
+-rw-rw-r--   0  1981811  1981811     1068 2023-05-03 06:05:46.000000 gp2-0.5.23.23/LICENSE
+-rw-r--r--   0  1981811  1981811      630 2023-05-18 22:00:01.000000 gp2-0.5.23.23/PKG-INFO
+-rw-rw-r--   0  1981811  1981811     3677 2023-05-03 06:16:48.000000 gp2-0.5.23.23/README.md
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:46.000000 gp2-0.5.23.23/gp2/
+-rw-rw-r--   0  1981811  1981811       91 2023-05-18 21:13:26.000000 gp2-0.5.23.23/gp2/__init__.py
+-rw-r--r--   0  1981811  1981811       53 2023-05-18 21:58:08.000000 gp2-0.5.23.23/gp2/__version__.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:50.000000 gp2-0.5.23.23/gp2/data/
+-rw-rw-r--   0  1981811  1981811       89 2023-05-18 21:21:25.000000 gp2-0.5.23.23/gp2/data/__init__.py
+-rw-rw-r--   0  1981811  1981811     2970 2023-05-03 06:40:53.000000 gp2-0.5.23.23/gp2/data/collection.py
+-rw-rw-r--   0  1981811  1981811     5051 2023-05-03 06:31:35.000000 gp2-0.5.23.23/gp2/data/manager.py
+-rw-rw-r--   0  1981811  1981811      296 2023-05-03 06:25:06.000000 gp2-0.5.23.23/gp2/data/point.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:52.000000 gp2-0.5.23.23/gp2/gp2/
+-rw-rw-r--   0  1981811  1981811      118 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/__init__.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:58.000000 gp2-0.5.23.23/gp2/gp2/classifiers/
+-rw-rw-r--   0  1981811  1981811      458 2023-05-18 21:21:50.000000 gp2-0.5.23.23/gp2/gp2/classifiers/__init__.py
+-rw-rw-r--   0  1981811  1981811     3918 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py
+-rw-rw-r--   0  1981811  1981811      829 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/classifier.py
+-rw-rw-r--   0  1981811  1981811     7114 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_att_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5010 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_r2_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5786 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_res_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5564 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_unet.py
+-rw-rw-r--   0  1981811  1981811     6349 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_unet2d.py
+-rw-rw-r--   0  1981811  1981811     8242 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_unet3_plus2d.py
+-rw-rw-r--   0  1981811  1981811     6692 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_unet_plus2d.py
+-rw-rw-r--   0  1981811  1981811     5124 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_vnet2d.py
+-rw-rw-r--   0  1981811  1981811    10246 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/unet.py
+-rw-rw-r--   0  1981811  1981811     6248 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/unet_plus.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 22:00:01.000000 gp2-0.5.23.23/gp2/gp2/discriminators/
+-rw-rw-r--   0  1981811  1981811      206 2023-05-18 21:22:00.000000 gp2-0.5.23.23/gp2/gp2/discriminators/__init__.py
+-rw-rw-r--   0  1981811  1981811     4430 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/discriminators/base_cnn_discriminator.py
+-rw-rw-r--   0  1981811  1981811     3660 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/discriminators/cnn_discriminator_plus.py
+-rw-rw-r--   0  1981811  1981811     5157 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/discriminators/cnndiscriminator.py
+-rw-rw-r--   0  1981811  1981811      505 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/discriminators/discriminator.py
+-rw-rw-r--   0  1981811  1981811     8123 2023-05-18 21:23:11.000000 gp2-0.5.23.23/gp2/gp2/util.py
+-rw-rw-r--   0  1981811  1981811    29021 2023-05-18 21:21:26.000000 gp2-0.5.23.23/gp2/runner.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:48.000000 gp2-0.5.23.23/gp2.egg-info/
+-rw-r--r--   0  1981811  1981811      630 2023-05-18 21:59:39.000000 gp2-0.5.23.23/gp2.egg-info/PKG-INFO
+-rw-r--r--   0  1981811  1981811     1019 2023-05-18 21:59:41.000000 gp2-0.5.23.23/gp2.egg-info/SOURCES.txt
+-rw-r--r--   0  1981811  1981811        1 2023-05-18 21:59:39.000000 gp2-0.5.23.23/gp2.egg-info/dependency_links.txt
+-rw-r--r--   0  1981811  1981811       97 2023-05-18 21:59:39.000000 gp2-0.5.23.23/gp2.egg-info/requires.txt
+-rw-r--r--   0  1981811  1981811        4 2023-05-18 21:59:40.000000 gp2-0.5.23.23/gp2.egg-info/top_level.txt
+-rw-r--r--   0  1981811  1981811      141 2023-05-18 21:33:10.000000 gp2-0.5.23.23/pyproject.toml
+-rw-r--r--   0  1981811  1981811       38 2023-05-18 22:00:01.000000 gp2-0.5.23.23/setup.cfg
+-rw-r--r--   0  1981811  1981811      993 2023-05-18 21:44:28.000000 gp2-0.5.23.23/setup.py
```

### Comparing `gp2-0.5.22.23/LICENSE` & `gp2-0.5.23.23/LICENSE`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/PKG-INFO` & `gp2-0.5.23.23/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2
-Version: 0.5.22.23
+Version: 0.5.23.23
 Summary: A framework for tuning segmentation classifiers and discriminators
 Home-page: https://github.com/RyanZurrin/CS410-GP2
 Author: mpsych lab
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gp2-0.5.22.23/README.md` & `gp2-0.5.23.23/README.md`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/data/collection.py` & `gp2-0.5.23.23/gp2/data/collection.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/data/manager.py` & `gp2-0.5.23.23/gp2/data/manager.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/classifier.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/classifier.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/k_att_unet2d.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/k_att_unet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/k_r2_unet2d.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/k_r2_unet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/k_res_unet2d.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/k_res_unet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/k_unet.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/k_unet.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/k_unet2d.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/k_unet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/k_unet3_plus2d.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/k_unet3_plus2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/k_unet_plus2d.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/k_unet_plus2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/k_vnet2d.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/k_vnet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/unet.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/unet.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/classifiers/unet_plus.py` & `gp2-0.5.23.23/gp2/gp2/classifiers/unet_plus.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/discriminators/base_cnn_discriminator.py` & `gp2-0.5.23.23/gp2/gp2/discriminators/base_cnn_discriminator.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/discriminators/cnn_discriminator_plus.py` & `gp2-0.5.23.23/gp2/gp2/discriminators/cnn_discriminator_plus.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/discriminators/cnndiscriminator.py` & `gp2-0.5.23.23/gp2/gp2/discriminators/cnndiscriminator.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/gp2/util.py` & `gp2-0.5.23.23/gp2/gp2/util.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2/runner.py` & `gp2-0.5.23.23/gp2/runner.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.22.23/gp2.egg-info/PKG-INFO` & `gp2-0.5.23.23/gp2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2
-Version: 0.5.22.23
+Version: 0.5.23.23
 Summary: A framework for tuning segmentation classifiers and discriminators
 Home-page: https://github.com/RyanZurrin/CS410-GP2
 Author: mpsych lab
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gp2-0.5.22.23/gp2.egg-info/SOURCES.txt` & `gp2-0.5.23.23/gp2.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 gp2/__init__.py
 gp2/__version__.py
 gp2/runner.py
 gp2.egg-info/PKG-INFO
 gp2.egg-info/SOURCES.txt
 gp2.egg-info/dependency_links.txt
```

### Comparing `gp2-0.5.22.23/setup.py` & `gp2-0.5.23.23/setup.py`

 * *Files identical despite different names*

