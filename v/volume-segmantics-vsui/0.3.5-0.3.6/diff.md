# Comparing `tmp/volume_segmantics_vsui-0.3.5.tar.gz` & `tmp/volume_segmantics_vsui-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volume_segmantics_vsui-0.3.5.tar", max compression
+gzip compressed data, was "volume_segmantics_vsui-0.3.6.tar", max compression
```

## Comparing `volume_segmantics_vsui-0.3.5.tar` & `volume_segmantics_vsui-0.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-04-11 12:00:14.923609 volume_segmantics_vsui-0.3.5/LICENSE.md
--rw-r--r--   0        0        0     7861 2023-04-13 08:54:44.656609 volume_segmantics_vsui-0.3.5/README.md
--rw-r--r--   0        0        0     1827 2023-05-19 09:30:43.427028 volume_segmantics_vsui-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-11 12:00:20.688662 volume_segmantics_vsui-0.3.5/volume_segmantics/__init__.py
--rw-r--r--   0        0        0      184 2023-04-11 12:00:20.691680 volume_segmantics_vsui-0.3.5/volume_segmantics/data/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-11 12:00:20.693685 volume_segmantics_vsui-0.3.5/volume_segmantics/data/augmentations.py
--rw-r--r--   0        0        0     1611 2023-04-11 12:00:20.696663 volume_segmantics_vsui-0.3.5/volume_segmantics/data/base_data_manager.py
--rw-r--r--   0        0        0     2564 2023-04-11 12:00:20.699676 volume_segmantics_vsui-0.3.5/volume_segmantics/data/dataloaders.py
--rw-r--r--   0        0        0     5531 2023-05-19 08:28:50.924189 volume_segmantics_vsui-0.3.5/volume_segmantics/data/datasets.py
--rw-r--r--   0        0        0    13578 2023-04-11 12:00:20.706691 volume_segmantics_vsui-0.3.5/volume_segmantics/data/pytorch3dunet_losses.py
--rw-r--r--   0        0        0     5315 2023-04-11 12:00:20.709679 volume_segmantics_vsui-0.3.5/volume_segmantics/data/pytorch3dunet_metrics.py
--rw-r--r--   0        0        0      947 2023-04-17 10:14:00.079580 volume_segmantics_vsui-0.3.5/volume_segmantics/data/settings_data.py
--rw-r--r--   0        0        0     5947 2023-04-11 12:00:20.714678 volume_segmantics_vsui-0.3.5/volume_segmantics/data/slicers.py
--rw-r--r--   0        0        0      251 2023-04-11 12:00:20.720659 volume_segmantics_vsui-0.3.5/volume_segmantics/model/__init__.py
--rw-r--r--   0        0        0     2464 2023-04-13 08:54:44.689601 volume_segmantics_vsui-0.3.5/volume_segmantics/model/model_2d.py
--rw-r--r--   0        0        0     6626 2023-04-17 08:56:54.644642 volume_segmantics_vsui-0.3.5/volume_segmantics/model/operations/vol_seg_2d_predictor.py
--rw-r--r--   0        0        0    24903 2023-04-17 10:14:20.555320 volume_segmantics_vsui-0.3.5/volume_segmantics/model/operations/vol_seg_2d_trainer.py
--rw-r--r--   0        0        0     4128 2023-04-11 12:00:20.731684 volume_segmantics_vsui-0.3.5/volume_segmantics/model/operations/vol_seg_prediction_manager.py
--rw-r--r--   0        0        0     2484 2023-04-20 09:00:23.582010 volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/predict_2d_model.py
--rw-r--r--   0        0        0     3764 2023-04-13 14:00:02.078267 volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/predict_2d_model_oo.py
--rw-r--r--   0        0        0     4412 2023-05-19 08:27:50.233268 volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/train_2d_model.py
--rw-r--r--   0        0        0     5737 2023-04-17 10:15:51.296357 volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/train_2d_model_oo.py
--rw-r--r--   0        0        0   570399 2023-04-13 08:23:05.091847 volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/volume_segmantics
--rw-r--r--   0        0        0      280 2023-04-13 08:23:05.093867 volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/__init__.py
--rw-r--r--   0        0        0     5838 2023-05-19 09:26:39.916183 volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/arg_parsing.py
--rw-r--r--   0        0        0    11367 2023-04-17 10:15:27.528305 volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/base_data_utils.py
--rw-r--r--   0        0        0     1197 2023-04-13 08:23:05.101850 volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/cmdline.py
--rw-r--r--   0        0        0     1866 2023-05-19 08:24:01.998424 volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/config.py
--rw-r--r--   0        0        0     2537 2023-04-11 12:00:20.774685 volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/early_stopping.py
--rw-r--r--   0        0        0     1903 2023-04-11 12:00:20.777682 volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/pytorch3dunet_utils.py
--rw-r--r--   0        0        0     9232 1970-01-01 00:00:00.000000 volume_segmantics_vsui-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 12:00:14.923609 volume_segmantics_vsui-0.3.6/LICENSE.md
+-rw-r--r--   0        0        0     7861 2023-04-13 08:54:44.656609 volume_segmantics_vsui-0.3.6/README.md
+-rw-r--r--   0        0        0     1827 2023-05-19 10:30:06.819807 volume_segmantics_vsui-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-11 12:00:20.688662 volume_segmantics_vsui-0.3.6/volume_segmantics/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-11 12:00:20.691680 volume_segmantics_vsui-0.3.6/volume_segmantics/data/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-11 12:00:20.693685 volume_segmantics_vsui-0.3.6/volume_segmantics/data/augmentations.py
+-rw-r--r--   0        0        0     1611 2023-04-11 12:00:20.696663 volume_segmantics_vsui-0.3.6/volume_segmantics/data/base_data_manager.py
+-rw-r--r--   0        0        0     2564 2023-04-11 12:00:20.699676 volume_segmantics_vsui-0.3.6/volume_segmantics/data/dataloaders.py
+-rw-r--r--   0        0        0     5531 2023-05-19 08:28:50.924189 volume_segmantics_vsui-0.3.6/volume_segmantics/data/datasets.py
+-rw-r--r--   0        0        0    13578 2023-04-11 12:00:20.706691 volume_segmantics_vsui-0.3.6/volume_segmantics/data/pytorch3dunet_losses.py
+-rw-r--r--   0        0        0     5315 2023-04-11 12:00:20.709679 volume_segmantics_vsui-0.3.6/volume_segmantics/data/pytorch3dunet_metrics.py
+-rw-r--r--   0        0        0      947 2023-04-17 10:14:00.079580 volume_segmantics_vsui-0.3.6/volume_segmantics/data/settings_data.py
+-rw-r--r--   0        0        0     5947 2023-04-11 12:00:20.714678 volume_segmantics_vsui-0.3.6/volume_segmantics/data/slicers.py
+-rw-r--r--   0        0        0      251 2023-04-11 12:00:20.720659 volume_segmantics_vsui-0.3.6/volume_segmantics/model/__init__.py
+-rw-r--r--   0        0        0     2464 2023-04-13 08:54:44.689601 volume_segmantics_vsui-0.3.6/volume_segmantics/model/model_2d.py
+-rw-r--r--   0        0        0     6626 2023-04-17 08:56:54.644642 volume_segmantics_vsui-0.3.6/volume_segmantics/model/operations/vol_seg_2d_predictor.py
+-rw-r--r--   0        0        0    24903 2023-04-17 10:14:20.555320 volume_segmantics_vsui-0.3.6/volume_segmantics/model/operations/vol_seg_2d_trainer.py
+-rw-r--r--   0        0        0     4128 2023-04-11 12:00:20.731684 volume_segmantics_vsui-0.3.6/volume_segmantics/model/operations/vol_seg_prediction_manager.py
+-rw-r--r--   0        0        0     2544 2023-05-19 10:29:58.855952 volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/predict_2d_model.py
+-rw-r--r--   0        0        0     3764 2023-04-13 14:00:02.078267 volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/predict_2d_model_oo.py
+-rw-r--r--   0        0        0     4450 2023-05-19 10:29:47.156675 volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/train_2d_model.py
+-rw-r--r--   0        0        0     5737 2023-04-17 10:15:51.296357 volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/train_2d_model_oo.py
+-rw-r--r--   0        0        0   570399 2023-04-13 08:23:05.091847 volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/volume_segmantics
+-rw-r--r--   0        0        0      280 2023-04-13 08:23:05.093867 volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/__init__.py
+-rw-r--r--   0        0        0     5838 2023-05-19 09:26:39.916183 volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/arg_parsing.py
+-rw-r--r--   0        0        0    11367 2023-04-17 10:15:27.528305 volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/base_data_utils.py
+-rw-r--r--   0        0        0     1197 2023-04-13 08:23:05.101850 volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/cmdline.py
+-rw-r--r--   0        0        0     1866 2023-05-19 08:24:01.998424 volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/config.py
+-rw-r--r--   0        0        0     2537 2023-04-11 12:00:20.774685 volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/early_stopping.py
+-rw-r--r--   0        0        0     1903 2023-04-11 12:00:20.777682 volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/pytorch3dunet_utils.py
+-rw-r--r--   0        0        0     9232 1970-01-01 00:00:00.000000 volume_segmantics_vsui-0.3.6/PKG-INFO
```

### Comparing `volume_segmantics_vsui-0.3.5/LICENSE.md` & `volume_segmantics_vsui-0.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/README.md` & `volume_segmantics_vsui-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/pyproject.toml` & `volume_segmantics_vsui-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volume-segmantics-vsui"
-version = "0.3.5"
+version = "0.3.6"
 description = "A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models"
 authors = ["Oliver King <olly.king@diamond.ac.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "volume_segmantics"}]
 repository = "https://github.com/DiamondLightSource/volume-segmantics"
 keywords = ["segmentation", "deep-learning", "volumetric", "3d"]
```

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/data/augmentations.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/data/augmentations.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/data/base_data_manager.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/data/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/data/dataloaders.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/data/datasets.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/data/datasets.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/data/pytorch3dunet_losses.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/data/pytorch3dunet_losses.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/data/pytorch3dunet_metrics.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/data/pytorch3dunet_metrics.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/data/settings_data.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/data/settings_data.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/data/slicers.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/data/slicers.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/model/model_2d.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/model/model_2d.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/model/operations/vol_seg_2d_predictor.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/model/operations/vol_seg_2d_predictor.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/model/operations/vol_seg_2d_trainer.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/model/operations/vol_seg_2d_trainer.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/model/operations/vol_seg_prediction_manager.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/model/operations/vol_seg_prediction_manager.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/predict_2d_model.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/predict_2d_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,25 +33,26 @@
     print(f'rootpath: {root_path}')
     settings_path = Path(root_path, cfg.SETTINGS_DIR, cfg.PREDICTION_SETTINGS_FN)
 
     model_file_path = getattr(args, cfg.MODEL_PTH_ARG)
     data_vol_path = Path(getattr(args, cfg.PREDICT_DATA_ARG))
     vsui_id = getattr(args, cfg.VSUI_PROCESS_ID_ARG)
     error = getattr(args, 'error', None)
+    port = getattr(args, 'port', None)[0]
 
     if error is not None:
         print("Parsing encountered an error")
         if vsui_id != "vsui_disabled":
             VSUI = init_vsui(True, vsui_id, 'Logs')
-            VSUI.connect()
+            VSUI.connect(port=port)
             raise ArgumentError(None, {'error': error})
 
     if vsui_id != "vsui_disabled":
         VSUI = init_vsui(True, vsui_id, 'Logs')
-        VSUI.connect()
+        VSUI.connect(port=port)
         handler = VSUI.get_handler()
         logger.addHandler(handler)
     else:
         VSUI = init_vsui(False)
 
     if isinstance(model_file_path, str):
         model_file_path = Path(model_file_path)
```

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/predict_2d_model_oo.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/predict_2d_model_oo.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/train_2d_model.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/train_2d_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,24 +23,25 @@
     # Parse args and check correct number of volumes given
     parser = get_2d_training_parser()
     args = parser.parse_args()
     data_vols = getattr(args, cfg.TRAIN_DATA_ARG)
     label_vols = getattr(args, cfg.LABEL_DATA_ARG)
     vsui_id = getattr(args, cfg.VSUI_PROCESS_ID_ARG)
     error = getattr(args, 'error', None)
-    port = getattr(args, 'port', None)
+    port = getattr(args, 'port', None)[0]
     print(f'data_vols: {data_vols}')
     print(f'label_vols: {label_vols}')
     print(f'error: {error}')
+    print('port: ', port)
 
     if error is not None:
         print("Parsing encountered an error")
         if vsui_id != "vsui_disabled":
             VSUI = init_vsui(True, vsui_id, 'Logs')
-            VSUI.connect()
+            VSUI.connect(port=port)
             raise ArgumentError(None, {'error': error})
 
     if vsui_id != "vsui_disabled":
         VSUI = init_vsui(True, vsui_id, 'Logs')
         VSUI.connect(port=port)
         handler = VSUI.get_handler()
         logger.addHandler(handler)
```

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/train_2d_model_oo.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/train_2d_model_oo.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/scripts/volume_segmantics` & `volume_segmantics_vsui-0.3.6/volume_segmantics/scripts/volume_segmantics`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/arg_parsing.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/arg_parsing.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/base_data_utils.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/base_data_utils.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/cmdline.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/cmdline.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/config.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/config.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/early_stopping.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/early_stopping.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/volume_segmantics/utilities/pytorch3dunet_utils.py` & `volume_segmantics_vsui-0.3.6/volume_segmantics/utilities/pytorch3dunet_utils.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.3.5/PKG-INFO` & `volume_segmantics_vsui-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volume-segmantics-vsui
-Version: 0.3.5
+Version: 0.3.6
 Summary: A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models
 Home-page: https://github.com/DiamondLightSource/volume-segmantics
 License: Apache-2.0
 Keywords: segmentation,deep-learning,volumetric,3d
 Author: Oliver King
 Author-email: olly.king@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
```

