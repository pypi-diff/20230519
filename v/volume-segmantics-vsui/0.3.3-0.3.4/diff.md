# Comparing `tmp/volume_segmantics_vsui-0.3.3.tar.gz` & `tmp/volume_segmantics_vsui-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volume_segmantics_vsui-0.3.3.tar", max compression
+gzip compressed data, was "volume_segmantics_vsui-0.3.4.tar", max compression
```

## Comparing `volume_segmantics_vsui-0.3.3.tar` & `volume_segmantics_vsui-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-04-11 12:00:14.923609 volume_segmantics_vsui-0.3.3/LICENSE.md
--rw-r--r--   0        0        0     7861 2023-04-13 08:54:44.656609 volume_segmantics_vsui-0.3.3/README.md
--rw-r--r--   0        0        0     1827 2023-04-18 10:52:38.326202 volume_segmantics_vsui-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-11 12:00:20.688662 volume_segmantics_vsui-0.3.3/volume_segmantics/__init__.py
--rw-r--r--   0        0        0      184 2023-04-11 12:00:20.691680 volume_segmantics_vsui-0.3.3/volume_segmantics/data/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-11 12:00:20.693685 volume_segmantics_vsui-0.3.3/volume_segmantics/data/augmentations.py
--rw-r--r--   0        0        0     1611 2023-04-11 12:00:20.696663 volume_segmantics_vsui-0.3.3/volume_segmantics/data/base_data_manager.py
--rw-r--r--   0        0        0     2564 2023-04-11 12:00:20.699676 volume_segmantics_vsui-0.3.3/volume_segmantics/data/dataloaders.py
--rw-r--r--   0        0        0     5532 2023-04-11 12:00:20.702694 volume_segmantics_vsui-0.3.3/volume_segmantics/data/datasets.py
--rw-r--r--   0        0        0    13578 2023-04-11 12:00:20.706691 volume_segmantics_vsui-0.3.3/volume_segmantics/data/pytorch3dunet_losses.py
--rw-r--r--   0        0        0     5315 2023-04-11 12:00:20.709679 volume_segmantics_vsui-0.3.3/volume_segmantics/data/pytorch3dunet_metrics.py
--rw-r--r--   0        0        0      947 2023-04-17 10:14:00.079580 volume_segmantics_vsui-0.3.3/volume_segmantics/data/settings_data.py
--rw-r--r--   0        0        0     5947 2023-04-11 12:00:20.714678 volume_segmantics_vsui-0.3.3/volume_segmantics/data/slicers.py
--rw-r--r--   0        0        0      251 2023-04-11 12:00:20.720659 volume_segmantics_vsui-0.3.3/volume_segmantics/model/__init__.py
--rw-r--r--   0        0        0     2464 2023-04-13 08:54:44.689601 volume_segmantics_vsui-0.3.3/volume_segmantics/model/model_2d.py
--rw-r--r--   0        0        0     6626 2023-04-17 08:56:54.644642 volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_2d_predictor.py
--rw-r--r--   0        0        0    24903 2023-04-17 10:14:20.555320 volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_2d_trainer.py
--rw-r--r--   0        0        0     4128 2023-04-11 12:00:20.731684 volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_prediction_manager.py
--rw-r--r--   0        0        0     2161 2023-04-17 09:38:50.301696 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/predict_2d_model.py
--rw-r--r--   0        0        0     3764 2023-04-13 14:00:02.078267 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/predict_2d_model_oo.py
--rw-r--r--   0        0        0     4364 2023-04-18 10:08:58.833356 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/train_2d_model.py
--rw-r--r--   0        0        0     5737 2023-04-17 10:15:51.296357 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/train_2d_model_oo.py
--rw-r--r--   0        0        0   570399 2023-04-13 08:23:05.091847 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/volume_segmantics
--rw-r--r--   0        0        0      280 2023-04-13 08:23:05.093867 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/__init__.py
--rw-r--r--   0        0        0     5382 2023-04-18 10:07:47.981474 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/arg_parsing.py
--rw-r--r--   0        0        0    11367 2023-04-17 10:15:27.528305 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/base_data_utils.py
--rw-r--r--   0        0        0     1197 2023-04-13 08:23:05.101850 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/cmdline.py
--rw-r--r--   0        0        0     1843 2023-04-13 08:23:05.103851 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/config.py
--rw-r--r--   0        0        0     2537 2023-04-11 12:00:20.774685 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/early_stopping.py
--rw-r--r--   0        0        0     1903 2023-04-11 12:00:20.777682 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/pytorch3dunet_utils.py
--rw-r--r--   0        0        0     9232 1970-01-01 00:00:00.000000 volume_segmantics_vsui-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 12:00:14.923609 volume_segmantics_vsui-0.3.4/LICENSE.md
+-rw-r--r--   0        0        0     7861 2023-04-13 08:54:44.656609 volume_segmantics_vsui-0.3.4/README.md
+-rw-r--r--   0        0        0     1827 2023-05-19 08:37:18.249202 volume_segmantics_vsui-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-11 12:00:20.688662 volume_segmantics_vsui-0.3.4/volume_segmantics/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-11 12:00:20.691680 volume_segmantics_vsui-0.3.4/volume_segmantics/data/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-11 12:00:20.693685 volume_segmantics_vsui-0.3.4/volume_segmantics/data/augmentations.py
+-rw-r--r--   0        0        0     1611 2023-04-11 12:00:20.696663 volume_segmantics_vsui-0.3.4/volume_segmantics/data/base_data_manager.py
+-rw-r--r--   0        0        0     2564 2023-04-11 12:00:20.699676 volume_segmantics_vsui-0.3.4/volume_segmantics/data/dataloaders.py
+-rw-r--r--   0        0        0     5531 2023-05-19 08:28:50.924189 volume_segmantics_vsui-0.3.4/volume_segmantics/data/datasets.py
+-rw-r--r--   0        0        0    13578 2023-04-11 12:00:20.706691 volume_segmantics_vsui-0.3.4/volume_segmantics/data/pytorch3dunet_losses.py
+-rw-r--r--   0        0        0     5315 2023-04-11 12:00:20.709679 volume_segmantics_vsui-0.3.4/volume_segmantics/data/pytorch3dunet_metrics.py
+-rw-r--r--   0        0        0      947 2023-04-17 10:14:00.079580 volume_segmantics_vsui-0.3.4/volume_segmantics/data/settings_data.py
+-rw-r--r--   0        0        0     5947 2023-04-11 12:00:20.714678 volume_segmantics_vsui-0.3.4/volume_segmantics/data/slicers.py
+-rw-r--r--   0        0        0      251 2023-04-11 12:00:20.720659 volume_segmantics_vsui-0.3.4/volume_segmantics/model/__init__.py
+-rw-r--r--   0        0        0     2464 2023-04-13 08:54:44.689601 volume_segmantics_vsui-0.3.4/volume_segmantics/model/model_2d.py
+-rw-r--r--   0        0        0     6626 2023-04-17 08:56:54.644642 volume_segmantics_vsui-0.3.4/volume_segmantics/model/operations/vol_seg_2d_predictor.py
+-rw-r--r--   0        0        0    24903 2023-04-17 10:14:20.555320 volume_segmantics_vsui-0.3.4/volume_segmantics/model/operations/vol_seg_2d_trainer.py
+-rw-r--r--   0        0        0     4128 2023-04-11 12:00:20.731684 volume_segmantics_vsui-0.3.4/volume_segmantics/model/operations/vol_seg_prediction_manager.py
+-rw-r--r--   0        0        0     2484 2023-04-20 09:00:23.582010 volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/predict_2d_model.py
+-rw-r--r--   0        0        0     3764 2023-04-13 14:00:02.078267 volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/predict_2d_model_oo.py
+-rw-r--r--   0        0        0     4412 2023-05-19 08:27:50.233268 volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/train_2d_model.py
+-rw-r--r--   0        0        0     5737 2023-04-17 10:15:51.296357 volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/train_2d_model_oo.py
+-rw-r--r--   0        0        0   570399 2023-04-13 08:23:05.091847 volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/volume_segmantics
+-rw-r--r--   0        0        0      280 2023-04-13 08:23:05.093867 volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/__init__.py
+-rw-r--r--   0        0        0     5842 2023-05-19 08:25:05.965538 volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/arg_parsing.py
+-rw-r--r--   0        0        0    11367 2023-04-17 10:15:27.528305 volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/base_data_utils.py
+-rw-r--r--   0        0        0     1197 2023-04-13 08:23:05.101850 volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/cmdline.py
+-rw-r--r--   0        0        0     1866 2023-05-19 08:24:01.998424 volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/config.py
+-rw-r--r--   0        0        0     2537 2023-04-11 12:00:20.774685 volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/early_stopping.py
+-rw-r--r--   0        0        0     1903 2023-04-11 12:00:20.777682 volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/pytorch3dunet_utils.py
+-rw-r--r--   0        0        0     9232 1970-01-01 00:00:00.000000 volume_segmantics_vsui-0.3.4/PKG-INFO
```

### Comparing `volume_segmantics_vsui-0.3.3/LICENSE.md` & `volume_segmantics_vsui-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/README.md` & `volume_segmantics_vsui-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/pyproject.toml` & `volume_segmantics_vsui-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volume-segmantics-vsui"
-version = "0.3.3"
+version = "0.3.4"
 description = "A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models"
 authors = ["Oliver King <olly.king@diamond.ac.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "volume_segmantics"}]
 repository = "https://github.com/DiamondLightSource/volume-segmantics"
 keywords = ["segmentation", "deep-learning", "volumetric", "3d"]
```

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/data/augmentations.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/data/augmentations.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/data/base_data_manager.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/data/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/data/dataloaders.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/data/datasets.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/data/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         self.masks_fps = sorted(list(masks_dir.glob("*.png")), key=self.natsort)
         self.augmentation = augmentation
         self.preprocessing = preprocessing
         self.imagenet_norm = imagenet_norm
         self.postprocessing = postprocessing
 
     def __getitem__(self, i):
-
         # read data
         image = cv2.imread(str(self.images_fps[i]), cv2.IMREAD_GRAYSCALE)
         mask = cv2.imread(str(self.masks_fps[i]), 0)
 
         # apply pre-processing
         if self.preprocessing:
             sample = self.preprocessing(image=image, mask=mask)
```

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/data/pytorch3dunet_losses.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/data/pytorch3dunet_losses.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/data/pytorch3dunet_metrics.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/data/pytorch3dunet_metrics.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/data/settings_data.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/data/settings_data.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/data/slicers.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/data/slicers.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/model/model_2d.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/model/model_2d.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_2d_predictor.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/model/operations/vol_seg_2d_predictor.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_2d_trainer.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/model/operations/vol_seg_2d_trainer.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_prediction_manager.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/model/operations/vol_seg_prediction_manager.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/predict_2d_model.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/predict_2d_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import logging
 import warnings
 from datetime import date
 from pathlib import Path
+from argparse import ArgumentError
 
 import volume_segmantics.utilities.config as cfg
 from volume_segmantics.data import get_settings_data
 from volume_segmantics.model import VolSeg2DPredictionManager
 from volume_segmantics.utilities import get_2d_prediction_parser
 from vsui_client import vsui_process, init_vsui
 
@@ -23,31 +24,39 @@
     logging.basicConfig(
         level=logging.INFO, format=cfg.LOGGING_FMT, datefmt=cfg.LOGGING_DATE_FMT
     )
     # Parse Args
     parser = get_2d_prediction_parser()
     args = parser.parse_args()
 
+    # Define paths
+    root_path = Path(getattr(args, cfg.DATA_DIR_ARG)).resolve()
+    print(f'rootpath: {root_path}')
+    settings_path = Path(root_path, cfg.SETTINGS_DIR, cfg.PREDICTION_SETTINGS_FN)
+
+    model_file_path = getattr(args, cfg.MODEL_PTH_ARG)
+    data_vol_path = Path(getattr(args, cfg.PREDICT_DATA_ARG))
     vsui_id = getattr(args, cfg.VSUI_PROCESS_ID_ARG)
+    error = getattr(args, 'error', None)
+
+    if error is not None:
+        print("Parsing encountered an error")
+        if vsui_id != "vsui_disabled":
+            VSUI = init_vsui(True, vsui_id, 'Logs')
+            VSUI.connect()
+            raise ArgumentError(None, {'error': error})
+
     if vsui_id != "vsui_disabled":
         VSUI = init_vsui(True, vsui_id, 'Logs')
         VSUI.connect()
         handler = VSUI.get_handler()
         logger.addHandler(handler)
     else:
         VSUI = init_vsui(False)
 
-    # Define paths
-    root_path = Path(getattr(args, cfg.DATA_DIR_ARG)).resolve()
-    print(f'rootpath: {root_path}')
-    settings_path = Path(root_path, cfg.SETTINGS_DIR, cfg.PREDICTION_SETTINGS_FN)
-
-    model_file_path = getattr(args, cfg.MODEL_PTH_ARG)
-    data_vol_path = Path(getattr(args, cfg.PREDICT_DATA_ARG))
-
     if isinstance(model_file_path, str):
         model_file_path = Path(model_file_path)
         
     output_path = create_output_path(root_path, data_vol_path)
     print(f'model_file_path: {model_file_path}')
     print(f'data_vol_path: {data_vol_path}')
     print(f'output_path: {output_path}')
```

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/predict_2d_model_oo.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/predict_2d_model_oo.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/train_2d_model.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/train_2d_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,28 +23,29 @@
     # Parse args and check correct number of volumes given
     parser = get_2d_training_parser()
     args = parser.parse_args()
     data_vols = getattr(args, cfg.TRAIN_DATA_ARG)
     label_vols = getattr(args, cfg.LABEL_DATA_ARG)
     vsui_id = getattr(args, cfg.VSUI_PROCESS_ID_ARG)
     error = getattr(args, 'error', None)
+    port = getattr(args, 'port', None)
     print(f'data_vols: {data_vols}')
     print(f'label_vols: {label_vols}')
     print(f'error: {error}')
 
     if error is not None:
         print("Parsing encountered an error")
         if vsui_id != "vsui_disabled":
             VSUI = init_vsui(True, vsui_id, 'Logs')
             VSUI.connect()
             raise ArgumentError(None, {'error': error})
 
     if vsui_id != "vsui_disabled":
         VSUI = init_vsui(True, vsui_id, 'Logs')
-        VSUI.connect()
+        VSUI.connect(port=port)
         handler = VSUI.get_handler()
         logger.addHandler(handler)
     else:
         VSUI = init_vsui(False)
 
     if isinstance(data_vols, str):
         data_vols = [Path(data_vols)]
```

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/train_2d_model_oo.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/train_2d_model_oo.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/volume_segmantics` & `volume_segmantics_vsui-0.3.4/volume_segmantics/scripts/volume_segmantics`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/arg_parsing.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/arg_parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,22 @@
         "--" + cfg.VSUI_PROCESS_ID_ARG,
         metavar="ID for VSUI (required for VSUI Integration)",
         type=str,
         nargs="?",
         default="vsui_disabled",
         help="unique task id for this process in gui"
     )
+    parser.add_argument(
+        "--" + cfg.VSUI_PORT_ARG,
+        metavar="Port for VSUI (required for VSUI Integration)",
+        type=int,
+        nargs="1",
+        required=True,
+        help="port for the VSUI server"
+    )
     return parser
 
 
 def get_2d_prediction_parser() -> argparse.ArgumentParser:
     """Argument parser for scripts that use a 2d network to predict segmenation for a 3d volume.
 
     Returns:
@@ -139,8 +147,16 @@
         "--" + cfg.VSUI_PROCESS_ID_ARG,
         metavar="ID for VSUI (required for VSUI Integration)",
         type=str,
         nargs="?",
         default="vsui_disabled",
         help="unique task id for this process in gui"
     )
+    parser.add_argument(
+        "--" + cfg.VSUI_PORT_ARG,
+        metavar="Port for VSUI (required for VSUI Integration)",
+        type=int,
+        nargs="1",
+        required=True,
+        help="port for the VSUI server"
+    )
     return parser
```

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/base_data_utils.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/base_data_utils.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/cmdline.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/cmdline.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/config.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Parser strings
 TRAIN_DATA_ARG = "data"
 LABEL_DATA_ARG = "labels"
 MODEL_PTH_ARG = "model"
 PREDICT_DATA_ARG = "data"
 DATA_DIR_ARG = "data_dir"
 VSUI_PROCESS_ID_ARG = "vsui_id"
+VSUI_PORT_ARG = "port"
 
 # File extensions
 TIFF_SUFFIXES = {".tiff", ".tif"}
 HDF5_SUFFIXES = {".h5", ".hdf5", ".nxs"}
 TRAIN_DATA_EXT = {*HDF5_SUFFIXES, *TIFF_SUFFIXES}
 LABEL_DATA_EXT = {*HDF5_SUFFIXES, *TIFF_SUFFIXES}
 MODEL_DATA_EXT = {".pytorch", ".pth"}
```

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/early_stopping.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/early_stopping.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/pytorch3dunet_utils.py` & `volume_segmantics_vsui-0.3.4/volume_segmantics/utilities/pytorch3dunet_utils.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.3/PKG-INFO` & `volume_segmantics_vsui-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volume-segmantics-vsui
-Version: 0.3.3
+Version: 0.3.4
 Summary: A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models
 Home-page: https://github.com/DiamondLightSource/volume-segmantics
 License: Apache-2.0
 Keywords: segmentation,deep-learning,volumetric,3d
 Author: Oliver King
 Author-email: olly.king@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
```

