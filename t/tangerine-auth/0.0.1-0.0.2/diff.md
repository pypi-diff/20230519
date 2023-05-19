# Comparing `tmp/tangerine_auth-0.0.1-py3-none-any.whl.zip` & `tmp/tangerine_auth-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10547 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      122 b- defN 23-May-18 22:36 tangerine_auth/__init__.py
--rw-rw-r--  2.0 unx      412 b- defN 23-May-18 22:36 tangerine_auth/__version__.py
--rw-rw-r--  2.0 unx     1502 b- defN 23-May-18 22:36 tangerine_auth/key_lime.py
--rw-rw-r--  2.0 unx     5009 b- defN 23-May-18 22:36 tangerine_auth/yuzu.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-May-18 22:37 tangerine_auth-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx    13859 b- defN 23-May-18 22:37 tangerine_auth-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-18 22:37 tangerine_auth-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       68 b- defN 23-May-18 22:37 tangerine_auth-0.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 23-May-18 22:37 tangerine_auth-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      853 b- defN 23-May-18 22:37 tangerine_auth-0.0.1.dist-info/RECORD
-10 files, 23000 bytes uncompressed, 9077 bytes compressed:  60.5%
+Zip file size: 7598 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      212 b- defN 23-May-19 02:18 tangerine_auth/__init__.py
+-rw-rw-r--  2.0 unx      412 b- defN 23-May-19 02:18 tangerine_auth/__version__.py
+-rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 02:18 tangerine_auth/key_lime.py
+-rw-rw-r--  2.0 unx     5162 b- defN 23-May-19 02:18 tangerine_auth/yuzu.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6130 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       68 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      852 b- defN 23-May-19 02:19 tangerine_auth-0.0.2.dist-info/RECORD
+10 files, 15513 bytes uncompressed, 6128 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tangerine_auth/key_lime.py
 Comment: 
 
 Filename: tangerine_auth/yuzu.py
 Comment: 
 
-Filename: tangerine_auth-0.0.1.dist-info/LICENSE
+Filename: tangerine_auth-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: tangerine_auth-0.0.1.dist-info/METADATA
+Filename: tangerine_auth-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: tangerine_auth-0.0.1.dist-info/WHEEL
+Filename: tangerine_auth-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: tangerine_auth-0.0.1.dist-info/entry_points.txt
+Filename: tangerine_auth-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.1.dist-info/top_level.txt
+Filename: tangerine_auth-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.1.dist-info/RECORD
+Filename: tangerine_auth-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tangerine_auth/__init__.py

```diff
@@ -1,5 +1,9 @@
 """
 tangerine_auth
 ~~~~~~
 The tangerine_auth package - An easy to use authentication manager for Tangerine and Flask.
 """
+
+from .yuzu import Yuzu
+from .key_lime import KeyLime
+from __version__ import __version__
```

## tangerine_auth/__version__.py

```diff
@@ -3,12 +3,12 @@
 ~~~~~~~~~~~~~~
 
 Information about the current version of the py-package-template package.
 """
 
 __title__ = 'tangerine-auth'
 __description__ = 'Tangerine Auth: An easy to use authentication manager for Tangerine and Flask.'
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 __author__ = 'Noraa Stoke'
 __author_email__ = 'noraa.july.stoke@gmail.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/noraa-july-stoke/yuzu'
```

## tangerine_auth/yuzu.py

