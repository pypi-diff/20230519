# Comparing `tmp/mmlab_lightning-1.0.5.tar.gz` & `tmp/mmlab-lightning-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmlab_lightning-1.0.5.tar", last modified: Tue May 16 09:41:54 2023, max compression
+gzip compressed data, was "mmlab-lightning-1.0.6.tar", last modified: Fri May 19 03:41:18 2023, max compression
```

## Comparing `mmlab_lightning-1.0.5.tar` & `mmlab-lightning-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.196824 mmlab_lightning-1.0.5/mmlab_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/mmlab_lightning/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/datasets/mmlab_dataset_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/mmlab_lightning/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/models/mmlab_model_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/mmlab_lightning/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/mmlab_lightning/tools/config/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/tools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/tools/config/get_mmconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.196824 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.900697 mmlab-lightning-1.0.6/mmlab_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/datasets/mmlab_dataset_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/models/mmlab_model_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning/tools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/tools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/mmlab_lightning/tools/config/get_mmconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 03:41:18.000000 mmlab-lightning-1.0.6/mmlab_lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 03:41:18.904697 mmlab-lightning-1.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-19 03:41:03.000000 mmlab-lightning-1.0.6/setup.py
```

### Comparing `mmlab_lightning-1.0.5/LICENSE` & `mmlab-lightning-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.5/PKG-INFO` & `mmlab-lightning-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mmlab_lightning
-Version: 1.0.5
+Name: mmlab-lightning
+Version: 1.0.6
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab_lightning-1.0.5/README.md` & `mmlab-lightning-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.5/mmlab_lightning/datasets/mmlab_dataset_adapter.py` & `mmlab-lightning-1.0.6/mmlab_lightning/datasets/mmlab_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.5/mmlab_lightning/models/mmlab_model_adapter.py` & `mmlab-lightning-1.0.6/mmlab_lightning/models/mmlab_model_adapter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC
+from typing import Any, Optional
 
-import torch
 from lightning_template.models import LightningModule
+from mmengine import MessageHub
 from mmengine.model import BaseModule
-from torch import nn
 
 
 class MMLabModelAdapter(LightningModule, BaseModule, ABC):
     def __init__(self, visualizer_kwargs=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if visualizer_kwargs is None:
@@ -18,14 +18,21 @@
     def _dump_init_info(self, *args, **kwargs):
         pass
 
     def set_data_preprocessor_device(self):
         self.model.data_preprocessor.to(self.device)
 
     def on_fit_start(self):
+        message_hub = MessageHub.get_current_instance()
+        message_hub.update_info(
+            "epoch", self.trainer.fit_loop.epoch_progress.current.completed
+        )
+        message_hub.update_info("iter", self.trainer.global_step)
+        message_hub.update_info("max_epochs", self.trainer.max_epochs)
+        message_hub.update_info("max_iters", self.trainer.max_steps)
         self.set_data_preprocessor_device()
         self.init_weights()
 
     def on_validation_start(self):
         self.set_data_preprocessor_device()
 
     def on_test_start(self):
@@ -47,14 +54,26 @@
     def on_forward_epoch_end(self, *args, split="val", **kwargs):
         log_vars = self.trainer.datamodule.evaluators[split].evaluate(
             len(self.trainer.datamodule.datasets[split])
         )
         self.log_dict(self.flatten_dict(log_vars, split), sync_dist=True)
         return log_vars
 
+    def on_train_epoch_start(self) -> None:
+        message_hub = MessageHub.get_current_instance()
+        message_hub.update_info(
+            "epoch", self.trainer.fit_loop.epoch_progress.current.completed
+        )
+        return super().on_train_epoch_start()
+
+    def on_train_batch_start(self, batch: Any, batch_idx: int) -> int | None:
+        message_hub = MessageHub.get_current_instance()
+        message_hub.update_info("iter", self.trainer.global_step)
+        return super().on_train_batch_start(batch, batch_idx)
+
     def training_step(self, batch, *args, **kwargs):
         _, log_vars = self.model.parse_losses(self(batch))
         self.log_dict(self.flatten_dict(log_vars))
         return log_vars
 
     def predict_forward(self, batch, *args, **kwargs):
         predict_result = {"predict_outputs": self(batch, mode="predict")}
```

### Comparing `mmlab_lightning-1.0.5/mmlab_lightning.egg-info/PKG-INFO` & `mmlab-lightning-1.0.6/mmlab_lightning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab-lightning
-Version: 1.0.5
+Version: 1.0.6
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab_lightning-1.0.5/mmlab_lightning.egg-info/SOURCES.txt` & `mmlab-lightning-1.0.6/mmlab_lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.5/setup.py` & `mmlab-lightning-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
-    name="mmlab_lightning",
-    version="1.0.5",
+    name="mmlab-lightning",
+    version="1.0.6",
     description="A wrapper for mmlab repos to use in project_template.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/mmlab_lightning",
     project_urls={
```

