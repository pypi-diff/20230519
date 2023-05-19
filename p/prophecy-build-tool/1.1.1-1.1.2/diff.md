# Comparing `tmp/prophecy-build-tool-1.1.1.tar.gz` & `tmp/prophecy-build-tool-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prophecy-build-tool/prophecy-build-tool/dist/.tmp-3as3mteb/prophecy-build-tool-1.1.1.tar", last modified: Wed May 17 09:23:57 2023, max compression
+gzip compressed data, was "/home/runner/work/prophecy-build-tool/prophecy-build-tool/dist/.tmp-ykce7y69/prophecy-build-tool-1.1.2.tar", last modified: Fri May 19 07:27:35 2023, max compression
```

## Comparing `prophecy-build-tool-1.1.1.tar` & `prophecy-build-tool-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/pbt/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/src/pbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/src/pbt/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    37709 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/src/pbt/prophecy_build_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/test/test_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/pbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/src/pbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/src/pbt/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38325 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/src/pbt/prophecy_build_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/test/test_deploy.py
```

### Comparing `prophecy-build-tool-1.1.1/LICENSE` & `prophecy-build-tool-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.1/PKG-INFO` & `prophecy-build-tool-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.1
+Version: 1.1.2
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.1/README.md` & `prophecy-build-tool-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.1/setup.py` & `prophecy-build-tool-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool",
-    version="1.1.1",
+    version="1.1.2",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
     "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
```

### Comparing `prophecy-build-tool-1.1.1/src/pbt/__init__.py` & `prophecy-build-tool-1.1.2/src/pbt/__init__.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.1/src/pbt/process.py` & `prophecy-build-tool-1.1.2/src/pbt/process.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.1/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-1.1.2/src/pbt/prophecy_build_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from databricks_cli.configure.config import _get_api_client
 from databricks_cli.configure.provider import EnvironmentVariableConfigProvider
 from databricks_cli.sdk import DbfsService, JobsService
 from requests import HTTPError
 from rich import print
 
 from .process import Process
+import tempfile
 
 
 class ProphecyBuildTool:
     def __init__(
         self,
         path_root: str,
         dependent_projects_path: str = "",
@@ -317,14 +318,24 @@
                     continue
                 else:
                     print("[DEPLOY]: Job being deployed for fabric id: %s" % fabric_id)
 
             generate_pipeline_config_from_pipeline_component = False
 
             for component in components:
+                if "ScriptComponent" in component:
+                    script_component = component["ScriptComponent"]
+                    content = script_component["content"]
+                    path = script_component["path"]
+                    temp_file = tempfile.NamedTemporaryFile(delete=False)
+                    temp_file.write(content.encode('ascii'))
+                    temp_file.close()
+                    print(f"Uploading script to path: {path}")
+                    self.dbfs_service.put(path, overwrite=True, src_path=temp_file.name)
+                    os.unlink(temp_file.name)
                 if "PipelineComponent" in component:
                     pipeline_component = component["PipelineComponent"]
                     if "pipelineId" in pipeline_component:
                         pipeline_uri = pipeline_component["pipelineId"]
                     else:
                         pipeline_uri = pipeline_component["id"]
```

### Comparing `prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/PKG-INFO` & `prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.1
+Version: 1.1.2
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.1/test/test_build.py` & `prophecy-build-tool-1.1.2/test/test_build.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.1/test/test_deploy.py` & `prophecy-build-tool-1.1.2/test/test_deploy.py`

 * *Files identical despite different names*

