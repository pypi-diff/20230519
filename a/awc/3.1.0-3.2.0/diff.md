# Comparing `tmp/awc-3.1.0-py2.py3-none-any.whl.zip` & `tmp/awc-3.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23909 bytes, number of entries: 16
--rw-r--r--  2.0 unx     6843 b- defN 23-May-09 16:10 awc/__init__.py
+Zip file size: 23939 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     6843 b- defN 23-May-19 15:54 awc/__init__.py
 -rw-r--r--  2.0 unx      678 b- defN 23-Apr-11 16:56 awc/__main__.py
--rw-r--r--  2.0 unx     6030 b- defN 23-May-07 23:42 awc/api.py
+-rw-r--r--  2.0 unx     6207 b- defN 23-May-19 15:55 awc/api.py
 -rw-r--r--  2.0 unx      305 b- defN 23-Apr-12 22:27 awc/const.py
 -rw-r--r--  2.0 unx     1479 b- defN 23-Apr-15 21:04 awc/exc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 12:49 awc/py.typed
 -rw-r--r--  2.0 unx     1422 b- defN 23-May-09 16:09 awc/util.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 22:27 awc/wrn.py
 -rw-r--r--  2.0 unx     4658 b- defN 23-May-09 15:41 awc/sql/__init__.py
 -rw-r--r--  2.0 unx     3459 b- defN 23-May-09 15:41 awc/sql/helpers.py
--rw-------  2.0 unx    35107 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3812 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-3.1.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1145 b- defN 23-May-09 16:11 awc-3.1.0.dist-info/RECORD
-16 files, 65667 bytes uncompressed, 22073 bytes compressed:  66.4%
+-rw-------  2.0 unx    35107 b- defN 23-May-19 15:56 awc-3.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3812 b- defN 23-May-19 15:56 awc-3.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-19 15:56 awc-3.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-May-19 15:56 awc-3.2.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-3.2.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1145 b- defN 23-May-19 15:56 awc-3.2.0.dist-info/RECORD
+16 files, 65844 bytes uncompressed, 22103 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: awc/sql/__init__.py
 Comment: 
 
 Filename: awc/sql/helpers.py
 Comment: 
 
-Filename: awc-3.1.0.dist-info/LICENSE
+Filename: awc-3.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: awc-3.1.0.dist-info/METADATA
+Filename: awc-3.2.0.dist-info/METADATA
 Comment: 
 
-Filename: awc-3.1.0.dist-info/WHEEL
+Filename: awc-3.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: awc-3.1.0.dist-info/top_level.txt
+Filename: awc-3.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: awc-3.1.0.dist-info/zip-safe
+Filename: awc-3.2.0.dist-info/zip-safe
 Comment: 
 
-Filename: awc-3.1.0.dist-info/RECORD
+Filename: awc-3.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc/__init__.py

```diff
@@ -7,15 +7,15 @@
 from functools import wraps
 
 import requests
 from furl import furl  # type: ignore
 
 from . import const, exc, util
 
-__version__: typing.Final[str] = "3.1.0"
+__version__: typing.Final[str] = "3.2.0"
 
 
 class Awc:
     """ari-web comments interface
 
     this is where all API requests begin, you must
     pass an instance of this object to every api wrapper
```

## awc/api.py

```diff
@@ -192,7 +192,17 @@
 
     return awc.post(
         api="anon",
         data={
             "content": util.truncate(content, const.MAX_CONTENT_LEN),
         },
     ).text
+
+
+def visit(awc: Awc) -> str:
+    """visit api
+
+    awc: awc.Awc -- the awc.Awc instance to work on
+
+    return str -- the returned svg"""
+
+    return awc.get(api="visit").text
```

## Comparing `awc-3.1.0.dist-info/LICENSE` & `awc-3.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc-3.1.0.dist-info/METADATA` & `awc-3.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc
-Version: 3.1.0
+Version: 3.2.0
 Summary: wrapper for ari-web comments API
 Home-page: https://ari-web.xyz/gh/awc
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,comments,api,wrapper,https
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `awc-3.1.0.dist-info/RECORD` & `awc-3.2.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-awc/__init__.py,sha256=CjXEhXjtr8lIHmY3TSFtlATvbQhSsu5SbvFGbqiLNus,6843
+awc/__init__.py,sha256=z56cw6DGaFBHWOgw2FGEYdgkHchpEQRA6bnV_1mrToA,6843
 awc/__main__.py,sha256=d1UfoKcH5bl9qoqWowmcARIitWbbGsasAZfq8RHHsE4,678
-awc/api.py,sha256=f02eIZdXfOZo9f-f7YhN1Rhcz4a55KAzxRfTIxSrzTg,6030
+awc/api.py,sha256=2ZxQF6YBgzpOYUqXug-_MS0CtGDfEpmMi9LTdMId468,6207
 awc/const.py,sha256=0ctjO9muVRU7kBkqF9LjcgwvP4baLum63UUOxTE1oLw,305
 awc/exc.py,sha256=kGwH4_a8C1EpYx3PvoBXyWiiW451YbHsKi_JGtnsiuk,1479
 awc/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awc/util.py,sha256=VkpiEdESLdZWwAv8OaNkJHVjzP4gmkF8Z4pGplbX0l4,1422
 awc/wrn.py,sha256=K84cpt9OdHQi76vhgMsWFbl8rIN_sH6EkOGptZOUWmQ,614
 awc/sql/__init__.py,sha256=JgJLCahZVJD0Sa9TXjrffMqCyDjxTKEQw5nxwAEOp2s,4658
 awc/sql/helpers.py,sha256=wdaRfqpbuSvtDwMhBl9OFreithQRJQ2NfnKwbdqJGSg,3459
-awc-3.1.0.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
-awc-3.1.0.dist-info/METADATA,sha256=FaFOVdRNFy4eTcu3Av0wRoOhl5tNtX6xwQDA9eAbITQ,3812
-awc-3.1.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc-3.1.0.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
-awc-3.1.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc-3.1.0.dist-info/RECORD,,
+awc-3.2.0.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
+awc-3.2.0.dist-info/METADATA,sha256=xsMQq98JXjt_gFyeH5o7n3Q39_OGPAKvlfUfQ53ovj4,3812
+awc-3.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc-3.2.0.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
+awc-3.2.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc-3.2.0.dist-info/RECORD,,
```

