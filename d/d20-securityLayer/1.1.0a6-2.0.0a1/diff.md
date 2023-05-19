# Comparing `tmp/d20-securityLayer-1.1.0a6.tar.gz` & `tmp/d20-securityLayer-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-1bo08q_5\d20-securityLayer-1.1.0a6.tar", last modified: Wed Mar  1 00:06:16 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-0f4f7sg2\d20-securityLayer-2.0.0a1.tar", last modified: Fri May 19 00:34:42 2023, max compression
```

## Comparing `d20-securityLayer-1.1.0a6.tar` & `d20-securityLayer-2.0.0a1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 00:06:16.318081 d20-securityLayer-1.1.0a6/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-1.1.0a6/LICENSE
--rw-rw-rw-   0        0        0      677 2023-03-01 00:06:16.317085 d20-securityLayer-1.1.0a6/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-1.1.0a6/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-1.1.0a6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-01 00:06:16.319082 d20-securityLayer-1.1.0a6/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-03-01 00:05:58.000000 d20-securityLayer-1.1.0a6/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-01 00:06:16.257081 d20-securityLayer-1.1.0a6/src/
-drwxrwxrwx   0        0        0        0 2023-03-01 00:06:16.288082 d20-securityLayer-1.1.0a6/src/d20_securityLayer.egg-info/
--rw-rw-rw-   0        0        0      677 2023-03-01 00:06:16.000000 d20-securityLayer-1.1.0a6/src/d20_securityLayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-03-01 00:06:16.000000 d20-securityLayer-1.1.0a6/src/d20_securityLayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 00:06:16.000000 d20-securityLayer-1.1.0a6/src/d20_securityLayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-03-01 00:06:16.000000 d20-securityLayer-1.1.0a6/src/d20_securityLayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-01 00:06:16.000000 d20-securityLayer-1.1.0a6/src/d20_securityLayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-01 00:06:16.315081 d20-securityLayer-1.1.0a6/src/securityLayer/
--rw-rw-rw-   0        0        0    10496 2023-01-02 23:21:42.000000 d20-securityLayer-1.1.0a6/src/securityLayer/AccessControl.py
--rw-rw-rw-   0        0        0      238 2021-09-23 21:53:33.000000 d20-securityLayer-1.1.0a6/src/securityLayer/AuthAnswer.py
--rw-rw-rw-   0        0        0     7293 2022-01-13 00:21:13.000000 d20-securityLayer-1.1.0a6/src/securityLayer/Error.py
--rw-rw-rw-   0        0        0    19774 2023-02-02 02:02:52.000000 d20-securityLayer-1.1.0a6/src/securityLayer/SSO.py
--rw-rw-rw-   0        0        0    23271 2023-03-01 00:05:31.000000 d20-securityLayer-1.1.0a6/src/securityLayer/SecurityLayer.py
--rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-1.1.0a6/src/securityLayer/__init__.py
--rw-rw-rw-   0        0        0      161 2023-02-28 23:57:27.000000 d20-securityLayer-1.1.0a6/src/securityLayer/__version__.py
--rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-1.1.0a6/src/securityLayer/default.py
+drwxrwxrwx   0        0        0        0 2023-05-19 00:34:42.012267 d20-securityLayer-2.0.0a1/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a1/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-05-19 00:34:42.011299 d20-securityLayer-2.0.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a1/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 00:34:42.012267 d20-securityLayer-2.0.0a1/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-05-19 00:34:24.000000 d20-securityLayer-2.0.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 00:34:41.670903 d20-securityLayer-2.0.0a1/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 00:34:41.820267 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 00:34:42.009262 d20-securityLayer-2.0.0a1/src/securityLayer/
+-rw-rw-rw-   0        0        0    10081 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a1/src/securityLayer/AccessControl.py
+-rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a1/src/securityLayer/AuthAnswer.py
+-rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a1/src/securityLayer/Error.py
+-rw-rw-rw-   0        0        0    16923 2023-05-16 03:11:04.000000 d20-securityLayer-2.0.0a1/src/securityLayer/SSO.py
+-rw-rw-rw-   0        0        0    15241 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a1/src/securityLayer/SecurityLayer.py
+-rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a1/src/securityLayer/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-05-12 02:57:34.000000 d20-securityLayer-2.0.0a1/src/securityLayer/__version__.py
+-rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a1/src/securityLayer/default.py
```

### Comparing `d20-securityLayer-1.1.0a6/LICENSE` & `d20-securityLayer-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-1.1.0a6/PKG-INFO` & `d20-securityLayer-2.0.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 1.1.0a6
+Version: 2.0.0a1
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-1.1.0a6/src/d20_securityLayer.egg-info/PKG-INFO` & `d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 1.1.0a6
+Version: 2.0.0a1
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-1.1.0a6/src/securityLayer/AccessControl.py` & `d20-securityLayer-2.0.0a1/src/securityLayer/AccessControl.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from future.utils import raise_
 from .SecurityLayer import SecurityLayer
+from .AuthAnswer import AuthAnswer
 from cryptography.fernet import Fernet
 from .Error import *
 import os
 import json
 from .default import crypt as D20_SL_CRYPTOKEY
 
 def api_back_auth(request=None, **kwargs):
@@ -16,44 +17,56 @@
         jr.update(request.form)
     except:
         pass
     if request != None and request.method != 'GET' and request.get_json() != None:
         jr.update(request.get_json())
     if request.headers.get('Authorization', '').split(" ")[0].upper() == 'BEARER':
         token_id = request.headers.get('Authorization').split(" ")[1]
-        token = SecurityLayer.AccessToken('find', {'_key':token_id, 'origin' : request.headers.get('origin',request.headers.get('referer',''))})
+        token = SecurityLayer.AccessToken(data= {'_key':token_id, 'origin' : request.headers.get('origin',request.headers.get('referer',''))})
+        try:
+            token.find()
+        except HTTPError as e:
+            AuthAnswer(False, error= e())
     elif request.headers.get('Authorization', '').split(" ")[0].upper() == 'BASIC':
         jr['apiuser'] = request.authorization.get('username')
         jr['apisecret'] = request.authorization.get('password')
         jr['origin'] = request.headers.get('origin',request.headers.get('referer',''))
         jr['permalink'] = kwargs.get('permalink', False)
         if jr.get('permalink', False) == True:
             jr['permalink'] = jr.get('permalink', False)
             jr['origin'] = jr.get('permalink_origin', jr['origin'])
         jr['oauth'] = kwargs.get('oauth', False)
-        token = SecurityLayer.AccessToken('auth', jr)
+        token = SecurityLayer.AccessToken(data=jr)
+        try:
+            token.auth()
+        except HTTPError as e:
+            AuthAnswer(False, error= e())
     elif (kwargs.get('oauth', False) == True or kwargs.get('file_req', False) == True) and request.args.get('client_id', '') != '':
         token_id = request.args.get('client_id', '')
