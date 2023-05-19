# Comparing `tmp/dummypkggg-0.0.1-py3-none-any.whl.zip` & `tmp/dummypkggg-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 2602 bytes, number of entries: 8
+Zip file size: 2801 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       38 b- defN 23-May-19 13:44 dummypkggg/__init__.py
 -rw-rw-r--  2.0 unx       51 b- defN 23-May-19 13:46 dummypkggg/c1.py
--rw-rw-r--  2.0 unx       51 b- defN 23-May-19 13:46 dummypkggg/c2.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-May-19 13:53 dummypkggg-0.0.1.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      480 b- defN 23-May-19 13:53 dummypkggg-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 13:53 dummypkggg-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-19 13:53 dummypkggg-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 23-May-19 13:53 dummypkggg-0.0.1.dist-info/RECORD
-8 files, 2419 bytes uncompressed, 1508 bytes compressed:  37.7%
+-rw-rw-r--  2.0 unx       51 b- defN 23-May-19 14:02 dummypkggg/c2.py
+-rw-rw-r--  2.0 unx       51 b- defN 23-May-19 14:02 dummypkggg/c3.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-19 14:05 dummypkggg-0.0.2.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      480 b- defN 23-May-19 14:05 dummypkggg-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 14:05 dummypkggg-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-19 14:05 dummypkggg-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      694 b- defN 23-May-19 14:05 dummypkggg-0.0.2.dist-info/RECORD
+9 files, 2541 bytes uncompressed, 1599 bytes compressed:  37.1%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: dummypkggg/c1.py
 Comment: 
 
 Filename: dummypkggg/c2.py
 Comment: 
 
-Filename: dummypkggg-0.0.1.dist-info/LICENCE.txt
+Filename: dummypkggg/c3.py
 Comment: 
 
-Filename: dummypkggg-0.0.1.dist-info/METADATA
+Filename: dummypkggg-0.0.2.dist-info/LICENCE.txt
 Comment: 
 
-Filename: dummypkggg-0.0.1.dist-info/WHEEL
+Filename: dummypkggg-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: dummypkggg-0.0.1.dist-info/top_level.txt
+Filename: dummypkggg-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: dummypkggg-0.0.1.dist-info/RECORD
+Filename: dummypkggg-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: dummypkggg-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dummypkggg-0.0.1.dist-info/LICENCE.txt` & `dummypkggg-0.0.2.dist-info/LICENCE.txt`

 * *Files identical despite different names*

