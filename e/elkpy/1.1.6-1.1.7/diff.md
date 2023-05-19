# Comparing `tmp/elkpy-1.1.6.tar.gz` & `tmp/elkpy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkpy-1.1.6.tar", last modified: Mon May 15 14:50:26 2023, max compression
+gzip compressed data, was "elkpy-1.1.7.tar", last modified: Fri May 19 04:56:58 2023, max compression
```

## Comparing `elkpy-1.1.6.tar` & `elkpy-1.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-15 14:50:26.035057 elkpy-1.1.6/
--rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.6/COPYING
--rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.6/LICENSE
--rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-15 14:50:26.035155 elkpy-1.1.6/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.6/README.md
--rw-r--r--   0 max        (501) staff       (20)      757 2023-05-15 14:48:54.000000 elkpy-1.1.6/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)      368 2023-05-15 14:50:26.035419 elkpy-1.1.6/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.6/setup.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-15 14:50:26.029260 elkpy-1.1.6/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-15 14:50:26.034355 elkpy-1.1.6/src/elkpy/
--rw-r--r--   0 max        (501) staff       (20)        0 2023-03-30 13:21:26.000000 elkpy-1.1.6/src/elkpy/__init__.py
--rw-r--r--   0 max        (501) staff       (20)    19397 2023-05-15 12:31:59.000000 elkpy-1.1.6/src/elkpy/audiographcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     9934 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/audioroutingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    16365 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/cvgatecontroller.py
--rw-r--r--   0 max        (501) staff       (20)     1989 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/grpc_gen.py
--rw-r--r--   0 max        (501) staff       (20)     8021 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/keyboardcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    19656 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/midicontroller.py
--rw-r--r--   0 max        (501) staff       (20)    16178 2023-04-14 14:06:32.000000 elkpy-1.1.6/src/elkpy/notificationcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     5032 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/osccontroller.py
--rw-r--r--   0 max        (501) staff       (20)    15841 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/parametercontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6506 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/programcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     3056 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/sessioncontroller.py
--rw-r--r--   0 max        (501) staff       (20)    22973 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/sushi_info_types.py
--rw-r--r--   0 max        (501) staff       (20)     6191 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/sushicontroller.py
--rw-r--r--   0 max        (501) staff       (20)     2143 2023-04-13 14:13:40.000000 elkpy-1.1.6/src/elkpy/sushierrors.py
--rw-r--r--   0 max        (501) staff       (20)     9701 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/sushiprocessor.py
--rw-r--r--   0 max        (501) staff       (20)     3024 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/systemcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6641 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/timingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     7011 2023-03-30 13:19:14.000000 elkpy-1.1.6/src/elkpy/transportcontroller.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-15 14:50:26.034948 elkpy-1.1.6/src/elkpy.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      790 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       29 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        6 2023-05-15 14:50:26.000000 elkpy-1.1.6/src/elkpy.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-19 04:56:58.181955 elkpy-1.1.7/
+-rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.7/COPYING
+-rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.7/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-19 04:56:58.182009 elkpy-1.1.7/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.7/README.md
+-rw-r--r--   0 max        (501) staff       (20)      757 2023-05-19 04:55:44.000000 elkpy-1.1.7/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)      352 2023-05-19 04:56:58.182226 elkpy-1.1.7/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.7/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-19 04:56:58.176044 elkpy-1.1.7/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-19 04:56:58.181303 elkpy-1.1.7/src/elkpy/
+-rw-r--r--   0 max        (501) staff       (20)        0 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    19397 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/audiographcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     9934 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/audioroutingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16365 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/cvgatecontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     1989 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/grpc_gen.py
+-rw-r--r--   0 max        (501) staff       (20)     8021 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/keyboardcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    19656 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/midicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16458 2023-05-19 04:52:31.000000 elkpy-1.1.7/src/elkpy/notificationcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     5032 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/osccontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    15841 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/parametercontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6506 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/programcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     3056 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/sessioncontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    22973 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/sushi_info_types.py
+-rw-r--r--   0 max        (501) staff       (20)     6148 2023-05-19 04:53:24.000000 elkpy-1.1.7/src/elkpy/sushicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     2143 2023-05-19 04:42:11.000000 elkpy-1.1.7/src/elkpy/sushierrors.py
+-rw-r--r--   0 max        (501) staff       (20)     9701 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/sushiprocessor.py
+-rw-r--r--   0 max        (501) staff       (20)     3024 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/systemcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6641 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/timingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     7011 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/transportcontroller.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-19 04:56:58.181862 elkpy-1.1.7/src/elkpy.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      790 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       29 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        6 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/top_level.txt
```

### Comparing `elkpy-1.1.6/COPYING` & `elkpy-1.1.7/COPYING`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/LICENSE` & `elkpy-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/PKG-INFO` & `elkpy-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.1.6
+Version: 1.1.7
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elkpy-1.1.6/README.md` & `elkpy-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/pyproject.toml` & `elkpy-1.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elkpy"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="Maxime Gendebien", email="max@elk.audio" },
   { name="Ruben Svensson", email="ruben@elk.audio" },
 ]
 description = "A basic controller for sushi using gRPC"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `elkpy-1.1.6/src/elkpy/audiographcontroller.py` & `elkpy-1.1.7/src/elkpy/audiographcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/audioroutingcontroller.py` & `elkpy-1.1.7/src/elkpy/audioroutingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/cvgatecontroller.py` & `elkpy-1.1.7/src/elkpy/cvgatecontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/grpc_gen.py` & `elkpy-1.1.7/src/elkpy/grpc_gen.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/keyboardcontroller.py` & `elkpy-1.1.7/src/elkpy/keyboardcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/midicontroller.py` & `elkpy-1.1.7/src/elkpy/midicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/notificationcontroller.py` & `elkpy-1.1.7/src/elkpy/notificationcontroller.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License along with elkpy.  If
     not, see <http://www.gnu.org/licenses/>.
 """
 __license__ = "GPL-3.0"
 
+import time
+
 import grpc.experimental.aio
 import asyncio
 from threading import Thread
 from . import sushierrors
 from . import sushi_info_types as info_types
 from . import grpc_gen
 from typing import List
@@ -53,14 +55,15 @@
 
         Parameters:
             address (str): 'ip-address:port' The ip-address and port at which to connect to sushi.
             sushi_proto_def (str): path to .proto file with SUSHI's gRPC services definition.
         """
         self.address = address
         self._sushi_proto, self._sushi_grpc = grpc_gen.modules_from_proto(sushi_proto_def)
