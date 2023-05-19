# Comparing `tmp/gp2-0.5.23.23.tar.gz` & `tmp/gp2-0.5.24.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2-0.5.23.23.tar", last modified: Thu May 18 22:07:12 2023, max compression
+gzip compressed data, was "gp2-0.5.24.23.tar", last modified: Fri May 19 01:40:22 2023, max compression
```

## Comparing `gp2-0.5.23.23.tar` & `gp2-0.5.24.23.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 22:00:01.000000 gp2-0.5.23.23/
--rw-rw-r--   0  1981811  1981811     1068 2023-05-03 06:05:46.000000 gp2-0.5.23.23/LICENSE
--rw-r--r--   0  1981811  1981811      630 2023-05-18 22:00:01.000000 gp2-0.5.23.23/PKG-INFO
--rw-rw-r--   0  1981811  1981811     3677 2023-05-03 06:16:48.000000 gp2-0.5.23.23/README.md
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:46.000000 gp2-0.5.23.23/gp2/
--rw-rw-r--   0  1981811  1981811       91 2023-05-18 21:13:26.000000 gp2-0.5.23.23/gp2/__init__.py
--rw-r--r--   0  1981811  1981811       53 2023-05-18 21:58:08.000000 gp2-0.5.23.23/gp2/__version__.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:50.000000 gp2-0.5.23.23/gp2/data/
--rw-rw-r--   0  1981811  1981811       89 2023-05-18 21:21:25.000000 gp2-0.5.23.23/gp2/data/__init__.py
--rw-rw-r--   0  1981811  1981811     2970 2023-05-03 06:40:53.000000 gp2-0.5.23.23/gp2/data/collection.py
--rw-rw-r--   0  1981811  1981811     5051 2023-05-03 06:31:35.000000 gp2-0.5.23.23/gp2/data/manager.py
--rw-rw-r--   0  1981811  1981811      296 2023-05-03 06:25:06.000000 gp2-0.5.23.23/gp2/data/point.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:52.000000 gp2-0.5.23.23/gp2/gp2/
--rw-rw-r--   0  1981811  1981811      118 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/__init__.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:58.000000 gp2-0.5.23.23/gp2/gp2/classifiers/
--rw-rw-r--   0  1981811  1981811      458 2023-05-18 21:21:50.000000 gp2-0.5.23.23/gp2/gp2/classifiers/__init__.py
--rw-rw-r--   0  1981811  1981811     3918 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py
--rw-rw-r--   0  1981811  1981811      829 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/classifier.py
--rw-rw-r--   0  1981811  1981811     7114 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_att_unet2d.py
--rw-rw-r--   0  1981811  1981811     5010 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_r2_unet2d.py
--rw-rw-r--   0  1981811  1981811     5786 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_res_unet2d.py
--rw-rw-r--   0  1981811  1981811     5564 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_unet.py
--rw-rw-r--   0  1981811  1981811     6349 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_unet2d.py
--rw-rw-r--   0  1981811  1981811     8242 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_unet3_plus2d.py
--rw-rw-r--   0  1981811  1981811     6692 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_unet_plus2d.py
--rw-rw-r--   0  1981811  1981811     5124 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/k_vnet2d.py
--rw-rw-r--   0  1981811  1981811    10246 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/unet.py
--rw-rw-r--   0  1981811  1981811     6248 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/classifiers/unet_plus.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 22:00:01.000000 gp2-0.5.23.23/gp2/gp2/discriminators/
--rw-rw-r--   0  1981811  1981811      206 2023-05-18 21:22:00.000000 gp2-0.5.23.23/gp2/gp2/discriminators/__init__.py
--rw-rw-r--   0  1981811  1981811     4430 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/discriminators/base_cnn_discriminator.py
--rw-rw-r--   0  1981811  1981811     3660 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/discriminators/cnn_discriminator_plus.py
--rw-rw-r--   0  1981811  1981811     5157 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/discriminators/cnndiscriminator.py
--rw-rw-r--   0  1981811  1981811      505 2023-05-03 03:30:40.000000 gp2-0.5.23.23/gp2/gp2/discriminators/discriminator.py
--rw-rw-r--   0  1981811  1981811     8123 2023-05-18 21:23:11.000000 gp2-0.5.23.23/gp2/gp2/util.py
--rw-rw-r--   0  1981811  1981811    29021 2023-05-18 21:21:26.000000 gp2-0.5.23.23/gp2/runner.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 21:59:48.000000 gp2-0.5.23.23/gp2.egg-info/
--rw-r--r--   0  1981811  1981811      630 2023-05-18 21:59:39.000000 gp2-0.5.23.23/gp2.egg-info/PKG-INFO
--rw-r--r--   0  1981811  1981811     1019 2023-05-18 21:59:41.000000 gp2-0.5.23.23/gp2.egg-info/SOURCES.txt
--rw-r--r--   0  1981811  1981811        1 2023-05-18 21:59:39.000000 gp2-0.5.23.23/gp2.egg-info/dependency_links.txt
--rw-r--r--   0  1981811  1981811       97 2023-05-18 21:59:39.000000 gp2-0.5.23.23/gp2.egg-info/requires.txt
--rw-r--r--   0  1981811  1981811        4 2023-05-18 21:59:40.000000 gp2-0.5.23.23/gp2.egg-info/top_level.txt
--rw-r--r--   0  1981811  1981811      141 2023-05-18 21:33:10.000000 gp2-0.5.23.23/pyproject.toml
--rw-r--r--   0  1981811  1981811       38 2023-05-18 22:00:01.000000 gp2-0.5.23.23/setup.cfg
--rw-r--r--   0  1981811  1981811      993 2023-05-18 21:44:28.000000 gp2-0.5.23.23/setup.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-19 01:33:11.000000 gp2-0.5.24.23/
+-rw-rw-r--   0  1981811  1981811     1068 2023-05-03 06:05:46.000000 gp2-0.5.24.23/LICENSE
+-rw-r--r--   0  1981811  1981811      630 2023-05-19 01:33:11.000000 gp2-0.5.24.23/PKG-INFO
+-rw-rw-r--   0  1981811  1981811     3677 2023-05-03 06:16:48.000000 gp2-0.5.24.23/README.md
+drwxr-xr-x   0  1981811  1981811        0 2023-05-19 01:32:41.000000 gp2-0.5.24.23/gp2/
+-rw-rw-r--   0  1981811  1981811       91 2023-05-18 21:13:26.000000 gp2-0.5.24.23/gp2/__init__.py
+-rw-r--r--   0  1981811  1981811       53 2023-05-19 01:29:45.000000 gp2-0.5.24.23/gp2/__version__.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-19 01:32:50.000000 gp2-0.5.24.23/gp2/data/
+-rw-rw-r--   0  1981811  1981811       89 2023-05-18 21:21:25.000000 gp2-0.5.24.23/gp2/data/__init__.py
+-rw-rw-r--   0  1981811  1981811     3004 2023-05-19 00:50:31.000000 gp2-0.5.24.23/gp2/data/collection.py
+-rw-rw-r--   0  1981811  1981811     5051 2023-05-03 06:31:35.000000 gp2-0.5.24.23/gp2/data/manager.py
+-rw-rw-r--   0  1981811  1981811      296 2023-05-03 06:25:06.000000 gp2-0.5.24.23/gp2/data/point.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-19 01:32:52.000000 gp2-0.5.24.23/gp2/gp2/
+-rw-rw-r--   0  1981811  1981811      118 2023-05-03 03:30:40.000000 gp2-0.5.24.23/gp2/gp2/__init__.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-19 01:33:05.000000 gp2-0.5.24.23/gp2/gp2/classifiers/
+-rw-rw-r--   0  1981811  1981811      458 2023-05-18 21:21:50.000000 gp2-0.5.24.23/gp2/gp2/classifiers/__init__.py
+-rw-rw-r--   0  1981811  1981811     3954 2023-05-19 01:14:46.000000 gp2-0.5.24.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py
+-rw-rw-r--   0  1981811  1981811      829 2023-05-03 03:30:40.000000 gp2-0.5.24.23/gp2/gp2/classifiers/classifier.py
+-rw-rw-r--   0  1981811  1981811     7140 2023-05-19 00:58:17.000000 gp2-0.5.24.23/gp2/gp2/classifiers/k_att_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5030 2023-05-19 00:58:55.000000 gp2-0.5.24.23/gp2/gp2/classifiers/k_r2_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5808 2023-05-19 00:59:46.000000 gp2-0.5.24.23/gp2/gp2/classifiers/k_res_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5586 2023-05-19 01:04:40.000000 gp2-0.5.24.23/gp2/gp2/classifiers/k_unet.py
+-rw-rw-r--   0  1981811  1981811     6371 2023-05-19 01:05:30.000000 gp2-0.5.24.23/gp2/gp2/classifiers/k_unet2d.py
+-rw-rw-r--   0  1981811  1981811     8266 2023-05-19 01:06:51.000000 gp2-0.5.24.23/gp2/gp2/classifiers/k_unet3_plus2d.py
+-rw-rw-r--   0  1981811  1981811     6710 2023-05-19 01:08:28.000000 gp2-0.5.24.23/gp2/gp2/classifiers/k_unet_plus2d.py
+-rw-rw-r--   0  1981811  1981811     5148 2023-05-19 01:10:48.000000 gp2-0.5.24.23/gp2/gp2/classifiers/k_vnet2d.py
+-rw-rw-r--   0  1981811  1981811    10236 2023-05-19 00:56:09.000000 gp2-0.5.24.23/gp2/gp2/classifiers/unet.py
+-rw-rw-r--   0  1981811  1981811     6248 2023-05-03 03:30:40.000000 gp2-0.5.24.23/gp2/gp2/classifiers/unet_plus.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-19 01:33:10.000000 gp2-0.5.24.23/gp2/gp2/discriminators/
+-rw-rw-r--   0  1981811  1981811      206 2023-05-18 21:22:00.000000 gp2-0.5.24.23/gp2/gp2/discriminators/__init__.py
+-rw-rw-r--   0  1981811  1981811     4430 2023-05-03 03:30:40.000000 gp2-0.5.24.23/gp2/gp2/discriminators/base_cnn_discriminator.py
+-rw-rw-r--   0  1981811  1981811     4787 2023-05-19 01:29:10.000000 gp2-0.5.24.23/gp2/gp2/discriminators/cnn_discriminator_plus.py
+-rw-rw-r--   0  1981811  1981811     6170 2023-05-19 01:24:00.000000 gp2-0.5.24.23/gp2/gp2/discriminators/cnndiscriminator.py
+-rw-rw-r--   0  1981811  1981811      505 2023-05-03 03:30:40.000000 gp2-0.5.24.23/gp2/gp2/discriminators/discriminator.py
+-rw-rw-r--   0  1981811  1981811     8038 2023-05-19 00:52:30.000000 gp2-0.5.24.23/gp2/gp2/util.py
+-rw-rw-r--   0  1981811  1981811    29218 2023-05-19 00:49:41.000000 gp2-0.5.24.23/gp2/runner.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-19 01:32:47.000000 gp2-0.5.24.23/gp2.egg-info/
+-rw-r--r--   0  1981811  1981811      630 2023-05-19 01:32:28.000000 gp2-0.5.24.23/gp2.egg-info/PKG-INFO
+-rw-r--r--   0  1981811  1981811     1019 2023-05-19 01:32:31.000000 gp2-0.5.24.23/gp2.egg-info/SOURCES.txt
+-rw-r--r--   0  1981811  1981811        1 2023-05-19 01:32:29.000000 gp2-0.5.24.23/gp2.egg-info/dependency_links.txt
+-rw-r--r--   0  1981811  1981811       97 2023-05-19 01:32:29.000000 gp2-0.5.24.23/gp2.egg-info/requires.txt
+-rw-r--r--   0  1981811  1981811        4 2023-05-19 01:32:29.000000 gp2-0.5.24.23/gp2.egg-info/top_level.txt
+-rw-r--r--   0  1981811  1981811      141 2023-05-18 21:33:10.000000 gp2-0.5.24.23/pyproject.toml
+-rw-r--r--   0  1981811  1981811       38 2023-05-19 01:33:12.000000 gp2-0.5.24.23/setup.cfg
+-rw-r--r--   0  1981811  1981811      993 2023-05-18 21:44:28.000000 gp2-0.5.24.23/setup.py
```

### Comparing `gp2-0.5.23.23/LICENSE` & `gp2-0.5.24.23/LICENSE`

 * *Files identical despite different names*

### Comparing `gp2-0.5.23.23/PKG-INFO` & `gp2-0.5.24.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2
-Version: 0.5.23.23
+Version: 0.5.24.23
 Summary: A framework for tuning segmentation classifiers and discriminators
 Home-page: https://github.com/RyanZurrin/CS410-GP2
 Author: mpsych lab
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gp2-0.5.23.23/README.md` & `gp2-0.5.24.23/README.md`

 * *Files identical despite different names*

### Comparing `gp2-0.5.23.23/gp2/data/collection.py` & `gp2-0.5.24.23/gp2/data/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from uuid import uuid4
 from .point import Point
 
 
 class Collection:
     """ A collection of DataPoints
     """