-        token = SecurityLayer.AccessToken('find', {'_key':token_id, 'origin' : request.headers.get('origin',request.headers.get('referer',''))})
+        token = SecurityLayer.AccessToken(data= {'_key':token_id, 'origin' : request.headers.get('origin',request.headers.get('referer',''))})
+        try:
+            token.find()
+        except HTTPError as e:
+            AuthAnswer(False, error= e())
     else:
-        return {'res': False, 'error': SSONoCredentialsError()}
+        return AuthAnswer(False, error= SSONoCredentialsError())
     if token.get('_key') == None:
-        return {'res': False, 'error': SSOInvalidCredentialsError()}
+        return AuthAnswer(False, error= SSOInvalidCredentialsError())
     if jr.get('permalink', False) == True and 'pl' not in token.get('actions') and 'sso' not in token.get('actions'):
-        return {'res': False, 'error': SSONoPermalinksAllowedError()}
+        return AuthAnswer(False, error= SSONoPermalinksAllowedError())
     if 'action' in kwargs:
         if action_clearance(token, kwargs.get('action'),  jr=jr) != True:
-            return {'res': False, 'error': SSOAccessDeniedError(kwargs.get('action'))}
+            return AuthAnswer(False, error=  SSOAccessDeniedError(kwargs.get('action')))
     if 'clearance' in kwargs:
         if access_clearance(token, kwargs.get('clearance'), request.method, jr=jr) != True:
-            return {'res': False, 'error': SSOAccessDeniedError(kwargs.get('clearance'), request.method)}
+            return AuthAnswer(False, error=   SSOAccessDeniedError(kwargs.get('clearance'), request.method))
     if 'object_action' in kwargs:
         if object_action_clearance(token, kwargs.get('object_action'), request.method, jr=jr) != True:
-            return {'res': False, 'error': SSOAccessDeniedError(kwargs.get('clearance'), request.method)}
-    return {'res': True, 'token': token}
+            return AuthAnswer(False, error=   SSOAccessDeniedError(kwargs.get('clearance'), request.method))
+    return AuthAnswer(True, token=token)
 
 def user_back_auth(request=None, **kwargs):
     jr={}
     try:
         jr.update(kwargs.get('jr', {}))
     except:
         pass
@@ -63,44 +76,54 @@
         pass
     if request != None and request.method != 'GET' and request.get_json() != None:
         jr.update(request.get_json())
     access_code = request.headers.get('Oauth-Token', request.headers.get('Access-Token', jr.get('Oauth-Token', jr.get('access_token', request.args.get('user_token', '')))))
     token_id = request.headers.get('UserToken', jr.get('UserToken', ''))
     user_id = request.headers.get('UserId', kwargs.get('UserId', jr.get('UserId', jr.get('_key', ''))))
     if token_id != '':
-        token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': user_id})
+        token = SecurityLayer.UserToken(data={'_key': token_id, 'userid': user_id})
+        try:
+            token.find()
+        except HTTPError as e:
+            AuthAnswer(False, error= e())
     elif jr.get('password', '') != '':
-        token = SecurityLayer.UserToken('auth', jr)
-        if token.get('status') != True:
-            return {'res': False, 'error': SSOInvalidCredentialsError()}
+        token = SecurityLayer.UserToken(data=jr)
+        try:
+            token.auth()
+        except HTTPError as e:
+            AuthAnswer(False, error= e())
     elif jr.get('otp', '') != '':
         jr['password']=jr.get('otp', '')
-        token = SecurityLayer.UserToken('auth', jr)
-        if token.get('status') != True:
+        token = SecurityLayer.UserToken(data=jr)
+        try:
+            token.auth()
+        except HTTPError:
             token_id = jr.get('otp')
-            otp = SecurityLayer.OneTimeAccess('find', {'_key': token_id, 'username': jr['username']})
-            if otp.get('status') == True:
-                token = SecurityLayer.UserToken('create', {'username': jr.get('username'), 'oauth': jr.get('oauth'), 'oauth_client': token.get('apiuser'), 'scopes': jr.get('scopes'), 'userid': otp.get('userid')})
-            else:
-                return {'res': False, 'error': SSOInvalidCredentialsError()}
+            otp = SecurityLayer.OneTimeAccess(data= {'_key': token_id, 'username': jr['username']})
+            try:
+                otp.find()
+                token = SecurityLayer.UserToken(data={'username': jr.get('username'), 'oauth': jr.get('oauth'), 'oauth_client': token.get('apiuser'), 'scopes': jr.get('scopes'), 'userid': otp.get('userid')})
+                token.create()
+            except HTTPError as e:
+                AuthAnswer(False, error= e())           
     elif (kwargs.get('oauth', False) == True or kwargs.get('TPAMI', False) == True or kwargs.get('file_req', False) == True) and access_code != '':
         try:
             token = break_access_token(access_code)
         except:
-            return {'res': False, 'error': SSOInvalidUserTokenError()}
+            return AuthAnswer(False, error= SSOInvalidUserTokenError())
         # token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
         if token.get('status') != True:
-            return {'res': False, 'error': SSOInvalidUserTokenError()}
+            return AuthAnswer(False, error= SSOInvalidUserTokenError())
     else:
-        return {'res': False, 'error': SSONoCredentialsError()}
+        return AuthAnswer(False, error= SSONoCredentialsError())
     if token.get("_key", None) == None:
-        return {'res': False, 'error': SSOInvalidUserTokenError()}
+        return AuthAnswer(False, error= SSOInvalidUserTokenError())
     if token.get('delegated', None) != None and delegated_clearance(token, request.method) != True:
-        return {'res': False, 'error': SSOInvalidUserTokenError()}
-    return {'res': True, 'token': token}
+        return AuthAnswer(False, error= SSOInvalidUserTokenError())
+    return AuthAnswer(True, token=token)
 
 def access_clearance(api_token: SecurityLayer.AccessToken, obj_type: str, action: str, **kwargs) -> bool:
     if not obj_type in api_token.get('allowed_types'):
         return False
     if action == 'PUT':
         permission = 'create'
     elif action == 'DELETE':
@@ -147,83 +170,66 @@
 
 def action_user(user_token: SecurityLayer.UserToken, **kwargs) -> str:
     return user_token.get('delegated', user_token.get('userid'))
 
 def gen_access_token(user_token: SecurityLayer.UserToken, **kwargs) -> str:
     userid = user_token.get('userid')
     tokenid = user_token.get('_key')
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
     f = Fernet(crypt)
     access_token = f.encrypt(bytes(f'{userid}.{tokenid}', 'utf-8')).decode()
     return access_token
 
 def break_access_token(access_token:str) -> SecurityLayer.UserToken:
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
     f = Fernet(crypt)
     userid, token_id = f.decrypt(bytes(access_token, 'utf-8')).decode().split('.')
