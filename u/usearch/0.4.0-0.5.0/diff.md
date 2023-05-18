# Comparing `tmp/usearch-0.4.0-cp39-cp39-win_amd64.whl.zip` & `tmp/usearch-0.5.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 134062 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-17 23:01 usearch/__init__.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-May-17 23:01 usearch/client.py
--rw-rw-rw-  2.0 fat   275968 b- defN 23-May-17 23:09 usearch/index.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2298 b- defN 23-May-17 23:01 usearch/io.py
--rw-rw-rw-  2.0 fat     1203 b- defN 23-May-17 23:01 usearch/server.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    19489 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      770 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/RECORD
-10 files, 312445 bytes uncompressed, 132766 bytes compressed:  57.5%
+Zip file size: 136379 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-18 22:39 usearch/__init__.py
+-rw-rw-rw-  2.0 fat     1462 b- defN 23-May-18 22:39 usearch/client.py
+-rw-rw-rw-  2.0 fat   284160 b- defN 23-May-18 22:47 usearch/index.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2298 b- defN 23-May-18 22:39 usearch/io.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-May-18 22:39 usearch/server.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    19489 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      770 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/RECORD
+10 files, 322593 bytes uncompressed, 135083 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: usearch/io.py
 Comment: 
 
 Filename: usearch/server.py
 Comment: 
 
-Filename: usearch-0.4.0.dist-info/LICENSE
+Filename: usearch-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: usearch-0.4.0.dist-info/METADATA
+Filename: usearch-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: usearch-0.4.0.dist-info/WHEEL
+Filename: usearch-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: usearch-0.4.0.dist-info/top_level.txt
+Filename: usearch-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch-0.4.0.dist-info/RECORD
+Filename: usearch-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## usearch/client.py

```diff
@@ -5,17 +5,17 @@
 class IndexClient:
 
     def __init__(self, uri: str = '127.0.0.1', port: int = 8545, use_http: bool = True) -> None:
         self.client = Client(uri=uri, port=port, use_http=use_http)
 
     def add(self, labels: np.array, vectors: np.array):
         if isinstance(labels, int):
-            return self.client.add_one(label=labels, vectors=vectors)
+            self.client.add_one(label=labels, vectors=vectors)
         else:
-            return self.client.add_many(labels=labels, vectors=vectors)
+            self.client.add_many(labels=labels, vectors=vectors)
 
     def search(self, vectors: np.array, count: int) -> tuple[np.array, np.array, np.array]:
         matches = []
         distances = []
         counts = []
         # return self.client.search_one(vectors=vectors, count=count)
         return matches, distances, counts
@@ -28,7 +28,23 @@
         return self.client.ndim()
 
     def capacity(self):
         return self.client.capacity()
 
     def connectivity(self):
         return self.client.connectivity()
+
+    def load(self, path: str):
+        raise NotImplementedError()
+
+    def view(self, path: str):
+        raise NotImplementedError()
+
+    def save(self, path: str):
+        raise NotImplementedError()
+
+
+if __name__ == '__main__':
+    index = IndexClient()
+    index.add(42, np.array([0.4] * 256, dtype=np.float32))
+    results = index.search(np.array([0.4] * 256, dtype=np.float32), 10)
+    print(results)
```

## usearch/server.py

