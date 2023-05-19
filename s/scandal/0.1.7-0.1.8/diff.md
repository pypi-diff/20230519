# Comparing `tmp/scandal-0.1.7.tar.gz` & `tmp/scandal-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scandal-0.1.7.tar", max compression
+gzip compressed data, was "scandal-0.1.8.tar", max compression
```

## Comparing `scandal-0.1.7.tar` & `scandal-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0       10 2023-05-19 06:21:56.344340 scandal-0.1.7/README.md
--rw-r--r--   0        0        0     1433 2023-05-19 06:21:56.348340 scandal-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/__init__.py
--rw-r--r--   0        0        0      522 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/__main__.py
--rw-r--r--   0        0        0      784 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/_config.py
--rw-r--r--   0        0        0      114 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/_connection.py
--rw-r--r--   0        0        0      401 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/dbapi/__init__.py
--rw-r--r--   0        0        0     1441 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/dbapi/connection.py
--rw-r--r--   0        0        0      308 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/dbapi/proxy.py
--rw-r--r--   0        0        0     3175 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/oauth.py
--rw-r--r--   0        0        0        0 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/sqlalchemy/base.py
--rw-r--r--   0        0        0     5905 2023-05-19 06:21:56.348340 scandal-0.1.7/scandal/sqlalchemy/bigquery.py
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 scandal-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-05-19 08:25:56.301742 scandal-0.1.8/README.md
+-rw-r--r--   0        0        0     1433 2023-05-19 08:25:56.301742 scandal-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/__init__.py
+-rw-r--r--   0        0        0      921 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/_config.py
+-rw-r--r--   0        0        0      226 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/credentials/__init__.py
+-rw-r--r--   0        0        0      130 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/credentials/base.py
+-rw-r--r--   0        0        0      687 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/credentials/client.py
+-rw-r--r--   0        0        0     3472 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/credentials/device.py
+-rw-r--r--   0        0        0      724 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/credentials/oauth.py
+-rw-r--r--   0        0        0      401 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/dbapi/__init__.py
+-rw-r--r--   0        0        0     1596 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/dbapi/connection.py
+-rw-r--r--   0        0        0      552 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/dbapi/credentials.py
+-rw-r--r--   0        0        0      308 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/dbapi/proxy.py
+-rw-r--r--   0        0        0        0 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     6152 2023-05-19 08:25:56.301742 scandal-0.1.8/scandal/sqlalchemy/bigquery.py
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 scandal-0.1.8/PKG-INFO
```

### Comparing `scandal-0.1.7/pyproject.toml` & `scandal-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scandal-0.1.7/scandal/dbapi/connection.py` & `scandal-0.1.8/scandal/dbapi/connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from typing import Optional
 
 from adbc_driver_flightsql import dbapi as adbc_dbapi
 
 from scandal._config import get_scandal_host
-from scandal.oauth import auth_user
+from scandal.credentials import Credential
 
 
 def connect(
     org: Optional[str] = None,
     project: Optional[str] = None,
     auth_token: Optional[str] = None,
+    credential: Optional[Credential] = None,
     scandal_host: str = get_scandal_host(),
     **kwargs,
 ):
     """Connect to Scandal.
 
     By default,
         - For interactive users we log in using an OAuth2 device code flow to the user's default organization.
         - For non-interactive users, we pick up creds from a credentials chain.
     """
     if not auth_token:
-        auth_token = auth_user()
+        if not credential:
+            raise Exception("Expected auth_token or credential")
+        auth_token = credential.get_token()
 
     # For now, we send the token as the Basic Auth password. This is because the response headers
     # aren't respected when using Bearer auth: https://github.com/apache/arrow-adbc/issues/584
     db_kwargs = {"username": "scandal", "password": auth_token}
 
     if project:
         # Connect directly to a project
```

### Comparing `scandal-0.1.7/scandal/oauth.py` & `scandal-0.1.8/scandal/credentials/device.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,97 @@
 import time
 import webbrowser
 
-import jwt
 import keyring
 import requests
 
-from scandal._config import get_archimedes_url, get_client_id
+from scandal.credentials.base import Credential
+from scandal.credentials.oauth import check_token, wellknown
 
-CLIENT_IDS = {"scandal-py": "a358618b-92ea-411f-b8f1-99be0f557da0"}
+_device_endpoint = wellknown()["device_authorization_endpoint"]
+_token_endpoint = wellknown()["token_endpoint"]
+# Usually, device flows should use the token_endpoint. But our flow is hosted on a different server for now.
+_device_token_endpoint = wellknown().get("device_token_endpoint", _token_endpoint)
 
-SERVICE = "scandal-py"
-GRANT_TYPE = "urn:ietf:params:oauth:grant-type:device_code"
 
-# Refresh token 5 minutes before it expires
-EXPIRY_WINDOW = 5 * 60
+class DeviceCredential(Credential):
+    """A credential that triggers a Fulcrum OAuth2 Device Authorization flow."""
 
+    def __init__(self, client_id: str):
+        self._client_id = client_id
+        self._client_name = f"scandal_{client_id}"
 
-def auth_user():
-    # _try_delete_password(SERVICE, "access_token")
-    # _try_delete_password(SERVICE, "refresh_token")
-    client_id = get_client_id(SERVICE)
+    def get_token(self):
+        access_token = keyring.get_password(self._client_name, "access_token")
+        refresh_token = keyring.get_password(self._client_name, "refresh_token")
 
