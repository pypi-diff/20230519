# Comparing `tmp/bridgeql-0.2.0.tar.gz` & `tmp/bridgeql-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgeql-0.2.0.tar", last modified: Thu May 18 11:11:46 2023, max compression
+gzip compressed data, was "bridgeql-0.2.1.tar", last modified: Fri May 19 13:51:20 2023, max compression
```

## Comparing `bridgeql-0.2.0.tar` & `bridgeql-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-05-18 11:11:46.003674 bridgeql-0.2.0/
--rw-r--r--   0 piyusk     (502) staff       (20)     1512 2023-04-18 14:03:59.000000 bridgeql-0.2.0/LICENSE
--rw-r--r--   0 piyusk     (502) staff       (20)      403 2023-04-18 14:03:59.000000 bridgeql-0.2.0/NOTICE
--rw-r--r--   0 piyusk     (502) staff       (20)     6636 2023-05-18 11:11:46.003043 bridgeql-0.2.0/PKG-INFO
--rw-r--r--   0 piyusk     (502) staff       (20)     5457 2023-05-18 11:09:44.000000 bridgeql-0.2.0/README.md
-drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-05-18 11:11:45.987875 bridgeql-0.2.0/bridgeql/
--rw-r--r--   0 piyusk     (502) staff       (20)      647 2023-05-18 11:09:44.000000 bridgeql-0.2.0/bridgeql/__init__.py
-drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-05-18 11:11:46.000201 bridgeql-0.2.0/bridgeql/django/
--rw-r--r--   0 piyusk     (502) staff       (20)      173 2023-04-18 14:03:59.000000 bridgeql-0.2.0/bridgeql/django/__init__.py
--rw-r--r--   0 piyusk     (502) staff       (20)     1391 2023-05-18 11:09:44.000000 bridgeql-0.2.0/bridgeql/django/auth.py
--rw-r--r--   0 piyusk     (502) staff       (20)     3147 2023-05-18 11:09:44.000000 bridgeql-0.2.0/bridgeql/django/bridge.py
--rw-r--r--   0 piyusk     (502) staff       (20)     1269 2023-05-18 11:09:44.000000 bridgeql-0.2.0/bridgeql/django/exceptions.py
--rw-r--r--   0 piyusk     (502) staff       (20)      749 2023-04-27 11:57:21.000000 bridgeql-0.2.0/bridgeql/django/fields.py
--rw-r--r--   0 piyusk     (502) staff       (20)     2293 2023-05-18 11:09:44.000000 bridgeql-0.2.0/bridgeql/django/helpers.py
--rw-r--r--   0 piyusk     (502) staff       (20)    12595 2023-05-18 11:09:44.000000 bridgeql-0.2.0/bridgeql/django/models.py
--rw-r--r--   0 piyusk     (502) staff       (20)     1405 2023-04-27 11:57:21.000000 bridgeql-0.2.0/bridgeql/django/query.py
--rw-r--r--   0 piyusk     (502) staff       (20)     1040 2023-04-27 11:57:21.000000 bridgeql-0.2.0/bridgeql/django/schema.py
--rw-r--r--   0 piyusk     (502) staff       (20)     3598 2023-05-18 11:09:44.000000 bridgeql-0.2.0/bridgeql/django/settings.py
--rw-r--r--   0 piyusk     (502) staff       (20)     1158 2023-05-18 11:09:44.000000 bridgeql-0.2.0/bridgeql/django/urls.py
--rw-r--r--   0 piyusk     (502) staff       (20)     1700 2023-04-27 11:57:21.000000 bridgeql-0.2.0/bridgeql/django/views.py
-drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-05-18 11:11:45.983389 bridgeql-0.2.0/bridgeql/templates/
-drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-05-18 11:11:46.002054 bridgeql-0.2.0/bridgeql/templates/bridgeql/
--rw-r--r--   0 piyusk     (502) staff       (20)      504 2023-04-18 14:03:59.000000 bridgeql-0.2.0/bridgeql/templates/bridgeql/index.html
--rw-r--r--   0 piyusk     (502) staff       (20)     2308 2023-04-27 11:57:21.000000 bridgeql-0.2.0/bridgeql/templates/bridgeql/schema.html
--rw-r--r--   0 piyusk     (502) staff       (20)      221 2023-04-27 11:57:21.000000 bridgeql-0.2.0/bridgeql/types.py
--rw-r--r--   0 piyusk     (502) staff       (20)     1459 2023-04-18 14:03:59.000000 bridgeql-0.2.0/bridgeql/utils.py
-drwxr-xr-x   0 piyusk     (502) staff       (20)        0 2023-05-18 11:11:45.990492 bridgeql-0.2.0/bridgeql.egg-info/
--rw-rw-rw-   0 piyusk     (502) staff       (20)     6636 2023-05-18 11:11:45.000000 bridgeql-0.2.0/bridgeql.egg-info/PKG-INFO
--rw-rw-rw-   0 piyusk     (502) staff       (20)      627 2023-05-18 11:11:45.000000 bridgeql-0.2.0/bridgeql.egg-info/SOURCES.txt
--rw-rw-rw-   0 piyusk     (502) staff       (20)        1 2023-05-18 11:11:45.000000 bridgeql-0.2.0/bridgeql.egg-info/dependency_links.txt
--rw-rw-rw-   0 piyusk     (502) staff       (20)        9 2023-05-18 11:11:45.000000 bridgeql-0.2.0/bridgeql.egg-info/top_level.txt
--rw-r--r--   0 piyusk     (502) staff       (20)       84 2023-04-18 14:03:59.000000 bridgeql-0.2.0/pyproject.toml
--rw-r--r--   0 piyusk     (502) staff       (20)       38 2023-05-18 11:11:46.003799 bridgeql-0.2.0/setup.cfg
--rw-r--r--   0 piyusk     (502) staff       (20)     1789 2023-04-18 14:03:59.000000 bridgeql-0.2.0/setup.py
+drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.267971 bridgeql-0.2.1/
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1512 2023-03-23 06:35:39.000000 bridgeql-0.2.1/LICENSE
+-rw-r--r--   0 priyanksi   (501) staff       (20)      403 2023-03-17 14:43:32.000000 bridgeql-0.2.1/NOTICE
+-rw-r--r--   0 priyanksi   (501) staff       (20)     6636 2023-05-19 13:51:20.267564 bridgeql-0.2.1/PKG-INFO
+-rw-r--r--   0 priyanksi   (501) staff       (20)     5457 2023-05-16 11:17:14.000000 bridgeql-0.2.1/README.md
+drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.255346 bridgeql-0.2.1/bridgeql/
+-rw-r--r--   0 priyanksi   (501) staff       (20)      647 2023-05-19 11:26:04.000000 bridgeql-0.2.1/bridgeql/__init__.py
+drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.265448 bridgeql-0.2.1/bridgeql/django/
+-rw-r--r--   0 priyanksi   (501) staff       (20)      173 2023-04-18 04:55:32.000000 bridgeql-0.2.1/bridgeql/django/__init__.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1391 2023-05-16 11:17:14.000000 bridgeql-0.2.1/bridgeql/django/auth.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     3309 2023-05-19 11:26:04.000000 bridgeql-0.2.1/bridgeql/django/bridge.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1269 2023-05-16 11:17:14.000000 bridgeql-0.2.1/bridgeql/django/exceptions.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)      749 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/django/fields.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     2293 2023-05-16 11:17:14.000000 bridgeql-0.2.1/bridgeql/django/helpers.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)    13017 2023-05-19 11:26:31.000000 bridgeql-0.2.1/bridgeql/django/models.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1405 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/django/query.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1040 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/django/schema.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     3598 2023-05-16 11:46:14.000000 bridgeql-0.2.1/bridgeql/django/settings.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1312 2023-05-19 11:26:04.000000 bridgeql-0.2.1/bridgeql/django/urls.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1700 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/django/views.py
+drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.251021 bridgeql-0.2.1/bridgeql/templates/
+drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.267176 bridgeql-0.2.1/bridgeql/templates/bridgeql/
+-rw-r--r--   0 priyanksi   (501) staff       (20)      504 2023-04-18 14:44:49.000000 bridgeql-0.2.1/bridgeql/templates/bridgeql/index.html
+-rw-r--r--   0 priyanksi   (501) staff       (20)     2308 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/templates/bridgeql/schema.html
+-rw-r--r--   0 priyanksi   (501) staff       (20)      221 2023-05-04 09:12:29.000000 bridgeql-0.2.1/bridgeql/types.py
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1459 2023-04-03 10:34:25.000000 bridgeql-0.2.1/bridgeql/utils.py
+drwxr-xr-x   0 priyanksi   (501) staff       (20)        0 2023-05-19 13:51:20.257640 bridgeql-0.2.1/bridgeql.egg-info/
+-rw-rw-rw-   0 priyanksi   (501) staff       (20)     6636 2023-05-19 13:51:20.000000 bridgeql-0.2.1/bridgeql.egg-info/PKG-INFO
+-rw-rw-rw-   0 priyanksi   (501) staff       (20)      627 2023-05-19 13:51:20.000000 bridgeql-0.2.1/bridgeql.egg-info/SOURCES.txt
+-rw-rw-rw-   0 priyanksi   (501) staff       (20)        1 2023-05-19 13:51:20.000000 bridgeql-0.2.1/bridgeql.egg-info/dependency_links.txt
+-rw-rw-rw-   0 priyanksi   (501) staff       (20)        9 2023-05-19 13:51:20.000000 bridgeql-0.2.1/bridgeql.egg-info/top_level.txt
+-rw-r--r--   0 priyanksi   (501) staff       (20)       84 2023-03-17 14:43:32.000000 bridgeql-0.2.1/pyproject.toml
+-rw-r--r--   0 priyanksi   (501) staff       (20)       38 2023-05-19 13:51:20.268018 bridgeql-0.2.1/setup.cfg
+-rw-r--r--   0 priyanksi   (501) staff       (20)     1789 2023-04-06 17:49:48.000000 bridgeql-0.2.1/setup.py
```

### Comparing `bridgeql-0.2.0/LICENSE` & `bridgeql-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/PKG-INFO` & `bridgeql-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: bridgeql
-Version: 0.2.0
+Version: 0.2.1
 Summary: Query language to bridge the gap between REST API and ORM capability
 Home-page: https://github.com/vmware/bridgeql
 Author: Piyus Kumar
 Author-email: piyusk@vmware.com
 License: BSD-2
 Project-URL: Bug Tracker, https://github.com/vmware/bridgeql/issues
 Keywords: django
 Platform: Any
