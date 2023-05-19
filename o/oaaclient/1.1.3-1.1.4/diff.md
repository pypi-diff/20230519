# Comparing `tmp/oaaclient-1.1.3.tar.gz` & `tmp/oaaclient-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaaclient-1.1.3.tar", last modified: Thu May 11 14:59:15 2023, max compression
+gzip compressed data, was "oaaclient-1.1.4.tar", last modified: Fri May 19 16:13:51 2023, max compression
```

## Comparing `oaaclient-1.1.3.tar` & `oaaclient-1.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:59:15.344697 oaaclient-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-11 14:58:58.000000 oaaclient-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-11 14:59:15.344697 oaaclient-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-11 14:58:58.000000 oaaclient-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:59:15.340697 oaaclient-1.1.3/oaaclient/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39285 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    90348 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:59:15.340697 oaaclient-1.1.3/oaaclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-11 14:58:58.000000 oaaclient-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:59:15.344697 oaaclient-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-11 14:58:58.000000 oaaclient-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:59:15.344697 oaaclient-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    34102 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_custom_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_custom_idp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_payload_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_reprs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_template_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:51.809729 oaaclient-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-19 16:13:29.000000 oaaclient-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-19 16:13:51.809729 oaaclient-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-19 16:13:29.000000 oaaclient-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:51.809729 oaaclient-1.1.4/oaaclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-19 16:13:29.000000 oaaclient-1.1.4/oaaclient/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39285 2023-05-19 16:13:29.000000 oaaclient-1.1.4/oaaclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-19 16:13:29.000000 oaaclient-1.1.4/oaaclient/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90602 2023-05-19 16:13:29.000000 oaaclient-1.1.4/oaaclient/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-05-19 16:13:29.000000 oaaclient-1.1.4/oaaclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:51.809729 oaaclient-1.1.4/oaaclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-19 16:13:51.000000 oaaclient-1.1.4/oaaclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-19 16:13:51.000000 oaaclient-1.1.4/oaaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:13:51.000000 oaaclient-1.1.4/oaaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-19 16:13:51.000000 oaaclient-1.1.4/oaaclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 16:13:51.000000 oaaclient-1.1.4/oaaclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 16:13:51.000000 oaaclient-1.1.4/oaaclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-19 16:13:29.000000 oaaclient-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:13:51.809729 oaaclient-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-19 16:13:29.000000 oaaclient-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:51.809729 oaaclient-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    34102 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_custom_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_custom_idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_payload_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_reprs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_template_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-19 16:13:29.000000 oaaclient-1.1.4/tests/test_utils.py
```

### Comparing `oaaclient-1.1.3/LICENSE` & `oaaclient-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/PKG-INFO` & `oaaclient-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaaclient
-Version: 1.1.3
+Version: 1.1.4
 Summary: Veza Open Authorization API (OAA) SDK
 Author-email: "Veza Technologies Inc." <oaa_dev@veza.com>
 License: MIT
 Project-URL: homepage, https://github.com/veza/oaaclient-py
 Project-URL: repository, https://github.com/veza/oaaclient-py
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `oaaclient-1.1.3/README.md` & `oaaclient-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/oaaclient/client.py` & `oaaclient-1.1.4/oaaclient/client.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/oaaclient/structures.py` & `oaaclient-1.1.4/oaaclient/structures.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/oaaclient/templates.py` & `oaaclient-1.1.4/oaaclient/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,14 +813,18 @@
 
         if not self.property_definitions:
             raise OAATemplateException("No custom property definitions found for entity")
 
         self.property_definitions.validate_property_name(property_name, entity_type=self.identity_type)
         self.properties[property_name] = property_value
 
+class LocalUserType(str, Enum):
+    """ Enum for """
+    Human = "human"
+    ServiceAccount = "service_account"
 
 class LocalUser(Identity):
     """ LocalUser identity, derived from Identity base class.
 
     Used to model an application user. Can be associated with an external IdP user, or represent a local account.
 
     Args:
@@ -842,27 +846,29 @@
         properties (dict): Dictionary of properties for identity, allowed values will vary by identity type
         tags (list[Tag]): List of tags
         is_active (bool): Defaults to None for unset
         created_at (str): RFC3339 time stamp for user creation
         last_login_at (str): RFC3339 time stamp for last login
         deactivated_at (str): RFC3339 for user deactivate time
         password_last_changed_at (str): RFC3339 time stamp for last password change
+        user_type (LocalUserType): Set the local user account type
     """
 
     def __init__(self, name: str, identities: List[str] = None, groups: List[str] = None, unique_id: str = None, property_definitions: ApplicationPropertyDefinitions = None) -> None:
         super().__init__(name, identity_type=OAAIdentityType.LocalUser, unique_id=unique_id, property_definitions=property_definitions)
         self.identities = append_helper(None, identities)
         self.groups = append_helper(None, groups)
 
         # properties available for local users
         self.is_active = None
         self.created_at = None
         self.last_login_at = None
         self.deactivated_at = None
         self.password_last_changed_at = None
+        self.user_type = None
 
     def __str__(self) -> str:
         return f"Local User - {self.name} ({self.unique_id})"
 
     def __repr__(self) -> str:
         return f"LocalUser(name={self.name!r}, unique_id={self.unique_id!r}, identities={self.identities})"
 
@@ -919,14 +925,15 @@
                 "identities": self.identities,
                 "groups": self.groups,
                 "is_active": self.is_active,
                 "created_at": self.created_at,
                 "last_login_at": self.last_login_at,
                 "deactivated_at": self.deactivated_at,
                 "password_last_changed_at":  self.password_last_changed_at,
+                "user_type": self.user_type,
                 "tags": [tag.__dict__ for tag in self.tags],
                 "custom_properties": self.properties
                 }
 
         if self.unique_id:
             user['id'] = self.unique_id
```

### Comparing `oaaclient-1.1.3/oaaclient/utils.py` & `oaaclient-1.1.4/oaaclient/utils.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/oaaclient.egg-info/PKG-INFO` & `oaaclient-1.1.4/oaaclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaaclient
-Version: 1.1.3
+Version: 1.1.4
 Summary: Veza Open Authorization API (OAA) SDK
 Author-email: "Veza Technologies Inc." <oaa_dev@veza.com>
 License: MIT
 Project-URL: homepage, https://github.com/veza/oaaclient-py
 Project-URL: repository, https://github.com/veza/oaaclient-py
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `oaaclient-1.1.3/oaaclient.egg-info/SOURCES.txt` & `oaaclient-1.1.4/oaaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/pyproject.toml` & `oaaclient-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_client.py` & `oaaclient-1.1.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_commands.py` & `oaaclient-1.1.4/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_custom_application.py` & `oaaclient-1.1.4/tests/test_custom_application.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_custom_idp.py` & `oaaclient-1.1.4/tests/test_custom_idp.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_payload_push.py` & `oaaclient-1.1.4/tests/test_payload_push.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_reprs.py` & `oaaclient-1.1.4/tests/test_reprs.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_structures.py` & `oaaclient-1.1.4/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_tags.py` & `oaaclient-1.1.4/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.3/tests/test_utils.py` & `oaaclient-1.1.4/tests/test_utils.py`

 * *Files identical despite different names*

