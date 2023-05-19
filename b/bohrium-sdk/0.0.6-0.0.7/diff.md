# Comparing `tmp/bohrium-sdk-0.0.6.tar.gz` & `tmp/bohrium-sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.0.6.tar", last modified: Thu May 18 03:23:25 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.0.7.tar", last modified: Fri May 19 01:49:10 2023, max compression
```

## Comparing `bohrium-sdk-0.0.6.tar` & `bohrium-sdk-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:23:25.324065 bohrium-sdk-0.0.6/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-18 03:23:25.323440 bohrium-sdk-0.0.6/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.0.6/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:23:25.320198 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      295 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        7 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:23:25.323080 bohrium-sdk-0.0.6/brmsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.0.6/brmsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4232 2023-05-18 03:20:07.000000 bohrium-sdk-0.0.6/brmsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:16.000000 bohrium-sdk-0.0.6/brmsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:13.000000 bohrium-sdk-0.0.6/brmsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:16:57.000000 bohrium-sdk-0.0.6/brmsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:51.000000 bohrium-sdk-0.0.6/brmsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-18 03:23:25.324160 bohrium-sdk-0.0.6/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      499 2023-05-18 03:23:22.000000 bohrium-sdk-0.0.6/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 01:49:10.245603 bohrium-sdk-0.0.7/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-19 01:49:10.245189 bohrium-sdk-0.0.7/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.0.7/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 01:49:10.240782 bohrium-sdk-0.0.7/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-19 01:49:10.000000 bohrium-sdk-0.0.7/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      319 2023-05-19 01:49:10.000000 bohrium-sdk-0.0.7/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-19 01:49:10.000000 bohrium-sdk-0.0.7/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-19 01:49:10.000000 bohrium-sdk-0.0.7/bohrium_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-19 01:49:10.000000 bohrium-sdk-0.0.7/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 01:49:10.244778 bohrium-sdk-0.0.7/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.0.7/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3534 2023-05-19 01:46:15.000000 bohrium-sdk-0.0.7/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:16.000000 bohrium-sdk-0.0.7/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3465 2023-05-19 01:48:37.000000 bohrium-sdk-0.0.7/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1608 2023-05-19 01:47:21.000000 bohrium-sdk-0.0.7/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:51.000000 bohrium-sdk-0.0.7/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-19 01:49:10.245714 bohrium-sdk-0.0.7/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      499 2023-05-19 01:48:42.000000 bohrium-sdk-0.0.7/setup.py
```

### Comparing `bohrium-sdk-0.0.6/brmsdk/client.py` & `bohrium-sdk-0.0.7/bohriumsdk/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,54 @@
 import requests
 import os
 import json
 import urllib
 import getpass
 import time
+import configparser
 
 class RequestInfoException(Exception):
     pass
 
 class Client:
-    def __init__(self, 
-                 debug=False,
-                 email="",
-                 password="",
-                 base_url="https://bohrium.dp.tech",
-                 token="",
-                 config_file_location='~/.brmconfig',
-                 use_config_file=False):
-        self.debug = debug
-        self.debug = os.getenv('LBG_CLI_DEBUG_PRINT', debug)
-        self.config = {}
-        self.accesskey = ""
-        config_file_location_expand = os.path.expanduser(config_file_location)
-        file_data = {}
-        self.token = ""
-        self.user_id = None
-        if use_config_file:
-            if os.path.exists(config_file_location_expand):
-                with open(config_file_location_expand, "r") as f:
-                    file_data = json.loads(f.read())
-
-        else:
-            self.config["email"] = email
-            self.config["password"] = password
-            self.base_url = base_url
-        if token is not None:
-            self.token = token
-        else:
-            self._login()
+    def __init__(self, config_file_location='~/.brmconfig'):
         
+        config_file_location_expand = os.path.expanduser(config_file_location)
 
