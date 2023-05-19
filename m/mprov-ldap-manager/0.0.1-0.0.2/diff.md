# Comparing `tmp/mprov_ldap_manager-0.0.1.tar.gz` & `tmp/mprov_ldap_manager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mprov_ldap_manager-0.0.1.tar", last modified: Thu Feb 23 18:58:08 2023, max compression
+gzip compressed data, was "mprov_ldap_manager-0.0.2.tar", last modified: Fri May 19 18:35:07 2023, max compression
```

## Comparing `mprov_ldap_manager-0.0.1.tar` & `mprov_ldap_manager-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:58:08.348302 mprov_ldap_manager-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-02-23 18:58:08.348302 mprov_ldap_manager-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-23 18:57:59.000000 mprov_ldap_manager-0.0.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-02-23 18:58:08.348302 mprov_ldap_manager-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:58:08.344302 mprov_ldap_manager-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:58:08.344302 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-23 18:57:18.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:58:08.348302 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-02-23 18:58:08.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-23 18:58:08.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 18:58:08.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 18:58:08.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 18:58:08.000000 mprov_ldap_manager-0.0.1/src/mprov_ldap_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 18:34:59.000000 mprov_ldap_manager-0.0.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:35:07.219207 mprov_ldap_manager-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/top_level.txt
```

### Comparing `mprov_ldap_manager-0.0.1/LICENSE` & `mprov_ldap_manager-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mprov_ldap_manager-0.0.1/PKG-INFO` & `mprov_ldap_manager-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mprov_ldap_manager
-Version: 0.0.1
+Version: 0.0.2
 Summary: An add-on to the mPCC to enable it to manage an LDAP directory.
 Home-page: https://github.com/mprov-ng/mprov_ldap_manager
 Author: Jason Williams
 Author-email: jasonw@jhu.edu
 Project-URL: Bug Tracker, https://github.com/mprov-ng/mprov_ldap_manager/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -31,17 +31,21 @@
 ```
 DATABASES = {
     'ldap': {
         'ENGINE': 'ldapdb.backends.ldap',
         'NAME': 'ldap://ldap.nodomain.org/',
         'USER': 'cn=admin,dc=nodomain,dc=org',
         'PASSWORD': 'some_secret_password',
+        'BASEDN': 'dc=somedomain,dc=something',
+        'CONNECTION_OPTIONS': {
+           ldap.OPT_X_TLS_REQUIRE_CERT: ldap.OPT_X_TLS_NEVER 
+         }
      },
      'default': {
         # your default DB config
      }
 }
 DATABASE_ROUTERS = ['ldapdb.router.Router']
 '''
 
-`mprov_ldap_manager.middleware.LDAPManagerMiddleware` to the `MIDDLEWARE` array.
+
 5. Run `touch /var/www/mprov_control_center/mprov_control_center/wsgi.py` to refresh the mPCC or restart your webserver.
```