```diff
@@ -1,28 +1,33 @@
 # ╦ ╦╦ ╦╔═╗╦ ╦
 # ╚╦╝║ ║╔═╝║ ║
 #  ╩ ╚═╝╚═╝╚═╝
 # File: yuzu.py
 # Description: This file contains the Auth class which is used to store the
 # auth status of a user. This is used to determine if a user is logged in
 # or not. And also provides the logic for logging in and out.
+
 import bcrypt
 import datetime
 # from tangerine.key_lime import KeyLime
 import jwt
 from typing import Tuple, Callable, Optional
 
 class Yuzu:
-    def __init__(self, keychain, get_user_by_email, create_user, hash_func: Optional[Callable] = None):
+    def __init__(self, keychain, get_user_by_email, create_user,
+                 hash_func: Optional[Callable] = bcrypt.hashpw,
+                 checkpw_func: Optional[Callable] = bcrypt.checkpw):
         self.keychain = keychain
         self.get_user_by_email = get_user_by_email
         self.create_user = create_user
         self.auth = False
         self.user = None
-        self.hash_func
+        self.hash_func = hash_func
+        self.checkpw_func = checkpw_func
+
 
     def get_config(self, key_name: str) -> str:
         return self.keychain.get_key(key_name)
 
     def setup_database(self):
         # Set up the database using self.db_connection_string
         pass
@@ -31,15 +36,15 @@
         # Set up other configurations using self.google_cloud or other configs from the keychain
         pass
 
     def authenticate(self, email: str, password: str) -> bool:
         try:
             user = self.get_user_by_email(email)
 
-            if user and bcrypt.checkpw(password.encode(), user['password'].encode()):
+            if user and self.checkpw_func(password.encode(), user['password'].encode()):
                 return True
             else:
                 return False
 
         except Exception as e:
             print(f'Error authenticating user: {e}')
             return False
@@ -79,15 +84,15 @@
             user = self.verify_auth_token(token)
             ctx.auth = {"user": user}
             next()  # Call next() only if the user is authenticated
 
 
     def sign_up(self, user_data: dict) -> dict:
         try:
-            hashed = bcrypt.hashpw(user_data['password'].encode(), bcrypt.gensalt())
+            hashed = self.hash_func(user_data['password'].encode(), bcrypt.gensalt())
             user_data['password'] = hashed.decode()  # Convert bytes to string
 
             created_user = self.create_user(user_data)
 
             if created_user:
                 user_id = created_user.get('_id', created_user.get('id'))
                 print(f'User created with id: {user_id}')
```

## Comparing `tangerine_auth-0.0.1.dist-info/LICENSE` & `tangerine_auth-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tangerine_auth-0.0.1.dist-info/RECORD` & `tangerine_auth-0.0.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tangerine_auth/__init__.py,sha256=f4vZT0k1wQY5np0D0-75C2Eh0t9s02KmxI1MpfkvvYk,122
-tangerine_auth/__version__.py,sha256=FjeU6m5uXp3HZSD63eluu0MWqBxjOb1MfB0bv5NRnCc,412
+tangerine_auth/__init__.py,sha256=mnMCywfbZCBaqAePkqLrZ9sUBnXcPP7jntG5DRFcrq4,212
+tangerine_auth/__version__.py,sha256=lvndGtLMsDX1-L-x9AR_z_7-HgwKL2klz1GEZbrbYPY,412
 tangerine_auth/key_lime.py,sha256=DdhUe4EyBcn7q9yQn1nmV7TiqoY38D-xtCoGB4_Yl0U,1502
-tangerine_auth/yuzu.py,sha256=J5kVOXvZy6BauwYHRHfViw_MscXNgoo__er5G9-mL8Y,5009
-tangerine_auth-0.0.1.dist-info/LICENSE,sha256=eRYD4YdUmiZDtOxhZOWwXTSI1CokgEpp0eWHzea7oy8,1068
-tangerine_auth-0.0.1.dist-info/METADATA,sha256=46UHiItghfFCZ43CRdXW5JA8B1ETpII7r1G2foyGjyQ,13859
-tangerine_auth-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tangerine_auth-0.0.1.dist-info/entry_points.txt,sha256=qTzSogO0ZlVKqQV5i4gnbewFBTu5XAR8xRzZTGQAJ3g,68
-tangerine_auth-0.0.1.dist-info/top_level.txt,sha256=kpS9rEx3_FHuAPPxUa1yYeXFxm3A25KHbchHVChRBoU,15
-tangerine_auth-0.0.1.dist-info/RECORD,,
+tangerine_auth/yuzu.py,sha256=vfs1uwDI0loGeDXufL0hpwiDd5hgHqZEHrjqRVmovnE,5162
+tangerine_auth-0.0.2.dist-info/LICENSE,sha256=eRYD4YdUmiZDtOxhZOWwXTSI1CokgEpp0eWHzea7oy8,1068
+tangerine_auth-0.0.2.dist-info/METADATA,sha256=DmPDc7M0Y0rJRKXMxZqljfkPz2cL5JjM1ahthWSlhkU,6130
+tangerine_auth-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tangerine_auth-0.0.2.dist-info/entry_points.txt,sha256=qTzSogO0ZlVKqQV5i4gnbewFBTu5XAR8xRzZTGQAJ3g,68
+tangerine_auth-0.0.2.dist-info/top_level.txt,sha256=kpS9rEx3_FHuAPPxUa1yYeXFxm3A25KHbchHVChRBoU,15
+tangerine_auth-0.0.2.dist-info/RECORD,,
```