+        self.tasks = []
         try:
             self.loop = asyncio.get_running_loop()
             self._async = True
         except RuntimeError:
             self._async = False
             self.loop = asyncio.get_event_loop()
             self.notification_thread = Thread(target=self._run_notification_loop, args=(self.loop,))
@@ -72,14 +75,20 @@
         """ Attaches the asyncio event loop to the thread and start looping over it.
             Should not be called by the User.
             """
         asyncio.set_event_loop(loop)
         loop.run_forever()
 
     def close(self):
+        for t in self.tasks:
+            try:
+                t.cancel()
+            except Exception as e:
+                print(e)
+
         if self._async:
             return
         else:
             self.loop.call_soon_threadsafe(self.loop.stop)
             self.notification_thread.join()
 
     def __del__(self):
@@ -202,16 +211,16 @@
 
     async def process_property_update_notifications(self, call_back=None, property_list=None):
         if not property_list:
             block_list = self._sushi_proto.GenericVoidValue()
         else:
             p_list = []
             for p in property_list:
-                property = self._sushi_proto.PropertyIdentifier(processor_id=p[0], property_id=p[1])
-                p_list.append(param)
+                prop = self._sushi_proto.PropertyIdentifier(processor_id=p[0], property_id=p[1])
+                p_list.append(prop)
             block_list = self._sushi_proto.PropertyNotificationBlocklist(properties=p_list)
         try:
             async with grpc.experimental.aio.insecure_channel(self.address) as channel:
                 stub = self._sushi_grpc.NotificationControllerStub(channel)
                 stream = stub.SubscribeToPropertyUpdates(block_list)
                 async for notification in stream:
                     # User logic here
