# Comparing `tmp/biometeo-0.2.3-cp39-cp39-win_amd64.whl.zip` & `tmp/biometeo-0.2.4-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 574676 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   130560 b- defN 23-Jan-10 12:56 biometeo/Tmrt_utils.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  1282560 b- defN 23-Jan-10 12:56 biometeo/__init__.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1417 b- defN 23-Jan-10 12:56 biometeo-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jan-10 12:56 biometeo-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jan-10 12:56 biometeo-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      495 b- defN 23-Jan-10 12:56 biometeo-0.2.3.dist-info/RECORD
-6 files, 1415141 bytes uncompressed, 573786 bytes compressed:  59.5%
+Zip file size: 574670 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   130560 b- defN 23-May-18 17:10 biometeo/Tmrt_utils.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1282560 b- defN 23-May-18 17:09 biometeo/__init__.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1417 b- defN 23-May-18 17:10 biometeo-0.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-18 17:10 biometeo-0.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-18 17:10 biometeo-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      495 b- defN 23-May-18 17:10 biometeo-0.2.4.dist-info/RECORD
+6 files, 1415141 bytes uncompressed, 573780 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: biometeo/Tmrt_utils.cp39-win_amd64.pyd
 Comment: 
 
 Filename: biometeo/__init__.cp39-win_amd64.pyd
 Comment: 
 
-Filename: biometeo-0.2.3.dist-info/METADATA
+Filename: biometeo-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: biometeo-0.2.3.dist-info/WHEEL
+Filename: biometeo-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: biometeo-0.2.3.dist-info/top_level.txt
+Filename: biometeo-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: biometeo-0.2.3.dist-info/RECORD
+Filename: biometeo-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `biometeo-0.2.3.dist-info/METADATA` & `biometeo-0.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biometeo
-Version: 0.2.3
+Version: 0.2.4
 Summary: This package is applied to calculate thermal indicators for human biometeorology.  The available thermal indicators are Physiological Equivalent Temperature (PET), modified Physiological Equivalent Temperature (mPET), Predicted Mean Vote (PMV), Standard Effective Temperature* (SET*) and Universal Thermal Climate Index (UTCI) in this package.  An additional function named GlobalRadiation_Tmrt is appended in the package for applying G, N, and Omega to calculate Tmrt from part of original RayMan model code.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: numpy (>=1.19.2)
 Requires-Dist: Cython (>=0.29.28)
```