-    def post(self, url, data=None, header=None, params=None, retry=5):
-        return self._req('POST', url, data=data, header=header, params=params, retry=retry)
-
-    def get(self, url, data=None, header=None, params=None, retry=5):
-        return self._req('GET', url, data=data, header=header, params=params, retry=retry)
-
-    def _req(self, method, url, data=None, header=None, params=None, retry=5):
-        short_url = url
-        url = urllib.parse.urljoin(self.base_url, short_url)
-        if header is None:
-            header = {}
-        if self.token:
-            header['Authorization'] = f'Bearer {self.token}'
-        header['bohr-client'] = f'utility:0.0.2'
+        if not os.path.exists(config_file_location_expand):
+            raise FileNotFoundError("Config File ~/.brmconfig not found!")
+        config = configparser.ConfigParser()
+        config.read(config_file_location_expand)
+        self.base_url = config.get('Credentials', 'baseUrl')
+        self.access_key = config.get('Credentials', 'accessKey')
+        self.params = {"accessKey": self.access_key}
+
+    def post(self, url, data=None, headers=None, params=None, retry=5):
+        return self._req('POST', url, data=data, headers=headers, params=params, retry=retry)
+
+    def get(self, url, data=None, headers=None, params=None, retry=5):
+        return self._req('GET', url, data=data, headers=headers, params=params, retry=retry)
+
+    def _req(self, method, url, data=None, headers=None, params=None, retry=5):
+        url = urllib.parse.urljoin(self.base_url, url)
+
+        # Set Headers
+        if headers is None: header = {}
+        # if self.token: headers['Authorization'] = f'Bearer {self.token}'
+        # headers['bohr-client'] = f'utility:0.0.2'
         resp_code = None
         for i in range(retry):
             resp = None
+            err = ""
             if method == 'GET':
-                resp = requests.get(url, params=params, headers=header)
+                resp = requests.get(url, params=params, headers=headers)
             if method == 'POST':
-                resp = requests.post(url=url, json=data, params=params, headers=header)
-            if self.debug:
-                print(resp.text)
+                resp = requests.post(url=url, json=data, params=params, headers=headers)
             resp_code = resp.status_code
             if not resp.ok:
-                if self.debug:
-                    print(f"retry: {i}, statusCode: {resp.status_code}")
                 try:
                     result = resp.json()
                     err = result.get("error")
                 except:
                     pass
                 time.sleep(0.1 * i)
                 continue
@@ -78,46 +56,45 @@
             if result.get('model', '') == 'gpt-35-turbo':
                 return result['choices'][0]['message']['content']
             elif result['code'] == 0:
                 return result.get('data', {})
             else:
                 err = result.get("message") or result.get("error")
                 break
-        raise RequestInfoException(resp_code, short_url, err)
+        raise RequestInfoException(resp_code, url, err)
 
     def get_token(self):
         self.login()
         return self.token
 
 
     def login(self):
         email = input("Please enter Bohrium Account Email: ")
         password = getpass.getpass(prompt="Please enter password: ")
         post_data = {
             'username': email,
             'password': password
         }
-        resp = self.post('/account_gw/login', post_data)
+        resp = self.post('https://bohrium.dp.tech/account_gw/login', post_data)
         self.token = resp['token']
         print("Login successfully!")
 
-    def generate_accesskey(self, name="default"):
+    def generate_access_key(self, name="default"):
         post_data = {
             "name": name
         }
         resp = self.post(url="https://bohrium.dp.tech/bohrapi/v1/ak/add", data=post_data)
-        self.accesskey = resp["accessKey"]
+        self.access_key = resp["accessKey"]
         return resp
 
 
     def chat(self, prompt, temperature=0):
         post_data = {
             "messages":[{"role":"user","content":f"{prompt}"}],
             "stream":False,
             "model":"gpt-3.5-turbo",
             "temperature":temperature,
             "presence_penalty":0
         }
         
-        url = f"https://openapi.dp.tech/openapi/v1/chat/complete?accessKey={self.accesskey}"
-        resp = requests.post(url=url, json=post_data).json()
-        return resp['choices'][0]['message']['content']
+        resp = self.post(f"/openapi/v1/chat/complete", data=post_data, params=self.params)
+        return resp
```