@@ -62,27 +61,28 @@
         """
 
         return self.data[_id]
 
     def shuffle(self):
         """ Shuffle the collection
         """
+        import numpy as np
         all_ids = list(self.data.keys())
         np.random.shuffle(all_ids)
 
         shuffled_data = {}
         for k in all_ids:
             shuffled_data[k] = self.data[k]
 
         self.data = shuffled_data
 
     def to_array(self):
         """ Convert the collection to a numpy array
         """
-
+        import numpy as np
         datasize = len(self.data.keys())
         datashape = self.get(0).shape
         datatype = self.get(0).dtype
 
         a = np.zeros(((datasize,) + datashape), dtype=datatype)
         ids = []
```

### Comparing `gp2-0.5.23.23/gp2/data/manager.py` & `gp2-0.5.24.23/gp2/data/manager.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import pickle
-from tensorflow.keras import callbacks
 from .classifier import Classifier
 from gp2.gp2.util import Util
 
 
 class BaseKerasSegmentationClassifier(Classifier):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, verbose, workingdir, **kwargs):
+        super().__init__(verbose, workingdir, **kwargs)
 
     def build(self):
         """ Build the model. """
         self.model.compile(optimizer=self.optimizer,
                            loss=self.loss,
                            metrics=self.metric)
 
@@ -41,14 +40,15 @@
         batch_size : int
             The batch size to use.
         epochs : int
             The number of epochs to train for.
         call_backs : list
             The list of callbacks to use.
         """