```diff
@@ -1,30 +1,42 @@
-import ucall.rich_posix as ucall
-import usearch
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 
-import fire
+import os
+import argparse
 import numpy as np
-from PIL import Image
 
+from ucall.rich_posix import Server
+from usearch.index import Index
 
-def serve(ndim: int, metric: str = 'ip'):
 
-    server = ucall.Server()
-    index = usearch.Index(ndim=ndim, metric=metric)
+def serve(
+        ndim: int, metric: str = 'ip',
+        port: int = 8545, threads: int = 1,
+        path: str = 'index.usearch', immutable: bool = False):
+
+    server = Server(port=port)
+    index = Index(ndim=ndim, metric=metric)
+
+    if os.path.exists(path):
+        if immutable:
+            index.view(path)
+        else:
+            index.load(path)
 
     @server
     def add_one(label: int, vector: np.array):
         labels = np.array([label], dtype=np.longlong)
         vectors = vector.reshape(vector.shape[0], 1)
         index.add(labels, vectors, copy=True)
 
     @server
     def add_many(labels: np.array, vectors: np.array):
         labels = labels.astype(np.longlong)
-        index.add(labels, vectors, copy=True)
+        index.add(labels, vectors, threads=threads, copy=True)
 
     @server
     def search_one(vector: np.array, count: int) -> np.ndarray:
         vectors = vector.reshape(vector.shape[0], 1)
         results = index.search(vectors, 3)
         return results[0][:results[2][0]]
 
@@ -40,12 +52,44 @@
     def capacity() -> int:
         return index.capacity()
 
     @server
     def connectivity() -> int:
         return index.connectivity()
 
-    server.run()
+    try:
+        server.run()
+    except KeyboardInterrupt:
+        if not immutable:
+            index.save(path)
 
 
 if __name__ == '__main__':
-    fire(serve)
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-v', '--verbose', help='log server activity')
+    parser.add_argument(
+        '--ndim', type=int,
+        help='dimensionality of the vectors')
+    parser.add_argument(
+        '--immutable', type=bool, default=False,
+        help='the index can not be updated')
+
+    parser.add_argument(
+        '--metric', type=str, default='ip', choices=['ip', 'cos', 'l2', 'haversine'],
+        help='distance function to compare vectors')
+    parser.add_argument(
+        '-p', '--port', type=int, default=8545,
+        help='port to open for client connections')
+    parser.add_argument(
+        '-j', '--threads', type=int, default=1,
+        help='number of CPU threads to use')
+    parser.add_argument(
+        '--path', type=str, default='index.usearch',
+        help='where to store the index')
+
+    args = parser.parse_args()
+    assert args.ndim is not None, 'Define the number of dimensions!'
+    serve(
+        ndim=args.ndim, metric=args.metric,
+        threads=args.threads, port=args.port,
+        path=args.path, immutable=args.immutable)
```

## Comparing `usearch-0.4.0.dist-info/LICENSE` & `usearch-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `usearch-0.4.0.dist-info/METADATA` & `usearch-0.5.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usearch
-Version: 0.4.0
+Version: 0.5.0
 Summary: Smaller & Faster Single-File Vector Search Engine from Unum
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usearch Version: 0.4.0 Summary: Smaller & Faster
+Metadata-Version: 2.1 Name: usearch Version: 0.5.0 Summary: Smaller & Faster
 Single-File Vector Search Engine from Unum License: Apache-2.0 Classifier:
 Development Status :: 4 - Beta Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: C++ Classifier: Operating System :: MacOS Classifier:
```

## Comparing `usearch-0.4.0.dist-info/RECORD` & `usearch-0.5.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 usearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-usearch/client.py,sha256=0QBbWSF-4qBm94f0sHVt1CmuL9Xi3b7tCnNSqt3Da9Q,1051
-usearch/index.cp39-win_amd64.pyd,sha256=eYC32ADxqEcBiOQsSQ7cp4MpG6ni7vA76rjdMoLmStg,275968
+usearch/client.py,sha256=bxfhEqgyrhb0ImT1e2uLiO-RKjq7cQZoIhNcR7fFGt8,1462
+usearch/index.cp39-win_amd64.pyd,sha256=A5Sv5aQNMrAHclgTlqxaq7VPm0WH99KIEttf9viJNXU,284160
 usearch/io.py,sha256=xbieZtFNHPaG_1xFsoqQQdtuT_7s7DowdXK2BEphtzk,2298
-usearch/server.py,sha256=UmP2jabcTKeUVGU0Z-PMvEnjU9tkJDx-qstigg6Y0E4,1203
-usearch-0.4.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-usearch-0.4.0.dist-info/METADATA,sha256=HIvAiyybAOkzMeB-vZPhzoTxNzO9uars7tWUtT_oxJc,19489
-usearch-0.4.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-usearch-0.4.0.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
-usearch-0.4.0.dist-info/RECORD,,
+usearch/server.py,sha256=bSgoM2fzltLvSA-gMknS80_JYFsOOXrMsWTWEgNiGIE,2748
+usearch-0.5.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+usearch-0.5.0.dist-info/METADATA,sha256=pxmfu5fCnaeZjpxlwXwbArHDPCmMYeuiaFBhdTDWFdc,19489
+usearch-0.5.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+usearch-0.5.0.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
+usearch-0.5.0.dist-info/RECORD,,
```

