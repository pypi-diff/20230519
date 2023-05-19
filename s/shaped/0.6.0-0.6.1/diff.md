# Comparing `tmp/shaped-0.6.0.tar.gz` & `tmp/shaped-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/io/dist/.tmp-4iecjmto/shaped-0.6.0.tar", last modified: Wed Mar 29 21:25:03 2023, max compression
+gzip compressed data, was "/io/dist/.tmp-hczybsli/shaped-0.6.1.tar", last modified: Fri May 19 21:06:41 2023, max compression
```

## Comparing `shaped-0.6.0.tar` & `shaped-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 21:25:03.000000 shaped-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     2474 2023-03-29 21:25:03.000000 shaped-0.6.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1936 2023-03-29 21:24:24.000000 shaped-0.6.0/README.md
--rwxrwxr-x   0 root         (0) root         (0)       81 2023-03-29 21:24:24.000000 shaped-0.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 21:25:03.000000 shaped-0.6.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1254 2023-03-29 21:24:24.000000 shaped-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 21:25:03.000000 shaped-0.6.0/shaped.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2474 2023-03-29 21:25:03.000000 shaped-0.6.0/shaped.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      274 2023-03-29 21:25:03.000000 shaped-0.6.0/shaped.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 21:25:03.000000 shaped-0.6.0/shaped.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-03-29 21:25:03.000000 shaped-0.6.0/shaped.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-03-29 21:25:03.000000 shaped-0.6.0/shaped.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-29 21:25:03.000000 shaped-0.6.0/shaped.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 21:25:02.000000 shaped-0.6.0/shaped.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 21:25:03.000000 shaped-0.6.0/src/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 21:24:24.000000 shaped-0.6.0/src/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7734 2023-03-29 21:24:24.000000 shaped-0.6.0/src/shaped_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:41.000000 shaped-0.6.1/
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-19 21:06:41.000000 shaped-0.6.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1936 2023-05-19 21:06:12.000000 shaped-0.6.1/README.md
+-rwxrwxr-x   0 root         (0) root         (0)       81 2023-05-19 21:06:12.000000 shaped-0.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 21:06:41.000000 shaped-0.6.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1254 2023-05-19 21:06:12.000000 shaped-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:41.000000 shaped-0.6.1/shaped.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-19 21:06:41.000000 shaped-0.6.1/shaped.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-19 21:06:41.000000 shaped-0.6.1/shaped.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 21:06:41.000000 shaped-0.6.1/shaped.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-19 21:06:41.000000 shaped-0.6.1/shaped.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 21:06:41.000000 shaped-0.6.1/shaped.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-19 21:06:41.000000 shaped-0.6.1/shaped.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 21:06:41.000000 shaped-0.6.1/shaped.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:41.000000 shaped-0.6.1/src/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 21:06:12.000000 shaped-0.6.1/src/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7979 2023-05-19 21:06:12.000000 shaped-0.6.1/src/shaped_cli.py
```

### Comparing `shaped-0.6.0/PKG-INFO` & `shaped-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaped
-Version: 0.6.0
+Version: 0.6.1
 Summary: A CLI tool for interacting with the Shaped API.
 Home-page: https://github.com/shaped-ai/shaped-cli
 Author: Shaped Team
 Author-email: support@shaped.ai
 Keywords: shaped-ai
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `shaped-0.6.0/README.md` & `shaped-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `shaped-0.6.0/setup.py` & `shaped-0.6.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
-version = "0.6.0"
+version = "0.6.1"
 circleci_build_number = os.getenv("CIRCLE_BUILD_NUM", "")
 if circleci_build_number != "":
     version = f"{version}.dev{circleci_build_number}"
 
 setup(
     name="shaped",
     version=version,
```

### Comparing `shaped-0.6.0/shaped.egg-info/PKG-INFO` & `shaped-0.6.1/shaped.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaped
-Version: 0.6.0
+Version: 0.6.1
 Summary: A CLI tool for interacting with the Shaped API.
 Home-page: https://github.com/shaped-ai/shaped-cli
 Author: Shaped Team
 Author-email: support@shaped.ai
 Keywords: shaped-ai
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `shaped-0.6.0/src/shaped_cli.py` & `shaped-0.6.1/src/shaped_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,24 +119,27 @@
 
 @app.command()
 def rank(
     model_name: str = typer.Option(...),
     user_id: str = typer.Option(...),
     limit=typer.Option(15),
     retrieval_query=typer.Option(None),
-    with_metadata: bool = typer.Option(False),
+    return_metadata: bool = typer.Option(False),
+    exploration_factor: float = typer.Option(0.0),
 ):
     config = _read_config()
     url = f"{_get_shaped_url(config)}/models/{model_name}/rank"
     headers = {"accept": "application/json", "x-api-key": config.api_key}
-    query_args = {}
+    if exploration_factor < 0.0 or exploration_factor > 1.0:
+        raise typer.BadParameter("`exploration_factor` must be between 0.0 and 1.0")
+    query_args = {"exploration_factor": exploration_factor}
     if retrieval_query is not None:
         query_args |= {"retrieval": json.loads(retrieval_query)}
-    if with_metadata:
-        query_args |= {"with_metadata": bool(with_metadata)}
+    if return_metadata:
+        query_args |= {"return_metadata": bool(return_metadata)}
 
     response = requests.post(
         url,
         headers=headers,
         json={"user_id": user_id, "limit": str(limit), **query_args},
     )
     typer.echo(_parse_response_as_yaml(response.text))
```