@@ -238,53 +247,53 @@
         Subscribes to Transport changes notification stream from Sushi
         User needs to implement their own stream consumer logic and pass it as cb.
 
         Parameters:
             cb: a callable that will be called for each notification received from the stream.
         """
         if self._async:
-            asyncio.create_task(self.process_transport_change_notifications(cb))
+            self.tasks.append(asyncio.create_task(self.process_transport_change_notifications(cb)))
         else:
             asyncio.run_coroutine_threadsafe(self.process_transport_change_notifications(cb), self.loop)
 
     def subscribe_to_timing_updates(self, cb):
         """
         Subscribes to Timing update notification stream from Sushi
         User needs to implement their own stream consumer logic and pass it as cb.
 
         Parameters:
             cb: a callable that will be called for each notification received from the stream.        """
         if self._async:
-            asyncio.create_task(self.process_timing_update_notifications(cb))
+            self.tasks.append(asyncio.create_task(self.process_timing_update_notifications(cb)))
         else:
             asyncio.run_coroutine_threadsafe(self.process_timing_update_notifications(cb), self.loop)
 
     def subscribe_to_track_changes(self, cb):
         """
         Subscribes to Track change notification stream from Sushi.
         User needs to implement their own stream consumer logic and pass it as cb.
 
         Parameters:
             cb: a callable that will be called for each notification received from the stream.
         """
         if self._async:
-            asyncio.create_task(self.process_track_change_notifications(cb))
+            self.tasks.append(asyncio.create_task(self.process_track_change_notifications(cb)))
         else:
             asyncio.run_coroutine_threadsafe(self.process_track_change_notifications(cb), self.loop)
 
     def subscribe_to_processor_changes(self, cb):
         """
         Subscribes to Processor change notification stream from Sushi.
         User needs to implement their own stream consumer logic and pass it as cb.
 
         Parameters:
             cb: a callable that will be called for each notification received from the stream.
         """
         if self._async:
-            asyncio.create_task(self.process_processor_change_notifications(cb))
+            self.tasks.append(asyncio.create_task(self.process_processor_change_notifications(cb)))
         else:
             asyncio.run_coroutine_threadsafe(self.process_processor_change_notifications(cb), self.loop)
 
     def subscribe_to_parameter_updates(self, cb, param_blocklist=None):
         """
         Subscribes to Parameter update notification stream from Sushi
         User needs to implement their own logic to process these notification in the placeholder methods below
@@ -301,15 +310,15 @@
             ex: notification.parameter.parameter_id (gets the parameter ID)
             ex: notification.parameter.processor_id (gets the processor ID)
             ex: notification.normalized_value (gets the value normalized between 0 and 1)
             ex: notification.domain_value (gets the domain value)
             ex: notification.formatted_value (gets the value formatted as a string)
         """
         if self._async:
-            asyncio.create_task(self.process_parameter_update_notifications(cb))
+            self.tasks.append(asyncio.create_task(self.process_parameter_update_notifications(cb)))
         else:
             asyncio.run_coroutine_threadsafe(self.process_parameter_update_notifications(cb, param_blocklist), self.loop)
 
     def subscribe_to_property_updates(self, cb, property_blocklist=None):
         """
         Subscribes to Property update notification stream from Sushi
         User needs to implement their own logic to process these notification in the placeholder methods below
