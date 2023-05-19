# Comparing `tmp/tangerine_auth-0.0.4-py3-none-any.whl.zip` & `tmp/tangerine_auth-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9504 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      176 b- defN 23-May-19 04:16 tangerine_auth/__init__.py
--rw-rw-r--  2.0 unx      412 b- defN 23-May-19 04:16 tangerine_auth/__version__.py
--rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 04:16 tangerine_auth/key_lime.py
--rw-rw-r--  2.0 unx     5228 b- defN 23-May-19 04:16 tangerine_auth/yuzu.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 04:16 tangerine_auth-0.0.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx    12246 b- defN 23-May-19 04:16 tangerine_auth-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 04:16 tangerine_auth-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       68 b- defN 23-May-19 04:16 tangerine_auth-0.0.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 23-May-19 04:16 tangerine_auth-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      853 b- defN 23-May-19 04:16 tangerine_auth-0.0.4.dist-info/RECORD
-10 files, 21660 bytes uncompressed, 8034 bytes compressed:  62.9%
+Zip file size: 9446 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      176 b- defN 23-May-19 04:34 tangerine_auth/__init__.py
+-rw-rw-r--  2.0 unx      412 b- defN 23-May-19 04:34 tangerine_auth/__version__.py
+-rw-rw-r--  2.0 unx     1502 b- defN 23-May-19 04:34 tangerine_auth/key_lime.py
+-rw-rw-r--  2.0 unx     5043 b- defN 23-May-19 04:34 tangerine_auth/yuzu.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 04:34 tangerine_auth-0.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    12247 b- defN 23-May-19 04:34 tangerine_auth-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 04:34 tangerine_auth-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       68 b- defN 23-May-19 04:34 tangerine_auth-0.0.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-19 04:34 tangerine_auth-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      853 b- defN 23-May-19 04:34 tangerine_auth-0.0.5.dist-info/RECORD
+10 files, 21476 bytes uncompressed, 7976 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tangerine_auth/key_lime.py
 Comment: 
 
 Filename: tangerine_auth/yuzu.py
 Comment: 
 
-Filename: tangerine_auth-0.0.4.dist-info/LICENSE
+Filename: tangerine_auth-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: tangerine_auth-0.0.4.dist-info/METADATA
+Filename: tangerine_auth-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: tangerine_auth-0.0.4.dist-info/WHEEL
+Filename: tangerine_auth-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: tangerine_auth-0.0.4.dist-info/entry_points.txt
+Filename: tangerine_auth-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.4.dist-info/top_level.txt
+Filename: tangerine_auth-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tangerine_auth-0.0.4.dist-info/RECORD
+Filename: tangerine_auth-0.0.5.dist-info/RECORD
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
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 __author__ = 'Noraa Stoke'
 __author_email__ = 'noraa.july.stoke@gmail.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/noraa-july-stoke/yuzu'
```

## tangerine_auth/yuzu.py

```diff
@@ -50,34 +50,32 @@
             return False
 
     def generate_auth_token(self, user_id: str, email: str) -> str:
         """
         The generate auth token class method generates an auth token.
         """
         secret_key = self.get_config("SECRET_KEY")
-        print("GENERATE AUTH TOKEN VARIABLES", user_id, email, secret_key)
         token_payload = {
             "user_id": user_id,
             "email": email,
             "exp": datetime.datetime.utcnow() + datetime.timedelta(hours=24)
         }
         return jwt.encode(token_payload, secret_key, algorithm='HS256')
 
 
     def verify_auth_token(self, token: str) -> dict:
         try:
             secret_key = self.get_config('SECRET_KEY')
             decoded_token = jwt.decode(token, secret_key, algorithms=['HS256'])
             return decoded_token
         except jwt.ExpiredSignatureError:
-            print("Token has expired")
-            return None
+            raise Exception("Token has expired")
         except jwt.InvalidTokenError:
-            print("Invalid token")
-            return None
+            raise Exception("Invalid token")
+
 
     def jwt_middleware(self, ctx, next) -> None:
         # Extract the token from the request headers or cookies
         token = ctx.get_req_header("Authorization")
         user = None
         # Verify the token and get the user
         if token:
@@ -106,20 +104,18 @@
 
 
     def login(self, email: str, password: str) -> Tuple[str, str]:
         print(self.authenticate(email, password))
         if self.authenticate(email, password):
             try:
                 user_data = self.get_user_by_email(email)
-                print(user_data)
 
                 if user_data:
                     self.auth = True
                     self.user = user_data
-                    print(self.user, "SELF.USER")
                     user_id = user_data.get('_id', user_data.get('id'))
                     token = self.generate_auth_token(str(user_id), email)
                     return str(user_id), token
                 else:
                     return None, None
 
             except Exception as e:
```

## Comparing `tangerine_auth-0.0.4.dist-info/LICENSE` & `tangerine_auth-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tangerine_auth-0.0.4.dist-info/METADATA` & `tangerine_auth-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangerine-auth
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tangerine Auth: An easy to use authentication manager for Tangerine and Flask.
 Home-page: https://github.com/noraa-july-stoke/yuzu
 Author: Noraa Stoke
 Author-email: noraa.july.stoke@gmail.com
 License: MIT
 Keywords: package development template
 Classifier: Development Status :: 4 - Beta
@@ -126,14 +126,15 @@
 - `sign_up(self, user_data: dict) -> dict`: Signs up a new user with the given user data.
 - `login(self, email: str, password: str) -> Tuple[str, str]`: Logs in a user with the given email and password.
 - `logout(self)`: Logs out the current user.
 - `jwt_middleware()`: Tangerine middleware for JWT authentication.
 - `flask_jwt_middleware(yuzu_instance)`: Flask middleware for JWT authentication.
 ```
 
+
 ### KeyLime
 
 KeyLime is a class that provides functionalities for securely handling keys and encrypted data.
 
 Below are the key methods of the KeyLime class:
 
 ```python
```

