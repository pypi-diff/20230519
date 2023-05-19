# Comparing `tmp/teleapp-0.1.2-cp38-cp38-manylinux1_x86_64.whl.zip` & `tmp/teleapp-0.2.0-cp38-cp38-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 35155 bytes, number of entries: 11
+Zip file size: 35156 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-02 04:47 teleapp/__init__.py
 -rw-rw-r--  2.0 unx      354 b- defN 23-Apr-13 03:33 teleapp/teleapp.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-02 04:47 teleapp/cmd/__init__.py
--rwxrwxr-x  2.0 unx    65568 b- defN 23-Apr-13 08:38 teleapp/cmd/cmd.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx    65568 b- defN 23-May-19 10:33 teleapp/cmd/cmd.cpython-38-x86_64-linux-gnu.so
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-02 04:47 teleapp/const/__init__.py
--rwxrwxr-x  2.0 unx    28352 b- defN 23-Apr-13 08:38 teleapp/const/click_setting.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx      480 b- defN 23-Apr-13 08:38 teleapp-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx      108 b- defN 23-Apr-13 08:38 teleapp-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-Apr-13 08:38 teleapp-0.1.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-13 08:38 teleapp-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      915 b- defN 23-Apr-13 08:38 teleapp-0.1.2.dist-info/RECORD
-11 files, 95833 bytes uncompressed, 33583 bytes compressed:  65.0%
+-rwxrwxr-x  2.0 unx    28352 b- defN 23-May-19 10:33 teleapp/const/click_setting.cpython-38-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx      480 b- defN 23-May-19 10:33 teleapp-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      108 b- defN 23-May-19 10:33 teleapp-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 23-May-19 10:33 teleapp-0.2.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-May-19 10:33 teleapp-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      915 b- defN 23-May-19 10:33 teleapp-0.2.0.dist-info/RECORD
+11 files, 95833 bytes uncompressed, 33584 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: teleapp/const/__init__.py
 Comment: 
 
 Filename: teleapp/const/click_setting.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: teleapp-0.1.2.dist-info/METADATA
+Filename: teleapp-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: teleapp-0.1.2.dist-info/WHEEL
+Filename: teleapp-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: teleapp-0.1.2.dist-info/entry_points.txt
+Filename: teleapp-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: teleapp-0.1.2.dist-info/top_level.txt
+Filename: teleapp-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: teleapp-0.1.2.dist-info/RECORD
+Filename: teleapp-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `teleapp-0.1.2.dist-info/RECORD` & `teleapp-0.2.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 teleapp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 teleapp/teleapp.py,sha256=5Lv_u40NX-cuoiZmO0qm2yMrnos3iObvBvmmA345qro,354
 teleapp/cmd/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 teleapp/cmd/cmd.cpython-38-x86_64-linux-gnu.so,sha256=ZXU4WwEyM4jSyhztHcy2mFd7RsqM8mUf3MCJvk_Do78,65568
 teleapp/const/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 teleapp/const/click_setting.cpython-38-x86_64-linux-gnu.so,sha256=YiZKIPxbfAwUcpMG7bULjkQsWyOxeuu6D0phBSAvwdM,28352
-teleapp-0.1.2.dist-info/METADATA,sha256=bBK_N5ehu4MrRN7ZR8_vCwONlNAhlnbYt2IQgY9hUkY,480
-teleapp-0.1.2.dist-info/WHEEL,sha256=w1d_q2QQYYWFjc1BOr71GnX8BifSnUvEochN_fqB7tA,108
-teleapp-0.1.2.dist-info/entry_points.txt,sha256=H_uFG4ET9L8PlP15nQfr5cQjFPR6ZM77qAo2iOCB-_c,48
-teleapp-0.1.2.dist-info/top_level.txt,sha256=G3Rrxv-NGa5KIrAY1hyXAaB1atDue3_cmd_Xd4R_c-A,8
-teleapp-0.1.2.dist-info/RECORD,,
+teleapp-0.2.0.dist-info/METADATA,sha256=jm99tJiay9wBM71e7sGcNyquM1ovKc7PAYg7tpTN8mI,480
+teleapp-0.2.0.dist-info/WHEEL,sha256=w1d_q2QQYYWFjc1BOr71GnX8BifSnUvEochN_fqB7tA,108
+teleapp-0.2.0.dist-info/entry_points.txt,sha256=H_uFG4ET9L8PlP15nQfr5cQjFPR6ZM77qAo2iOCB-_c,48
+teleapp-0.2.0.dist-info/top_level.txt,sha256=G3Rrxv-NGa5KIrAY1hyXAaB1atDue3_cmd_Xd4R_c-A,8
+teleapp-0.2.0.dist-info/RECORD,,
```

