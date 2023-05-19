# Comparing `tmp/dialog-workflow-local-0.0.25.tar.gz` & `tmp/dialog-workflow-local-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.25.tar", last modified: Fri May 19 10:05:23 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.26.tar", last modified: Fri May 19 10:13:47 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.25.tar` & `dialog-workflow-local-0.0.26.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:05:23.885345 dialog-workflow-local-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 10:05:23.885345 dialog-workflow-local-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:05:23.885345 dialog-workflow-local-0.0.25/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:05:23.885345 dialog-workflow-local-0.0.25/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 10:05:23.000000 dialog-workflow-local-0.0.25/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 10:05:23.000000 dialog-workflow-local-0.0.25/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:05:23.000000 dialog-workflow-local-0.0.25/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 10:05:23.000000 dialog-workflow-local-0.0.25/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:05:23.885345 dialog-workflow-local-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 10:05:07.000000 dialog-workflow-local-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 10:13:47.000000 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 10:13:47.000000 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:13:47.000000 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 10:13:47.000000 dialog-workflow-local-0.0.26/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:13:47.476469 dialog-workflow-local-0.0.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 10:13:34.000000 dialog-workflow-local-0.0.26/setup.py
```

### Comparing `dialog-workflow-local-0.0.25/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.26/dialog_workflow/Act.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.25/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.26/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.25/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.26/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.25/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.26/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.25/dialog_workflow/test.py` & `dialog-workflow-local-0.0.26/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.25/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.26/dialog_workflow/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             SELECT group_view.id FROM group_view 
             JOIN cte ON group_view.parent_group_id = cte.id
         )
         SELECT * FROM cte""", [self.parameter1])  
         group_id_dict = cursor.fetchall()
         return [group['id'] for group in group_id_dict]
 
-    def get_child_group_names(self) -> list[str]:
+    def get_child_group_names(self) -> list:
         """Gets all of the child title names from the ml table of the given parent_id."""
         group_ids = self.get_group_childs_id_bellow_parent_id()
         group_id_string = ','.join(str(id) for id in group_ids)
         cursor.execute(f"SELECT title FROM group_ml_en_view WHERE group_id IN ({group_id_string}) ")
         group_name_dict = cursor.fetchall()
         return [group['title'] for group in group_name_dict]
```

### Comparing `dialog-workflow-local-0.0.25/setup.py` & `dialog-workflow-local-0.0.26/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local',  
-     version='0.0.25',
+     version='0.0.26',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