-    token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
+    token = SecurityLayer.UserToken(data={'_key': token_id, 'userid': userid})
+    token.find()
     return token
 
 def gen_refresh_token(user_token: SecurityLayer.UserToken, **kwargs) -> str:
     userid = user_token.get('userid')
     tokenid = user_token.get('_key')
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
     f = Fernet(crypt)
     access_token = f.encrypt(bytes(f'{tokenid}.{userid}', 'utf-8')).decode()
     return access_token
 
 def break_refresh_token(access_token:str) -> SecurityLayer.UserToken:
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
     f = Fernet(crypt)
     token_id, userid = f.decrypt(bytes(access_token, 'utf-8')).decode().split('.')
-    token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
+    token = SecurityLayer.UserToken(data={'_key': token_id, 'userid': userid})
+    token.find()
     return token
 
 def api_access_from_token(api_token: SecurityLayer.AccessToken) -> SecurityLayer.APIAccess:
-    credentials = SecurityLayer.APIAccess('fetch_exact', {'username':api_token.get('apiuser')}).found
-    if credentials == None or len(credentials) == 0:
-        raise ObjectNotFoundException
-    api_access = SecurityLayer.APIAccess('find', {'_key' : credentials[0].get('_key')})
+    api_access = SecurityLayer.APIAccess(data={'username':api_token.get('apiuser')})
+    api_access.load_multikey(['username'])
     return api_access
 
 def gen_password_token(user_token: SecurityLayer.UserToken, **kwargs) -> str:
     userid = user_token.get('userid')
     tokenid = user_token.get('_key')
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
     f = Fernet(crypt)
     access_token = f.encrypt(bytes(f'passwordrec.{tokenid}.{userid}', 'utf-8')).decode()
     return access_token
 
 def break_password_token(access_token:str) -> SecurityLayer.UserToken:
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
     f = Fernet(crypt)
     val, userid, token_id = f.decrypt(bytes(access_token, 'utf-8')).decode().split('.')
     if val != 'passwordrec':
         raise ObjectNotFoundException
-    token = SecurityLayer.PasswordRecoveryToken('find', {'_key': token_id, 'userid': userid})
+    token = SecurityLayer.PasswordRecoveryToken(data={'_key': token_id, 'userid': userid})
+    token.find()
     return token
```

### Comparing `d20-securityLayer-1.1.0a6/src/securityLayer/Error.py` & `d20-securityLayer-2.0.0a1/src/securityLayer/Error.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 
 class ObjectNotFoundException(Exception):
     
     def __init__(self, message="Not found."):
         self.message = message
         super().__init__(self.message)
 
-class Error():
+class Error(Exception):
     """ Base class for errors. 
         Holds basic error structure: name, hint, message """
 
     def __init__(self, id="", name="", hint="", message="") -> None:
         self.id = id
         self.name = name
         self.hint = hint
         self.message = message
+        super().__init__(self.message)
 
     def to_dict(self):
         dict = {'name':self.name, 'hint':self.hint, 'message':self.message, 'id':self.id}
         return dict
 
 class HTTPError(Error):
     """ Base class for HTTP Errors. Extends Error and adds code """
@@ -80,16 +81,17 @@
         self.message = 'The server ran into an unexpected error, we are already working on it'
         self.code = 500
         super().__init__(self.id, self.name, self.hint, self.message, self.code)
 
 class SSOError(HTTPError):
     """ Generic error for SSO endpoints """
 
-    def __init__(self, id="", name="", hint="", message="", code=500, back_url_params="server_error") -> None:
+    def __init__(self, id="", name="", sso_error="", hint="", message="", code=500, back_url_params="server_error") -> None:
         self.id = id
+        self.sso_error = sso_error
         self.name = name
         self.hint = hint
         self.message = message
         self.code = code
         self.back_url_params = back_url_params
         super().__init__(self.id, self.name, self.hint, self.message, self.code)
 
@@ -135,18 +137,32 @@
         super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
     
 class SSOAccessDeniedError(SSOError):
     """ Scope not authorized for object-action combination """
 
     def __init__(self, obj_type = "", action = "") -> None:
         self.id = 'sso_access_denied'
+        self.sso_error = 'access_denied'
         self.name = 'Action access not granted'
         self.hint = f'Check your scopes for this object type and action: {obj_type} | {action}'
         self.message = f'User is not allowed to {action} on {obj_type}'
-        self.code = 401
+        self.code = 403
+        self.back_url_params = 'error=client_id'
+        super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
+        
+class SSOScopeError(SSOError):
+    """ Scope not authorized """
+
+    def __init__(self) -> None:
+        self.id = 'sso_invalid_scope'
+        self.sso_error = 'invalid_scope'
+        self.name = 'Scope is invalid'
+        self.hint = f'Check your scopes are in the right format and grant'
+        self.message = f'Requested scope is invalid for credentials supplied'
+        self.code = 403
         self.back_url_params = 'error=client_id'
         super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
     
 class SSOInvalidUserTokenError(SSOError):
     """ The user token provided is not valid """
 
     def __init__(self) -> None:
@@ -159,14 +175,15 @@
         super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
     
 class SSOInvalidRequestError(SSOError):
     """ The request format or attributes are not valid """
 
     def __init__(self) -> None:
         self.id = 'sso_invalid_request'
+        self.sso_error = 'invalid_request'
         self.name = 'Invalid request'
         self.hint = 'Check the attributes and parameters and try again'
         self.message = 'The structure of the request is no valid'
         self.code = 400
         self.back_url_params = 'error=invalid_request'
         super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
     
@@ -177,8 +194,49 @@
         self.id = 'sso_invalid_token'
         self.name = 'Invalid  token'
         self.hint = 'Check the validity of the token provided'
         self.message = 'The  token provided is not valid'
         self.code = 401
         self.back_url_params = 'error=invalid_token'
         super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
