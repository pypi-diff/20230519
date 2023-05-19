# Comparing `tmp/netsuite_python-1.5.7.tar.gz` & `tmp/netsuite_python-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.5.7.tar", last modified: Fri May 19 18:03:50 2023, max compression
+gzip compressed data, was "netsuite_python-1.5.8.tar", last modified: Fri May 19 19:17:08 2023, max compression
```

## Comparing `netsuite_python-1.5.7.tar` & `netsuite_python-1.5.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 18:03:50.571069 netsuite_python-1.5.7/
--rw-rw-rw-   0        0        0     5438 2023-05-19 18:03:50.571069 netsuite_python-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     5108 2023-04-25 19:14:38.000000 netsuite_python-1.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 18:03:50.539057 netsuite_python-1.5.7/netsuite/
--rw-rw-rw-   0        0        0    12072 2023-04-25 18:30:40.000000 netsuite_python-1.5.7/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:03:50.547144 netsuite_python-1.5.7/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.7/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:03:50.552071 netsuite_python-1.5.7/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.7/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.7/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2408 2023-05-19 18:03:38.000000 netsuite_python-1.5.7/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.7/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.7/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.7/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:03:50.554070 netsuite_python-1.5.7/netsuite/netsuite_rest_client/
--rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.7/netsuite/netsuite_rest_client/__init__.py
--rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.7/netsuite/netsuite_rest_client/rest_api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:03:50.557070 netsuite_python-1.5.7/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0    11634 2023-04-28 19:27:52.000000 netsuite_python-1.5.7/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.7/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:03:50.564070 netsuite_python-1.5.7/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.7/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:03:50.570070 netsuite_python-1.5.7/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0     5438 2023-05-19 18:03:50.000000 netsuite_python-1.5.7/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-05-19 18:03:50.000000 netsuite_python-1.5.7/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 18:03:50.000000 netsuite_python-1.5.7/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-19 18:03:50.000000 netsuite_python-1.5.7/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-05-19 18:03:50.000000 netsuite_python-1.5.7/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 18:03:50.000000 netsuite_python-1.5.7/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 18:03:50.571069 netsuite_python-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-05-19 18:03:16.000000 netsuite_python-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.560851 netsuite_python-1.5.8/
+-rw-rw-rw-   0        0        0     5438 2023-05-19 19:17:08.560851 netsuite_python-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5108 2023-04-25 19:14:38.000000 netsuite_python-1.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.541852 netsuite_python-1.5.8/netsuite/
+-rw-rw-rw-   0        0        0    12072 2023-04-25 18:30:40.000000 netsuite_python-1.5.8/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.545854 netsuite_python-1.5.8/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.8/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.547852 netsuite_python-1.5.8/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.8/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.8/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2518 2023-05-19 19:16:57.000000 netsuite_python-1.5.8/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.8/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.8/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.8/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.549851 netsuite_python-1.5.8/netsuite/netsuite_rest_client/
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.8/netsuite/netsuite_rest_client/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.8/netsuite/netsuite_rest_client/rest_api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.550852 netsuite_python-1.5.8/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0    11634 2023-04-28 19:27:52.000000 netsuite_python-1.5.8/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.8/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.554851 netsuite_python-1.5.8/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.559852 netsuite_python-1.5.8/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0     5438 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:17:08.560851 netsuite_python-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-05-19 19:17:03.000000 netsuite_python-1.5.8/setup.py
```

### Comparing `netsuite_python-1.5.7/PKG-INFO` & `netsuite_python-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.5.7
+Version: 1.5.8
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.5.7/README.md` & `netsuite_python-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/Netsuite.py` & `netsuite_python-1.5.8/netsuite/Netsuite.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.5.8/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.5.8/netsuite/api_clients/api/restlet_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,26 +19,30 @@
 class RestletApi(object):
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def execute_restlet(self, body_params, method='POST', **kwargs):
+    def execute_restlet(self, path_params, body_params, method='POST', **kwargs):
         all_params = ['script', 'deploy']  # noqa: E501
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method customer_get" % key
                 )
             params[key] = val
         del params['kwargs']
-        path_params = {}
+
+        if path_params is not None:
+            path_params = path_params
+        else:
+            path_params = {}
 
         if 'script' in params:
             path_params['script'] = params['script']
         else:
             raise ValueError("Script cannot be Null")
 
         if 'deploy' in params:
```

### Comparing `netsuite_python-1.5.7/netsuite/api_clients/api_client.py` & `netsuite_python-1.5.8/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/api_clients/configuration.py` & `netsuite_python-1.5.8/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/api_clients/rest.py` & `netsuite_python-1.5.8/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/module_loading.py` & `netsuite_python-1.5.8/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/scripts/cli.py` & `netsuite_python-1.5.8/netsuite/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/settings.py` & `netsuite_python-1.5.8/netsuite/settings.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.5.8/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite/storages/JSONStorage.py` & `netsuite_python-1.5.8/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.5.8/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.5.7
+Version: 1.5.8
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.5.7/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.5.8/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.7/setup.py` & `netsuite_python-1.5.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.5.7',
+    version='1.5.8',
     description='Python SDK for Netsuite API with Flask Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

