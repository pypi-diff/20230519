# Comparing `tmp/dragonfirerequests-0.1.1.tar.gz` & `tmp/dragonfirerequests-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonfirerequests-0.1.1.tar", last modified: Thu May 18 07:19:17 2023, max compression
+gzip compressed data, was "dragonfirerequests-0.2.0.tar", last modified: Fri May 19 06:01:18 2023, max compression
```

## Comparing `dragonfirerequests-0.1.1.tar` & `dragonfirerequests-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 saidkomilmakhamadkhojayev   (501) staff       (20)        0 2023-05-18 07:19:17.087542 dragonfirerequests-0.1.1/
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      944 2023-05-18 07:19:17.087392 dragonfirerequests-0.1.1/PKG-INFO
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      152 2023-05-17 19:46:45.000000 dragonfirerequests-0.1.1/README.md
-drwxr-xr-x   0 saidkomilmakhamadkhojayev   (501) staff       (20)        0 2023-05-18 07:19:17.086316 dragonfirerequests-0.1.1/dragonfirerequests/
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      122 2023-05-18 07:00:17.000000 dragonfirerequests-0.1.1/dragonfirerequests/__init__.py
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)     1773 2023-05-18 07:15:23.000000 dragonfirerequests-0.1.1/dragonfirerequests/dragon.py
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      406 2023-05-18 07:15:23.000000 dragonfirerequests-0.1.1/dragonfirerequests/response.py
-drwxr-xr-x   0 saidkomilmakhamadkhojayev   (501) staff       (20)        0 2023-05-18 07:19:17.087161 dragonfirerequests-0.1.1/dragonfirerequests.egg-info/
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      944 2023-05-18 07:19:17.000000 dragonfirerequests-0.1.1/dragonfirerequests.egg-info/PKG-INFO
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      318 2023-05-18 07:19:17.000000 dragonfirerequests-0.1.1/dragonfirerequests.egg-info/SOURCES.txt
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)        1 2023-05-18 07:19:17.000000 dragonfirerequests-0.1.1/dragonfirerequests.egg-info/dependency_links.txt
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)        9 2023-05-18 07:19:17.000000 dragonfirerequests-0.1.1/dragonfirerequests.egg-info/requires.txt
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)       19 2023-05-18 07:19:17.000000 dragonfirerequests-0.1.1/dragonfirerequests.egg-info/top_level.txt
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)       38 2023-05-18 07:19:17.087591 dragonfirerequests-0.1.1/setup.cfg
--rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)     1413 2023-05-18 06:36:46.000000 dragonfirerequests-0.1.1/setup.py
+drwxr-xr-x   0 saidkomilmakhamadkhojayev   (501) staff       (20)        0 2023-05-19 06:01:18.897302 dragonfirerequests-0.2.0/
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      944 2023-05-19 06:01:18.897128 dragonfirerequests-0.2.0/PKG-INFO
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      152 2023-05-17 19:46:45.000000 dragonfirerequests-0.2.0/README.md
+drwxr-xr-x   0 saidkomilmakhamadkhojayev   (501) staff       (20)        0 2023-05-19 06:01:18.895822 dragonfirerequests-0.2.0/dragonfirerequests/
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      122 2023-05-18 07:00:17.000000 dragonfirerequests-0.2.0/dragonfirerequests/__init__.py
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)     2207 2023-05-19 05:49:28.000000 dragonfirerequests-0.2.0/dragonfirerequests/dragon.py
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      370 2023-05-19 05:49:52.000000 dragonfirerequests-0.2.0/dragonfirerequests/response.py
+drwxr-xr-x   0 saidkomilmakhamadkhojayev   (501) staff       (20)        0 2023-05-19 06:01:18.896888 dragonfirerequests-0.2.0/dragonfirerequests.egg-info/
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      944 2023-05-19 06:01:18.000000 dragonfirerequests-0.2.0/dragonfirerequests.egg-info/PKG-INFO
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)      318 2023-05-19 06:01:18.000000 dragonfirerequests-0.2.0/dragonfirerequests.egg-info/SOURCES.txt
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)        1 2023-05-19 06:01:18.000000 dragonfirerequests-0.2.0/dragonfirerequests.egg-info/dependency_links.txt
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)        9 2023-05-19 06:01:18.000000 dragonfirerequests-0.2.0/dragonfirerequests.egg-info/requires.txt
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)       19 2023-05-19 06:01:18.000000 dragonfirerequests-0.2.0/dragonfirerequests.egg-info/top_level.txt
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)       38 2023-05-19 06:01:18.897352 dragonfirerequests-0.2.0/setup.cfg
+-rw-r--r--   0 saidkomilmakhamadkhojayev   (501) staff       (20)     1413 2023-05-19 06:01:16.000000 dragonfirerequests-0.2.0/setup.py
```

### Comparing `dragonfirerequests-0.1.1/PKG-INFO` & `dragonfirerequests-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfirerequests
-Version: 0.1.1
+Version: 0.2.0
 Summary: Requests runner library
 Home-page: https://SaidkomilMS.t.me/
 Author: Saidkomil Makhamadkhojayev
 Author-email: msaidkomils@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dragonfirerequests-0.1.1/dragonfirerequests/dragon.py` & `dragonfirerequests-0.2.0/dragonfirerequests/dragon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 from typing import Any, Iterable
 
 import requests
 
 from dragonfirerequests.response import DragonResponse
 
 