### Comparing `mprov_ldap_manager-0.0.1/README.md` & `mprov_ldap_manager-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 ```
 DATABASES = {
     'ldap': {
         'ENGINE': 'ldapdb.backends.ldap',
         'NAME': 'ldap://ldap.nodomain.org/',
         'USER': 'cn=admin,dc=nodomain,dc=org',
         'PASSWORD': 'some_secret_password',
+        'BASEDN': 'dc=somedomain,dc=something',
+        'CONNECTION_OPTIONS': {
+           ldap.OPT_X_TLS_REQUIRE_CERT: ldap.OPT_X_TLS_NEVER 
+         }
      },
      'default': {
         # your default DB config
      }
 }
 DATABASE_ROUTERS = ['ldapdb.router.Router']
 '''
 
-`mprov_ldap_manager.middleware.LDAPManagerMiddleware` to the `MIDDLEWARE` array.
+
 5. Run `touch /var/www/mprov_control_center/mprov_control_center/wsgi.py` to refresh the mPCC or restart your webserver.
```

### Comparing `mprov_ldap_manager-0.0.1/setup.cfg` & `mprov_ldap_manager-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/admin.py` & `mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) The django-ldapdb project
 
 
 from django import forms
 from django.contrib import admin
 from django.contrib.admin.widgets import FilteredSelectMultiple
 
-from .models import LdapGroup, LdapUser
+from .models import LdapGroup, LdapUser, LdapServer
 
 
 class LdapUserAdmin(admin.ModelAdmin):
     exclude = ['dn', 'password', 'photo']
     list_display = ['username', 'first_name', 'last_name', 'email', 'uid']
     search_fields = ['first_name', 'last_name', 'full_name', 'username']
 
@@ -37,10 +37,12 @@
 
 class LdapGroupAdmin(admin.ModelAdmin):
     form = LdapGroupForm
     exclude = ['dn', 'usernames', 'member']
     list_display = ['name', 'gid']
     search_fields = ['name']
 
+class LdapServerAdmin(admin.ModelAdmin):
+    pass
 
 admin.site.register(LdapGroup, LdapGroupAdmin)
 admin.site.register(LdapUser, LdapUserAdmin)
```

### Comparing `mprov_ldap_manager-0.0.1/src/mprov_ldap_manager/models.py` & `mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,27 +10,14 @@
 from ldapdb.models import fields
 
 from django.db import models
 from django.conf import settings
 from django.dispatch import receiver
 from django.db.models.signals import pre_save, pre_delete, post_save
 
-# Server Config
-# - URL 
-# - BaseDN
-# - Cert/key/ca
-# (How to do auth?)
-
-class LdapServer(models.Model):
-    url = models.CharField(max_length=4096)
-    basedn = models.CharField(max_length=4096)
-    cert = models.TextField(blank=True)
-    cert_key = models.TextField(blank=True)
-    cert_ca = models.TextField(blank=True)
-
 
 # Users
 # - uid -> username
 # - uidNumber -> uid
 # - gidNumber -> primary GID
 # - cn -> fisrt name
 # - sn -> last name
@@ -38,15 +25,15 @@
 # - 
 
 class LdapUser(ldapdb.models.Model):
     """
     Class for representing an LDAP user entry.
     """
     # LDAP meta-data
-    base_dn = "dc=cm,dc=cluster"
+    base_dn = settings.DATABASES['ldap']['BASEDN']
     object_classes = ['posixAccount', 'shadowAccount', 'inetOrgPerson']
     last_modified = fields.DateTimeField(db_column='modifyTimestamp', editable=False)
 
     # inetOrgPerson
     first_name = fields.CharField(db_column='givenName', verbose_name="First name")
     last_name = fields.CharField("Last name", db_column='sn')
     full_name = fields.CharField(db_column='cn')
@@ -79,15 +66,15 @@
 # memberUid -> uid of member (multiple allowed)
 
 class LdapGroup(ldapdb.models.Model):
     """
     Class for representing an LDAP group entry.
     """
     # LDAP meta-data
-    base_dn = "dc=cm,dc=cluster"
+    base_dn =  settings.DATABASES['ldap']['BASEDN']
     object_classes = ['posixGroup']
 
     # posixGroup attributes
     gid = fields.IntegerField(db_column='gidNumber', unique=True)
     name = fields.CharField(db_column='cn', max_length=200, primary_key=True)
     usernames = fields.ListField(db_column='memberUid')
```

### Comparing `mprov_ldap_manager-0.0.1/src/mprov_ldap_manager.egg-info/PKG-INFO` & `mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mprov-ldap-manager
-Version: 0.0.1
+Version: 0.0.2
 Summary: An add-on to the mPCC to enable it to manage an LDAP directory.
 Home-page: https://github.com/mprov-ng/mprov_ldap_manager
 Author: Jason Williams
 Author-email: jasonw@jhu.edu
 Project-URL: Bug Tracker, https://github.com/mprov-ng/mprov_ldap_manager/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -31,17 +31,21 @@
 ```
 DATABASES = {
     'ldap': {
         'ENGINE': 'ldapdb.backends.ldap',
         'NAME': 'ldap://ldap.nodomain.org/',
         'USER': 'cn=admin,dc=nodomain,dc=org',
         'PASSWORD': 'some_secret_password',
+        'BASEDN': 'dc=somedomain,dc=something',
+        'CONNECTION_OPTIONS': {
+           ldap.OPT_X_TLS_REQUIRE_CERT: ldap.OPT_X_TLS_NEVER 
+         }
      },
      'default': {
         # your default DB config
      }
 }
 DATABASE_ROUTERS = ['ldapdb.router.Router']
 '''
 
-`mprov_ldap_manager.middleware.LDAPManagerMiddleware` to the `MIDDLEWARE` array.
+
 5. Run `touch /var/www/mprov_control_center/mprov_control_center/wsgi.py` to refresh the mPCC or restart your webserver.
```

### Comparing `mprov_ldap_manager-0.0.1/src/mprov_ldap_manager.egg-info/SOURCES.txt` & `mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

