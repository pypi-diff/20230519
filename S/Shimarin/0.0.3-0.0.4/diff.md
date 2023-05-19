# Comparing `tmp/Shimarin-0.0.3.tar.gz` & `tmp/Shimarin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimarin-0.0.3.tar", last modified: Wed May  3 11:53:55 2023, max compression
+gzip compressed data, was "Shimarin-0.0.4.tar", last modified: Fri May 19 20:47:46 2023, max compression
```

## Comparing `Shimarin-0.0.3.tar` & `Shimarin-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:53:55.463367 Shimarin-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-03 11:53:55.463367 Shimarin-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-03 11:53:44.000000 Shimarin-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:53:55.459367 Shimarin-0.0.3/Shimarin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 11:53:44.000000 Shimarin-0.0.3/Shimarin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:53:55.463367 Shimarin-0.0.3/Shimarin/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 11:53:44.000000 Shimarin-0.0.3/Shimarin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-03 11:53:44.000000 Shimarin-0.0.3/Shimarin/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-03 11:53:44.000000 Shimarin-0.0.3/Shimarin/client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-03 11:53:44.000000 Shimarin-0.0.3/Shimarin/client/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:53:55.463367 Shimarin-0.0.3/Shimarin/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 11:53:44.000000 Shimarin-0.0.3/Shimarin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-03 11:53:44.000000 Shimarin-0.0.3/Shimarin/server/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:53:55.459367 Shimarin-0.0.3/Shimarin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-03 11:53:55.000000 Shimarin-0.0.3/Shimarin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-03 11:53:55.000000 Shimarin-0.0.3/Shimarin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:53:55.000000 Shimarin-0.0.3/Shimarin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:53:55.000000 Shimarin-0.0.3/Shimarin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 11:53:55.000000 Shimarin-0.0.3/Shimarin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 11:53:44.000000 Shimarin-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 11:53:55.463367 Shimarin-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.218026 Shimarin-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 20:47:46.218026 Shimarin-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 20:47:35.000000 Shimarin-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.214026 Shimarin-0.0.4/Shimarin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.218026 Shimarin-0.0.4/Shimarin/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/client/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.218026 Shimarin-0.0.4/Shimarin/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/server/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.214026 Shimarin-0.0.4/Shimarin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-19 20:47:35.000000 Shimarin-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-19 20:47:46.218026 Shimarin-0.0.4/setup.cfg
```

### Comparing `Shimarin-0.0.3/PKG-INFO` & `Shimarin-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.3
+Version: 0.0.4
 Summary: asynchronous event-based communication between client and server
 Home-page: 
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

### Comparing `Shimarin-0.0.3/Shimarin/client/events.py` & `Shimarin-0.0.4/Shimarin/client/events.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.0.3/Shimarin/client/networking.py` & `Shimarin-0.0.4/Shimarin/client/networking.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,14 @@
     :session A client session object from aiohttp
     :param *args and *kwargs to be used on the request
     :return a Response object with the content of the endpoint
     """
     response: typing.Union[Response, None] = None
     async with session.request("GET", *args, **kwargs) as resp:
         response = Response(resp.status, await resp.read())
-        if response.status != 200:
-            print(response.content)
     return response
 
 
 async def send_post_request(session: aiohttp.ClientSession, *args, **kwargs) -> Response:
     """
     Function to send a rest request and return the Response
     :session A client session object from aiohttp
```

### Comparing `Shimarin-0.0.3/Shimarin/server/events.py` & `Shimarin-0.0.4/Shimarin/server/events.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.0.3/Shimarin.egg-info/PKG-INFO` & `Shimarin-0.0.4/Shimarin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.3
+Version: 0.0.4
 Summary: asynchronous event-based communication between client and server
 Home-page: 
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

