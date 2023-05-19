# Comparing `tmp/py_auth_micro-0.1.1.tar.gz` & `tmp/py_auth_micro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_micro-0.1.1.tar", last modified: Mon May  8 13:46:29 2023, max compression
+gzip compressed data, was "py_auth_micro-0.1.2.tar", last modified: Fri May 19 10:10:50 2023, max compression
```

## Comparing `py_auth_micro-0.1.1.tar` & `py_auth_micro-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.544164 py_auth_micro-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:46:29.544164 py_auth_micro-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Config/_appconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Config/_dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Config/_ldapconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Core/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Core/_ldap_interactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginbaseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginkerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginlocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/Models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Models/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Models/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/Models/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_groupworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_sessionworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_userworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/py_auth_micro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:46:29.540164 py_auth_micro-0.1.1/py_auth_micro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 13:46:29.000000 py_auth_micro-0.1.1/py_auth_micro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-08 13:46:29.544164 py_auth_micro-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 13:45:45.000000 py_auth_micro-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.530916 py_auth_micro-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-19 10:10:50.530916 py_auth_micro-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.522916 py_auth_micro-0.1.2/py_auth_micro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.522916 py_auth_micro-0.1.2/py_auth_micro/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Config/_appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Config/_dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Config/_ldapconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.526916 py_auth_micro-0.1.2/py_auth_micro/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Core/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Core/_ldap_interactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.526916 py_auth_micro-0.1.2/py_auth_micro/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.526916 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginbaseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginkerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginlocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.526916 py_auth_micro-0.1.2/py_auth_micro/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Models/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Models/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Models/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.530916 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_groupworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_sessionworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_userworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.522916 py_auth_micro-0.1.2/py_auth_micro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-19 10:10:50.530916 py_auth_micro-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/setup.py
```

### Comparing `py_auth_micro-0.1.1/LICENSE` & `py_auth_micro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/PKG-INFO` & `py_auth_micro-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_auth_micro
-Version: 0.1.1
+Version: 0.1.2
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.1.1/README.rst` & `py_auth_micro-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/py_auth_micro/Config/_appconfig.py` & `py_auth_micro-0.1.2/py_auth_micro/Config/_appconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,10 +17,11 @@
     """
     id_token_valid_time:int = 1440
     access_token_valid_time:int = 5
     allow_registration: bool = False
     auto_activate_accounts: bool = True
     admin_group: str = "admin"
     default_vhost: str = "prod"
+    group_regex:str = r"[a-zA-Z0-9_-]{1,50}"
     username_regex: str = r"[a-zA-Z-_0-9]{4,30}"
     password_regex: str = r".{4,}"
     email_regex: str = r"[a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)"
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro/Config/_dbconfig.py` & `py_auth_micro-0.1.2/py_auth_micro/Config/_dbconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/py_auth_micro/Config/_ldapconfig.py` & `py_auth_micro-0.1.2/py_auth_micro/Config/_ldapconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/py_auth_micro/Core/_ldap_interactions.py` & `py_auth_micro-0.1.2/py_auth_micro/Core/_ldap_interactions.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,39 +27,27 @@
 
     @property
     def email(self):
         """Extracts the Users email after he sucessfully logged in (if he needs to be created in the Database)
         """
         return self._userinfo["email"]
 
-    def _get_connection(self):
-        conn = ldap.initialize(self.config.address)
-        conn.protocol_version = 3
-        conn.set_option(ldap.OPT_REFERRALS, 0)
-        # if a ca_file is specified create an tls context for ldaps
-        if self.config.ca_file is not None:
-            conn.set_option(ldap.OPT_X_TLS_CACERTFILE, self.config.ca_file)
-            conn.set_option(ldap.OPT_X_TLS_NEWCTX, 0)
-
-        username = f"{self.config.domain}\\{self.username}"
-        conn.simple_bind_s(username, self.password)
-        return conn
-
     def _get_user_info(self):
-        ldap_connection = self._get_connection()
-        userfilter = f"(&(objectClass=user)(sAMAccountName={self.username}))"
-        _, data = ldap_connection.search_s(
-            self.config.base_dn, ldap.SCOPE_SUBTREE, userfilter, None
-        )[0]
-        groups_raw = data["memberOf"]
-        groups = []
-        for group in groups_raw:
-            group = group.decode("utf-8")
-            group = group[group.index("CN=") + 3 : group.index(",")]
-            groups.append(group)
+        connection_handler = _ConnectionHandler(self.config,self.username,self.password)
+        with connection_handler as ldap_connection:
+            userfilter = f"(&(objectClass=user)(sAMAccountName={self.username}))"
+            _, data = ldap_connection.search_s(
+                self.config.base_dn, ldap.SCOPE_SUBTREE, userfilter, None
+            )[0]
+            groups_raw = data["memberOf"]
+            groups = []
+            for group in groups_raw:
+                group = group.decode("utf-8")
+                group = group[group.index("CN=") + 3 : group.index(",")]
+                groups.append(group)
 
         try:
             mail = data["mail"][0]
         except IndexError:
             mail = data["mail"]
 
         self._userinfo = {"groups": groups, "email": mail.decode("utf-8")}
@@ -91,7 +79,34 @@
             bool: True if the user is allowed to.
         """
 
         if self.config.group in self._userinfo["groups"]:
             return True
 
         return False
