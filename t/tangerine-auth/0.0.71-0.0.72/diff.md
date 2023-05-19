# Comparing `tmp/tangerine_auth-0.0.71-py3-none-any.whl.zip` & `tmp/tangerine_auth-0.0.72-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9416 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      176 b- defN 23-May-19 13:17 tangerine_auth/__init__.py
--rw-rw-r--  2.0 unx      413 b- defN 23-May-19 13:17 tangerine_auth/__version__.py
--rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 13:17 tangerine_auth/key_lime.py
--rw-rw-r--  2.0 unx     4921 b- defN 23-May-19 13:17 tangerine_auth/yuzu.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 13:17 tangerine_auth-0.0.71.dist-info/LICENSE
--rw-rw-r--  2.0 unx    12272 b- defN 23-May-19 13:17 tangerine_auth-0.0.71.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 13:17 tangerine_auth-0.0.71.dist-info/WHEEL
--rw-rw-r--  2.0 unx       68 b- defN 23-May-19 13:17 tangerine_auth-0.0.71.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 23-May-19 13:17 tangerine_auth-0.0.71.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      859 b- defN 23-May-19 13:17 tangerine_auth-0.0.71.dist-info/RECORD
-10 files, 21386 bytes uncompressed, 7934 bytes compressed:  62.9%
+Zip file size: 9418 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      176 b- defN 23-May-19 13:20 tangerine_auth/__init__.py
+-rw-rw-r--  2.0 unx      413 b- defN 23-May-19 13:20 tangerine_auth/__version__.py
+-rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 13:20 tangerine_auth/key_lime.py
+-rw-rw-r--  2.0 unx     4921 b- defN 23-May-19 13:20 tangerine_auth/yuzu.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 13:21 tangerine_auth-0.0.72.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    12271 b- defN 23-May-19 13:21 tangerine_auth-0.0.72.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 13:21 tangerine_auth-0.0.72.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       68 b- defN 23-May-19 13:21 tangerine_auth-0.0.72.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-19 13:21 tangerine_auth-0.0.72.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      859 b- defN 23-May-19 13:21 tangerine_auth-0.0.72.dist-info/RECORD
+10 files, 21385 bytes uncompressed, 7936 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tangerine_auth/key_lime.py
 Comment: 
 
 Filename: tangerine_auth/yuzu.py
 Comment: 
 
-Filename: tangerine_auth-0.0.71.dist-info/LICENSE
+Filename: tangerine_auth-0.0.72.dist-info/LICENSE
 Comment: 
 
-Filename: tangerine_auth-0.0.71.dist-info/METADATA
+Filename: tangerine_auth-0.0.72.dist-info/METADATA
 Comment: 
 
-Filename: tangerine_auth-0.0.71.dist-info/WHEEL
+Filename: tangerine_auth-0.0.72.dist-info/WHEEL
 Comment: 
 
-Filename: tangerine_auth-0.0.71.dist-info/entry_points.txt
+Filename: tangerine_auth-0.0.72.dist-info/entry_points.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.71.dist-info/top_level.txt
+Filename: tangerine_auth-0.0.72.dist-info/top_level.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.71.dist-info/RECORD
+Filename: tangerine_auth-0.0.72.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tangerine_auth/__version__.py

```diff
@@ -3,12 +3,12 @@
 ~~~~~~~~~~~~~~
 
 Information about the current version of the py-package-template package.
 """
 
 __title__ = 'tangerine-auth'
 __description__ = 'Tangerine Auth: An easy to use authentication manager for Tangerine and Flask.'
-__version__ = '0.0.71'
+__version__ = '0.0.72'
 __author__ = 'Noraa Stoke'
 __author_email__ = 'noraa.july.stoke@gmail.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/noraa-july-stoke/yuzu'
```

## Comparing `tangerine_auth-0.0.71.dist-info/LICENSE` & `tangerine_auth-0.0.72.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tangerine_auth-0.0.71.dist-info/METADATA` & `tangerine_auth-0.0.72.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangerine-auth
-Version: 0.0.71
+Version: 0.0.72
 Summary: Tangerine Auth: An easy to use authentication manager for Tangerine and Flask.
 Home-page: https://github.com/noraa-july-stoke/yuzu
 Author: Noraa Stoke
 Author-email: noraa.july.stoke@gmail.com
 License: MIT
 Keywords: package development template
 Classifier: Development Status :: 4 - Beta
@@ -22,15 +22,15 @@
 Tangerine-Auth is a Python library that provides utilities for user authentication and secure handling of keys and encrypted data. It uses bcrypt for password hashing and JWT for token-based authentication.
 
 ## Installation
 
 Use pip to install the package:
 
 ```sh
-pip install tangerine-auths
+pip install tangerine-auth
 ```
 
 ## Usage
 
 ### Yuzu
 
 The general steps to integrating Yuzu into your application are as follows:
```

## Comparing `tangerine_auth-0.0.71.dist-info/RECORD` & `tangerine_auth-0.0.72.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tangerine_auth/__init__.py,sha256=toCPREZnXuu2V92GLi_nzATVzaQ3883Z_yrUXPXJFYQ,176
-tangerine_auth/__version__.py,sha256=tuegMMrklMHeM3_3GM3WnyHrgg39XlBtTWOm7tHdhc4,413
+tangerine_auth/__version__.py,sha256=9s6TGO8kwDJFxUxrh4saPxfD1gMEUyRDr9X-pN71AhY,413
 tangerine_auth/key_lime.py,sha256=DdhUe4EyBcn7q9yQn1nmV7TiqoY38D-xtCoGB4_Yl0U,1502
 tangerine_auth/yuzu.py,sha256=vNtDO2tUny7G3Gsk-3fkYwsJmFU2-r3gSVF_38BaqQQ,4921
-tangerine_auth-0.0.71.dist-info/LICENSE,sha256=eRYD4YdUmiZDtOxhZOWwXTSI1CokgEpp0eWHzea7oy8,1068
-tangerine_auth-0.0.71.dist-info/METADATA,sha256=GvCn4dI_mfWFYMxKhotKpgRc_FpmoYfAhuonCJRpcAU,12272
-tangerine_auth-0.0.71.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tangerine_auth-0.0.71.dist-info/entry_points.txt,sha256=qTzSogO0ZlVKqQV5i4gnbewFBTu5XAR8xRzZTGQAJ3g,68
-tangerine_auth-0.0.71.dist-info/top_level.txt,sha256=kpS9rEx3_FHuAPPxUa1yYeXFxm3A25KHbchHVChRBoU,15
-tangerine_auth-0.0.71.dist-info/RECORD,,
+tangerine_auth-0.0.72.dist-info/LICENSE,sha256=eRYD4YdUmiZDtOxhZOWwXTSI1CokgEpp0eWHzea7oy8,1068
+tangerine_auth-0.0.72.dist-info/METADATA,sha256=N3uQ9YTwM1D7jvdLqXl1XyZA7aKS21VzhxglwFyfGQg,12271
+tangerine_auth-0.0.72.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tangerine_auth-0.0.72.dist-info/entry_points.txt,sha256=qTzSogO0ZlVKqQV5i4gnbewFBTu5XAR8xRzZTGQAJ3g,68
+tangerine_auth-0.0.72.dist-info/top_level.txt,sha256=kpS9rEx3_FHuAPPxUa1yYeXFxm3A25KHbchHVChRBoU,15
+tangerine_auth-0.0.72.dist-info/RECORD,,
```

