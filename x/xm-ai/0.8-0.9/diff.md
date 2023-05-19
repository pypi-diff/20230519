# Comparing `tmp/xm_ai-0.8-py3-none-any.whl.zip` & `tmp/xm_ai-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5826 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-18 17:22 xm_ai/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 23-May-18 17:22 xm_ai/aws_utils.py
--rw-r--r--  2.0 unx     2430 b- defN 23-May-18 17:22 xm_ai/database_utils.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-18 17:22 xm_ai/email_utils.py
--rw-r--r--  2.0 unx      238 b- defN 23-May-18 17:22 xm_ai/excel_utils.py
--rw-r--r--  2.0 unx     2338 b- defN 23-May-18 17:22 xm_ai/query_utils.py
--rw-r--r--  2.0 unx      134 b- defN 23-May-18 17:22 xm_ai/syntax_utils.py
--rw-r--r--  2.0 unx      600 b- defN 23-May-18 17:22 xm_ai/time_utils.py
--rw-r--r--  2.0 unx      471 b- defN 23-May-18 17:22 xm_ai-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 17:22 xm_ai-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-18 17:22 xm_ai-0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      888 b- defN 23-May-18 17:22 xm_ai-0.8.dist-info/RECORD
-12 files, 10608 bytes uncompressed, 4352 bytes compressed:  59.0%
+Zip file size: 5402 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-19 19:57 xm_ai/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-May-19 19:57 xm_ai/aws_utils.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-19 19:57 xm_ai/database_utils.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-May-19 19:57 xm_ai/email_utils.py
+-rw-r--r--  2.0 unx      238 b- defN 23-May-19 19:57 xm_ai/excel_utils.py
+-rw-r--r--  2.0 unx     2338 b- defN 23-May-19 19:57 xm_ai/query_utils.py
+-rw-r--r--  2.0 unx      134 b- defN 23-May-19 19:57 xm_ai/syntax_utils.py
+-rw-r--r--  2.0 unx      600 b- defN 23-May-19 19:57 xm_ai/time_utils.py
+-rw-r--r--  2.0 unx      471 b- defN 23-May-19 19:58 xm_ai-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 19:58 xm_ai-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-19 19:58 xm_ai-0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      887 b- defN 23-May-19 19:58 xm_ai-0.9.dist-info/RECORD
+12 files, 8754 bytes uncompressed, 3928 bytes compressed:  55.1%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: xm_ai/syntax_utils.py
 Comment: 
 
 Filename: xm_ai/time_utils.py
 Comment: 
 
-Filename: xm_ai-0.8.dist-info/METADATA
+Filename: xm_ai-0.9.dist-info/METADATA
 Comment: 
 
-Filename: xm_ai-0.8.dist-info/WHEEL
+Filename: xm_ai-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xm_ai-0.8.dist-info/top_level.txt
+Filename: xm_ai-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xm_ai-0.8.dist-info/RECORD
+Filename: xm_ai-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xm_ai/database_utils.py

