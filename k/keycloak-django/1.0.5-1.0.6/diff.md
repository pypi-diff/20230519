# Comparing `tmp/keycloak_django-1.0.5.tar.gz` & `tmp/keycloak_django-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.0.5.tar", max compression
+gzip compressed data, was "keycloak_django-1.0.6.tar", max compression
```

## Comparing `keycloak_django-1.0.5.tar` & `keycloak_django-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.5/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.5/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.5/README.md
--rwxr-xr-x   0        0        0      971 2023-05-05 20:21:55.583273 keycloak_django-1.0.5/pyproject.toml
--rwxr-xr-x   0        0        0      113 2023-05-05 20:21:48.872754 keycloak_django-1.0.5/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.5/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.5/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.5/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.5/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      671 2023-05-05 04:43:24.794624 keycloak_django-1.0.5/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.5/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.5/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.5/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    15212 2023-05-05 04:43:24.957503 keycloak_django-1.0.5/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.5/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0      995 2023-05-05 04:43:25.024955 keycloak_django-1.0.5/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.5/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11384 2023-05-05 04:43:25.089664 keycloak_django-1.0.5/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.5/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.5/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     1464 2023-05-05 04:43:25.156477 keycloak_django-1.0.5/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.5/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     2634 2023-05-05 04:43:25.215958 keycloak_django-1.0.5/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.5/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     3941 2023-05-05 04:43:25.273702 keycloak_django-1.0.5/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1445 2023-05-05 04:43:25.329684 keycloak_django-1.0.5/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.6/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.6/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.6/README.md
+-rwxr-xr-x   0        0        0      971 2023-05-19 01:55:03.002972 keycloak_django-1.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0      113 2023-05-19 01:55:44.420272 keycloak_django-1.0.6/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.6/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.6/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.6/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.6/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      671 2023-05-05 04:43:24.794624 keycloak_django-1.0.6/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.6/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.6/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.6/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    16305 2023-05-19 01:39:45.435944 keycloak_django-1.0.6/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.6/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0      995 2023-05-05 04:43:25.024955 keycloak_django-1.0.6/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.6/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11384 2023-05-05 04:43:25.089664 keycloak_django-1.0.6/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.6/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.6/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.0.6/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.6/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     2634 2023-05-05 04:43:25.215958 keycloak_django-1.0.6/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.6/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.0.6/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1445 2023-05-05 04:43:25.329684 keycloak_django-1.0.6/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.6/PKG-INFO
```

### Comparing `keycloak_django-1.0.5/LICENSE` & `keycloak_django-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/pyproject.toml` & `keycloak_django-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.0.5"
+version = "1.0.6"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.0.5/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.0.6/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/authentication.py` & `keycloak_django-1.0.6/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.0.6/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/keycloak.py` & `keycloak_django-1.0.6/src/keycloak_django/keycloak.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
 from django.conf import settings
-from keycloak import urls_patterns
+from keycloak import KeycloakPutError, urls_patterns
 import json
 from typing import List, Dict
 from keycloak.keycloak_admin import KeycloakAdmin
 from keycloak.exceptions import (
     KeycloakAuthenticationError,
     KeycloakAuthorizationConfigError,
     KeycloakDeprecationError,
@@ -197,14 +197,42 @@
         )
         raise_error_from_response(
             data_raw, KeycloakPostError, expected_codes=[201], skip_exists=skip_exists
         )
         _last_slash_idx = data_raw.headers["Location"].rindex("/")
         return data_raw.headers["Location"][_last_slash_idx + 1:]  # noqa: E203
 
