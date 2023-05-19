# Comparing `tmp/irisml-tasks-azureml-0.1.3.tar.gz` & `tmp/irisml-tasks-azureml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-azureml-0.1.3.tar", last modified: Wed Apr 19 07:26:46 2023, max compression
+gzip compressed data, was "irisml-tasks-azureml-0.1.4.tar", last modified: Fri May 19 06:09:56 2023, max compression
```

## Comparing `irisml-tasks-azureml-0.1.3.tar` & `irisml-tasks-azureml-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.688895 irisml-tasks-azureml-0.1.3/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.688895 irisml-tasks-azureml-0.1.3/irisml/azureml/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/azureml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/azureml/azureml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.688895 irisml-tasks-azureml-0.1.3/irisml/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/commands/cancel_aml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/commands/run_aml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/tasks/add_aml_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/tasks/run_azureml_child.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/test/test_add_aml_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/test/test_azureml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.492418 irisml-tasks-azureml-0.1.4/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.492418 irisml-tasks-azureml-0.1.4/irisml/azureml/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/azureml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/azureml/azureml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.492418 irisml-tasks-azureml-0.1.4/irisml/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/commands/cancel_aml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/commands/run_aml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/tasks/add_aml_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/tasks/run_azureml_child.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/test/test_add_aml_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/test/test_azureml.py
```

### Comparing `irisml-tasks-azureml-0.1.3/LICENSE` & `irisml-tasks-azureml-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.3/PKG-INFO` & `irisml-tasks-azureml-0.1.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azureml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Utility tools to use IrisML on AzureML
 Home-page: https://github.com/microsoft/irisml-tasks-azureml
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azureml-0.1.3/README.md` & `irisml-tasks-azureml-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.3/irisml/azureml/azureml.py` & `irisml-tasks-azureml-0.1.4/irisml/azureml/azureml.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 
 logger = logging.getLogger(__name__)
 
 SHARED_MEMORY_SIZE = '16g'
 
 
 class AMLJobManager:
-    def __init__(self, subscription_id, workspace_name, experiment_name, compute_target_name, use_sp_on_remote=False, cache_url=None):
+    def __init__(self, subscription_id, workspace_name, experiment_name, compute_target_name, use_sp_on_remote=False, cache_url=None, no_cache_read=False):
         """
         Args:
             subscription_id (str): The subscription ID for the azureml resource.
             workspace_name (str): Workspace name
             experiment_name (str): Experiment name
             compute_target_name (str): Compute Target name
             use_sp_on_remote (bool): If True, get AZURE_TENANT_ID, AZURE_CLIENT_ID, AZURE_CLIENT_SECRET from environment and send it to the AzureML.
             cache_url (str): URL to a cache storage. If provided, it will be used in an AzureML job.
+            no_cache_read (bool): If True, disable cache read.
        """
         self._workspace = self._get_workspace(subscription_id, workspace_name)
         self._experiment = azureml.core.Experiment(workspace=self._workspace, name=experiment_name)
         self._compute_target_name = compute_target_name
         self._use_sp_on_remote = use_sp_on_remote
         self._cache_url = cache_url
+        self._no_cache_read = no_cache_read
 
     def _get_workspace(self, subscription_id, workspace_name):
         auth = None
         if os.getenv('AZURE_TENANT_ID') and os.getenv('AZURE_CLIENT_ID') and os.getenv('AZURE_CLIENT_SECRET'):
             logger.info(f"Using Service Principal to authenticate to AzureML. tenant_id={os.getenv('AZURE_TENANT_ID')}, client_id={os.getenv('AZURE_CLIENT_ID')}")
             auth = azureml.core.authentication.ServicePrincipalAuthentication(os.getenv('AZURE_TENANT_ID'), os.getenv('AZURE_CLIENT_ID'), os.getenv('AZURE_CLIENT_SECRET'))
 