+
+class _ConnectionHandler:
+    conn = None
+    config:LDAPConfig = None
+    def __init__(self,ldap_config:LDAPConfig,username:str,password:str):
+        self.config = ldap_config
+        self.username = username
+        self.password = password
+
+
+    def __enter__(self):
+        self.conn = ldap.initialize(self.config.address)
+        self.conn.protocol_version = 3
+        self.conn.set_option(ldap.OPT_REFERRALS, 0)
+        # if a ca_file is specified create an tls context for ldaps
+        if self.config.ca_file is not None:
+            self.conn.set_option(ldap.OPT_X_TLS_CACERTFILE, self.config.ca_file)
+            self.conn.set_option(ldap.OPT_X_TLS_NEWCTX, 0)
+
+        username = f"{self.config.domain}\\{self.username}"
+        self.conn.simple_bind_s(username, self.password)
+        
+        return self.conn
+
+    def __exit__(self, *args):
+        if self.conn is not None:
+            self.conn.unbind_s()
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro/LoginHandler/__init__.py` & `py_auth_micro-0.1.2/py_auth_micro/LoginHandler/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginbaseclass.py` & `py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginbaseclass.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginldap.py` & `py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,20 @@
         Note:
             calls :code:`self._sync_groups` to sync the LDAP/AD Group memberships of the User with the Database.
 
         Returns:
             bool: Successfull Login
         """
         logger = logging.getLogger(__name__)
+
+        if self.ldap_config is None:
+            logger.debug(f"no ldap_config provided... cant do ldap logins")
+            return False
+
+
         logger.debug(f"tyring to login {self.username} via LDAP")
 
         try:
             ldaphelper = LDAPHelper(self.ldap_config, self.username, self.password)
         except ldap.INVALID_CREDENTIALS:
             logger.debug(f"invalid credentials for {self.username}")
             return False
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro/LoginHandler/_loginlocal.py` & `py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginlocal.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/py_auth_micro/Models/_token.py` & `py_auth_micro-0.1.2/py_auth_micro/Models/_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import datetime
 
 from tortoise import fields
 from tortoise.models import Model
 from typing import Optional
 from jwt_helper import SignMethod, JWTEncoder, JWTValidator
 
-from ..Config import AppConfig
+from py_auth_micro.Config import AppConfig
 
 
 class Token(Model):
     """Databse Entity Holding Information around issued Identity Tokens
 
     This Entity holds Information about issued Tokens. The Token ID is supplied in the JWT Header.
     A User can only have one valid Identity Token Per Time. A Token is bound to a vhost for the Message Broker.
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro/Models/_user.py` & `py_auth_micro-0.1.2/py_auth_micro/Models/_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import datetime
 
 from typing import Optional
 from tortoise import fields
 from tortoise.models import Model
 from jwt_helper import JWTEncoder
 
-from ..Core import AuthSource
-from ..Config import AppConfig
-from ._token import Token
+from py_auth_micro.Core import AuthSource
+from py_auth_micro.Config import AppConfig
+from py_auth_micro.Models._token import Token
 
 
 class User(Model):
     """Model Representing a User
 
     Attributes:
         username (str): Name of the User.
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/__init__.py` & `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_groupworkflow.py` & `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_groupworkflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import re
+
 from jwt_helper import JWTValidator
 from dataclasses import dataclass
 from typing import Optional
 
-from ..Models import Group, User
-from ..Config import AppConfig
+from py_auth_micro.Models import Group, User
+from py_auth_micro.Config import AppConfig
 
-from ._misc import _get_info_from_token
+from py_auth_micro.WorkFlows._misc import _get_info_from_token
 
 
 @dataclass
 class GroupWorkflow:
     """This Helper Class contains all interactions related to Groups and Group Memberships.
 
     Attributes:
@@ -55,27 +57,48 @@
         Args:
             access_token (str): Access-Token of the Requesting User.
 
         Returns:
             dict: `resp_data` contains the key groups which is a list of all groups.
         """
         self.jwt_validator.verify_jwt(access_token)
-        groups_raw = await Group.all()
-
-        groups = []
 
-        for group in groups_raw:
-            groups.append(group.name)
+        groups = await Group.all().values_list("name", flat=True)
 
+        resp_code = 200
         if len(groups) == 0:
-            status_code = 204
-        else:
-            status_code = 200
+            resp_code = 204
+
+        return {"resp_code": resp_code, "resp_data": {"groups": groups}}
+
+    async def group_members(
+        self, *, access_token: str, groupname: str, **kwargs
+    ) -> list:
+        """This Function returns all Users in a group
 