+def _make_string(response):
+    return f'\n\tRequest: {response.request.body.decode()}\n'\
+           f'\tResponse: {response.content.decode()}'
+
+
 class Dragon:
     __base_url: str
     __response_content_type: str
     __logger: Any
     __logger_method: str
     __headers: dict
 
     def __init__(self, base_url: str, *, response_content_type: str = "json", logger: Any = None,
-                 logger_method: str = None, headers: dict = None):
+                 logger_method: str = "info", headers: dict = None):
         if headers is None:
             headers = dict()
         self.__base_url = base_url
         self.__response_content_type = response_content_type
         self.__logger = logger
         self.__logger_method = logger_method
         self.__headers = headers
 
     def update_headers(self, new_headers: dict):
         self.__headers.update(new_headers)
 
+    def __log(self, response: requests.Response):
+        string_to_log = _make_string(response)
+        log = getattr(self.__logger, self.__logger_method, print)
+        try:
+            log(string_to_log)
+        except Exception as e:
+            print(e)
+
     def fire(self, method: str, url: str = "", **kwargs) -> DragonResponse:
+        # TODO: Durations
         headers = self.__headers | kwargs.get('headers', dict())
         kwargs['headers'] = headers
         response: requests.Response = requests.request(method, self.__base_url + url, **kwargs)
         success = True
         if self.__logger is not None:
-            pass  # TODO: Logging
+            self.__log(response)
         if self.__response_content_type == 'json':
             try:
                 data = response.json()
             except requests.JSONDecodeError:
                 data = {}
                 success = False
             return DragonResponse(response, data, success, response.request)
```

### Comparing `dragonfirerequests-0.1.1/dragonfirerequests.egg-info/PKG-INFO` & `dragonfirerequests-0.2.0/dragonfirerequests.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfirerequests
-Version: 0.1.1
+Version: 0.2.0
 Summary: Requests runner library
 Home-page: https://SaidkomilMS.t.me/
 Author: Saidkomil Makhamadkhojayev
 Author-email: msaidkomils@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dragonfirerequests-0.1.1/setup.py` & `dragonfirerequests-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="dragonfirerequests",
-    version="0.1.1",
+    version="0.2.0",
     description="Requests runner library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://SaidkomilMS.t.me/",
     author="Saidkomil Makhamadkhojayev",
     author_email="msaidkomils@gmail.com",
     license="MIT",
```

