# Comparing `tmp/vedro-replay-0.1.2.tar.gz` & `tmp/vedro-replay-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-replay-0.1.2.tar", last modified: Thu Dec  8 07:25:17 2022, max compression
+gzip compressed data, was "vedro-replay-0.1.3.tar", last modified: Fri May 19 14:00:34 2023, max compression
```

## Comparing `vedro-replay-0.1.2.tar` & `vedro-replay-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 07:25:17.463320 vedro-replay-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      548 2022-12-08 07:25:17.463320 vedro-replay-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 07:25:17.463320 vedro-replay-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      919 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 07:25:17.459320 vedro-replay-0.1.2/vedro_replay/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/excluder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 07:25:17.463320 vedro-replay-0.1.2/vedro_replay/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/templates/contexts.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/templates/helper_method.j2
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/templates/helpers.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      308 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/templates/interfaces.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/templates/scenario.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      227 2022-12-08 07:25:07.000000 vedro-replay-0.1.2/vedro_replay/templates/vedro.cfg.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 07:25:17.459320 vedro-replay-0.1.2/vedro_replay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2022-12-08 07:25:17.000000 vedro-replay-0.1.2/vedro_replay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-08 07:25:17.000000 vedro-replay-0.1.2/vedro_replay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 07:25:17.000000 vedro-replay-0.1.2/vedro_replay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-08 07:25:17.000000 vedro-replay-0.1.2/vedro_replay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-08 07:25:17.000000 vedro-replay-0.1.2/vedro_replay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-08 07:25:17.000000 vedro-replay-0.1.2/vedro_replay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:00:34.750037 vedro-replay-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-19 14:00:34.750037 vedro-replay-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-19 14:00:34.750037 vedro-replay-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:00:34.746037 vedro-replay-0.1.3/vedro_replay/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/excluder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:00:34.750037 vedro-replay-0.1.3/vedro_replay/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/templates/config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/templates/contexts.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/templates/helper_method.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/templates/helpers.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/templates/interfaces.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/templates/scenario.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-19 14:00:22.000000 vedro-replay-0.1.3/vedro_replay/templates/vedro.cfg.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:00:34.750037 vedro-replay-0.1.3/vedro_replay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-19 14:00:34.000000 vedro-replay-0.1.3/vedro_replay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-19 14:00:34.000000 vedro-replay-0.1.3/vedro_replay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:00:34.000000 vedro-replay-0.1.3/vedro_replay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 14:00:34.000000 vedro-replay-0.1.3/vedro_replay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-19 14:00:34.000000 vedro-replay-0.1.3/vedro_replay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 14:00:34.000000 vedro-replay-0.1.3/vedro_replay.egg-info/top_level.txt
```

### Comparing `vedro-replay-0.1.2/LICENSE` & `vedro-replay-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-replay-0.1.2/setup.py` & `vedro-replay-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 def find_required():
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-replay",
-    version="0.1.2",
+    version="0.1.3",
     description="vedro-replay package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    author="2GIS Test Labs",
-    author_email="test-labs@2gis.ru",
+    author="Konstantin Shefer",
+    author_email="kostya.shefer.999@gmail.com",
     python_requires=">=3.9",
-    url="https://github.com/2gis-test-labs/vedro-replay",
+    url="https://github.com/kvs8/vedro-replay",
     license="Apache-2.0",
     packages=['vedro_replay'],
     install_requires=find_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     entry_points={
         "console_scripts": [
-            "vedro-replay-generate = vedro_replay:generation",
+            "vedro-replay = vedro_replay:command",
         ],
     },
     include_package_data=True,
 )
```

### Comparing `vedro-replay-0.1.2/vedro_replay/excluder.py` & `vedro-replay-0.1.3/vedro_replay/excluder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import re
 from copy import deepcopy
-from typing import List
+from typing import Any, Dict, List
 
 from vedro_replay.response import Response
 
 
 class Excluder:
     @staticmethod
-    def excludes_headers(excludes: list, headers: dict):
+    def excludes_headers(excludes: List[Any], headers: Dict[str, str]) -> None:
         for exclude in excludes:
             if exclude in headers.keys():
                 del headers[exclude]
 
     @classmethod
-    def exclude_by_several_path(cls, excluded_paths: list, data: dict):
+    def exclude_by_several_path(cls, excluded_paths: List[Any], data: Dict[str, Any]) -> None:
         for excluded_path in excluded_paths:
             cls.exclude_by_path(data=data, excluded_path=excluded_path)
 
     @classmethod
