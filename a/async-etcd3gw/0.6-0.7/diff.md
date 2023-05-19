# Comparing `tmp/async_etcd3gw-0.6.tar.gz` & `tmp/async_etcd3gw-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_etcd3gw-0.6.tar", last modified: Thu May  4 08:01:52 2023, max compression
+gzip compressed data, was "async_etcd3gw-0.7.tar", last modified: Fri May 19 08:49:38 2023, max compression
```

## Comparing `async_etcd3gw-0.6.tar` & `async_etcd3gw-0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:52.675927 async_etcd3gw-0.6/async_etcd3gw/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/async_lease.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/async_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/async_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/async_etcd3gw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/async_etcd3gw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:01:52.000000 async_etcd3gw-0.6/async_etcd3gw.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:52.679927 async_etcd3gw-0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/tests/test_async_etcd3gw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-04 08:01:22.000000 async_etcd3gw-0.6/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:49:38.122823 async_etcd3gw-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-19 08:49:38.122823 async_etcd3gw-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:49:38.122823 async_etcd3gw-0.7/async_etcd3gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/async_etcd3gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/async_etcd3gw/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/async_etcd3gw/async_lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/async_etcd3gw/async_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/async_etcd3gw/async_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/async_etcd3gw/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/async_etcd3gw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:49:38.122823 async_etcd3gw-0.7/async_etcd3gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-19 08:49:38.000000 async_etcd3gw-0.7/async_etcd3gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-19 08:49:38.000000 async_etcd3gw-0.7/async_etcd3gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:49:38.000000 async_etcd3gw-0.7/async_etcd3gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 08:49:38.000000 async_etcd3gw-0.7/async_etcd3gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 08:49:38.000000 async_etcd3gw-0.7/async_etcd3gw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:49:37.000000 async_etcd3gw-0.7/async_etcd3gw.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 08:49:38.126823 async_etcd3gw-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:49:38.122823 async_etcd3gw-0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/tests/test_async_etcd3gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-19 08:49:13.000000 async_etcd3gw-0.7/tests/test_client.py
```

### Comparing `async_etcd3gw-0.6/LICENSE` & `async_etcd3gw-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/PKG-INFO` & `async_etcd3gw-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_etcd3gw
-Version: 0.6
+Version: 0.7
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
```

### Comparing `async_etcd3gw-0.6/README.md` & `async_etcd3gw-0.7/README.md`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/async_etcd3gw/__init__.py` & `async_etcd3gw-0.7/async_etcd3gw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    https://opendev.org/openstack/etcd3gw/src/tag/2.1.0/etcd3gw/__init__.py
 
 from . import utils
 from .async_client import AsyncEtcd3Client, async_client
 from .async_lease import AsyncLease
 from .async_lock import AsyncLock
 
-__version__ = "0.6"
+__version__ = "0.7"
 
 __all__ = (
     "AsyncEtcd3Client",
     "AsyncLease",
     "AsyncLock",
     "async_client",
     "utils",
```

### Comparing `async_etcd3gw-0.6/async_etcd3gw/async_client.py` & `async_etcd3gw-0.7/async_etcd3gw/async_client.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/async_etcd3gw/async_lease.py` & `async_etcd3gw-0.7/async_etcd3gw/async_lease.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/async_etcd3gw/async_lock.py` & `async_etcd3gw-0.7/async_etcd3gw/async_lock.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/async_etcd3gw/async_watch.py` & `async_etcd3gw-0.7/async_etcd3gw/async_watch.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             pass
 
     async def process_chunk(self, line):
         "Process a chuck"
         decoded_line = line.decode("utf-8")
         try:
             payload = json.loads(decoded_line)
-        except Exception as ex:
+        except json.JSONDecodeError as ex:
             raise ex
         if "error" in payload:
             raise get_exception(
                 payload["error"].get("http_code", 500), payload["error"].get("http_status", ""), payload["error"].get("message", "")
             )
         if "created" in payload["result"]:
             if not payload["result"]["created"]:
@@ -81,15 +81,19 @@
         while True:
             if content._exception is not None:
                 raise content._exception
 
             if not content._buffer and not content._eof:
                 await content._wait("readany")
 
-            data = content._read_nowait(-1)
+            (data, end_of_http_chunk) = await content.readchunk()
+            while not end_of_http_chunk:
+                (more_data, end_of_http_chunk) = await content.readchunk()
+                data += more_data
+
             await self.process_chunk(data)
 
     async def watch(self):
         try:
             timeout = aiohttp.ClientTimeout(total=None, sock_read=None)
             async with self.async_client.session.post(
                 self.async_client.get_url("/watch"), json=self.create_request, timeout=timeout
```

### Comparing `async_etcd3gw-0.6/async_etcd3gw/exceptions.py` & `async_etcd3gw-0.7/async_etcd3gw/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/async_etcd3gw/utils.py` & `async_etcd3gw-0.7/async_etcd3gw/utils.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/async_etcd3gw.egg-info/PKG-INFO` & `async_etcd3gw-0.7/async_etcd3gw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-etcd3gw
-Version: 0.6
+Version: 0.7
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
```

### Comparing `async_etcd3gw-0.6/setup.cfg` & `async_etcd3gw-0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/tests/test_async_etcd3gw.py` & `async_etcd3gw-0.7/tests/test_async_etcd3gw.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.6/tests/test_client.py` & `async_etcd3gw-0.7/tests/test_client.py`

 * *Files identical despite different names*

