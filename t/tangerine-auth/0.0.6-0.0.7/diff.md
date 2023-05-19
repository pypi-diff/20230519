# Comparing `tmp/tangerine_auth-0.0.6-py3-none-any.whl.zip` & `tmp/tangerine_auth-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9418 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      176 b- defN 23-May-19 04:49 tangerine_auth/__init__.py
--rw-rw-r--  2.0 unx      412 b- defN 23-May-19 04:49 tangerine_auth/__version__.py
--rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 04:49 tangerine_auth/key_lime.py
--rw-rw-r--  2.0 unx     4995 b- defN 23-May-19 04:49 tangerine_auth/yuzu.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 04:50 tangerine_auth-0.0.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx    12247 b- defN 23-May-19 04:50 tangerine_auth-0.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 04:50 tangerine_auth-0.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       68 b- defN 23-May-19 04:50 tangerine_auth-0.0.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 23-May-19 04:50 tangerine_auth-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      853 b- defN 23-May-19 04:50 tangerine_auth-0.0.6.dist-info/RECORD
-10 files, 21428 bytes uncompressed, 7948 bytes compressed:  62.9%
+Zip file size: 9421 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      176 b- defN 23-May-19 05:08 tangerine_auth/__init__.py
+-rw-rw-r--  2.0 unx      412 b- defN 23-May-19 05:08 tangerine_auth/__version__.py
+-rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 05:08 tangerine_auth/key_lime.py
+-rw-rw-r--  2.0 unx     4999 b- defN 23-May-19 05:08 tangerine_auth/yuzu.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 05:09 tangerine_auth-0.0.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    12247 b- defN 23-May-19 05:09 tangerine_auth-0.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 05:09 tangerine_auth-0.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       68 b- defN 23-May-19 05:09 tangerine_auth-0.0.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-19 05:09 tangerine_auth-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      853 b- defN 23-May-19 05:09 tangerine_auth-0.0.7.dist-info/RECORD
+10 files, 21432 bytes uncompressed, 7951 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tangerine_auth/key_lime.py
 Comment: 
 
 Filename: tangerine_auth/yuzu.py
 Comment: 
 
-Filename: tangerine_auth-0.0.6.dist-info/LICENSE
+Filename: tangerine_auth-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: tangerine_auth-0.0.6.dist-info/METADATA
+Filename: tangerine_auth-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: tangerine_auth-0.0.6.dist-info/WHEEL
+Filename: tangerine_auth-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: tangerine_auth-0.0.6.dist-info/entry_points.txt
+Filename: tangerine_auth-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.6.dist-info/top_level.txt
+Filename: tangerine_auth-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.6.dist-info/RECORD
+Filename: tangerine_auth-0.0.7.dist-info/RECORD
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
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 __author__ = 'Noraa Stoke'
 __author_email__ = 'noraa.july.stoke@gmail.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/noraa-july-stoke/yuzu'
```

## tangerine_auth/yuzu.py

```diff
@@ -143,10 +143,10 @@
             return wrapper
 
         return decorator
 
 
 
 
-    def logout(self):
+    def logout(self, ctx):
         self.auth = False
-        self.user = None
+        ctx.user = None
```

## Comparing `tangerine_auth-0.0.6.dist-info/LICENSE` & `tangerine_auth-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tangerine_auth-0.0.6.dist-info/METADATA` & `tangerine_auth-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangerine-auth
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tangerine Auth: An easy to use authentication manager for Tangerine and Flask.
 Home-page: https://github.com/noraa-july-stoke/yuzu
 Author: Noraa Stoke
 Author-email: noraa.july.stoke@gmail.com
 License: MIT
 Keywords: package development template
 Classifier: Development Status :: 4 - Beta
```

## Comparing `tangerine_auth-0.0.6.dist-info/RECORD` & `tangerine_auth-0.0.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tangerine_auth/__init__.py,sha256=toCPREZnXuu2V92GLi_nzATVzaQ3883Z_yrUXPXJFYQ,176
-tangerine_auth/__version__.py,sha256=8DfPRXXsFnyQpAs-34eGApvcEWSQlc2JeDolfXdMfiw,412
+tangerine_auth/__version__.py,sha256=Q5W55hLzFASWoG6PakCuIgOLIWON-t2Y_PJ_BwH2T1I,412
 tangerine_auth/key_lime.py,sha256=DdhUe4EyBcn7q9yQn1nmV7TiqoY38D-xtCoGB4_Yl0U,1502
-tangerine_auth/yuzu.py,sha256=Pwqw8Nrva2ya-zqUMkHyxgT7sjSjV0J4rbXqLxu5vuw,4995
-tangerine_auth-0.0.6.dist-info/LICENSE,sha256=eRYD4YdUmiZDtOxhZOWwXTSI1CokgEpp0eWHzea7oy8,1068
-tangerine_auth-0.0.6.dist-info/METADATA,sha256=SVlYeLEJwrV1mQXbgdYmYz9cTTvgEKVuydnIOSilrks,12247
-tangerine_auth-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tangerine_auth-0.0.6.dist-info/entry_points.txt,sha256=qTzSogO0ZlVKqQV5i4gnbewFBTu5XAR8xRzZTGQAJ3g,68
-tangerine_auth-0.0.6.dist-info/top_level.txt,sha256=kpS9rEx3_FHuAPPxUa1yYeXFxm3A25KHbchHVChRBoU,15
-tangerine_auth-0.0.6.dist-info/RECORD,,
+tangerine_auth/yuzu.py,sha256=11TVonww9uJ2ey9DU5ePMcwHPym5rPVYThv7B0Jg8JE,4999
+tangerine_auth-0.0.7.dist-info/LICENSE,sha256=eRYD4YdUmiZDtOxhZOWwXTSI1CokgEpp0eWHzea7oy8,1068
+tangerine_auth-0.0.7.dist-info/METADATA,sha256=u5Ys1hU_mIuiWZ7N4vtWdjccblpO0O1rWmObwR3XcPs,12247
+tangerine_auth-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tangerine_auth-0.0.7.dist-info/entry_points.txt,sha256=qTzSogO0ZlVKqQV5i4gnbewFBTu5XAR8xRzZTGQAJ3g,68
+tangerine_auth-0.0.7.dist-info/top_level.txt,sha256=kpS9rEx3_FHuAPPxUa1yYeXFxm3A25KHbchHVChRBoU,15
+tangerine_auth-0.0.7.dist-info/RECORD,,
```