```diff
@@ -1,58 +1,18 @@
-import pymongo.errors
-from botocore.exceptions import EndpointConnectionError
 from pymongo import MongoClient
 from pymongo.database import Database
-from enum import Enum
-from xm_ai.aws_utils import get_secret
 
 
-class xMentiumMongoSecret(Enum):
-    username = 'username'
-    password = 'password'
-    address = 'address'
-    port = 'port'
-    database = 'database'
-    production_name: str = 'production'
+def get_database(connstring: str, server_name: str) -> Database:
 
-
-def get_database(server_name: str) -> Database:
-    database_name = server_name
-    if server_name == "production" or server_name == "staging":
-        secret = get_secret("xmentium_mongo")
-        connstring = f"mongodb:" \
-                     f"//{secret[xMentiumMongoSecret.username.value]}" \
-                     f":{secret[xMentiumMongoSecret.password.value]}" \
-                     f"@{secret[xMentiumMongoSecret.address.value]}" \
-                     f":{secret[xMentiumMongoSecret.port.value]}" \
-                     f"/{secret[xMentiumMongoSecret.database.value]}"
-        database_name = secret[
-            xMentiumMongoSecret.production_name.value] if server_name == "production" else server_name
-    elif server_name == "develop":
-        connstring = "mongodb://localhost:27017"
-        database_name = "xm"
-    elif server_name == "ai":
-        secret = get_secret("ai_mongo")
-        connstring = f"mongodb+srv:" \
-                     f"//{secret[xMentiumMongoSecret.username.value]}" \
-                     f":{secret[xMentiumMongoSecret.password.value]}" \
-                     f"@{secret[xMentiumMongoSecret.address.value]}" \
-                     f"/{secret[xMentiumMongoSecret.database.value]}"
+    if server_name == "staging" or server_name == "production":
+        database_name = "ft-01"
     else:
-        raise ValueError("Invalid Option Selected")
+        database_name = "xm"
 
+    db = MongoClient(connstring)[database_name]
     try:
-        db = MongoClient(connstring)[database_name]
-        try:
-            _ = db.templates.find_one({})['name']
-            return db
-        except TypeError as error:
-            print(error)
-            raise ValueError(f"You tried to connect to a database: {database_name} that doesn't exist in this server: {server_name}")
-        except pymongo.errors.ServerSelectionTimeoutError as error:
-            print(error)
-            raise pymongo.errors.ServerSelectionTimeoutError("This connection string likely does not have access to the database")
-
-    except EndpointConnectionError as error:
+        _ = db.templates.find_one({})['name']
+        return db
+    except TypeError as error:
         print(error)
-        print("You are offline, so Boto3 could not create a session")
-        raise EndpointConnectionError
+        raise ValueError(f"You tried to connect to a database: {database_name} that doesn't exist in this server: {server_name}")
```

## Comparing `xm_ai-0.8.dist-info/RECORD` & `xm_ai-0.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 xm_ai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 xm_ai/aws_utils.py,sha256=BZ8lqidsBhckW2Jy6-eJVbomt5yyo7LWqmKuGu2Ewe0,1200
-xm_ai/database_utils.py,sha256=hxQ1F57aZ7A6BM4HBl5NtzAvkamHJj6e95pmNwXfEGA,2430
+xm_ai/database_utils.py,sha256=2CvzFtLHyU2EDnRmTjoDFKh5dW_nzi8qX5clkvzehaY,577
 xm_ai/email_utils.py,sha256=N0xmFD5eD3nG8nVejh9uF5w__XYHD9JSNTOVEAEHcrU,2211
 xm_ai/excel_utils.py,sha256=xafW_NtNMq6qETFisMDPohPfs34BbekUdyM1qQefr7o,238
 xm_ai/query_utils.py,sha256=hnIgx6uD5cBMeNUUZCUzUE5ICkmFR5x6EbxePFfbMms,2338
 xm_ai/syntax_utils.py,sha256=aWGhKkLLZQSOO4_gee_9EGO1b1KI8-KXZd45Ts2jNj4,134
 xm_ai/time_utils.py,sha256=qEsWIjq3GRG3a4L8yxQe2b_gJszsmXRDSsBZKR4b9cs,600
-xm_ai-0.8.dist-info/METADATA,sha256=P41H7yfGCAgEyMPFd0wsb5Z8jPLVPnUKWgsAEGOXSyI,471
-xm_ai-0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xm_ai-0.8.dist-info/top_level.txt,sha256=0tH-EgTFu93crY6L8lAB9az_LQotSkuUdG1rObgP0iA,6
-xm_ai-0.8.dist-info/RECORD,,
+xm_ai-0.9.dist-info/METADATA,sha256=nHWkREN3ulOL4zVSnbXgMRRn2wEZlXinwtHJGuCKIBg,471
+xm_ai-0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xm_ai-0.9.dist-info/top_level.txt,sha256=0tH-EgTFu93crY6L8lAB9az_LQotSkuUdG1rObgP0iA,6
+xm_ai-0.9.dist-info/RECORD,,
```