-    access_token = keyring.get_password(SERVICE, "access_token")
-    refresh_token = keyring.get_password(SERVICE, "refresh_token")
-
-    if access_token:
-        access_token_decoded = jwt.decode(
-            access_token, options={"verify_signature": False}
-        )
-
-        if access_token_decoded.get("exp") > (time.time() - EXPIRY_WINDOW):
-            return access_token
+        if access_token:
+            if check_token(access_token):
+                return access_token
 
         if refresh_token:
             refresh_resp = requests.post(
-                f"{get_archimedes_url()}/oauth/token",
+                _token_endpoint,
                 data={
-                    "client_id": client_id,
-                    "grant_type": GRANT_TYPE,
+                    "client_id": self._client_id,
+                    "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
                     "refresh_token": refresh_token,
                 },
             )
             if not refresh_resp.ok:
                 print("Failed to refresh Scandal token.")
-                keyring.delete_password(SERVICE, "access_token")
-                keyring.delete_password(SERVICE, "refresh_token")
-                return auth_user()
-
-    resp = requests.post(
-        f"{get_archimedes_url()}/oauth/device",
-        data={
-            "client_id": client_id,
-            # TODO(ngates): should this be scandal instead?
-            "audience": "https://scandal.fulcrum.so",
-            "scope": "offline_access",
-        },
-    )
-    if not resp.ok:
-        raise Exception(f"{resp.status_code}: {resp.text}")
-    code_resp = resp.json()
-
-    expiry = time.time() + code_resp["expires_in"]
-
-    print("Enter the following code at this URL: " + code_resp["verification_uri"])
-    print(code_resp["user_code"])
-    webbrowser.open(code_resp["verification_uri_complete"])
-
-    while time.time() < expiry:
-        time.sleep(code_resp["interval"])
-        token_resp = requests.post(
-            f"{get_archimedes_url()}/oauth/token",
+                keyring.delete_password(self._client_name, "access_token")
+                keyring.delete_password(self._client_name, "refresh_token")
+                return self.get_token()
+
+        resp = requests.post(
+            _device_endpoint,
             data={
-                "client_id": client_id,
-                "grant_type": GRANT_TYPE,
-                "device_code": code_resp["device_code"],
+                "client_id": self._client_id,
+                "scope": "offline_access",
             },
         )
+        if not resp.ok:
+            raise Exception(f"{resp.status_code}: {resp.text}")
+        code_resp = resp.json()
+
+        expiry = time.time() + code_resp["expires_in"]
+
+        print("Enter the following code at this URL: " + code_resp["verification_uri"])
+        print(code_resp["user_code"])
+        webbrowser.open(code_resp["verification_uri_complete"])
+
+        while time.time() < expiry:
+            time.sleep(code_resp["interval"])
+            token_resp = requests.post(
+                _device_token_endpoint,
+                data={
+                    "client_id": self._client_id,
+                    "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
+                    "device_code": code_resp["device_code"],
+                },
+            )
 
-        if token_resp.ok:
-            token_resp = token_resp.json()
-            access_token = token_resp["access_token"]
-            refresh_token = token_resp.get("refresh_token", "refresh")
-
-            keyring.set_password(SERVICE, "access_token", access_token)
-            keyring.set_password(SERVICE, "refresh_token", refresh_token)
+            if token_resp.ok:
+                token_resp = token_resp.json()
+                access_token = token_resp["access_token"]
+                keyring.set_password(self._client_name, "access_token", access_token)
+
+                refresh_token = token_resp.get("refresh_token", "refresh")
+                if refresh_token:
+                    keyring.set_password(
+                        self._client_name, "refresh_token", refresh_token
+                    )
 
-            return access_token
+                return access_token
 
-        if token_resp.json()["error"] != "authorization_pending":
-            token_resp.raise_for_status()
+            if token_resp.json()["error"] != "authorization_pending":
+                token_resp.raise_for_status()
 
-    raise Exception("Timed out waiting for authorization. Please try again")
+        raise Exception("Timed out waiting for authorization. Please try again")
 
 
 def _try_delete_password(service: str, username: str):
     try:
         keyring.delete_password(service, username)
     except Exception:
         pass
```

### Comparing `scandal-0.1.7/scandal/sqlalchemy/bigquery.py` & `scandal-0.1.8/scandal/sqlalchemy/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import pyarrow
 import sqlalchemy
 from sqlalchemy.engine import URL
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy_bigquery import BigQueryDialect
 
+from scandal.credentials import DeviceCredential
 from scandal.dbapi.proxy import ScandalDbApiProxy
 
 
 class BigQueryScandal(BigQueryDialect):
     def create_connect_args(self, url: URL):
         """The Scandal URI format is <dialect>+scandal://<org>/<project>."""
         org = url.host
         project = url.database
-        return [], {"org": org, "project": project}
+
+        if not url.username:
+            raise Exception("Expected Fulcrum client ID as URI username")
+
+        return [], {
+            "org": org,
+            "project": project,
+            "credential": DeviceCredential(url.username),
+        }
 
     @classmethod
     def dbapi(cls):
         return ScandalDbApiProxy(BigQueryDialect.dbapi())
 
     def has_table(self, connection, table_name, schema=None):
         return super(DefaultDialect, self).has_table(connection, table_name, schema)
@@ -128,15 +137,15 @@
         return super(DefaultDialect, self).get_view_definition(
             connection, view_name, schema, **kw
         )
 
 
 def _get_sqla_column_type(field: pyarrow.Field):
     _type_map = {
-        'date32[day]': sqlalchemy.types.Date,
+        "date32[day]": sqlalchemy.types.Date,
         "float": sqlalchemy.types.Float,
         "double": sqlalchemy.types.Float,  # Double exists in SQLAlchemy 2.0
         "int32": sqlalchemy.types.Integer,
         "int64": sqlalchemy.types.Integer,
         "string": sqlalchemy.types.String,
         # ... and so on
     }
```

### Comparing `scandal-0.1.7/PKG-INFO` & `scandal-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scandal
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Nicholas Gates
 Author-email: nick@nickgates.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