-Classifier: Natural Language :: English
-Classifier: Framework :: Django :: 4.1
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.2
+Classifier: Natural Language :: English
 Classifier: Framework :: Django :: 3.2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Framework :: Django :: 2.2
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Framework :: Django :: 4.1
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Django
-Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # BridgeQL
```

### Comparing `bridgeql-0.2.0/README.md` & `bridgeql-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/__init__.py` & `bridgeql-0.2.1/bridgeql/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,13 +10,13 @@
  | |_) | |  | | (_| | (_| |  __/ |__| | |____
  |____/|_|  |_|\__,_|\__, |\___|\___\_\______|
                       __/ |
                      |___/
 """
 
 __title__ = 'BridgeQL'
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __license__ = 'BSD 2-Clause'
 __copyright__ = 'Copyright © 2023 VMware, Inc.  All rights reserved.'
 
 # VERSION available outside module
 VERSION = __version__
```

### Comparing `bridgeql-0.2.0/bridgeql/django/auth.py` & `bridgeql-0.2.1/bridgeql/django/auth.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/django/bridge.py` & `bridgeql-0.2.1/bridgeql/django/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,25 @@
         e.log()
         res = {'data': [], 'message': str(e.detail), 'success': False}
         return JSONResponse(res, status=e.status_code)
 
 
 @require_http_methods(['GET'])
 @read_auth_decorator
-def read_django_model(request, db_name, app_label, model_name):
-    params = request.GET.get('payload', None)
+def read_django_model(request, db_name, app_label, model_name, pk=None):
     try:
-        params = json.loads(params)
+        if pk:
+            params = {
+                'filter': {
+                    'pk': pk
+                }
+            }
+        else:
+            params = request.GET.get('payload', None)
+            params = json.loads(params)
         mb = ModelBuilder(db_name, app_label, model_name, params)
         qset = mb.queryset()  # get the result based on the given parameters
         res = {'data': qset, 'message': '', 'success': True}
         return JSONResponse(res)
     except BridgeqlException as e:
         e.log()
         res = {'data': [], 'message': str(e.detail), 'success': False}
```

### Comparing `bridgeql-0.2.0/bridgeql/django/exceptions.py` & `bridgeql-0.2.1/bridgeql/django/exceptions.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/django/fields.py` & `bridgeql-0.2.1/bridgeql/django/fields.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/django/helpers.py` & `bridgeql-0.2.1/bridgeql/django/helpers.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/django/models.py` & `bridgeql-0.2.1/bridgeql/django/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,18 @@
     FieldError,
     ValidationError,
     ObjectDoesNotExist
 )
 from django.db.models import QuerySet, aggregates
 from django.db.models.base import ModelBase
 from django.db.utils import IntegrityError
-from django.utils.connection import ConnectionDoesNotExist
+try:
+    from django.utils.connection import ConnectionDoesNotExist
+except ImportError:
+    from django.db.utils import ConnectionDoesNotExist
 
 from bridgeql.django import logger
 from bridgeql.django.exceptions import (
     ForbiddenModelOrField,
     InvalidRequest,
     InvalidAppOrModelName,
     InvalidModelFieldName,
@@ -231,18 +234,19 @@
         self.model_config.validate_fields(set(requested_fields))
 
     def _apply_opts(self):
         for opt, qset_opt, opt_type in ModelBuilder._QUERYSET_OPTS:
             # offset and limit operation will return None
             func = getattr(self.qset, qset_opt, None)
             value = getattr(self.params, opt, None)
-            # do not execute operation if value is not passed,
+            # do not execute operation (except values)
+            # if value is not passed,
             # or it does not have default value specified in
             # Parameters class such as [], {}, False
-            if value is None:
+            if not value and qset_opt != 'values':
                 continue
             if not isinstance(value, opt_type):
                 raise InvalidQueryException('Invalid type %s for %s'
                                             ' expected %s'
                                             % (type(value), opt, opt_type))
             if isinstance(value, dict):
                 if qset_opt == 'aggregate':
@@ -265,14 +269,19 @@
                 self.qset = self.qset[:self.params.limit]
             elif isinstance(value, list):
                 # handle values case where property is passed in fields
                 if qset_opt == 'values' and self.query_has_properties():
                     # returns DBRows instance
                     self.qset = self._add_fields()
                 else:
+                    # in case if fields is not present in the query
+                    # return all fields but restricted
+                    if not value:
+                        value = list(
+                            self.model_config.fields - self.model_config.restricted_fields)
                     try:
                         self.qset = func(*value)
                     except FieldError as e:
                         raise InvalidModelFieldName(str(e))
             elif isinstance(value, bool) and value:
                 self.qset = func()
```

### Comparing `bridgeql-0.2.0/bridgeql/django/query.py` & `bridgeql-0.2.1/bridgeql/django/query.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/django/schema.py` & `bridgeql-0.2.1/bridgeql/django/schema.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/django/settings.py` & `bridgeql-0.2.1/bridgeql/django/settings.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/django/urls.py` & `bridgeql-0.2.1/bridgeql/django/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from bridgeql.django.views import index, generate_bridgeql_schema
 
 bridgeql_settings.validate()
 
 urlpatterns = [
     path('create/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/',
          bridge.create_django_model, name='bridgeql_django_create'),
+    path('read/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/',
+         bridge.read_django_model, name='bridgeql_django_read_pk'),
     path('read/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/',
          bridge.read_django_model, name='bridgeql_django_read'),
     path('update/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/',
          bridge.update_django_model, name='bridgeql_django_update'),
     path('delete/(?P<db_name>\w+)/(?P<app_label>\w+)/(?P<model_name>\w+)/(?P<pk>\w+)/',
          bridge.delete_django_model, name='bridgeql_django_delete'),
     path('schema/', generate_bridgeql_schema, name='generate_bridgeql_schema'),
```

### Comparing `bridgeql-0.2.0/bridgeql/django/views.py` & `bridgeql-0.2.1/bridgeql/django/views.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/templates/bridgeql/schema.html` & `bridgeql-0.2.1/bridgeql/templates/bridgeql/schema.html`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql/utils.py` & `bridgeql-0.2.1/bridgeql/utils.py`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/bridgeql.egg-info/PKG-INFO` & `bridgeql-0.2.1/bridgeql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: bridgeql
-Version: 0.2.0
+Version: 0.2.1
 Summary: Query language to bridge the gap between REST API and ORM capability
 Home-page: https://github.com/vmware/bridgeql
 Author: Piyus Kumar
 Author-email: piyusk@vmware.com
 License: BSD-2
 Project-URL: Bug Tracker, https://github.com/vmware/bridgeql/issues
 Keywords: django
 Platform: Any
-Classifier: Natural Language :: English
-Classifier: Framework :: Django :: 4.1
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.2
+Classifier: Natural Language :: English
 Classifier: Framework :: Django :: 3.2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Framework :: Django :: 2.2
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Framework :: Django :: 4.1
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Django
-Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # BridgeQL
```

### Comparing `bridgeql-0.2.0/bridgeql.egg-info/SOURCES.txt` & `bridgeql-0.2.1/bridgeql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bridgeql-0.2.0/setup.py` & `bridgeql-0.2.1/setup.py`

 * *Files identical despite different names*