+        from tensorflow.keras import callbacks
         super().train(X_train, y_train, X_val, y_val, patience_counter)
         checkpoint_file = os.path.join(self.workingdir, self.name)
         checkpoint_file = Util.create_numbered_file(checkpoint_file,
                                                     f'{self.name}_model')
 
         if call_backs is None:
             call_backs = [callbacks.EarlyStopping(patience=patience_counter,
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/classifier.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/classifier.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/k_att_unet2d.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/k_att_unet2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from keras import losses
-from tensorflow.keras import optimizers
 from gp2.gp2.util import Util
 from .base_keras_segmentation_classifier import \
     BaseKerasSegmentationClassifier
-from keras_unet_collection import models
+
 
 
 class KATTUnet2D(BaseKerasSegmentationClassifier):
     """
     Attention U-net with an optional ImageNet backbone
     """
 
@@ -31,15 +29,15 @@
                  name='attunet',
                  optimizer=None,
                  loss=None,
                  metric=None,
                  verbose=False,
                  workingdir='/tmp',
                  ):
-        '''
+        """
         Attention U-net with an optional ImageNet backbone
 
         att_unet_2d(input_size, filter_num, n_labels, stack_num_down=2, stack_num_up=2, activation='ReLU',
                     atten_activation='ReLU', attention='add', output_activation='Softmax', batch_norm=False, pool=True, unpool=True,
                     backbone=None, weights='imagenet', freeze_backbone=True, freeze_batch_norm=True, name='att-unet')
 
         ----------
@@ -86,15 +84,18 @@
             freeze_backbone: True for a frozen backbone.
             freeze_batch_norm: False for not freezing batch normalization layers.
 
         Output
         ----------
             model: a keras model
 
-        '''
+        """
+        from keras import losses
+        from tensorflow.keras import optimizers
+        from keras_unet_collection import models
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         self.input_size = input_size
         self.filter_num = filter_num or [32, 64, 128, 256, 512, 1024, 2048]
         self.n_labels = n_labels
         self.stack_num_down = stack_num_down
         self.stack_num_up = stack_num_up
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/k_r2_unet2d.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/k_r2_unet2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from keras import losses
-from tensorflow.keras import optimizers
-
 from .base_keras_segmentation_classifier import \
     BaseKerasSegmentationClassifier
-from keras_unet_collection import models
 from gp2.gp2.util import Util
 
 
 class KR2UNet2dD(BaseKerasSegmentationClassifier):
     """
     Keras UNet2D
     """
@@ -67,15 +63,17 @@
             name: prefix of the created keras layers.
 
         Output
         ----------
             model: a keras model.
 
         """
-
+        from keras import losses
+        from tensorflow.keras import optimizers
+        from keras_unet_collection import models
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         self.input_size = input_size
         self.filter_num = filter_num or [64, 128, 256, 512]
         self.stack_num_down = stack_num_down
         self.stack_num_up = stack_num_up
         self.recur_num = recur_num
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/k_res_unet2d.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/k_res_unet2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from keras import losses
-from tensorflow.keras import optimizers
-
 from .base_keras_segmentation_classifier import \
     BaseKerasSegmentationClassifier
-from keras_unet_collection import models
 from gp2.gp2.util import Util
 
 
 class KResUNet2D(BaseKerasSegmentationClassifier):
     """
     KResUNet2D
     """
@@ -73,14 +69,17 @@
             model: a keras model.
 
         * Downsampling is achieved through strided convolutional layers with 1-by-1 kernels in Diakogiannis et al., (2020),
           and is here is achieved either with pooling layers or strided convolutional layers with 2-by-2 kernels.
         * `resunet_a_2d` does not support NoneType input shape.
 
         """
+        from keras import losses
+        from tensorflow.keras import optimizers
+        from keras_unet_collection import models
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         self.input_size = input_size
         self.filter_num = filter_num or [16, 32, 64, 128]
         self.dilation_num = dilation_num or [[1, 3, 15, 31], [1, 3, 15], [1, ],
                                              [1, ]]
         self.n_labels = n_labels
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/k_unet.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/k_unet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-from keras import losses
-from tensorflow.keras import optimizers
-
 from .base_keras_segmentation_classifier import \
     BaseKerasSegmentationClassifier
-
-from keras_unet.models import custom_unet as custom
 from gp2.gp2.util import Util
 
 
 class KUNet(BaseKerasSegmentationClassifier):
     def __init__(self,
                  input_shape=(512, 512, 1),
                  num_classes=1,
@@ -83,14 +78,18 @@
 
         References
         ----------
         [1]: https://arxiv.org/abs/1505.04597
         [2]: https://arxiv.org/pdf/1411.4280.pdf
         [3]: https://arxiv.org/abs/1804.03999
         """
+        from keras import losses
+        from tensorflow.keras import optimizers
+        from keras_unet.models import custom_unet as custom
+
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         self.input_shape = input_shape
         self.num_classes = num_classes
         self.activation = activation
         self.use_batch_norm = use_batch_norm
         self.upsample_mode = upsample_mode
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/k_unet2d.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/k_unet2d.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from keras import losses
-from tensorflow.keras import optimizers
-
 from .base_keras_segmentation_classifier import \
     BaseKerasSegmentationClassifier
-from keras_unet_collection import models
 from gp2.gp2.util import Util
 
 
 class KUNet2D(BaseKerasSegmentationClassifier):
     """
     KU-Net 2D model.
     """
@@ -92,14 +88,17 @@
             False for not freezing batch normalization layers.
 
         Returns
         -------
         model: tensorflow.keras.models.Model
             model containing the U-net with an optional ImageNet-trained backbone.
         """
+        from keras import losses
+        from tensorflow.keras import optimizers
+        from keras_unet_collection import models
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         self.input_size = input_size
         self.filter_num = filter_num or [32, 64, 128, 256, 512, 1024]
         self.n_labels = n_labels
         self.stack_num_down = stack_num_down
         self.stack_num_up = stack_num_up
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/k_unet3_plus2d.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/k_unet3_plus2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from keras import losses
-from tensorflow.keras import optimizers
-
 from .base_keras_segmentation_classifier import \
     BaseKerasSegmentationClassifier
-from keras_unet_collection import models
 from gp2.gp2.util import Util
 
 
 class KUNet3Plus2D(BaseKerasSegmentationClassifier):
     """
     Keras implementation of UNET 3+ with an optional ImageNet-trained backbone.
     """
@@ -97,14 +93,18 @@
         * Upsampling is achieved through bilinear interpolation and can be replaced by transpose convolutional layers here.
 
         Output
         ----------
             model: a keras model.
 
         """
+        from keras import losses
+        from tensorflow.keras import optimizers
+        from keras_unet_collection import models
+
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         print(f'KUNet3Plus2D: {optimizer}, {loss}, {metric}')
 
         self.input_size = input_size
         self.n_labels = n_labels
         self.filter_num_down = filter_num_down or [32, 64, 128, 256]
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/k_unet_plus2d.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/k_unet_plus2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-from keras import losses
-from tensorflow.keras import optimizers
-
 from .base_keras_segmentation_classifier import \
     BaseKerasSegmentationClassifier
-from keras_unet_collection import models
-
 from gp2.gp2.util import Util
 
 
 class KUNetPlus2D(BaseKerasSegmentationClassifier):
     """
     Keras U-net++ 2D model.
     """
@@ -84,16 +79,18 @@
                      or the path to the weights file to be loaded.
             freeze_backbone: True for a frozen backbone.
             freeze_batch_norm: False for not freezing batch normalization layers.
 
         Output
         ----------
             model: a keras model.
-
         """
+        from keras import losses
+        from tensorflow.keras import optimizers
+        from keras_unet_collection import models
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         self.input_size = input_size
         self.filter_num = filter_num or [32, 64, 128, 256, 512, 1024, 2048]
         self.n_labels = n_labels
         self.stack_num_down = stack_num_down
         self.stack_num_up = stack_num_up
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/k_vnet2d.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/k_vnet2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from keras import losses
-from tensorflow.keras import optimizers
-
 from .base_keras_segmentation_classifier import \
     BaseKerasSegmentationClassifier
-from keras_unet_collection import models
+
 from gp2.gp2.util import Util
 
 
 class KVNet2D(BaseKerasSegmentationClassifier):
     """
     KVNet2D for binary segmentation
     """
@@ -72,14 +69,17 @@
             model: a keras model.
 
         * This is a modified version of V-net for 2-d inputw.
         * The original work supports `pool=False` only.
           If pool is True, 'max', or 'ave', an additional conv2d layer will be applied.
         * All the 5-by-5 convolutional kernels are changed (and fixed) to 3-by-3.
         """
+        from keras import losses
+        from tensorflow.keras import optimizers
+        from keras_unet_collection import models
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         self.input_size = input_size
         self.filter_num = filter_num or [32, 64, 128, 256]
         self.n_labels = n_labels
         self.res_num_ini = res_num_ini
         self.res_num_max = res_num_max
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/unet.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/unet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 from .classifier import Classifier
 from gp2.gp2.util import Util
 
 import os
 import pickle
 
-import tensorflow as tf
-from tensorflow.keras.models import Model
-from tensorflow.keras.layers import Input, concatenate, Conv2D, MaxPooling2D, \
-    Activation, UpSampling2D, BatchNormalization
-from tensorflow.keras.optimizers import RMSprop
-from tensorflow.keras import backend as K
-from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint, \
-    ReduceLROnPlateau
-from tensorflow.keras.losses import binary_crossentropy
-
 
 class UNet(Classifier):
 
     def __init__(self, verbose=True, workingdir='/tmp'):
         super().__init__(verbose, workingdir)
 
         print('*** GP2  Unet ***')
         print('Working directory:', self.workingdir)
 
         self.model = self.build()
 
     def build(self, input_shape=(512, 512, 1), num_classes=1):
+        from tensorflow.keras.models import Model
+        from tensorflow.keras.layers import Input, concatenate, Conv2D, \
+            MaxPooling2D,  Activation, UpSampling2D, BatchNormalization
+        from tensorflow.keras.optimizers import RMSprop
         super().build()
 
         inputs = Input(shape=input_shape)
         # 512
 
         encoder1 = Conv2D(16, (3, 3), padding='same', input_shape=input_shape)(
             inputs)
@@ -180,14 +174,16 @@
                       loss=UNet.bce_dice_loss,
                       metrics=[UNet.dice_coeff])
 
         return model
 
     def train(self, X_train, y_train, X_val, y_val,
               patience_counter=2, batch_size=64, epochs=100):