@@ -321,10 +330,10 @@
             Notification objects have 2 attributes: property and value;
             Property itself has 2 attributes: processor_id and property_id;
             ex: notification.parameter.property_id (gets the property ID)
             ex: notification.parameter.processor_id (gets the processor ID)
             ex: notification.value (gets the value)
         """
         if self._async:
-            asyncio.create_task(self.process_property_update_notifications(cb, property_blocklist))
+            self.tasks.append(asyncio.create_task(self.process_property_update_notifications(cb, property_blocklist)))
         else:
             asyncio.run_coroutine_threadsafe(self.process_property_update_notifications(cb, property_blocklist), self.loop)
```

### Comparing `elkpy-1.1.6/src/elkpy/osccontroller.py` & `elkpy-1.1.7/src/elkpy/osccontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/parametercontroller.py` & `elkpy-1.1.7/src/elkpy/parametercontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/programcontroller.py` & `elkpy-1.1.7/src/elkpy/programcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/sessioncontroller.py` & `elkpy-1.1.7/src/elkpy/sessioncontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/sushi_info_types.py` & `elkpy-1.1.7/src/elkpy/sushi_info_types.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/sushicontroller.py` & `elkpy-1.1.7/src/elkpy/sushicontroller.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,75 +36,80 @@
 from . import sessioncontroller
 from . import notificationcontroller
 
 from typing import List
 from typing import List, Callable
 
 
-
 ############################
 # Error handling functions #
 ############################
 class SushiUnkownError(Exception):
     """
     Error thrown when the source of the error can't be determined
     """
     pass
 
+
 class SushiUnsupportedOperationError(Exception):
     """
     Error thrown when the operation attempted is not currently supported in sushi
     """
     pass
 
+
 class SushiNotFoundError(Exception):
     """
     Error thrown if the requested entity is not found in sushi
     """
     pass
 
+
 class SushiOutOfRangeError(Exception):
     """
     Error thrown if one or more of the passed arguments are out of their allowed range
     """
     pass
 
+
 class SushiInvalidArgumentError(Exception):
     """
     Error thrown if one or more of the passed arguments are invalid
     """
     pass
 
+
 class SushiInternalError(Exception):
     """
     Error thrown if sushi encountered an internal error
     """
     pass
 
+
 def grpc_error_handling(e, context_info = ''):
     """
     Maps a gRPC exception to the corresponding sushi error. If the exception doesn't have a mapping
     the context info will be printed and the same exception will be re-raised
     """
-    if (e.code().name == 'UNKNOWN'):
+    if e.code().name == 'UNKNOWN':
         raise SushiUnkownError(e.details() , context_info) from e
-    elif (e.code().name == 'FAILED_PRECONDITION'):
+    elif e.code().name == 'FAILED_PRECONDITION':
         raise SushiUnsupportedOperationError(e.details() , context_info) from e
-    elif (e.code().name == 'NOT_FOUND'):
+    elif e.code().name == 'NOT_FOUND':
         raise SushiNotFoundError(e.details() , context_info) from e
-    elif (e.code().name == 'OUT_OF_RANGE'):
+    elif e.code().name == 'OUT_OF_RANGE':
         raise SushiOutOfRangeError(e.details() , context_info) from e
-    elif (e.code().name == 'INVALID_ARGUMENT'):
+    elif e.code().name == 'INVALID_ARGUMENT':
         raise SushiInvalidArgumentError(e.details() , context_info) from e
-    elif (e.code().name == 'INTERNAL'):
+    elif e.code().name == 'INTERNAL':
         raise SushiInternalError(e.details() , context_info) from e
     else:
-        print(context_info)
+        print('Grpc error: ' + str(e.code().name) + ', ' + e.details())
         raise e
-      #  print('Grpc error: ' + str e.code().name) + ', ' + e.details())
+
 
 ###############################
 # Main sushi controller class #
 ###############################
 
 class SushiController(object):
     """
@@ -145,13 +150,13 @@
         self.notifications = notificationcontroller.NotificationController(address, sushi_proto_def)
 
     def close(self):
         """
         This method should be called at app close.
         It should call any sub-controller close routines whenever they exist.
         i.e.: NotificationController has an infinite event loop running in its own thread, which has to be stopped and joined
-                to ensure clean closing and proper releasing of any resources.
+        to ensure clean closing and proper releasing of any resources.
         """
         self.notifications.close()
 
     def __del__(self):
         self.notifications.close()
```

### Comparing `elkpy-1.1.6/src/elkpy/sushierrors.py` & `elkpy-1.1.7/src/elkpy/sushierrors.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/sushiprocessor.py` & `elkpy-1.1.7/src/elkpy/sushiprocessor.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/systemcontroller.py` & `elkpy-1.1.7/src/elkpy/systemcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/timingcontroller.py` & `elkpy-1.1.7/src/elkpy/timingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy/transportcontroller.py` & `elkpy-1.1.7/src/elkpy/transportcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.6/src/elkpy.egg-info/PKG-INFO` & `elkpy-1.1.7/src/elkpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.1.6
+Version: 1.1.7
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elkpy-1.1.6/src/elkpy.egg-info/SOURCES.txt` & `elkpy-1.1.7/src/elkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

