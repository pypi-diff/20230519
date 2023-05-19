# Comparing `tmp/dialog-workflow-local-0.0.27.tar.gz` & `tmp/dialog-workflow-local-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.27.tar", last modified: Fri May 19 11:31:59 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.28.tar", last modified: Fri May 19 11:41:42 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.27.tar` & `dialog-workflow-local-0.0.28.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:59.672601 dialog-workflow-local-0.0.27/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:31:59.668601 dialog-workflow-local-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:59.668601 dialog-workflow-local-0.0.27/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20804 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:59.668601 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:31:59.000000 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 11:31:59.000000 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:31:59.000000 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 11:31:59.000000 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:31:59.672601 dialog-workflow-local-0.0.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20860 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:41:42.000000 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 11:41:42.000000 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:41:42.000000 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 11:41:42.000000 dialog-workflow-local-0.0.28/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:41:42.951239 dialog-workflow-local-0.0.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 11:41:29.000000 dialog-workflow-local-0.0.28/setup.py
```

### Comparing `dialog-workflow-local-0.0.27/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.28/dialog_workflow/Act.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dialog_workflow.utils import *
 from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
 import time
-import msvcrt
+# import msvcrt
 import requests
 from AgeDetection import DetectAge
 
 class action(object):
     def __init__(self, incoming_message: str, profile_id: int, language: str, profile_curr_state: int, variables: Variable):
         self.incoming_message = incoming_message
         self.profile_id = profile_id
@@ -91,21 +91,22 @@
                 return False, outgoing_message
             else:
                 self.accumulated_message = ""
             
             waiting_time = self.record.no_feedback_milliseconds 
             start_time = time.monotonic()
             input_str = None
-            while True:
-                if msvcrt.kbhit():
-                    input_str = input().strip()
-                    insert_profile_variable_value(self.profile_id, self.record.variable1_id, input_str, self.profile_curr_state)
-                    break
-                elif time.monotonic() - start_time > waiting_time:
-                    break
+            # while True:
+                # if msvcrt.kbhit():
+                    # input_str = input().strip()
+                    # insert_profile_variable_value(self.profile_id, self.record.variable1_id, input_str, self.profile_curr_state)
+                    # break
+                # elif time.monotonic() - start_time > waiting_time:
+                    # break
+            input_str = input().strip()
             if input_str == None:
                 self.profile_curr_state = self.record.next_state_id_if_there_is_no_feedback
                 return True, None
             else:
                 return False, None
         else:
             insert_profile_variable_value(self.profile_id, self.record.variable1_id, self.incoming_message, self.profile_curr_state)
```

### Comparing `dialog-workflow-local-0.0.27/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.28/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.27/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.28/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.27/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.28/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.27/dialog_workflow/test.py` & `dialog-workflow-local-0.0.28/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.27/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.28/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.27/setup.py` & `dialog-workflow-local-0.0.28/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local',  
-     version='0.0.27',
+     version='0.0.28',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