+    
+class SSOInvalidGrantError(SSOError):
+    """ The grant provided is not valid """
+
+    def __init__(self) -> None:
+        self.id = 'sso_invalid_grant'
+        self.sso_error = 'invalid_grant'
+        self.name = 'Invalid  grant'
+        self.hint = 'Check the grant required'
+        self.message = 'The  grant provided is not valid'
+        self.code = 403
+        self.back_url_params = 'error=invalid_grant'
+        super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
+
+class SSOUnsupportedGrantError(SSOError):
+    """ The grant provided is not valid """
+
+    def __init__(self) -> None:
+        self.id = 'sso_unsupported_grant_type'
+        self.sso_error = 'unsupported_grant_type'
+        self.name = 'Unsupported  grant'
+        self.hint = 'Check the grant required'
+        self.message = 'The  grant provided is not valid'
+        self.code = 403
+        self.back_url_params = 'error=unsupported_grant_type'
+        super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
+
+    
+    
+class SSOReturnURLError(SSOError):
+    """ The return url provided is not valid """
+
+    def __init__(self) -> None:
+        self.id = 'sso_invalid_return_url'
+        self.sso_error = 'invalid_client'
+        self.name = 'Return URL not listed'
+        self.hint = 'Check configured return URLs and make sure to supply a valid one'
+        self.message = 'The return URL provided is not listed as valid'
+        self.code = 401
+        self.back_url_params = 'error=invalid_client'
+        super().__init__(self.id, self.name, self.hint, self.message, self.code, self.back_url_params)
```

### Comparing `d20-securityLayer-1.1.0a6/src/securityLayer/SSO.py` & `d20-securityLayer-2.0.0a1/src/securityLayer/SSO.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,401 +1,342 @@
 from .SecurityLayer import SecurityLayer
 from .AccessControl import *
 from .Error import *
 from dtwentyORM import Metadata
 from dtwentyCommunications import Communications
 from flask import request, redirect, url_for
+from .AuthAnswer import AuthAnswer
 import json
 import datetime
 from .default import crypt as D20_SL_CRYPTOKEY
 
 
 def sso_authorize(user_id='', auth_token='',token={},grant_type='',state='',scopes='',redirect_uri='', code='', refresh_token='',mode='', lifespawn=10):
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
     if grant_type == 'auth':
         if not redirect_uri in token.get('oauth_urls') and max([redirect_uri.find(url) for url in token.get('oauth_urls')]) != 0:
-            return {'error': 'invalid_client', 'error_num':401}
+            return AuthAnswer(False, error=   SSOReturnURLError())
         if len(scopes) <= 0:
-            return {'error': 'access_denied', 'error_num':403}
+            return AuthAnswer(False, error=   SSOScopeError())
         for scope in scopes:
             if not scope in token.get('oauth_scopes'):
                 scopes.pop(scopes.index(scope))
         if len(scopes) <= 0:
-            return {'error': 'invalid_scope', 'error_num':403}
-        user_token = SecurityLayer.UserToken('find', {'_key': auth_token, 'userid': user_id})
-        if user_token.get('status') != True:
-            return {'error': 'unauthorized_client', 'error_num': 401}
+            return AuthAnswer(False, error=   SSOScopeError())
+        user_token = SecurityLayer.UserToken(data={'_key': auth_token, 'userid': user_id})
+        user_token.find()
         code = f'{user_id}.{auth_token}'
         rcode = f'{auth_token}.{user_id}'
         f = Fernet(crypt) 
         if mode == '0': # Implicit
             access_token = f.encrypt(bytes(code, 'utf-8')).decode()
             refresh_token = f.encrypt(bytes(rcode, 'utf-8')).decode()
             token_dict = {
                "access_token":access_token,
                 "token_type":"Oauth-Token",
                 "expires_in":lifespawn*59,
                 "refresh_token":refresh_token,
                 "state":state,
                 "scope":' '.join(scopes)
             }
-            return token_dict
-            # url_params = '&'.join([f'{key}={token_dict[key]}' for key in token_dict])
-            # return {'redirect_uri' : f'{redirect_uri}?{url_params}' }
+            return AuthAnswer(True, token=   token_dict)
         else:
             token_challenge = f.encrypt(bytes(f'challenge.{code}', 'utf-8')).decode()
             code_dict = {
                 "state":state,
                 "scope":' '.join(scopes),
                 "code":token_challenge
             }
-            return code_dict
-            # return {'redirect_uri': f'{redirect_uri}?state={state}&code={token_challenge}' }
+            return AuthAnswer(True, token=   code_dict)
     elif grant_type == 'code' or grant_type == 'authorization_code':
         if code == '':
-            return {'error': 'invalid_request', 'error_num': 401}
+            return AuthAnswer(False, error=   SSOInvalidRequestError())
         f = Fernet(crypt)
         try:
             val, user_id, auth_token = f.decrypt(bytes(code, 'utf-8')).decode().split('.')
         except:
             val = 'error'
         if val != 'challenge':
-            return {'error': 'invalid_grant', 'error_num': 403}
-        user_token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': user_id})
+            return AuthAnswer(False, error=   SSOInvalidGrantError())
+        user_token = SecurityLayer.UserToken(data={'_key': token_id, 'userid': user_id})
+        user_token.find()
         if user_token.get('status') != True:
-            return {'error': 'invalid_grant', 'error_num': 403}
+            return AuthAnswer(False, error=   SSOInvalidGrantError())
         rtoken = f.encrypt(bytes(f'{token_id}.{user_id}', 'utf-8')).decode()
         code = f.encrypt(bytes(f'{user_id}.{token_id}', 'utf-8')).decode()
