# Comparing `tmp/wbddh-0.0.1-py3-none-any.whl.zip` & `tmp/wbddh-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8850 bytes, number of entries: 11
+Zip file size: 8860 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      396 b- defN 23-May-15 19:53 wbddh/__init__.py
 -rw-rw-rw-  2.0 fat      990 b- defN 23-May-15 19:53 wbddh/exceptions.py
--rw-rw-rw-  2.0 fat     2403 b- defN 23-May-16 18:10 wbddh/request_manager.py
+-rw-rw-rw-  2.0 fat     2419 b- defN 23-May-19 15:09 wbddh/request_manager.py
 -rw-rw-rw-  2.0 fat     8796 b- defN 23-May-11 22:36 wbddh/session.py
 -rw-rw-rw-  2.0 fat     6057 b- defN 23-May-16 17:34 wbddh/session_manager.py
 -rw-rw-rw-  2.0 fat       50 b- defN 23-May-13 18:53 wbddh/test.py
 -rw-rw-rw-  2.0 fat     1318 b- defN 23-May-11 22:36 wbddh/utils.py
--rw-rw-rw-  2.0 fat      543 b- defN 23-May-16 19:17 wbddh-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-16 19:17 wbddh-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-16 19:17 wbddh-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      810 b- defN 23-May-16 19:17 wbddh-0.0.1.dist-info/RECORD
-11 files, 21461 bytes uncompressed, 7498 bytes compressed:  65.1%
+-rw-rw-rw-  2.0 fat      543 b- defN 23-May-19 15:12 wbddh-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-19 15:12 wbddh-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-19 15:12 wbddh-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      810 b- defN 23-May-19 15:12 wbddh-0.0.2.dist-info/RECORD
+11 files, 21477 bytes uncompressed, 7508 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: wbddh/test.py
 Comment: 
 
 Filename: wbddh/utils.py
 Comment: 
 
-Filename: wbddh-0.0.1.dist-info/METADATA
+Filename: wbddh-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: wbddh-0.0.1.dist-info/WHEEL
+Filename: wbddh-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: wbddh-0.0.1.dist-info/top_level.txt
+Filename: wbddh-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: wbddh-0.0.1.dist-info/RECORD
+Filename: wbddh-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wbddh/request_manager.py

```diff
@@ -64,10 +64,10 @@
         return requests.post(get_endpoint(endpoint, session), files=files, verify=session.verify, headers=session.get_headers(headers))
     else:
         raise DDHSessionException("DDH POST request requires a session")
 
 
 def get_endpoint(endpoint, session=None):
     if session:
-        return '/'.join([session.api_host, endpoint])
+        return '/'.join([session.api_host, endpoint.strip()])
     else:
-        return '/'.join([public_API_URL, endpoint])
+        return '/'.join([public_API_URL, endpoint.strip()])
```

## Comparing `wbddh-0.0.1.dist-info/METADATA` & `wbddh-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbddh
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for DDH Open API
 Home-page: https://github.com/WB-DECIS/WBDDH
 Author: DECIS
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Provides-Extra: admin
 Requires-Dist: msal ; extra == 'admin'
```

## Comparing `wbddh-0.0.1.dist-info/RECORD` & `wbddh-0.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 wbddh/__init__.py,sha256=Mzr-CFhoE5tVUGnBK0ErZp429LATAf-G0hBHW0NP4vE,396
 wbddh/exceptions.py,sha256=prNSwu_9o5NnGfRtZBe4OxifAcLM2eSlrgpiJkOz8-8,990
-wbddh/request_manager.py,sha256=BWPVJk-P7M1mJf2HgbUFIFFM0V4iLwoGr8V2vanUdmA,2403
+wbddh/request_manager.py,sha256=GEZzuUFDAEfiz6HvoxVHibfG7MLUfcEqioGYiUIu14o,2419
 wbddh/session.py,sha256=pW5SqU2LaWcsFqRlzYMjSDM3Dlag_7HsRQHDOufTeC0,8796
 wbddh/session_manager.py,sha256=ZL3LNHvuRrxDQeQGfmK_IZk95Qewi0t7rgBvb9FXpB4,6057
 wbddh/test.py,sha256=tuUyiKBC5AHoFjelqqMXWX_TrlE80HB37gJ7GidUp7U,50
 wbddh/utils.py,sha256=UhNse6FN2NzOtqL2v_js-l48MxGWLJLc-jusWSe1Zt0,1318
-wbddh-0.0.1.dist-info/METADATA,sha256=-Gzl9St5Qe1N-To8vFQQpTGoyu2RJga9r7L3IsMjW8s,543
-wbddh-0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-wbddh-0.0.1.dist-info/top_level.txt,sha256=QpvOJxdfZd0MJiwJGdLPwRZ_l998Zyc_HIJ2JF_3iTI,6
-wbddh-0.0.1.dist-info/RECORD,,
+wbddh-0.0.2.dist-info/METADATA,sha256=MybJniGjs04ZOZAAeDIXbZsYoUkzNdQ_dWVkOsYu0JE,543
+wbddh-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+wbddh-0.0.2.dist-info/top_level.txt,sha256=QpvOJxdfZd0MJiwJGdLPwRZ_l998Zyc_HIJ2JF_3iTI,6
+wbddh-0.0.2.dist-info/RECORD,,
```

