# Comparing `tmp/pybuilder-integration-89.tar.gz` & `tmp/pybuilder-integration-90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-integration-89.tar", last modified: Fri May 19 00:32:40 2023, max compression
+gzip compressed data, was "pybuilder-integration-90.tar", last modified: Fri May 19 00:33:09 2023, max compression
```

## Comparing `pybuilder-integration-89.tar` & `pybuilder-integration-90.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:32:40.281151 pybuilder-integration-89/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 00:32:40.277150 pybuilder-integration-89/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:32:40.277150 pybuilder-integration-89/pybuilder_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-19 00:32:00.000000 pybuilder-integration-89/pybuilder_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-19 00:32:00.000000 pybuilder-integration-89/pybuilder_integration/artifact_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-19 00:32:00.000000 pybuilder-integration-89/pybuilder_integration/cloudwatchlogs_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-19 00:32:00.000000 pybuilder-integration-89/pybuilder_integration/directory_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-19 00:32:00.000000 pybuilder-integration-89/pybuilder_integration/exec_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-19 00:32:00.000000 pybuilder-integration-89/pybuilder_integration/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-05-19 00:32:00.000000 pybuilder-integration-89/pybuilder_integration/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-19 00:32:00.000000 pybuilder-integration-89/pybuilder_integration/tool_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:32:40.277150 pybuilder-integration-89/pybuilder_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 00:32:40.000000 pybuilder-integration-89/pybuilder_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-19 00:32:40.000000 pybuilder-integration-89/pybuilder_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:32:40.000000 pybuilder-integration-89/pybuilder_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:32:40.000000 pybuilder-integration-89/pybuilder_integration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 00:32:40.000000 pybuilder-integration-89/pybuilder_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 00:32:40.000000 pybuilder-integration-89/pybuilder_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:32:40.000000 pybuilder-integration-89/pybuilder_integration.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:32:40.281151 pybuilder-integration-89/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-19 00:32:38.000000 pybuilder-integration-89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:33:09.091929 pybuilder-integration-90/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 00:33:09.091929 pybuilder-integration-90/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:33:09.087929 pybuilder-integration-90/pybuilder_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-19 00:32:31.000000 pybuilder-integration-90/pybuilder_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-19 00:32:31.000000 pybuilder-integration-90/pybuilder_integration/artifact_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-19 00:32:31.000000 pybuilder-integration-90/pybuilder_integration/cloudwatchlogs_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-19 00:32:31.000000 pybuilder-integration-90/pybuilder_integration/directory_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-19 00:32:31.000000 pybuilder-integration-90/pybuilder_integration/exec_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-19 00:32:31.000000 pybuilder-integration-90/pybuilder_integration/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-05-19 00:32:31.000000 pybuilder-integration-90/pybuilder_integration/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-19 00:32:31.000000 pybuilder-integration-90/pybuilder_integration/tool_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:33:09.091929 pybuilder-integration-90/pybuilder_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 00:33:09.000000 pybuilder-integration-90/pybuilder_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-19 00:33:09.000000 pybuilder-integration-90/pybuilder_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:33:09.000000 pybuilder-integration-90/pybuilder_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:33:09.000000 pybuilder-integration-90/pybuilder_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 00:33:09.000000 pybuilder-integration-90/pybuilder_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 00:33:09.000000 pybuilder-integration-90/pybuilder_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:33:09.000000 pybuilder-integration-90/pybuilder_integration.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:33:09.091929 pybuilder-integration-90/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-19 00:33:07.000000 pybuilder-integration-90/setup.py
```

### Comparing `pybuilder-integration-89/PKG-INFO` & `pybuilder-integration-90/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 89
+Version: 90
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-89/pybuilder_integration/__init__.py` & `pybuilder-integration-90/pybuilder_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-89/pybuilder_integration/artifact_manager.py` & `pybuilder-integration-90/pybuilder_integration/artifact_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                                          ],
                                          failure_message=f"Failed to find bucket",
                                          log_file_name='s3-head-bucket',
                                          project=project,
                                          reactor=reactor,
                                          logger=logger,
                                          raise_exception=True,
-                                         report=False)
+                                         report=True)
 
 
 artifact_managers: Dict[str, S3ArtifactManager] = {}
 manager = S3ArtifactManager()
 artifact_managers[manager.identifier] = manager
```

### Comparing `pybuilder-integration-89/pybuilder_integration/cloudwatchlogs_utility.py` & `pybuilder-integration-90/pybuilder_integration/cloudwatchlogs_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-89/pybuilder_integration/directory_utility.py` & `pybuilder-integration-90/pybuilder_integration/directory_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-89/pybuilder_integration/exec_utility.py` & `pybuilder-integration-90/pybuilder_integration/exec_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-89/pybuilder_integration/properties.py` & `pybuilder-integration-90/pybuilder_integration/properties.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-89/pybuilder_integration/tasks.py` & `pybuilder-integration-90/pybuilder_integration/tasks.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-89/pybuilder_integration/tool_utility.py` & `pybuilder-integration-90/pybuilder_integration/tool_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-89/pybuilder_integration.egg-info/PKG-INFO` & `pybuilder-integration-90/pybuilder_integration.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 89
+Version: 90
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-89/pybuilder_integration.egg-info/SOURCES.txt` & `pybuilder-integration-90/pybuilder_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-89/setup.py` & `pybuilder-integration-90/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-integration',
-        version = '89',
+        version = '90',
         description = 'A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.',
         long_description = 'A pybuilder plugin that runs integration tests against a target.  This is intended to be a broader scope than unit-tests encompassing dependant functionality.',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```