+    def update_client_by_realm_name(self, realm_name, payload, skip_exists=False):
+        """Update a client.
+
+        ClientRepresentation:
+        https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
+
+        :param skip_exists: If true then do not raise an error if client already exists
+        :param realm_name:  name of realm_name (not realm-id)
+        :type skip_exists: bool
+        :param payload: ClientRepresentation
+        :type payload: dict
+        :type realm_name: str
+        :return: Client ID
+        :rtype: str
+        """
+        if skip_exists:
+            client_id = self.get_client_id_by_realm(
+                client_id=payload["clientId"], realm_name=realm_name)
+
+            if client_id is not None:
+                return client_id
+
+        params_path = {"realm-name": realm_name}
+        data_raw = self.raw_put(
+            urls_patterns.URL_ADMIN_CLIENT.format(**params_path), data=json.dumps(payload)
+        )
+        return raise_error_from_response(data_raw, KeycloakPutError, expected_codes=[204])
+    
     def set_realm_name(self, realm_name: str) -> None:
         """Create a client.
 
         ClientRepresentation:
         https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
 
         :param realm_name:  name of realm_name (not realm-id)
```

### Comparing `keycloak_django-1.0.5/src/keycloak_django/middleware.py` & `keycloak_django-1.0.6/src/keycloak_django/middleware.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.0.6/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/models.py` & `keycloak_django-1.0.6/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/security.py` & `keycloak_django-1.0.6/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.0.6/src/keycloak_django/services/client_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 from ..keycloak import get_default_master_keycloak_admin
 
 
-def create_client_by_app_owner(client_model, realm_model, id=None):
-    keycloak_admin = get_default_master_keycloak_admin()
+def get_payload_data(client_model, id):
     payload = dict(client_model.base_config)
     if id:
         payload['id'] = str(id)
     payload['clientId'] = client_model.client_id
     payload['name'] = client_model.name
     payload['rootUrl'] = client_model.rootUrl
     payload['baseUrl'] = client_model.baseUrl
     payload['enabled'] = client_model.active
     payload['publicClient'] = not client_model.is_api
     if not client_model.is_api:
         payload['redirectUris'] = client_model.redirectUris.split(",")
         payload['webOrigins'] = client_model.webOrigins.split(",")
         payload['attributes']['post.logout.redirect.uris'] = "##".join(client_model.logoutUris.split(","))
+    return payload
+
+
+def create_client_by_app_owner(client_model, realm_model, id=None):
+    keycloak_admin = get_default_master_keycloak_admin()
+    payload = get_payload_data(client_model, id)
     keycloak_admin.create_client_by_realm_name(realm_name=realm_model.realm, payload=payload)
+
+    if client_model.is_api:
+        keycloak_admin.set_realm_name(realm_name=realm_model.realm)
+        client_id = keycloak_admin.get_client_id(client_model.client_id)
+        keycloak_admin.generate_client_secrets(client_id=client_id)
+
+
+def update_client_by_app_owner(client_model, realm_model, id=None):
+    keycloak_admin = get_default_master_keycloak_admin()
+    payload = get_payload_data(client_model, id)
+    keycloak_admin.update_client_by_realm_name(realm_name=realm_model.realm, payload=payload)
+
     if client_model.is_api:
         keycloak_admin.set_realm_name(realm_name=realm_model.realm)
         client_id = keycloak_admin.get_client_id(client_model.client_id)
         keycloak_admin.generate_client_secrets(client_id=client_id)
 
 
 def delete_client_by_app_owner(client_model, realm_model):
```

### Comparing `keycloak_django-1.0.5/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.0.6/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.0.6/src/keycloak_django/services/realm_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.0.6/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.0.6/src/keycloak_django/services/user_repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def get_base_user(user_model, password):
     return {
         "id": str(user_model.id),
         "email": user_model.email,
         "emailVerified": user_model.email_verified,
-        "enabled": True,
+        "enabled": user_model.is_active if hasattr(user_model, 'is_active') else True,
         "firstName": user_model.first_name,
         "lastName": user_model.last_name,
         "username": user_model.username,
         "attributes": {
             "is_staff": user_model.is_staff,
             "is_superuser": user_model.is_superuser
         },
@@ -36,14 +36,22 @@
 
 def create_user_by_master(user_model, password):
     keycloak_admin = get_default_master_keycloak_admin()
     payload = get_base_user(user_model, password)
     keycloak_admin.create_user(payload=payload)
 
 
+def update_user(user_model):
+    keycloak_admin = get_default_master_keycloak_admin()
+    keycloak_admin.set_realm_name(realm_name=user_model.realm_name)
+    payload = get_base_user(user_model, user_model.password)
+    payload.pop('credentials')
+    keycloak_admin.update_user(user_id=user_model.pk, payload=payload)
+
+
 def get_roles_representation(role_names, client_id, keycloak_admin):
     roles_representations = keycloak_admin.get_client_roles(client_id=client_id)
     return [r for r in roles_representations if r['name'] in role_names]
 
 
 def assign_client_role_to_user(user_model, role_model):
     keycloak_admin = get_default_master_keycloak_admin()
```

### Comparing `keycloak_django-1.0.5/src/keycloak_django/tools.py` & `keycloak_django-1.0.6/src/keycloak_django/tools.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.5/PKG-INFO` & `keycloak_django-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.0.5
+Version: 1.0.6
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