-        return {
+        code_dict= {
             "access_token":code,
             "token_type":"Oauth-Token",
             "expires_in":lifespawn*59,
             "refresh_token":rtoken,
         }
+        return AuthAnswer(True, token=   code_dict)
     elif grant_type == 'refresh_token':
         if 'refresh_token' == '' or 'refresh_token' == None:
-            return {'error': 'invalid_request', 'error_num': 400}
+            return AuthAnswer(False, error=   SSOInvalidRequestError())
         f = Fernet(crypt)
         try:
             token_id, user_id = f.decrypt(bytes(refresh_token, 'utf-8')).decode().split('.')
         except:
-            return {'error': 'invalid_grant', 'error_num': 400}
-        user_token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': user_id, 'oauth': True})
+            return AuthAnswer(False, error=   SSOInvalidGrantError())
+        user_token = SecurityLayer.UserToken(data={'_key': token_id, 'userid': user_id, 'oauth': True})
+        user_token.find()
         if user_token.get('status') != True:
-            return {'error': 'invalid_grant', 'error_num':400}
+            return AuthAnswer(False, error=   SSOInvalidGrantError())
         code = f.encrypt(bytes(f'{user_id}.{token_id}', 'utf-8')).decode()
         rtoken = f.encrypt(bytes(f'{token_id}.{user_id}', 'utf-8')).decode()
-        return {
+        code_dict= {
             "access_token":code,
             "token_type":"bearer",
             "expires_in":lifespawn*59,
             "refresh_token":rtoken,
         }
+        return AuthAnswer(True, token=   code_dict)
     else:
-        return {'error': 'unsupported_grant_type', 'error_num': 401 }
+        return AuthAnswer(False, error=   SSOUnsupportedGrantError())
 
 
 
-def sso_password_reset(**kwargs):
-    jr = kwargs.get('jr')
-    if not 'token' in jr or not 'password' in jr:
-        return SSOInvalidRequestError().make_error()
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+def sso_password_reset(token, password):
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
     f = Fernet(crypt)
     try:
-        val, userid, token_id = f.decrypt(bytes(jr['token'], 'utf-8')).decode().split('.')
+        val, userid, token_id = f.decrypt(bytes(token, 'utf-8')).decode().split('.')
     except:
         val = 'error'
     if val != 'passwordrec':
-        return SSOInvalidTokenError().make_error()
-    # TODO: destroying at first try generates non-second changes
-    token = SecurityLayer.PasswordRecoveryToken('find', {'_key': token_id, 'userid': userid})
-    if token.get('status') != True:
-        return SSOInvalidTokenError().make_error()
-    access = SecurityLayer.UserAccess('update', {'_key': userid, 'password':jr.get('password')})
-    # Differenciate between no change and error
-    # if access.get('status') != True:
-    #     return UnexpectedError().make_error()
-    act_token = SecurityLayer.UserToken('create', {'userid':userid})
+        return AuthAnswer(False, error=   SSOInvalidTokenError())
+    token = SecurityLayer.PasswordRecoveryToken(data={'_key': token_id, 'userid': userid})
+    token.find()
+    access = SecurityLayer.UserAccess()
+    access.load(userid)
+    access.password=password
+    access.update()
+    act_token = SecurityLayer.UserToken()
+    act_token.userid = userid
+    act_token.create()
     tokenid = act_token.get('_key')
-    p = Metadata.Parameter('find', {'_key' : 'reset_password_redirect'})
-    redir_uri = jr.get('redir_uri', p.get('value'))
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
     f = Fernet(crypt)
     refresh_token = f.encrypt(bytes(f'{tokenid}.{userid}', 'utf-8')).decode()
     access_token = f.encrypt(bytes(f'{userid}.{tokenid}', 'utf-8')).decode()
-    oauth_params = f'access_token={access_token}&refresh_token={refresh_token}'
-    return jsonify({'res': True, 'redirect_uri': f'{redir_uri}?{oauth_params}'})
+    token = {'access_token':access_token, 'refresh_token':refresh_token}
+    return AuthAnswer(True, token=   token)
     
-def oauth_sendpasswordrecovery(welcome = False):
-    auth = api_back_auth(request, oauth=True)
-    if auth.get('res') == False:
-        return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
-    atoken = auth.get('token')
-    if atoken.get('oauth') != True or not 'auth' in atoken.get('actions'):
-        return jsonify({'error': 'unauthorized_client'}), 401
-    jr = request.get_json()
-    m = Core.User('find', {'username': jr.get('username')})
-    if m.get('status') != True:
-        return jsonify("Member not found"), 404
-    email_parameters = m.to_dict()
-    userid = m.get('_key')
-    rtoken = SecurityLayer.PasswordRecoveryToken('create', {'userid':m.get('_key')})
-    tokenid = rtoken.get('_key')
-    code = f'{userid}.{tokenid}'
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
-    f = Fernet(crypt)
-    token = f.encrypt(bytes(f'passwordrec.{code}', 'utf-8')).decode()
-    p = Metadata.Parameter('find', {'_key' : 'oauth_passwordreset_url'})
-    base_url = p.get('value')
-    email_parameters['url'] = f'{base_url}?token={token}&client_id={atoken.get("_key")}'
-    if 'back_uri' in jr:
-        email_parameters['url'] = f'{email_parameters["url"]}&back_uri={jr.get("back_uri")}'
-    email_type = 'password_recovery_email'
-    if welcome == True:
-        email_type = 'welcome_email'
-        act_token = SecurityLayer.UserToken('create', {'userid':m.get('_key')})
-        act_token.valid_thru = act_token.valid_thru + datetime.timedelta(minutes=60*24*5)
-        act_token.update()
-        act_tokenid = act_token.get('_key')
-        act_code = f'{userid}.{act_tokenid}'
-        if os.environ.get('D20_SL_CONF') != None:
-            env = json.loads(os.environ.get('D20_SL_CONF'))
-            crypt = env.get('D20_SL_CRYPTOKEY').encode()
-        else:
-            crypt = D20_SL_CRYPTOKEY
-        f = Fernet(crypt)
-        activation_token = f.encrypt(bytes(f'{act_code}', 'utf-8')).decode()
-        p = Metadata.Parameter('find', {'_key' : 'oauth_account_activation_url'})
-        base_url = p.get('value')
-        email_parameters['url_2'] = f'{base_url}?token={activation_token}&client_id={atoken.get("_key")}&channel=email'
-        if 'back_uri' in jr:
-            email_parameters['url_2'] = f'{email_parameters["url_2"]}&back_uri={jr.get("back_uri")}'
-        else:
-            p = Metadata.Parameter('find', {'_key' : 'default_redir_url'})
-            email_parameters['url_2'] = f'{email_parameters["url_2"]}&back_uri={p.get("value")}'
-    email = Communications.Email('set', {'receiver': m.get('email'), 'type':email_type, 'params': email_parameters})
-    res = email.send()
-    if res.get('res') != True:
-        return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
-    return jsonify(res)
+# def oauth_sendpasswordrecovery(welcome = False):
+#     auth = api_back_auth(request, oauth=True)
+#     if auth.get('res') == False:
+#         return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
+#     atoken = auth.get('token')
+#     if atoken.get('oauth') != True or not 'auth' in atoken.get('actions'):
+#         return jsonify({'error': 'unauthorized_client'}), 401
+#     jr = request.get_json()
+#     m = Core.User('find', {'username': jr.get('username')})
+#     if m.get('status') != True:
+#         return jsonify("Member not found"), 404
+#     email_parameters = m.to_dict()
+#     userid = m.get('_key')
+#     rtoken = SecurityLayer.PasswordRecoveryToken()
+#     rtoken.userid=m.get('_key')
+#     rtoken.create()
+#     tokenid = rtoken.get('_key')
+#     code = f'{userid}.{tokenid}'
+#     crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
+#     f = Fernet(crypt)
+#     token = f.encrypt(bytes(f'passwordrec.{code}', 'utf-8')).decode()
+#     p = Metadata.Parameter('find', {'_key' : 'oauth_passwordreset_url'})
+#     base_url = p.get('value')
+#     email_parameters['url'] = f'{base_url}?token={token}&client_id={atoken.get("_key")}'
+#     if 'back_uri' in jr:
+#         email_parameters['url'] = f'{email_parameters["url"]}&back_uri={jr.get("back_uri")}'
+#     email_type = 'password_recovery_email'
+#     if welcome == True:
+#         email_type = 'welcome_email'
+#         act_token = SecurityLayer.UserToken('create', {'userid':m.get('_key')})
+#         act_token.valid_thru = act_token.valid_thru + datetime.timedelta(minutes=60*24*5)
+#         act_token.update()
+#         act_tokenid = act_token.get('_key')
+#         act_code = f'{userid}.{act_tokenid}'
+#         crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
+#         f = Fernet(crypt)
+#         activation_token = f.encrypt(bytes(f'{act_code}', 'utf-8')).decode()
+#         p = Metadata.Parameter('find', {'_key' : 'oauth_account_activation_url'})
+#         base_url = p.get('value')
+#         email_parameters['url_2'] = f'{base_url}?token={activation_token}&client_id={atoken.get("_key")}&channel=email'
+#         if 'back_uri' in jr:
+#             email_parameters['url_2'] = f'{email_parameters["url_2"]}&back_uri={jr.get("back_uri")}'
+#         else:
+#             p = Metadata.Parameter('find', {'_key' : 'default_redir_url'})
+#             email_parameters['url_2'] = f'{email_parameters["url_2"]}&back_uri={p.get("value")}'
+#     email = Communications.Email('set', {'receiver': m.get('email'), 'type':email_type, 'params': email_parameters})
+#     res = email.send()
+#     if res.get('res') != True:
+#         return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
+#     return jsonify(res)
     
-def oauth_passwordrecoverylink():
-    auth = api_back_auth(request, oauth=True)
-    if auth.get('res') == False:
-        return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
-    atoken = auth.get('token')
-    if atoken.get('oauth') != True or not 'auth' in atoken.get('actions'):
-        return jsonify({'error': 'unauthorized_client'}), 401
-    jr = request.get_json()
-    auth = user_back_auth(request, oauth=True)
-    if auth.get('res') == False:
-        return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
-    utoken = auth.get('token')
-    m = Core.User('find', {'username': utoken.get('userid')})
-    if m.get('status') != True:
-        return jsonify("Member not found"), 404
-    userid = m.get('_key')
-    rtoken = SecurityLayer.PasswordRecoveryToken('create', {'userid':m.get('_key')})
+def oauth_password_recovery_token(user_id):
+    rtoken = SecurityLayer.PasswordRecoveryToken()
+    rtoken.userid = user_id
+    rtoken.create()
     tokenid = rtoken.get('_key')
-    code = f'{userid}.{tokenid}'
-    if os.environ.get('D20_SL_CONF') != None:
-        env = json.loads(os.environ.get('D20_SL_CONF'))
-        crypt = env.get('D20_SL_CRYPTOKEY').encode()
-    else:
-        crypt = D20_SL_CRYPTOKEY
+    code = f'{user_id}.{tokenid}'
+    crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
     f = Fernet(crypt)
     token = f.encrypt(bytes(f'passwordrec.{code}', 'utf-8')).decode()
-    p = Metadata.Parameter('find', {'_key' : 'oauth_passwordreset_url'})
-    base_url = p.get('value')
-    url = f'{base_url}?token={token}&client_id={jr.get("oauth_client")}'
-    if 'back_uri' in jr:
-        url = f'{url}&back_uri={jr.get("back_uri")}'
-    return jsonify({'url': url })
-
-def oauth_error():
-    p = Metadata.Parameter('find', {'_key' : 'oauth_server_error_url'})
-    url = p.get('value')
-    return redirect(f"{url}?error={request.args.get('error', )}")
-
-def oauth_getactiontoken():
-    jr = request.get_json()
-    auth = api_back_auth(request, permalink=True, oauth=True)
-    if auth.get('res') == False:
-        return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
-    atoken = auth.get('token')
-    if atoken.get('oauth') != True or not 'sso_to_api' in atoken.get('actions'):
-        return jsonify({'error': 'unauthorized_client'}), 401 
-    if jr['token_type'].upper() != 'USER':
-        return jsonify({'atoken': atoken.get('_key')}) 
-    auth = user_back_auth(request, oauth=True)
-    if auth.get('res') == False:
-        return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
-    utoken = auth.get('token')
-    m = Core.User('find', {'_key': utoken.get('userid'), 'username': utoken.get('userid')})
-    if not m.get('status') or m.get('_key') != jr['user_id']:
-        return jsonify("Member not found"), 404
-    return jsonify({'atoken': atoken.get('_key'), 'utoken': utoken.get('_key')}) 
+    return token
+
+# def oauth_getactiontoken():
+#     jr = request.get_json()
+#     auth = api_back_auth(request, permalink=True, oauth=True)
+#     if auth.get('res') == False:
+#         return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
+#     atoken = auth.get('token')
+#     if atoken.get('oauth') != True or not 'sso_to_api' in atoken.get('actions'):
+#         return jsonify({'error': 'unauthorized_client'}), 401 
+#     if jr['token_type'].upper() != 'USER':
+#         return jsonify({'atoken': atoken.get('_key')}) 
+#     auth = user_back_auth(request, oauth=True)
+#     if auth.get('res') == False:
+#         return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
+#     utoken = auth.get('token')
+#     m = Core.User('find', {'_key': utoken.get('userid'), 'username': utoken.get('userid')})
+#     if not m.get('status') or m.get('_key') != jr['user_id']:
+#         return jsonify("Member not found"), 404
+#     return jsonify({'atoken': atoken.get('_key'), 'utoken': utoken.get('_key')}) 
 
 # def sso_getuserinfo(Core, **kwargs):
 #     atoken = kwargs.get('token')
 #     utoken = kwargs.get('user_token')
 #     m = Core.User('find', {'_key': utoken.get('userid'), 'username': utoken.get('userid')})
 #     if not m.get('status'):
 #         return UserNotFoundError().make_error()
 #     return jsonify(m.dict_by_scope(atoken.get('oauth_scopes')))
 
-def sso_logout(**kwargs):
-    utoken = kwargs.get('user_token')
-    if not utoken.get('status') == True:
-        return SSOInvalidUserTokenError().make_error()
+def sso_logout(user_token):
+    utoken = SecurityLayer.UserToken()
+    utoken.load(user_token)
     utoken.wipe()
-    if not utoken.get('status') == True:
-        return UnexpectedError().make_error()
-    return jsonify({'res': True})
-
-def oauth_auth():
-    auth = api_back_auth(request, permalink=True, oauth=True)
-    if auth.get('res') == False:
-        if request.method == 'GET':
-            redirect_url = url_for('oauth_error') + auth.get('err_params')
-            return redirect(redirect_url)
-        else:
-            return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
-    atoken = auth.get('token')
-    if request.method == 'GET':
-        redirect_url = request.args.get('redirect_uri', atoken.get('oauth_urls')[0])
-        if not redirect_url in atoken.get('oauth_urls') and max([redirect_url.find(url) for url in atoken.get('oauth_urls')]) != 0:
-            redirect_url = url_for('oauth_error') + '?error=invalid_redirect_uri'
-            return redirect(redirect_url)
-        if not 'sso' in atoken.get('actions'):
-            redirect_url = redirect_url + '?error=unauthorized_client'
-            return redirect(redirect_url)
-        if request.args.get('scopes', '') != '':
-            scopes = request.args.get('scopes', '').split(' ')
-        else:
-            scopes = atoken.get('oauth_scopes')
-        for scope in scopes:
-            if not scope in atoken.get('oauth_scopes'):
-                scopes.pop(scopes.index(scope))
-        if len(scopes) <= 0:
-            redirect_url = redirect_url + '?error=invalid_scope'
-            return redirect(redirect_url)
-        mode = ''
-        if request.args.get('response_type', '') == 'token':
-            mode = '0'
-        p = Metadata.Parameter('find', {'_key' : 'oauth_server_login_url'})
-        url = p.get('value')
-        if 'Register' in request.args:
-            return redirect(f"{url}?client_id={atoken.get('_key')}&state={request.args.get('state', '')}&redirect_uri={redirect_url}&scopes={' '.join(scopes)}&mode={mode}&orig=oauth2&Register")
-        return redirect(f"{url}?client_id={atoken.get('_key')}&state={request.args.get('state', '')}&redirect_uri={redirect_url}&scopes={' '.join(scopes)}&mode={mode}&orig=oauth2")
-    if request.method == 'POST':
-        jr = request.get_json()
-        if atoken.get('oauth') != True or not 'sso' in atoken.get('actions'):
-            return jsonify({'error': 'unauthorized_client'}), 401 
-        if jr.get('grant_type','') == 'auth':
-            state = jr.get('state')
-            redirect_url = jr.get('redirect_uri')
-            if not redirect_url in atoken.get('oauth_urls') and max([redirect_url.find(url) for url in atoken.get('oauth_urls')]) != 0:
-                return jsonify({'error': 'invalid_client', 'redirect_uri' : f'{redirect_url}?error=invalid_client'}), 401
-            scopes = jr.get('scopes', [])
-            if len(scopes) <= 0:
-                return jsonify({'error': 'access_denied', 'redirect_uri' : f'{redirect_url}?error=access_denied'}), 403
-            for scope in scopes:
-                if not scope in atoken.get('oauth_scopes'):
-                    scopes.pop(scopes.index(scope))
-            if len(scopes) <= 0:
-                return jsonify({'error': 'invalid_scope', 'redirect_uri' : f'{redirect_url}?error=invalid_scope'}), 403
-            token_id = jr.get('token')
-            userid = jr.get('userid')
-            user = Core.User('find', {'username':userid})
-            if user.get('status') != True:
-                return jsonify({'error': 'unauthorized_client', 'redirect_uri' : f'{redirect_url}?error=unauthorized_client'}), 401
-            userid = user.get('_key')
-            token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
-            if token.get('status') != True:
-                return jsonify({'error': 'unauthorized_client', 'redirect_uri' : f'{redirect_url}?error=unauthorized_client'}), 401
-            code = f'{userid}.{token_id}'
-            if os.environ.get('D20_SL_CONF') != None:
-                env = json.loads(os.environ.get('D20_SL_CONF'))
-                crypt = env.get('D20_SL_CRYPTOKEY').encode()
-            else:
-                crypt = D20_SL_CRYPTOKEY
-            f = Fernet(crypt)
-            if jr.get('mode') == '0': # Implicit
-                access_token = f.encrypt(bytes(code, 'utf-8')).decode()
-                return jsonify({'redirect_uri' : f'{redirect_url}?state={state}&acces_token={access_token}' })
-            else:
-                token_challenge = f.encrypt(bytes(f'challenge.{code}', 'utf-8')).decode()
-                return jsonify({'redirect_uri': f'{redirect_url}?state={state}&code={token_challenge}' })
-        elif jr.get('grant_type', '') == 'code' or jr.get('grant_type', '') == 'authorization_code':
-            if not 'code' in jr:
-                return jsonify({'error': 'invalid_request'}), 401
-            if os.environ.get('D20_SL_CONF') != None:
-                env = json.loads(os.environ.get('D20_SL_CONF'))
-                crypt = env.get('D20_SL_CRYPTOKEY').encode()
-            else:
-                crypt = D20_SL_CRYPTOKEY
-            f = Fernet(crypt)
-            try:
-                val, userid, token_id = f.decrypt(bytes(jr['code'], 'utf-8')).decode().split('.')
-            except:
-                val = 'error'
-            if val != 'challenge':
-                return jsonify({'error': 'invalid_grant'}), 403
-            token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
-            if token.get('status') != True:
-                return jsonify({'error': 'invalid_grant'}), 403
-            rtoken = f.encrypt(bytes(f'{token_id}.{userid}', 'utf-8')).decode()
-            code = f.encrypt(bytes(f'{userid}.{token_id}', 'utf-8')).decode()
-            p = Metadata.Parameter('find', {'_key' : 'user_token_lifespawn'})
-            lifespawn = p.get('value')
-            return jsonify({
-                "access_token":code,
-                "token_type":"bearer",
-                "expires_in":lifespawn*59,
-                "refresh_token":rtoken,
-            })
-        elif jr.get('grant_type', '') == 'refresh_token':
-            if not 'refresh_token' in jr:
-                return jsonify({'error': 'invalid_request'}), 400
-            if os.environ.get('D20_SL_CONF') != None:
-                env = json.loads(os.environ.get('D20_SL_CONF'))
-                crypt = env.get('D20_SL_CRYPTOKEY').encode()
-            else:
-                crypt = D20_SL_CRYPTOKEY
-            f = Fernet(crypt)
-            try:
-                token_id, userid = f.decrypt(bytes(jr['refresh_token'], 'utf-8')).decode().split('.')
-            except:
-                return jsonify({'error': 'invalid_grant'}), 400
-            token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
-            if token.get('status') != True:
-                return jsonify({'error': 'invalid_grant'}), 400
-            code = f.encrypt(bytes(f'{userid}.{token_id}', 'utf-8')).decode()
-            rtoken = f.encrypt(bytes(f'{token_id}.{userid}', 'utf-8')).decode()
-            p = Metadata.Parameter('find', {'_key' : 'user_token_lifespawn'})
-            lifespawn = p.get('value')
-            return jsonify({
-                "access_token":code,
-                "token_type":"bearer",
-                "expires_in":lifespawn*59,
-                "refresh_token":rtoken,
-            })
-        else:
-            return jsonify({'error': 'unsupported_grant_type'}), 401 
+    return True
+
+# def oauth_auth():
+#     auth = api_back_auth(request, permalink=True, oauth=True)
+#     if auth.get('res') == False:
+#         if request.method == 'GET':
+#             redirect_url = url_for('oauth_error') + auth.get('err_params')
+#             return redirect(redirect_url)
+#         else:
+#             return jsonify({'error': auth.get('err_desc')}), auth.get('err_code')
+#     atoken = auth.get('token')
+#     if request.method == 'GET':
+#         redirect_url = request.args.get('redirect_uri', atoken.get('oauth_urls')[0])
+#         if not redirect_url in atoken.get('oauth_urls') and max([redirect_url.find(url) for url in atoken.get('oauth_urls')]) != 0:
+#             redirect_url = url_for('oauth_error') + '?error=invalid_redirect_uri'
+#             return redirect(redirect_url)
+#         if not 'sso' in atoken.get('actions'):
+#             redirect_url = redirect_url + '?error=unauthorized_client'
+#             return redirect(redirect_url)
+#         if request.args.get('scopes', '') != '':
+#             scopes = request.args.get('scopes', '').split(' ')
+#         else:
+#             scopes = atoken.get('oauth_scopes')
+#         for scope in scopes:
+#             if not scope in atoken.get('oauth_scopes'):
+#                 scopes.pop(scopes.index(scope))
+#         if len(scopes) <= 0:
+#             redirect_url = redirect_url + '?error=invalid_scope'
+#             return redirect(redirect_url)
+#         mode = ''
+#         if request.args.get('response_type', '') == 'token':
+#             mode = '0'
+#         p = Metadata.Parameter('find', {'_key' : 'oauth_server_login_url'})
+#         url = p.get('value')
+#         if 'Register' in request.args:
+#             return redirect(f"{url}?client_id={atoken.get('_key')}&state={request.args.get('state', '')}&redirect_uri={redirect_url}&scopes={' '.join(scopes)}&mode={mode}&orig=oauth2&Register")
+#         return redirect(f"{url}?client_id={atoken.get('_key')}&state={request.args.get('state', '')}&redirect_uri={redirect_url}&scopes={' '.join(scopes)}&mode={mode}&orig=oauth2")
+#     if request.method == 'POST':
+#         jr = request.get_json()
+#         if atoken.get('oauth') != True or not 'sso' in atoken.get('actions'):
+#             return jsonify({'error': 'unauthorized_client'}), 401 
+#         if jr.get('grant_type','') == 'auth':
+#             state = jr.get('state')
+#             redirect_url = jr.get('redirect_uri')
+#             if not redirect_url in atoken.get('oauth_urls') and max([redirect_url.find(url) for url in atoken.get('oauth_urls')]) != 0:
+#                 return jsonify({'error': 'invalid_client', 'redirect_uri' : f'{redirect_url}?error=invalid_client'}), 401
+#             scopes = jr.get('scopes', [])
+#             if len(scopes) <= 0:
+#                 return jsonify({'error': 'access_denied', 'redirect_uri' : f'{redirect_url}?error=access_denied'}), 403
+#             for scope in scopes:
+#                 if not scope in atoken.get('oauth_scopes'):
+#                     scopes.pop(scopes.index(scope))
+#             if len(scopes) <= 0:
+#                 return jsonify({'error': 'invalid_scope', 'redirect_uri' : f'{redirect_url}?error=invalid_scope'}), 403
+#             token_id = jr.get('token')
+#             userid = jr.get('userid')
+#             user = Core.User('find', {'username':userid})
+#             if user.get('status') != True:
+#                 return jsonify({'error': 'unauthorized_client', 'redirect_uri' : f'{redirect_url}?error=unauthorized_client'}), 401
+#             userid = user.get('_key')
+#             token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
+#             if token.get('status') != True:
+#                 return jsonify({'error': 'unauthorized_client', 'redirect_uri' : f'{redirect_url}?error=unauthorized_client'}), 401
+#             code = f'{userid}.{token_id}'
+#             crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
+#             f = Fernet(crypt)
+#             if jr.get('mode') == '0': # Implicit
+#                 access_token = f.encrypt(bytes(code, 'utf-8')).decode()
+#                 return jsonify({'redirect_uri' : f'{redirect_url}?state={state}&acces_token={access_token}' })
+#             else:
+#                 token_challenge = f.encrypt(bytes(f'challenge.{code}', 'utf-8')).decode()
+#                 return jsonify({'redirect_uri': f'{redirect_url}?state={state}&code={token_challenge}' })
+#         elif jr.get('grant_type', '') == 'code' or jr.get('grant_type', '') == 'authorization_code':
+#             if not 'code' in jr:
+#                 return jsonify({'error': 'invalid_request'}), 401
+#             crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
+#             f = Fernet(crypt)
+#             try:
+#                 val, userid, token_id = f.decrypt(bytes(jr['code'], 'utf-8')).decode().split('.')
+#             except:
+#                 val = 'error'
+#             if val != 'challenge':
+#                 return jsonify({'error': 'invalid_grant'}), 403
+#             token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
+#             if token.get('status') != True:
+#                 return jsonify({'error': 'invalid_grant'}), 403
+#             rtoken = f.encrypt(bytes(f'{token_id}.{userid}', 'utf-8')).decode()
+#             code = f.encrypt(bytes(f'{userid}.{token_id}', 'utf-8')).decode()
+#             p = Metadata.Parameter('find', {'_key' : 'user_token_lifespawn'})
+#             lifespawn = p.get('value')
+#             return jsonify({
+#                 "access_token":code,
+#                 "token_type":"bearer",
+#                 "expires_in":lifespawn*59,
+#                 "refresh_token":rtoken,
+#             })
+#         elif jr.get('grant_type', '') == 'refresh_token':
+#             if not 'refresh_token' in jr:
+#                 return jsonify({'error': 'invalid_request'}), 400
+#             crypt =  os.environ.get('CRYPTOKEY', D20_SL_CRYPTOKEY)
+
+#             f = Fernet(crypt)
+#             try:
+#                 token_id, userid = f.decrypt(bytes(jr['refresh_token'], 'utf-8')).decode().split('.')
+#             except:
+#                 return jsonify({'error': 'invalid_grant'}), 400
+#             token = SecurityLayer.UserToken('find', {'_key': token_id, 'userid': userid})
+#             if token.get('status') != True:
+#                 return jsonify({'error': 'invalid_grant'}), 400
+#             code = f.encrypt(bytes(f'{userid}.{token_id}', 'utf-8')).decode()
+#             rtoken = f.encrypt(bytes(f'{token_id}.{userid}', 'utf-8')).decode()
+#             p = Metadata.Parameter('find', {'_key' : 'user_token_lifespawn'})
+#             lifespawn = p.get('value')
+#             return jsonify({
+#                 "access_token":code,
+#                 "token_type":"bearer",
+#                 "expires_in":lifespawn*59,
+#                 "refresh_token":rtoken,
+#             })
+#         else:
+#             return jsonify({'error': 'unsupported_grant_type'}), 401
```

