# Comparing `tmp/scandal-0.1.6.tar.gz` & `tmp/scandal-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scandal-0.1.6.tar", max compression
+gzip compressed data, was "scandal-0.1.7.tar", max compression
```

## Comparing `scandal-0.1.6.tar` & `scandal-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0       10 2023-05-18 09:11:52.614426 scandal-0.1.6/README.md
--rw-r--r--   0        0        0      693 2023-05-18 09:11:52.614426 scandal-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2467 2023-05-18 09:11:52.614426 scandal-0.1.6/scandal/__init__.py
--rw-r--r--   0        0        0      522 2023-05-18 09:11:52.614426 scandal-0.1.6/scandal/__main__.py
--rw-r--r--   0        0        0     3355 2023-05-18 09:11:52.614426 scandal-0.1.6/scandal/_auth.py
--rw-r--r--   0        0        0      114 2023-05-18 09:11:52.614426 scandal-0.1.6/scandal/_connection.py
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 scandal-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-05-19 06:21:56.344340 scandal-0.1.7/README.md
+-rw-r--r--   0        0        0     1433 2023-05-19 06:21:56.348340 scandal-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/__init__.py
+-rw-r--r--   0        0        0      522 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/__main__.py
+-rw-r--r--   0        0        0      784 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/_config.py
+-rw-r--r--   0        0        0      114 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/_connection.py
+-rw-r--r--   0        0        0      401 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/dbapi/__init__.py
+-rw-r--r--   0        0        0     1441 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/dbapi/connection.py
+-rw-r--r--   0        0        0      308 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/dbapi/proxy.py
+-rw-r--r--   0        0        0     3175 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/oauth.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/sqlalchemy/base.py
+-rw-r--r--   0        0        0     5905 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/sqlalchemy/bigquery.py
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 scandal-0.1.7/PKG-INFO
```

### Comparing `scandal-0.1.6/scandal/_auth.py` & `scandal-0.1.7/scandal/oauth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,60 @@
-import json
-import os.path
 import time
 import webbrowser
 
 import jwt
 import keyring
 import requests
 
+from scandal._config import get_archimedes_url, get_client_id
+
+CLIENT_IDS = {"scandal-py": "a358618b-92ea-411f-b8f1-99be0f557da0"}
+
 SERVICE = "scandal-py"
-AUTH_DOMAIN = "http://localhost:3000"
-CLIENT_ID = "app_3JQW6ThZHnj2VJMlemk6D"
 GRANT_TYPE = "urn:ietf:params:oauth:grant-type:device_code"
 
 # Refresh token 5 minutes before it expires
 EXPIRY_WINDOW = 5 * 60
 
-# Check for local development
-creds_file = os.path.join(os.path.dirname(__file__), "../../crowbar/.oauth.creds.json")
-if os.path.exists(creds_file):
-    with open(creds_file) as f:
-        creds = json.load(f)
-        CLIENT_ID = creds["clientCreds"][SERVICE]["clientId"]
-
 
 def auth_user():
     # _try_delete_password(SERVICE, "access_token")
     # _try_delete_password(SERVICE, "refresh_token")
+    client_id = get_client_id(SERVICE)
 
     access_token = keyring.get_password(SERVICE, "access_token")
     refresh_token = keyring.get_password(SERVICE, "refresh_token")
 
     if access_token:
         access_token_decoded = jwt.decode(
             access_token, options={"verify_signature": False}
         )
 
         if access_token_decoded.get("exp") > (time.time() - EXPIRY_WINDOW):
             return access_token
 
         if refresh_token:
             refresh_resp = requests.post(
-                f"{AUTH_DOMAIN}/oauth/token",
+                f"{get_archimedes_url()}/oauth/token",
                 data={
-                    "client_id": CLIENT_ID,
+                    "client_id": client_id,
                     "grant_type": GRANT_TYPE,
                     "refresh_token": refresh_token,
                 },
             )
             if not refresh_resp.ok:
                 print("Failed to refresh Scandal token.")
                 keyring.delete_password(SERVICE, "access_token")
                 keyring.delete_password(SERVICE, "refresh_token")
                 return auth_user()
 
     resp = requests.post(
-        f"{AUTH_DOMAIN}/oauth/device",
+        f"{get_archimedes_url()}/oauth/device",
         data={
-            "client_id": CLIENT_ID,
+            "client_id": client_id,
             # TODO(ngates): should this be scandal instead?
             "audience": "https://scandal.fulcrum.so",
             "scope": "offline_access",
         },
     )
     if not resp.ok:
         raise Exception(f"{resp.status_code}: {resp.text}")
@@ -71,17 +65,17 @@
     print("Enter the following code at this URL: " + code_resp["verification_uri"])
     print(code_resp["user_code"])
     webbrowser.open(code_resp["verification_uri_complete"])
 
     while time.time() < expiry:
         time.sleep(code_resp["interval"])
         token_resp = requests.post(
-            f"{AUTH_DOMAIN}/oauth/token",
+            f"{get_archimedes_url()}/oauth/token",
             data={
-                "client_id": CLIENT_ID,
+                "client_id": client_id,
                 "grant_type": GRANT_TYPE,
                 "device_code": code_resp["device_code"],
             },
         )
 
         if token_resp.ok:
             token_resp = token_resp.json()
```

### Comparing `scandal-0.1.6/PKG-INFO` & `scandal-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: scandal
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Nicholas Gates
 Author-email: nick@nickgates.com
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: sqlalchemy
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
-Requires-Dist: adbc-driver-flightsql (>=0.3.0,<0.4.0)
+Requires-Dist: adbc-driver-flightsql (>=0.4.0,<0.5.0)
 Requires-Dist: keyring (>=23.13.1,<24.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: sqlalchemy (>=1.2.0,<2.0.0dev) ; extra == "sqlalchemy"
+Requires-Dist: sqlalchemy-bigquery (>=1.6.1,<2.0.0) ; python_version >= "3.9" and python_version < "3.12"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: wrapt (>=1.15.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Scandal
```