+        from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint, \
+            ReduceLROnPlateau
         super().train(X_train, y_train, X_val, y_val, patience_counter)
 
         checkpoint_file = os.path.join(self.workingdir, 'unet')
         checkpoint_file = Util.create_numbered_file(checkpoint_file, '.model')
 
         callbacks = [EarlyStopping(patience=patience_counter,
                                    monitor='loss',
@@ -225,21 +221,23 @@
 
         scores = self.model.evaluate(X_test, y_test)
 
         return predictions, scores
 
     @staticmethod
     def bce_dice_loss(y_true, y_pred):
+        import tensorflow as tf
         y_true_f = tf.reshape(y_true, [-1])
         y_pred_f = tf.reshape(y_pred, [-1])
         return tf.keras.losses.binary_crossentropy(y_true, y_pred) + (
                     1 - UNet.dice_coeff(y_true, y_pred))
 
     @staticmethod
     def dice_coeff(y_true, y_pred):
+        import tensorflow as tf
         y_true_f = tf.reshape(y_true, [-1])
         y_pred_f = tf.reshape(y_pred, [-1])
         intersection = tf.math.reduce_sum(y_true_f * y_pred_f)
         smoothing_const = 1e-9
         return (2. * intersection + smoothing_const) / (
                     tf.math.reduce_sum(y_true_f) + tf.math.reduce_sum(
                 y_pred_f) + smoothing_const)
```

### Comparing `gp2-0.5.23.23/gp2/gp2/classifiers/unet_plus.py` & `gp2-0.5.24.23/gp2/gp2/classifiers/unet_plus.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.23.23/gp2/gp2/discriminators/base_cnn_discriminator.py` & `gp2-0.5.24.23/gp2/gp2/discriminators/base_cnn_discriminator.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.23.23/gp2/gp2/util.py` & `gp2-0.5.24.23/gp2/gp2/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import logging
 import os
 import warnings
-import matplotlib.pyplot as plt
-import numpy as np
-from keras_unet_collection import losses
+
 
 
 class Util:
     @staticmethod
     def disable_tensorflow_logging():
         import tensorflow as tf
         """ Disables tensorflow logging """
@@ -39,20 +37,16 @@
         A : numpy array
             The A split
         B : numpy array
             The B split
         Z : numpy array
             The Z split
         """
-        #
-        # We split as follows
-        # A 0.4*dataset_size
-        # B 0.4*dataset_size
-        # Z 0.2*dataset_size
-        #
+        import numpy as np
+
         A_split = int(0.4 * dataset_size)
         B_split = int(0.2 * dataset_size)
         Z_split = int(0.4 * dataset_size)
 
         if weights:
             A_split = int(weights['A'] * dataset_size)
             B_split = int(weights['B'] * dataset_size)
@@ -107,15 +101,15 @@
         train : numpy array
             The training split
         val : numpy array
             The validation split
         test : numpy array
             The test split
         """
-
+        import numpy as np
         if shuffle:
             np.random.shuffle(dataset)
 
         train = dataset[0:train_count]
         val = dataset[train_count:train_count + val_count]
         test = dataset[
                train_count + val_count:train_count + val_count + test_count]
@@ -159,14 +153,15 @@
         y2 : numpy.ndarray | list
             The y-axis values for the discriminator.
 
         Returns
         -------
         None
         """
+        import matplotlib.pyplot as plt
         fig, ax1 = plt.subplots(1, 1, figsize=(3, 3), dpi=80)
         line1, = ax1.plot(x, y1, color='tab:red', label='Classifier')
         line2, = ax1.plot(x, y2, color='tab:blue', label='Discriminator')
         ax1.legend(handles=[line1, line2])
         ax1.xaxis.set_major_locator(plt.MaxNLocator(integer=True))
 
         ax1.set_xlabel('Cycle', color='tab:gray', fontsize=14)
@@ -235,14 +230,15 @@
 
         Returns
         -------
         float
             The loss.
         """
         import tensorflow as tf
+        from keras_unet_collection import losses
         # check that the types of both y_true and y_pred are the same
         y_true = tf.cast(y_true, tf.float32)
         y_pred = tf.cast(y_pred, tf.float32)
 
         loss_focal = losses.focal_tversky(y_true, y_pred, alpha=0.5,
                                           gamma=4 / 3)
         loss_iou = losses.iou_seg(y_true, y_pred)
```

### Comparing `gp2-0.5.23.23/gp2/runner.py` & `gp2-0.5.24.23/gp2/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .data import *
 from .gp2 import UNet, UNetPLUS, KUNet, KATTUnet2D, KR2UNet2dD, KResUNet2D, \
     KUNet2D, KUNet3Plus2D, KUNetPlus2D, KVNet2D, CNNDiscriminator, \
     CNNDiscriminatorPLUS, Util
 import time
-import numpy as np
 import os
 import tempfile
 
+
 def validate_weights(weights, tolerance=1e-6):
     """ Validate the weights for training.
 
     What must be verified:
         A_train + A_val + A_test = 1. \n
         B_train + B_val + B_test = 1. \n
         A + B + Z = 1. \n
@@ -33,14 +33,15 @@
         True if the weights are valid.
 
     Raises
     ------
     ValueError
         If the weights are not valid.
     """
+    import numpy as np
     # Check if A_train + A_val + A_test = 1
     A_sum = weights['A_train'] + weights['A_val'] + weights['A_test']
     if not np.isclose(A_sum, 1, rtol=tolerance):
         raise ValueError("A_train + A_val + A_test must be equal to 1")
 
     # Check if B_train + B_val + B_test = 1
     B_sum = weights['B_train'] + weights['B_val'] + weights['B_test']
@@ -96,15 +97,15 @@
         discriminator : str or Discriminator
             The discriminator to use. If None or 'cnn', will use the default
             handcrafted cnn discriminator.
         **kwargs : dict
             Additional keyword arguments to pass to the classifier and
             discriminator.
         """
-
+        import numpy as np
         self.weights = weights
         self.store_after_each_step = store_after_each_step
 
         self.workingdir = workingdir
 
         self.verbose = verbose
         if not self.verbose:
@@ -266,14 +267,15 @@
         batch_size : int
             Batch size to use for training.
 
         Returns
         -------
         None
         """
+        import numpy as np
         M = self.M
 
         A_train = M.get('A_train')
         A_val = M.get('A_val')
         A_test = M.get('A_test')
 
         #
@@ -317,14 +319,15 @@
             M.save(os.path.join(self.workingdir, 'M_step1.pickle'))
 
     #
     # STEP 2 (gets called by 4)
     #
     def create_C_dataset(self):
         """ Create the C dataset from the classifier predictions (internal!)."""
+        import numpy as np
         M = self.M
 
         A_test = M.get('A_test')
         A_test_pred = M.get('A_test_pred')
         B = M.get('B')
 
         A_test_images_only_, A_test_images_only_ids = A_test.to_array()
@@ -523,14 +526,15 @@
     #
     # STEP 6
     #
     def find_machine_labels(self):
         """ This finds all machine labels, as indicated from the Discriminator
         and create dataset D.  Returns number of machine labels found.
         """
+        import numpy as np
         M = self.M
 
         C_test = M.get('C_test')
         C_test_pred = M.get('C_test_pred')
 
         C_test_, C_test_ids = C_test.to_array()
         C_test_pred_, C_test_pred_ids = C_test_pred.to_array()
@@ -583,14 +587,15 @@
         fillup : bool
             Whether to fillup when updating A_train
 
         Returns
         -------
         None
         """
+        import numpy as np
 
         M = self.M
 
         D = M.get('D')
 
         # check that D in not NoneType
         if D is None:
@@ -666,14 +671,15 @@
         fillup : bool
             If True, fill-up B and A_test with points from A_train
 
         Returns
         -------
         None
         """
+        import numpy as np
         M = self.M
 
         D_relabeled = M.get('D_relabeled')
 
         A_train = M.get('A_train')
         A_test = M.get('A_test')
         B = M.get('B')
@@ -755,14 +761,15 @@
         target : Collection
             Target collection
 
         Returns
         -------
         None
         """
+        import numpy as np
         print('Transfer from', source.name, 'to', target.name)
         M = self.M
         source_uniq_ids = list(source.data.keys())
         source_uniq_id = np.random.choice(source_uniq_ids, replace=False)
 
         p = Point(source.data[source_uniq_id])
         p.id = source_uniq_id
@@ -815,30 +822,30 @@
         dataset_size = len(images)
         self.setup_data(images=images, masks=masks,
                         dataset_size=dataset_size,
                         weights=weights)
 
         for run in range(runs):
             print('******')
-            print('Loop', run+1)
+            print('Loop', run + 1)
             t0 = time.time()
             self.run_classifier(patience_counter=patience_counter,
                                 epochs=epochs, batch_size=batch_size)
             self.run_discriminator(patience_counter=patience_counter,
                                    epochs=epochs, batch_size=batch_size)
             l = self.find_machine_labels()
             if l == 0:
                 print('No more machine labels.')
                 print('TOOK', time.time() - t0, 'seconds')
                 break
             self.relabel(percent_to_replace=percent_to_replace,
                          balance=balance,
                          fillup=fillup)
             print('TOOK', time.time() - t0, 'seconds')
-            print('==== DONE LOOP', run+1, '====')
+            print('==== DONE LOOP', run + 1, '====')
 
     #
     # PLOT!
     #
     def plot(self):
         """ Plot the accuracies of the classifier and discriminator based on
         the scores stored in classifier_scores and discriminator_scores.
```

### Comparing `gp2-0.5.23.23/gp2.egg-info/PKG-INFO` & `gp2-0.5.24.23/gp2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2
-Version: 0.5.23.23
+Version: 0.5.24.23
 Summary: A framework for tuning segmentation classifiers and discriminators
 Home-page: https://github.com/RyanZurrin/CS410-GP2
 Author: mpsych lab
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gp2-0.5.23.23/gp2.egg-info/SOURCES.txt` & `gp2-0.5.24.23/gp2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gp2-0.5.23.23/setup.py` & `gp2-0.5.24.23/setup.py`

 * *Files identical despite different names*

