# Comparing `tmp/keycloak_django-1.0.6.tar.gz` & `tmp/keycloak_django-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.0.6.tar", max compression
+gzip compressed data, was "keycloak_django-1.0.7.tar", max compression
```

## Comparing `keycloak_django-1.0.6.tar` & `keycloak_django-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.6/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.6/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.6/README.md
--rwxr-xr-x   0        0        0      971 2023-05-19 01:55:03.002972 keycloak_django-1.0.6/pyproject.toml
--rwxr-xr-x   0        0        0      113 2023-05-19 01:55:44.420272 keycloak_django-1.0.6/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.6/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.6/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.6/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.6/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      671 2023-05-05 04:43:24.794624 keycloak_django-1.0.6/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.6/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.6/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.6/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    16305 2023-05-19 01:39:45.435944 keycloak_django-1.0.6/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.6/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0      995 2023-05-05 04:43:25.024955 keycloak_django-1.0.6/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.6/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11384 2023-05-05 04:43:25.089664 keycloak_django-1.0.6/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.6/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.6/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.0.6/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.6/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     2634 2023-05-05 04:43:25.215958 keycloak_django-1.0.6/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.6/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.0.6/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1445 2023-05-05 04:43:25.329684 keycloak_django-1.0.6/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.7/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.7/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.7/README.md
+-rwxr-xr-x   0        0        0      971 2023-05-19 17:44:26.439350 keycloak_django-1.0.7/pyproject.toml
+-rwxr-xr-x   0        0        0      114 2023-05-19 17:44:32.418126 keycloak_django-1.0.7/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.7/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.7/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.7/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.7/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      671 2023-05-05 04:43:24.794624 keycloak_django-1.0.7/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.7/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.7/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.7/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    16285 2023-05-19 17:44:12.415179 keycloak_django-1.0.7/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.7/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0      995 2023-05-05 04:43:25.024955 keycloak_django-1.0.7/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.7/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11384 2023-05-05 04:43:25.089664 keycloak_django-1.0.7/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.7/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.7/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.0.7/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.7/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     2634 2023-05-05 04:43:25.215958 keycloak_django-1.0.7/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.7/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.0.7/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1445 2023-05-05 04:43:25.329684 keycloak_django-1.0.7/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.7/PKG-INFO
```

### Comparing `keycloak_django-1.0.6/LICENSE` & `keycloak_django-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/pyproject.toml` & `keycloak_django-1.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.0.6"
+version = "1.0.7"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.0.6/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.0.7/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/authentication.py` & `keycloak_django-1.0.7/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.0.7/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/keycloak.py` & `keycloak_django-1.0.7/src/keycloak_django/keycloak.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,27 +212,25 @@
         :type skip_exists: bool
         :param payload: ClientRepresentation
         :type payload: dict
         :type realm_name: str
         :return: Client ID
         :rtype: str
         """
-        if skip_exists:
-            client_id = self.get_client_id_by_realm(
-                client_id=payload["clientId"], realm_name=realm_name)
+        client_id = self.get_client_id_by_realm(
+            client_id=payload["clientId"], realm_name=realm_name)
+        if client_id is not None:
+            payload["id"] = client_id
 
-            if client_id is not None:
-                return client_id
-
-        params_path = {"realm-name": realm_name}
+        params_path = {"realm-name": realm_name, "id": client_id}
         data_raw = self.raw_put(
             urls_patterns.URL_ADMIN_CLIENT.format(**params_path), data=json.dumps(payload)
         )
         return raise_error_from_response(data_raw, KeycloakPutError, expected_codes=[204])
-    
+
     def set_realm_name(self, realm_name: str) -> None:
         """Create a client.
 
         ClientRepresentation:
         https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
 
         :param realm_name:  name of realm_name (not realm-id)
@@ -316,15 +314,14 @@
         :rtype: dict
         """
         # if 'audience' in kwargs:
         #     self.client_id = kwargs['audience']
         # del kwargs['audience']
         return jwt.decode(token, key, algorithms=algorithms, **kwargs)
 
-
     def _token_info(self, token, method_token_info, **kwargs):
         """Getter for the token data.
 
         :param token: Token
         :type token: str
         :param method_token_info: Token info method to use
         :type method_token_info: str
```

### Comparing `keycloak_django-1.0.6/src/keycloak_django/middleware.py` & `keycloak_django-1.0.7/src/keycloak_django/middleware.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.0.7/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/models.py` & `keycloak_django-1.0.7/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/security.py` & `keycloak_django-1.0.7/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.0.7/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.0.7/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.0.7/src/keycloak_django/services/realm_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.0.7/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.0.7/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/src/keycloak_django/tools.py` & `keycloak_django-1.0.7/src/keycloak_django/tools.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.6/PKG-INFO` & `keycloak_django-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.0.6
+Version: 1.0.7
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

