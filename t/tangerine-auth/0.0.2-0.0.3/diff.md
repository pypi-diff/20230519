# Comparing `tmp/tangerine_auth-0.0.2-py3-none-any.whl.zip` & `tmp/tangerine_auth-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7598 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      212 b- defN 23-May-19 02:18 tangerine_auth/__init__.py
--rw-rw-r--  2.0 unx      412 b- defN 23-May-19 02:18 tangerine_auth/__version__.py
--rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 02:18 tangerine_auth/key_lime.py
--rw-rw-r--  2.0 unx     5162 b- defN 23-May-19 02:18 tangerine_auth/yuzu.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6130 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       68 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      852 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/RECORD
-10 files, 15513 bytes uncompressed, 6128 bytes compressed:  60.5%
+Zip file size: 9513 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      212 b- defN 23-May-19 03:44 tangerine_auth/__init__.py
+-rw-rw-r--  2.0 unx      412 b- defN 23-May-19 03:44 tangerine_auth/__version__.py
+-rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 03:44 tangerine_auth/key_lime.py
+-rw-rw-r--  2.0 unx     5228 b- defN 23-May-19 03:44 tangerine_auth/yuzu.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 03:44 tangerine_auth-0.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    12246 b- defN 23-May-19 03:44 tangerine_auth-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 03:44 tangerine_auth-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       68 b- defN 23-May-19 03:44 tangerine_auth-0.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-19 03:44 tangerine_auth-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      853 b- defN 23-May-19 03:44 tangerine_auth-0.0.3.dist-info/RECORD
+10 files, 21696 bytes uncompressed, 8043 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tangerine_auth/key_lime.py
 Comment: 
 
 Filename: tangerine_auth/yuzu.py
 Comment: 
 
-Filename: tangerine_auth-0.0.2.dist-info/LICENSE
+Filename: tangerine_auth-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: tangerine_auth-0.0.2.dist-info/METADATA
+Filename: tangerine_auth-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: tangerine_auth-0.0.2.dist-info/WHEEL
+Filename: tangerine_auth-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: tangerine_auth-0.0.2.dist-info/entry_points.txt
+Filename: tangerine_auth-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.2.dist-info/top_level.txt
+Filename: tangerine_auth-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.2.dist-info/RECORD
+Filename: tangerine_auth-0.0.3.dist-info/RECORD
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
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 __author__ = 'Noraa Stoke'
 __author_email__ = 'noraa.july.stoke@gmail.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/noraa-july-stoke/yuzu'
```

## tangerine_auth/yuzu.py

```diff
@@ -79,17 +79,17 @@
         # Extract the token from the request headers or cookies
         token = ctx.get_req_header("Authorization")
         user = None
         # Verify the token and get the user
         if token:
             user = self.verify_auth_token(token)
             ctx.auth = {"user": user}
+            print(ctx.get("user"), ctx.auth.user, "USER FORM JWT")
             next()  # Call next() only if the user is authenticated
 
-
     def sign_up(self, user_data: dict) -> dict:
         try:
             hashed = self.hash_func(user_data['password'].encode(), bcrypt.gensalt())
             user_data['password'] = hashed.decode()  # Convert bytes to string
 
             created_user = self.create_user(user_data)
```

## Comparing `tangerine_auth-0.0.2.dist-info/LICENSE` & `tangerine_auth-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tangerine_auth-0.0.2.dist-info/RECORD` & `tangerine_auth-0.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tangerine_auth/__init__.py,sha256=mnMCywfbZCBaqAePkqLrZ9sUBnXcPP7jntG5DRFcrq4,212
-tangerine_auth/__version__.py,sha256=lvndGtLMsDX1-L-x9AR_z_7-HgwKL2klz1GEZbrbYPY,412
+tangerine_auth/__version__.py,sha256=tQa3YTzT9ZIzXRKTop0HnCzgMAYXTgt4Gjj7Z5iw2T4,412
 tangerine_auth/key_lime.py,sha256=DdhUe4EyBcn7q9yQn1nmV7TiqoY38D-xtCoGB4_Yl0U,1502
-tangerine_auth/yuzu.py,sha256=vfs1uwDI0loGeDXufL0hpwiDd5hgHqZEHrjqRVmovnE,5162
-tangerine_auth-0.0.2.dist-info/LICENSE,sha256=eRYD4YdUmiZDtOxhZOWwXTSI1CokgEpp0eWHzea7oy8,1068
-tangerine_auth-0.0.2.dist-info/METADATA,sha256=DmPDc7M0Y0rJRKXMxZqljfkPz2cL5JjM1ahthWSlhkU,6130
-tangerine_auth-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tangerine_auth-0.0.2.dist-info/entry_points.txt,sha256=qTzSogO0ZlVKqQV5i4gnbewFBTu5XAR8xRzZTGQAJ3g,68
-tangerine_auth-0.0.2.dist-info/top_level.txt,sha256=kpS9rEx3_FHuAPPxUa1yYeXFxm3A25KHbchHVChRBoU,15
-tangerine_auth-0.0.2.dist-info/RECORD,,
+tangerine_auth/yuzu.py,sha256=PhikZHh9sSQTxVaFynKj-Fx1qeSnwJPYz50M9dPKzRU,5228
+tangerine_auth-0.0.3.dist-info/LICENSE,sha256=eRYD4YdUmiZDtOxhZOWwXTSI1CokgEpp0eWHzea7oy8,1068
+tangerine_auth-0.0.3.dist-info/METADATA,sha256=M6GjxaYV-izbJzxb9HjY_MVMBtbOnoLLXM7iRB92h-A,12246
+tangerine_auth-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tangerine_auth-0.0.3.dist-info/entry_points.txt,sha256=qTzSogO0ZlVKqQV5i4gnbewFBTu5XAR8xRzZTGQAJ3g,68
+tangerine_auth-0.0.3.dist-info/top_level.txt,sha256=kpS9rEx3_FHuAPPxUa1yYeXFxm3A25KHbchHVChRBoU,15
+tangerine_auth-0.0.3.dist-info/RECORD,,
```