-    def exclude_by_path(cls, data: dict, excluded_path):
+    def exclude_by_path(cls, data: Dict[str, Any], excluded_path: str) -> None:
         if isinstance(excluded_path, str):
             cls.exclude(
                 data=data,
                 excluded_path=excluded_path.split('.'),
                 reg_for_exclude=''
             )
         elif isinstance(excluded_path, dict):
@@ -30,35 +30,37 @@
                 cls.exclude(
                     data=data,
                     excluded_path=key.split('.'),
                     reg_for_exclude=excluded_path[key]
                 )
 
     @classmethod
-    def exclude(cls, data, excluded_path: list, reg_for_exclude: str):
+    def exclude(cls, data: Dict[str, Any], excluded_path: List[str], reg_for_exclude: str) -> None:
         current_path_part = excluded_path[0]
         excluded_path.pop(0)
 
         if len(excluded_path) == 0:
             if current_path_part in data.keys():
                 if reg_for_exclude != '':
-                    data[current_path_part] = re.search(reg_for_exclude, data[current_path_part])[0]
+                    value = re.search(reg_for_exclude, data[current_path_part])
+                    if value is not None:
+                        data[current_path_part] = value[0]
                 else:
                     del data[current_path_part]
             return
 
         if isinstance(data, list) and current_path_part == '*':
             for elem in data:
                 cls.exclude(elem, deepcopy(excluded_path), reg_for_exclude)
         else:
             if isinstance(data, dict) and current_path_part in data.keys():
                 cls.exclude(data[current_path_part], deepcopy(excluded_path), reg_for_exclude)
 
 
-def filter_response(response: Response, exclude_headers: List, exclude_body: List) -> Response:
+def filter_response(response: Response, exclude_headers: List[Any], exclude_body: List[Any]) -> Response:
     Excluder.excludes_headers(exclude_headers, response.headers)
     if isinstance(response.body, list):
         for part in response.body:
             Excluder.exclude_by_several_path(exclude_body, part)
     else:
         Excluder.exclude_by_several_path(exclude_body, response.body)
     return response
```

### Comparing `vedro-replay-0.1.2/vedro_replay/templates/scenario.py.j2` & `vedro-replay-0.1.3/vedro_replay/templates/scenario.py.j2`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import vedro
-from vedro_replay import replay
+from contexts.api import golden_response, testing_response
 from d42 import from_native
+from helpers.helpers import {{helper_method_name}}
 
-from contexts.api import golden_response, testing_response
-from helpers.helpers import {{context_method_name}}
+from vedro_replay import replay
 
 
 class Scenario(vedro.Scenario):
     subject = "do request: {{api_route}}"
 
-    @replay("requests/{{file_requests}}")
+    @replay("{{path_requests}}/{{file_requests}}")
     def __init__(self, request):
         self.request = request
 
     async def given_golden_response(self):
-        self.golden_response = await golden_response(self.request, {{context_method_name}})
+        self.golden_response = await golden_response(self.request, {{helper_method_name}})
 
     async def when_user_sends_request(self):
-        self.testing_response = await testing_response(self.request, {{context_method_name}})
+        self.testing_response = await testing_response(self.request, {{helper_method_name}})
 
     def then_it_should_return_same_status(self):
-        assert self.golden_response.status == self.testing_response.status
+        assert self.testing_response.status == self.golden_response.status
 
     def and_it_should_return_same_headers(self):
-        assert from_native(self.golden_response.headers) == self.testing_response.headers
+        assert self.testing_response.headers == from_native(self.golden_response.headers)
 
     def and_it_should_return_same_body(self):
-        assert from_native(self.golden_response.body) == self.testing_response.body
+        assert self.testing_response.body == from_native(self.golden_response.body)
```

### Comparing `vedro-replay-0.1.2/vedro_replay.egg-info/SOURCES.txt` & `vedro-replay-0.1.3/vedro_replay.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 vedro_replay/__init__.py
-vedro_replay/config.py
+vedro_replay/command.py
 vedro_replay/excluder.py
 vedro_replay/generator.py
 vedro_replay/replay.py
 vedro_replay/request.py
 vedro_replay/response.py
 vedro_replay.egg-info/PKG-INFO
 vedro_replay.egg-info/SOURCES.txt
 vedro_replay.egg-info/dependency_links.txt
 vedro_replay.egg-info/entry_points.txt
 vedro_replay.egg-info/requires.txt
 vedro_replay.egg-info/top_level.txt
+vedro_replay/templates/config.py.j2
 vedro_replay/templates/contexts.py.j2
 vedro_replay/templates/helper_method.j2
 vedro_replay/templates/helpers.py.j2
 vedro_replay/templates/interfaces.py.j2
 vedro_replay/templates/scenario.py.j2
 vedro_replay/templates/vedro.cfg.py.j2
```

