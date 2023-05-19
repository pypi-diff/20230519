# Comparing `tmp/velour-client-0.1.1.tar.gz` & `tmp/velour-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velour-client-0.1.1.tar", last modified: Thu May 18 14:36:24 2023, max compression
+gzip compressed data, was "velour-client-0.1.2.tar", last modified: Fri May 19 15:15:43 2023, max compression
```

## Comparing `velour-client-0.1.1.tar` & `velour-client-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.493789 velour-client-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 14:36:10.000000 velour-client-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-18 14:36:24.493789 velour-client-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 14:36:10.000000 velour-client-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-18 14:36:10.000000 velour-client-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:36:24.493789 velour-client-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-18 14:36:10.000000 velour-client-0.1.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.489789 velour-client-0.1.1/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.489789 velour-client-0.1.1/velour/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.489789 velour-client-0.1.1/velour/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/integrations/chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/integrations/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.493789 velour-client-0.1.1/velour_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:15:43.772221 velour-client-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-19 15:15:30.000000 velour-client-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-19 15:15:43.772221 velour-client-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 15:15:30.000000 velour-client-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-19 15:15:30.000000 velour-client-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:15:43.772221 velour-client-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-19 15:15:30.000000 velour-client-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:15:43.772221 velour-client-0.1.2/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-19 15:15:30.000000 velour-client-0.1.2/unit-tests/test_chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-19 15:15:30.000000 velour-client-0.1.2/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-19 15:15:30.000000 velour-client-0.1.2/unit-tests/test_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-19 15:15:30.000000 velour-client-0.1.2/unit-tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-19 15:15:30.000000 velour-client-0.1.2/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:15:43.772221 velour-client-0.1.2/velour/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-19 15:15:30.000000 velour-client-0.1.2/velour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27670 2023-05-19 15:15:30.000000 velour-client-0.1.2/velour/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-19 15:15:30.000000 velour-client-0.1.2/velour/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:15:43.772221 velour-client-0.1.2/velour/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-05-19 15:15:30.000000 velour-client-0.1.2/velour/integrations/chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-19 15:15:30.000000 velour-client-0.1.2/velour/integrations/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-19 15:15:30.000000 velour-client-0.1.2/velour/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-19 15:15:30.000000 velour-client-0.1.2/velour/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:15:43.772221 velour-client-0.1.2/velour_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-19 15:15:43.000000 velour-client-0.1.2/velour_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 15:15:43.000000 velour-client-0.1.2/velour_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:15:43.000000 velour-client-0.1.2/velour_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 15:15:43.000000 velour-client-0.1.2/velour_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 15:15:43.000000 velour-client-0.1.2/velour_client.egg-info/top_level.txt
```

### Comparing `velour-client-0.1.1/LICENSE` & `velour-client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/PKG-INFO` & `velour-client-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.1.1/pyproject.toml` & `velour-client-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/unit-tests/test_chariot.py` & `velour-client-0.1.2/unit-tests/test_chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/unit-tests/test_client.py` & `velour-client-0.1.2/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/unit-tests/test_coco.py` & `velour-client-0.1.2/unit-tests/test_coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/unit-tests/test_data_types.py` & `velour-client-0.1.2/unit-tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/unit-tests/test_viz.py` & `velour-client-0.1.2/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/velour/client.py` & `velour-client-0.1.2/velour/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
             "settings": {
                 "model_name": self.name,
                 "dataset_name": dataset.name,
             }
         }
 
         resp = self.client._requests_post_rel_host(
-            "/clf-metrics", json=payload
+            "clf-metrics", json=payload
         ).json()
 
         return EvalJob(client=self.client, **resp)
 
     def get_evaluation_settings(self) -> List[dict]:
         # TODO: should probably have a dataclass for the output
         ret = self.client._requests_get_rel_host(
@@ -434,15 +434,15 @@
             ).json()
         ]
 
     def get_confusion_matrices_at_evaluation_settings_id(
         self, eval_settings_id: int
     ) -> List[dict]:
         return self.client._requests_get_rel_host(
-            f"/models/{self.name}/evaluation-settings/{eval_settings_id}/confusion-matrices"
+            f"models/{self.name}/evaluation-settings/{eval_settings_id}/confusion-matrices"
         ).json()
 
     def get_metric_dataframes(self):
         try:
             import pandas as pd
         except ModuleNotFoundError:
             raise ModuleNotFoundError(
@@ -595,15 +595,15 @@
 
         if iou_thresholds is not None:
             payload["iou_thresholds"] = iou_thresholds
         if ious_to_keep is not None:
             payload["ious_to_keep"] = ious_to_keep
 
         resp = self.client._requests_post_rel_host(
-            "/ap-metrics", json=payload
+            "ap-metrics", json=payload
         ).json()
         # resp should have keys "missing_pred_labels", "ignored_pred_labels", with values
         # list of label dicts. convert label dicts to Label objects
         for k in ["missing_pred_labels", "ignored_pred_labels"]:
             resp[k] = [Label(**la) for la in resp[k]]
 
         return EvalJob(client=self.client, **resp)
@@ -691,26 +691,32 @@
         return resp["email"]
 
     def _requests_wrapper(
         self, method_name: str, endpoint: str, *args, **kwargs
     ):
         assert method_name in ["get", "post", "put", "delete"]
 
+        if endpoint[0] == "/":
+            raise ValueError(
+                "`endpoint` should not start with a forward slash."
+            )
+
         url = urljoin(self.host, endpoint)
         requests_method = getattr(requests, method_name)
 
         if self.access_token is not None:
             headers = {"Authorization": f"Bearer {self.access_token}"}
         else:
             headers = None
         resp = requests_method(url, headers=headers, *args, **kwargs)
         if not resp.ok:
-            if resp.status_code == 500:
+            try:
+                raise ClientException(resp.json()["detail"])
+            except (requests.exceptions.JSONDecodeError, KeyError):
                 resp.raise_for_status()
-            raise ClientException(resp.json()["detail"])
 
         return resp
 
     def _requests_post_rel_host(self, endpoint: str, *args, **kwargs):
         return self._requests_wrapper(
             method_name="post", endpoint=endpoint, *args, **kwargs
         )
@@ -849,27 +855,27 @@
         self._id = job_id
         self.client = client
 
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def status(self) -> str:
-        resp = self.client._requests_get_rel_host(f"/jobs/{self._id}").json()
+        resp = self.client._requests_get_rel_host(f"jobs/{self._id}").json()
         return resp["status"]
 
 
 class EvalJob(Job):
     def metrics(self) -> List[dict]:
         return self.client._requests_get_rel_host(
-            f"/jobs/{self._id}/metrics"
+            f"jobs/{self._id}/metrics"
         ).json()
 
     def confusion_matrices(self) -> List[dict]:
         return self.client._requests_get_rel_host(
-            f"/jobs/{self._id}/confusion-matrices"
+            f"jobs/{self._id}/confusion-matrices"
         ).json()
 
     # TODO: replace value with a dataclass?
     def settings(self) -> dict:
         return self.client._requests_get_rel_host(
-            f"/jobs/{self._id}/settings"
+            f"jobs/{self._id}/settings"
         ).json()
```

### Comparing `velour-client-0.1.1/velour/data_types.py` & `velour-client-0.1.2/velour/data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/velour/integrations/chariot.py` & `velour-client-0.1.2/velour/integrations/chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/velour/integrations/coco.py` & `velour-client-0.1.2/velour/integrations/coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/velour/viz.py` & `velour-client-0.1.2/velour/viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.1/velour_client.egg-info/PKG-INFO` & `velour-client-0.1.2/velour_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

