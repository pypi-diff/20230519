# Comparing `tmp/dialog-workflow-local-0.0.28.tar.gz` & `tmp/dialog-workflow-local-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.28.tar", last modified: Fri May 19 11:41:42 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.29.tar", last modified: Fri May 19 11:48:11 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.28.tar` & `dialog-workflow-local-0.0.29.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20860 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:41:42.000000 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 11:41:42.000000 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:41:42.000000 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 11:41:42.000000 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:48:11.673079 dialog-workflow-local-0.0.29/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:48:11.673079 dialog-workflow-local-0.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:48:11.673079 dialog-workflow-local-0.0.29/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:48:11.673079 dialog-workflow-local-0.0.29/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:48:11.000000 dialog-workflow-local-0.0.29/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 11:48:11.000000 dialog-workflow-local-0.0.29/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:48:11.000000 dialog-workflow-local-0.0.29/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 11:48:11.000000 dialog-workflow-local-0.0.29/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:48:11.673079 dialog-workflow-local-0.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 11:47:58.000000 dialog-workflow-local-0.0.29/setup.py
```

### Comparing `dialog-workflow-local-0.0.28/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.29/dialog_workflow/Act.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dialog_workflow.utils import *
 from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
 import time
 # import msvcrt
-import requests
+# import requests
 from AgeDetection import DetectAge
 
 class action(object):
     def __init__(self, incoming_message: str, profile_id: int, language: str, profile_curr_state: int, variables: Variable):
         self.incoming_message = incoming_message
         self.profile_id = profile_id
         self.language = language
@@ -116,21 +116,21 @@
         """Jumps from one state to another."""
         self.profile_curr_state = int(self.record.parameter1)
         update_profile_curr_state_in_DB(self.profile_id, int(self.record.parameter1))
         return True, None
 
     def send_rest_api_action(self):
         """Sends a REST API post"""
-        api_url = self.record.parameter1
-        payload_variable_id = self.record.variable1_id
-        json_payload_string = get_variable_value_by_id(self.language, payload_variable_id)
-        json_payload = json.loads(json_payload_string)
-        incoming_message = requests.post(api_url, json=json_payload)
-        incoming_message_string = json.dumps(incoming_message.json())
-        insert_profile_variable_value(self.profile_id, self.variable.get_variable_id("Post Result"), incoming_message_string, self.profile_curr_state)
+        # api_url = self.record.parameter1
+        # payload_variable_id = self.record.variable1_id
+        # json_payload_string = get_variable_value_by_id(self.language, payload_variable_id)
+        # json_payload = json.loads(json_payload_string)
+        # incoming_message = requests.post(api_url, json=json_payload)
+        # incoming_message_string = json.dumps(incoming_message.json())
+        # insert_profile_variable_value(self.profile_id, self.variable.get_variable_id("Post Result"), incoming_message_string, self.profile_curr_state)
         return False, None
 
     def assign_variable_action(self):
         """Assigns a value to a given variable"""
         parameter_value = self.record.parameter1
         variable_id = self.record.variable1_id
         insert_profile_variable_value(self.profile_id, variable_id, parameter_value, self.profile_curr_state)
```

### Comparing `dialog-workflow-local-0.0.28/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.29/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.28/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.29/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.28/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.29/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.28/dialog_workflow/test.py` & `dialog-workflow-local-0.0.29/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.28/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.29/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.28/setup.py` & `dialog-workflow-local-0.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local',  
-     version='0.0.28',
+     version='0.0.29',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