-        return {"resp_code": status_code, "resp_data": {"groups": groups}}
+        Args:
+            access_token (str): Access-Token of the Requesting User.
+            groupname (str): Name of the Group of which we want the Users.
+
+        Raises:
+            ValueError: if Group does not exist.
+            PermissionError: if User is not an admin.
+
+        Returns:
+            list: List of all usernames in this group.
+        """
+
+        group = await self._perm_and_name_check(
+            access_token=access_token, groupname=groupname
+        )
+        if group is None:
+            raise ValueError("Group does not exist")
+
+        userlist = await group.users.values_list("username", True)
+        return {"resp_code": 200, "resp_data": {"users": userlist}}
 
     async def create_group(
         self, *, access_token: str, groupname: str, **kwargs
     ) -> dict:
         """Creates a Group with the specified Name
 
         Args:
@@ -93,21 +116,27 @@
             await self._perm_and_name_check(
                 access_token=access_token, groupname=groupname
             )
             is not None
         ):
             raise ValueError("Group already exist")
 
+        error_response = {
+            "resp_code": 500,
+            "resp_data": {"msg": f"could not create group {groupname}"},
+        }
+
+        if re.fullmatch(self.app_cfg.group_regex, groupname) is None:
+            error_response["resp_data"] = {"msg":"Group Name is invalid"}
+            return error_response
+
         try:
             await Group.create(name=groupname)
         except Exception:
-            return {
-                "resp_code": 500,
-                "resp_data": {"msg": f"could not create group {groupname}"},
-            }
+            return error_response
 
         return {"resp_code": 200, "resp_data": {"msg": f"created group {groupname}"}}
 
     async def delete_group(
         self, *, access_token: str, groupname: str, **kwargs
     ) -> dict:
         """Deletes the specified Group.
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_misc.py` & `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from jwt_helper import JWTValidator
 
-from ..Config import AppConfig
+from py_auth_micro.Config import AppConfig
 
 
 def _get_info_from_token(
     jwt_validator: JWTValidator, app_cfg: AppConfig, access_token: str
 ) -> tuple[str, bool]:
     """This Function gets Information from an Access-Token.
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_sessionworkflow.py` & `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_sessionworkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from jwt_helper import JWTEncoder, JWTValidator
 from dataclasses import dataclass
 from typing import Optional
 
-from ..LoginHandler import login
-from ..Models import User, Token
-from ..Config import AppConfig, LDAPConfig
+from py_auth_micro.LoginHandler import login
+from py_auth_micro.Models import User, Token
+from py_auth_micro.Config import AppConfig, LDAPConfig
 
 
 @dataclass
 class SessionWorkflow:
     """This Helper Class contains all interactions related to Sessions.
 
     Attributes:
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro/WorkFlows/_userworkflow.py` & `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_userworkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import re
 
 from dataclasses import dataclass
 from tortoise.exceptions import DoesNotExist
 from jwt_helper import JWTValidator
 from typing import Optional
 
-from ..Models import User
-from ..Exceptions import AlreadyExists
-from ..Config import AppConfig
-from ..Core import AuthSource
+from py_auth_micro.Models import User
+from py_auth_micro.Exceptions import AlreadyExists
+from py_auth_micro.Config import AppConfig
+from py_auth_micro.Core import AuthSource
 
-from ._misc import _get_info_from_token
+from py_auth_micro.WorkFlows._misc import _get_info_from_token
 
 
 @dataclass
 class UserWorkflow:
     """This Helper Class contains all interactions related to Users.
 
     Attributes:
@@ -39,15 +39,19 @@
             dict : A list of all known Users
         """
         if not self.jwt_validator.verify_jwt(access_token):
             raise PermissionError("Not Authorized")
 
         users = await User.all().values_list("username", flat=True)
 
-        return {"resp_code": 200, "resp_data": {"users": users}}
+        resp_code = 200
+        if len(users) == 0:
+            resp_code = 204
+
+        return {"resp_code": resp_code, "resp_data": {"users": users}}
 
     async def _create_user(
         self,
         *,
         username: str,
         password: str,
         email: str,
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro.egg-info/PKG-INFO` & `py_auth_micro-0.1.2/py_auth_micro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-auth-micro
-Version: 0.1.1
+Version: 0.1.2
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.1.1/py_auth_micro.egg-info/SOURCES.txt` & `py_auth_micro-0.1.2/py_auth_micro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.1/setup.cfg` & `py_auth_micro-0.1.2/setup.cfg`

 * *Files identical despite different names*