@@ -74,14 +76,17 @@
             env_vars['AZURE_TENANT_ID'] = tenant_id
             env_vars['AZURE_CLIENT_ID'] = client_id
             env_vars['AZURE_CLIENT_SECRET'] = client_secret
 
         if self._cache_url:
             env_vars['IRISML_CACHE_URL'] = self._cache_url
 
+        if self._no_cache_read:
+            env_vars['IRISML_NO_CACHE_READ'] = '1'
+
         return env_vars
 
     def get_script_run_config(self, project_dir, job, job_env, environment_variables):
         command = job.command
         if not environment_variables.get('AZURE_CLIENT_ID'):
             # For Managed Identity
             command = 'AZURE_CLIENT_ID=$DEFAULT_IDENTITY_CLIENT_ID ' + command
```

### Comparing `irisml-tasks-azureml-0.1.3/irisml/commands/cancel_aml.py` & `irisml-tasks-azureml-0.1.4/irisml/commands/cancel_aml.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.3/irisml/commands/run_aml.py` & `irisml-tasks-azureml-0.1.4/irisml/commands/run_aml.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     configure_logger()
 
     parser = argparse.ArgumentParser()
     parser.add_argument('job_filepath', type=pathlib.Path)
     parser.add_argument('--env', '-e', nargs=1, default={}, action=KeyValuePairAction)
     parser.add_argument('--no_cache', action='store_true')
+    parser.add_argument('--no_cache_read', action='store_true')
     parser.add_argument('--include_local_tasks', '-l', nargs='?', const=pathlib.Path(), default=None, type=pathlib.Path)
     parser.add_argument('--custom_packages', '-p', nargs='+', default=[])
     parser.add_argument('--requirement', '-r', type=pathlib.Path)
     parser.add_argument('--extra_index_url')
     parser.add_argument('--no_wait', action='store_true')
     parser.add_argument('--compute_target', default=os.getenv('IRISML_AML_COMPUTE_TARGET'))
     parser.add_argument('--subscription_id', default=os.getenv('IRISML_AML_SUBSCRIPTION_ID'))
@@ -57,15 +58,16 @@
 
     custom_packages = args.custom_packages
     if args.requirement:
         custom_packages = custom_packages + args.requirement.read_text().splitlines()
     env = JobEnvironment(args.base_docker_image, args.base_docker_image_registry, custom_packages, args.extra_index_url, not args.no_docker_build_date_label)
     print(env)
 
-    job_manager = AMLJobManager(args.subscription_id, args.workspace, args.experiment, args.compute_target, use_sp_on_remote=args.use_sp_on_remote, cache_url=cache_url)
+    job_manager = AMLJobManager(args.subscription_id, args.workspace, args.experiment, args.compute_target, use_sp_on_remote=args.use_sp_on_remote,
+                                cache_url=cache_url, no_cache_read=args.no_cache_read)
     run = job_manager.submit(job, env)
     print(run)
 
     if not args.no_wait:
         run.wait_for_completion()
```

### Comparing `irisml-tasks-azureml-0.1.3/irisml/tasks/add_aml_tag.py` & `irisml-tasks-azureml-0.1.4/irisml/tasks/add_aml_tag.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/PKG-INFO` & `irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azureml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Utility tools to use IrisML on AzureML
 Home-page: https://github.com/microsoft/irisml-tasks-azureml
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/SOURCES.txt` & `irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.3/setup.cfg` & `irisml-tasks-azureml-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-azureml
-version = 0.1.3
+version = 0.1.4
 url = https://github.com/microsoft/irisml-tasks-azureml
 description = Utility tools to use IrisML on AzureML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-azureml-0.1.3/test/test_add_aml_tag.py` & `irisml-tasks-azureml-0.1.4/test/test_add_aml_tag.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.3/test/test_azureml.py` & `irisml-tasks-azureml-0.1.4/test/test_azureml.py`

 * *Files identical despite different names*

