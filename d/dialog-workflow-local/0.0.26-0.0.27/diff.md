# Comparing `tmp/dialog-workflow-local-0.0.26.tar.gz` & `tmp/dialog-workflow-local-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.26.tar", last modified: Fri May 19 10:13:47 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.27.tar", last modified: Fri May 19 11:31:59 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.26.tar` & `dialog-workflow-local-0.0.27.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 10:13:47.000000 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 10:13:47.000000 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:13:47.000000 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 10:13:47.000000 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:59.672601 dialog-workflow-local-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:31:59.668601 dialog-workflow-local-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:59.668601 dialog-workflow-local-0.0.27/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20804 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:31:59.668601 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 11:31:59.000000 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 11:31:59.000000 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:31:59.000000 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 11:31:59.000000 dialog-workflow-local-0.0.27/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:31:59.672601 dialog-workflow-local-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 11:31:48.000000 dialog-workflow-local-0.0.27/setup.py
```

### Comparing `dialog-workflow-local-0.0.26/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.27/dialog_workflow/Act.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,48 +33,45 @@
         Note : some of the actions are divided into 2 parts: 
             1. The action before sendig the outgoing message to the user (i.e got_response = false)
             2. The action after sending the outgoing message, and getting an incoming_message reply back (i.e got_respone = true). """    
             
         self.record = dialog_workflow_record
         self.got_response = got_response
         action = self.record.workflow_action_id
-        match action:
-            case action_enum.LABEL_ACTION.value:
-                return False, None
-            case action_enum.TEXT_MESSAGE_ACTION.value:
-                return self.text_message_action()
-            case action_enum.QUESTION_ACTION.value:
-                return self.question_action()
-            case action_enum.JUMP_ACTION.value:
-                return self.jump_action()
-            case action_enum.SEND_REST_API_ACTION:
-                return self.send_rest_api_action()
-            case action_enum.ASSIGN_VARIABLE_ACTION.value:
-                return self.assign_variable_action()
-            case action_enum.INCREMENT_VARIABLE_ACTION.value:
-                return self.increment_variable_action()
-            case action_enum.DECREMENT_VARIABLE_ACTION.value:
-                return self.decrement_variable_action()
-            # case action_enum.CONDITION_ACTION.value:
-            #     return condition_action(record)
-            case action_enum.MENU_ACTION.value:
-                return self.menu_action()
-            case action_enum.AGE_DETECTION.value:
-                return self.age_detection()
-            case action_enum.MULTI_CHOICE_POLL.value:
-                return self.multi_choice_poll()
-            case action_enum.PRESENT_CHILD_GROUPS_NAMES_BY_ID.value:
-                return self.present_child_groups_names_by_id()   
-            case action_enum.PRESENT_GROUPS_WITH_CERTAIN_TEXT.value:
-                return self.present_groups_with_certain_text()     
-            case action_enum.INSERT_MISSING_DATA.value:
-                return self.insert_missing_data()   
-            case action_enum.PRESENT_AND_CHOOSE_SCRIPT.value:
-                return self.present_and_choose_script()             
-                                 
+        if action == action_enum.LABEL_ACTION.value:
+            return False, None
+        elif action == action_enum.TEXT_MESSAGE_ACTION.value:
+            return self.text_message_action()
+        elif action == action_enum.QUESTION_ACTION.value:
+            return self.question_action()
+        elif action == action_enum.JUMP_ACTION.value:
+            return self.jump_action()
+        elif action == action_enum.SEND_REST_API_ACTION:
+            return self.send_rest_api_action()
+        elif action == action_enum.ASSIGN_VARIABLE_ACTION.value:
+            return self.assign_variable_action()
+        elif action == action_enum.INCREMENT_VARIABLE_ACTION.value:
+            return self.increment_variable_action()
+        elif action == action_enum.DECREMENT_VARIABLE_ACTION.value:
+            return self.decrement_variable_action()
+        elif action == action_enum.MENU_ACTION.value:
+            return self.menu_action()
+        elif action == action_enum.AGE_DETECTION.value:
+            return self.age_detection()
+        elif action == action_enum.MULTI_CHOICE_POLL.value:
+            return self.multi_choice_poll()
+        elif action == action_enum.PRESENT_CHILD_GROUPS_NAMES_BY_ID.value:
+            return self.present_child_groups_names_by_id()   
+        elif action == action_enum.PRESENT_GROUPS_WITH_CERTAIN_TEXT.value:
+            return self.present_groups_with_certain_text()     
+        elif action == action_enum.INSERT_MISSING_DATA.value:
+            return self.insert_missing_data()   
+        elif action == action_enum.PRESENT_AND_CHOOSE_SCRIPT.value:
+            return self.present_and_choose_script()             
+
             
     def text_message_action(self):
         """Prints the paramter1 message after formatting: 
         "Hello {First Name}, how are you {feeling|doing}?" --> "Hello Tal, how are you doing? """
         message = self.record.parameter1
         replace_fields_with_values_class = replace_fields_with_values(message, self.language, self.variable)
         formatted_message = replace_fields_with_values_class.get_variable_values_and_chosen_option()
```

### Comparing `dialog-workflow-local-0.0.26/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.27/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.26/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.27/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.26/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.27/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.26/dialog_workflow/test.py` & `dialog-workflow-local-0.0.27/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.26/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.27/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.26/setup.py` & `dialog-workflow-local-0.0.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local',  
-     version='0.0.26',
+     version='0.0.27',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

