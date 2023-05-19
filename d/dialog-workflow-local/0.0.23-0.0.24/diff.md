# Comparing `tmp/dialog-workflow-local-0.0.23.tar.gz` & `tmp/dialog-workflow-local-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.23.tar", last modified: Fri May 19 07:50:41 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.24.tar", last modified: Fri May 19 09:42:30 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.23.tar` & `dialog-workflow-local-0.0.24.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:50:41.110957 dialog-workflow-local-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 07:50:41.110957 dialog-workflow-local-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:50:41.110957 dialog-workflow-local-0.0.23/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20907 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:50:41.110957 dialog-workflow-local-0.0.23/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 07:50:41.000000 dialog-workflow-local-0.0.23/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 07:50:41.000000 dialog-workflow-local-0.0.23/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:50:41.000000 dialog-workflow-local-0.0.23/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 07:50:41.000000 dialog-workflow-local-0.0.23/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 07:50:41.110957 dialog-workflow-local-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 07:50:25.000000 dialog-workflow-local-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:42:30.381974 dialog-workflow-local-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 09:42:30.381974 dialog-workflow-local-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:42:30.381974 dialog-workflow-local-0.0.24/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20907 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:42:30.381974 dialog-workflow-local-0.0.24/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 09:42:30.000000 dialog-workflow-local-0.0.24/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 09:42:30.000000 dialog-workflow-local-0.0.24/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:42:30.000000 dialog-workflow-local-0.0.24/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 09:42:30.000000 dialog-workflow-local-0.0.24/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:42:30.381974 dialog-workflow-local-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 09:42:18.000000 dialog-workflow-local-0.0.24/setup.py
```

### Comparing `dialog-workflow-local-0.0.23/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.24/dialog_workflow/Act.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.23/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.24/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.23/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.24/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.23/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.24/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.23/dialog_workflow/test.py` & `dialog-workflow-local-0.0.24/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.23/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.24/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.23/setup.py` & `dialog-workflow-local-0.0.24/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local',  
-     version='0.0.23',
+     version='0.0.24',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

