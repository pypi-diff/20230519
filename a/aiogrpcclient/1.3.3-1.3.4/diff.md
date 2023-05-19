# Comparing `tmp/aiogrpcclient-1.3.3-py3-none-any.whl.zip` & `tmp/aiogrpcclient-1.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3333 bytes, number of entries: 5
--rw-r--r--  2.0 unx       94 b- defN 22-Oct-25 08:23 aiogrpcclient/__init__.py
--rw-r--r--  2.0 unx     5494 b- defN 23-Feb-16 15:54 aiogrpcclient/base.py
-?rw-------  2.0 unx       91 b- defN 23-Feb-16 15:54 aiogrpcclient-1.3.3.dist-info/WHEEL
-?rw-------  2.0 unx      552 b- defN 23-Feb-16 15:54 aiogrpcclient-1.3.3.dist-info/METADATA
-?rw-------  2.0 unx      381 b- defN 23-Feb-16 15:54 aiogrpcclient-1.3.3.dist-info/RECORD
-5 files, 6612 bytes uncompressed, 2621 bytes compressed:  60.4%
+Zip file size: 3329 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       94 b- defN 22-Oct-25 09:23 aiogrpcclient/__init__.py
+-rw-r--r--  2.0 unx     5495 b- defN 23-Apr-16 19:34 aiogrpcclient/base.py
+?rw-------  2.0 unx       91 b- defN 23-May-19 17:49 aiogrpcclient-1.3.4.dist-info/WHEEL
+?rw-------  2.0 unx      552 b- defN 23-May-19 17:49 aiogrpcclient-1.3.4.dist-info/METADATA
+?rw-------  2.0 unx      381 b- defN 23-May-19 17:49 aiogrpcclient-1.3.4.dist-info/RECORD
+5 files, 6613 bytes uncompressed, 2617 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: aiogrpcclient/__init__.py
 Comment: 
 
 Filename: aiogrpcclient/base.py
 Comment: 
 
-Filename: aiogrpcclient-1.3.3.dist-info/WHEEL
+Filename: aiogrpcclient-1.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: aiogrpcclient-1.3.3.dist-info/METADATA
+Filename: aiogrpcclient-1.3.4.dist-info/METADATA
 Comment: 
 
-Filename: aiogrpcclient-1.3.3.dist-info/RECORD
+Filename: aiogrpcclient-1.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiogrpcclient/base.py

```diff
@@ -110,15 +110,15 @@
 
     def __init__(
         self,
         endpoint,
         max_retries: int = 2,
         retry_delay: float = 0.5,
         connection_timeout: float = None,
-        max_message_length: int = 300 * 1024 * 1024,
+        max_message_length: int = 1024 * 1024 * 1024,
     ):
         super().__init__()
         if endpoint is None:
             raise RuntimeError(f'`endpoint` must be passed for {self.__class__.__name__} constructor')
         options = [
             ('grpc.dns_min_time_between_resolutions_ms', 1000),
             ('grpc.initial_reconnect_backoff_ms', 1000),
```

## Comparing `aiogrpcclient-1.3.3.dist-info/METADATA` & `aiogrpcclient-1.3.4.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aiogrpcclient
-Version: 1.3.3
+Version: 1.3.4
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Home-page: https://github.com/izihawa/aiogrpcclient
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
-Requires-Dist: aiokit >= 1.0.0
+Requires-Dist: aiokit >= 1.2.2
 Requires-Dist: grpcio >= 1.45.0
 Requires-Dist: izihawa-utils >= 1.0.2
 Requires-Dist: orjson >= 3.6.8
 Requires-Dist: protobuf >= 3.19.4
 Requires-Dist: pyyaml >= 6.0
 Requires-Dist: termcolor >= 1.1.0
```

