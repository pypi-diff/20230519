# Comparing `tmp/usearch-0.5.0-cp39-cp39-win_amd64.whl.zip` & `tmp/usearch-0.5.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 136379 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-18 22:39 usearch/__init__.py
--rw-rw-rw-  2.0 fat     1462 b- defN 23-May-18 22:39 usearch/client.py
--rw-rw-rw-  2.0 fat   284160 b- defN 23-May-18 22:47 usearch/index.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2298 b- defN 23-May-18 22:39 usearch/io.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-May-18 22:39 usearch/server.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    19489 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      770 b- defN 23-May-18 22:47 usearch-0.5.0.dist-info/RECORD
-10 files, 322593 bytes uncompressed, 135083 bytes compressed:  58.1%
+Zip file size: 136394 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-19 00:53 usearch/__init__.py
+-rw-rw-rw-  2.0 fat     1462 b- defN 23-May-19 00:53 usearch/client.py
+-rw-rw-rw-  2.0 fat   284160 b- defN 23-May-19 01:01 usearch/index.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2298 b- defN 23-May-19 00:53 usearch/io.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-May-19 00:53 usearch/server.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    19489 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      770 b- defN 23-May-19 01:01 usearch-0.5.1.dist-info/RECORD
+10 files, 322593 bytes uncompressed, 135098 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: usearch/io.py
 Comment: 
 
 Filename: usearch/server.py
 Comment: 
 
-Filename: usearch-0.5.0.dist-info/LICENSE
+Filename: usearch-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: usearch-0.5.0.dist-info/METADATA
+Filename: usearch-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: usearch-0.5.0.dist-info/WHEEL
+Filename: usearch-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: usearch-0.5.0.dist-info/top_level.txt
+Filename: usearch-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch-0.5.0.dist-info/RECORD
+Filename: usearch-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `usearch-0.5.0.dist-info/LICENSE` & `usearch-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `usearch-0.5.0.dist-info/METADATA` & `usearch-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usearch
-Version: 0.5.0
+Version: 0.5.1
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
-Metadata-Version: 2.1 Name: usearch Version: 0.5.0 Summary: Smaller & Faster
+Metadata-Version: 2.1 Name: usearch Version: 0.5.1 Summary: Smaller & Faster
 Single-File Vector Search Engine from Unum License: Apache-2.0 Classifier:
 Development Status :: 4 - Beta Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: C++ Classifier: Operating System :: MacOS Classifier:
```

## Comparing `usearch-0.5.0.dist-info/RECORD` & `usearch-0.5.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 usearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 usearch/client.py,sha256=bxfhEqgyrhb0ImT1e2uLiO-RKjq7cQZoIhNcR7fFGt8,1462
-usearch/index.cp39-win_amd64.pyd,sha256=A5Sv5aQNMrAHclgTlqxaq7VPm0WH99KIEttf9viJNXU,284160
+usearch/index.cp39-win_amd64.pyd,sha256=pQ8PUfZDFndlyOHXSjCTFJPO91PJ1jU9ZyxGL7XmZA0,284160
 usearch/io.py,sha256=xbieZtFNHPaG_1xFsoqQQdtuT_7s7DowdXK2BEphtzk,2298
 usearch/server.py,sha256=bSgoM2fzltLvSA-gMknS80_JYFsOOXrMsWTWEgNiGIE,2748
-usearch-0.5.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-usearch-0.5.0.dist-info/METADATA,sha256=pxmfu5fCnaeZjpxlwXwbArHDPCmMYeuiaFBhdTDWFdc,19489
-usearch-0.5.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-usearch-0.5.0.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
-usearch-0.5.0.dist-info/RECORD,,
+usearch-0.5.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+usearch-0.5.1.dist-info/METADATA,sha256=CuPGGRe2qXz-OW0D4t53p4A3t9MJrFu2ev3leNvf_Hg,19489
+usearch-0.5.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+usearch-0.5.1.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
+usearch-0.5.1.dist-info/RECORD,,
```

