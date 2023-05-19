# Comparing `tmp/taskiq_aiohttp-0.1.2.tar.gz` & `tmp/taskiq_aiohttp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aiohttp-0.1.2.tar", max compression
+gzip compressed data, was "taskiq_aiohttp-0.1.3.tar", max compression
```

## Comparing `taskiq_aiohttp-0.1.2.tar` & `taskiq_aiohttp-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/LICENSE
--rw-r--r--   0        0        0     1067 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/README.md
--rw-r--r--   0        0        0     1716 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      106 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/taskiq_aiohttp/__init__.py
--rw-r--r--   0        0        0     4023 2023-05-11 12:40:45.933492 taskiq_aiohttp-0.1.2/taskiq_aiohttp/initializer.py
--rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-19 00:42:43.563116 taskiq_aiohttp-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2780 2023-05-19 00:42:43.563116 taskiq_aiohttp-0.1.3/README.md
+-rw-r--r--   0        0        0     1716 2023-05-19 00:42:43.567116 taskiq_aiohttp-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-05-19 00:42:43.567116 taskiq_aiohttp-0.1.3/taskiq_aiohttp/__init__.py
+-rw-r--r--   0        0        0     4469 2023-05-19 00:42:43.567116 taskiq_aiohttp-0.1.3/taskiq_aiohttp/initializer.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:42:43.567116 taskiq_aiohttp-0.1.3/taskiq_aiohttp/py.typed
+-rw-r--r--   0        0        0     4098 1970-01-01 00:00:00.000000 taskiq_aiohttp-0.1.3/PKG-INFO
```

### Comparing `taskiq_aiohttp-0.1.2/LICENSE` & `taskiq_aiohttp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aiohttp-0.1.2/pyproject.toml` & `taskiq_aiohttp-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "taskiq-aiohttp"
 description = "Taskiq integration with AioHTTP framework"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_aiohttp-0.1.2/taskiq_aiohttp/initializer.py` & `taskiq_aiohttp-0.1.3/taskiq_aiohttp/initializer.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,72 @@
 from aiohttp.web_request import RawRequestMessage
 from aiohttp.web_urldispatcher import SystemRoute, UrlMappingMatchInfo
 from multidict import CIMultiDict, CIMultiDictProxy
 from taskiq import AsyncBroker, TaskiqEvents, TaskiqState
 from taskiq.cli.utils import import_object
 
 
+def populate_context(
+    broker: AsyncBroker,
+    server: web.Server,
+    app: web.Application,
+    loop: asyncio.AbstractEventLoop,
+) -> None:
+    """
+    Function to add dependency context.
+
+    This function adds base dependency,
+    that you may need while working with AioHTTP application.
+
+    :param broker: current broker.
+    :param server: current server that handles requests.
+    :param app: your application.
+    :param loop: current event loop.
+    """
+    handler = RequestHandler(server, loop=loop)
+    handler.transport = asyncio.Transport()
+    request = web.Request(
+        RawRequestMessage(
+            "GET",
+            "/",
+            HttpVersion10,
+            headers=CIMultiDictProxy(CIMultiDict()),
+            raw_headers=(),
+            should_close=False,
+            upgrade=False,
+            chunked=False,
+            compression=None,
+            url=yarl.URL.build(
+                scheme="https",
+                host="test.com",
+                path="/",
+            ),
+        ),
+        None,
+        handler,
+        None,
+        None,
+        None,
+    )
+
+    request._match_info = UrlMappingMatchInfo(
+        match_dict={},
+        route=SystemRoute(web.HTTPBadRequest()),
+    )
+    request._match_info._apps = app._subapps
+    request._match_info._current_app = app
+
+    broker.add_dependency_context(
+        {
+            web.Application: app,
+            web.Request: request,
+        },
+    )
+
+
 def startup_event_generator(
     broker: AsyncBroker,
     app_path: str,
     app: Any,
 ) -> Callable[[TaskiqState], Awaitable[None]]:
     """
     Creates an event to run on broker's startup.
@@ -31,16 +89,14 @@
     :param app_path: path to the application.
     :param app: current application or a fractory.
 
     :returns: a function that is called on startup.
     """
 
     async def startup(state: TaskiqState) -> None:
-        loop = asyncio.get_event_loop()
-
         local_app = app
 
         if not isinstance(local_app, web.Application):
             local_app = local_app()
 
         if inspect.iscoroutine(local_app):
             local_app = await local_app
@@ -50,55 +106,24 @@
         # Starting the application.
         app_runner = web.AppRunner(local_app)
         await app_runner.setup()
 
         if app_runner.server is None:
             raise ValueError("Cannot construct aiohttp app to mock requests")
 
-        # Creating mocked request
-        handler = RequestHandler(app_runner.server, loop=loop)
-        handler.transport = asyncio.Transport()
-        request = web.Request(
-            RawRequestMessage(
-                "GET",
-                "/",
-                HttpVersion10,
-                headers=CIMultiDictProxy(CIMultiDict()),
-                raw_headers=(),
-                should_close=False,
-                upgrade=False,
-                chunked=False,
-                compression=None,
-                url=yarl.URL.build(
-                    scheme="https",
-                    host="test.com",
-                    path="/",
-                ),
-            ),
-            None,
-            handler,
-            None,
-            None,
-            None,
-        )
-
-        request._match_info = UrlMappingMatchInfo(
-            match_dict={},
-            route=SystemRoute(web.HTTPBadRequest()),
-        )
-        request._match_info._apps = local_app._subapps
-        request._match_info._current_app = local_app
+        loop = asyncio.get_running_loop()
 
-        broker.add_dependency_context(
-            {
-                web.Application: local_app,
-                web.Request: request,
-            },
+        populate_context(
+            broker=broker,
+            server=app_runner.server,
+            app=local_app,
+            loop=loop,
         )
 
+        # Creating mocked request
         state.aiohttp_runner = app_runner
         local_app.router._resources = []
 
     return startup
 
 
 async def shutdown(state: TaskiqState) -> None:
```

