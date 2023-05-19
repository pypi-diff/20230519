# Comparing `tmp/Shimarin-0.0.4.tar.gz` & `tmp/Shimarin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimarin-0.0.4.tar", last modified: Fri May 19 20:47:46 2023, max compression
+gzip compressed data, was "Shimarin-0.0.5.tar", last modified: Fri May 19 20:52:18 2023, max compression
```

## Comparing `Shimarin-0.0.4.tar` & `Shimarin-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.218026 Shimarin-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 20:47:46.218026 Shimarin-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 20:47:35.000000 Shimarin-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.214026 Shimarin-0.0.4/Shimarin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.218026 Shimarin-0.0.4/Shimarin/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/client/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.218026 Shimarin-0.0.4/Shimarin/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-19 20:47:35.000000 Shimarin-0.0.4/Shimarin/server/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:47:46.214026 Shimarin-0.0.4/Shimarin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 20:47:46.000000 Shimarin-0.0.4/Shimarin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-19 20:47:35.000000 Shimarin-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-19 20:47:46.218026 Shimarin-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:52:18.662891 Shimarin-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 20:52:18.662891 Shimarin-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 20:52:08.000000 Shimarin-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:52:18.658891 Shimarin-0.0.5/Shimarin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:52:08.000000 Shimarin-0.0.5/Shimarin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:52:18.662891 Shimarin-0.0.5/Shimarin/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:52:08.000000 Shimarin-0.0.5/Shimarin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 20:52:08.000000 Shimarin-0.0.5/Shimarin/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-19 20:52:08.000000 Shimarin-0.0.5/Shimarin/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-19 20:52:08.000000 Shimarin-0.0.5/Shimarin/client/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:52:18.662891 Shimarin-0.0.5/Shimarin/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:52:08.000000 Shimarin-0.0.5/Shimarin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-19 20:52:08.000000 Shimarin-0.0.5/Shimarin/server/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:52:18.658891 Shimarin-0.0.5/Shimarin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 20:52:18.000000 Shimarin-0.0.5/Shimarin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-19 20:52:18.000000 Shimarin-0.0.5/Shimarin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:52:18.000000 Shimarin-0.0.5/Shimarin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:52:18.000000 Shimarin-0.0.5/Shimarin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 20:52:18.000000 Shimarin-0.0.5/Shimarin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-19 20:52:08.000000 Shimarin-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-19 20:52:18.662891 Shimarin-0.0.5/setup.cfg
```

### Comparing `Shimarin-0.0.4/PKG-INFO` & `Shimarin-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.4
+Version: 0.0.5
 Summary: asynchronous event-based communication between client and server
 Home-page: 
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

### Comparing `Shimarin-0.0.4/Shimarin/client/events.py` & `Shimarin-0.0.5/Shimarin/client/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,14 @@
 
     async def start(self, polling_interval: int = 1, fetch: int = 10):
         self.is_polling = True
         while self.is_polling:
             events: Response = await send_get_request(self.session, f"{config.SERVER_ENDPOINT}/events?fetch={fetch}")
             if events.status == 200:
                 event_json = await events.json()
-                if event_json:
-                    print(event_json)
                 for event in event_json:
                     if event_json:
                         event = Event.new(event, self.session)
                         await self.__task_manager(event)
             await asyncio.sleep(polling_interval)
 
     async def __task_manager(self, event: Event):
```

### Comparing `Shimarin-0.0.4/Shimarin/client/networking.py` & `Shimarin-0.0.5/Shimarin/client/networking.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.0.4/Shimarin/server/events.py` & `Shimarin-0.0.5/Shimarin/server/events.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.0.4/Shimarin.egg-info/PKG-INFO` & `Shimarin-0.0.5/Shimarin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.4
+Version: 0.0.5
 Summary: asynchronous event-based communication between client and server
 Home-page: 
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

