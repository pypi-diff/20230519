# Comparing `tmp/pyC8-1.0.0.tar.gz` & `tmp/pyC8-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyC8-1.0.0.tar", last modified: Sun Apr  9 10:08:34 2023, max compression
+gzip compressed data, was "pyC8-1.0.1.tar", last modified: Fri May 19 17:06:00 2023, max compression
```

## Comparing `pyC8-1.0.0.tar` & `pyC8-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 10:08:26.000000 pyC8-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-09 10:08:26.000000 pyC8-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-09 10:08:34.730556 pyC8-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-09 10:08:26.000000 pyC8-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/c8/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/apikeys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/c8/billing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/billing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/billing/billing_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/billing/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/c8ql.py
--rw-r--r--   0 runner    (1001) docker     (123)   114125 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    87300 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20472 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    54622 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/c8/function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/function/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/function/function_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    27951 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/keyvalue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/c8/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/redis/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   118971 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/redis/redis_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/redis/redis_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/stream_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    24998 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/stream_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    37091 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/pyC8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-09 10:08:26.000000 pyC8-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 10:08:34.734556 pyC8-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 10:08:26.000000 pyC8-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:00.262729 pyC8-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 17:05:50.000000 pyC8-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 17:05:50.000000 pyC8-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-19 17:06:00.262729 pyC8-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-19 17:05:50.000000 pyC8-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:00.258729 pyC8-1.0.1/c8/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/apikeys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:00.258729 pyC8-1.0.1/c8/billing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/billing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/billing/billing_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/billing/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/c8ql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114388 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87300 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20472 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54622 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:00.258729 pyC8-1.0.1/c8/function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/function/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/function/function_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27951 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/keyvalue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:00.262729 pyC8-1.0.1/c8/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/redis/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118971 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/redis/redis_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/redis/redis_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/stream_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24998 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/stream_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37091 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 17:05:50.000000 pyC8-1.0.1/c8/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:00.262729 pyC8-1.0.1/pyC8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-19 17:06:00.000000 pyC8-1.0.1/pyC8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-19 17:06:00.000000 pyC8-1.0.1/pyC8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:06:00.000000 pyC8-1.0.1/pyC8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 17:06:00.000000 pyC8-1.0.1/pyC8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-19 17:06:00.000000 pyC8-1.0.1/pyC8.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 17:05:50.000000 pyC8-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 17:06:00.262729 pyC8-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 17:05:50.000000 pyC8-1.0.1/setup.py
```

### Comparing `pyC8-1.0.0/LICENSE` & `pyC8-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/PKG-INFO` & `pyC8-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyC8
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python SDK for Macrometa Global Data Mesh
 Home-page: https://www.macrometa.com
 Author: Macrometa
 Author-email: product@macrometa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pyC8-1.0.0/README.md` & `pyC8-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/api.py` & `pyC8-1.0.1/c8/api.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/apikeys.py` & `pyC8-1.0.1/c8/apikeys.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/billing/billing_interface.py` & `pyC8-1.0.1/c8/billing/billing_interface.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/c8ql.py` & `pyC8-1.0.1/c8/c8ql.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/client.py` & `pyC8-1.0.1/c8/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,29 +54,30 @@
         geofabric="_system",
         stream_port=constants.STREAM_PORT,
         email=None,
         password=None,
         http_client=None,
         token=None,
         apikey=None,
+        skip_tenant=False,
     ):
 
         self._protocol = protocol.strip("/")
         self._host = host.strip("/")
         self._port = int(port)
         self._email = email
         self._password = password
         self._fabric_name = geofabric
         self._token = token
         self._apikey = apikey
         self._stream_port = int(stream_port)
         self.set_port()
         self.set_url()
         self._http_client = http_client
-        self.get_tenant()
+        self.get_tenant(skip_tenant)
         # Domains
         self._redis = None
         self._billing = None
         self._function = None
 
     def set_url(self):
         if "api-" in self.host:
@@ -91,23 +92,23 @@
         elif self._protocol == "https":
             self._port = 443
         else:
             raise NotImplementedError(
                 f"Cannot determine port for unsupported protocol: {self._protocol}"
             )
 
-    def get_tenant(self):
+    def get_tenant(self, skip_tenant=False):
         if self._email and self._password:
             self._tenant = self.tenant(email=self._email, password=self._password)
             self._fabric = self._tenant.useFabric(self._fabric_name)
         if self._token:
-            self._tenant = self.tenant(token=self._token)
+            self._tenant = self.tenant(token=self._token, skip_tenant=skip_tenant)
             self._fabric = self._tenant.useFabric(self._fabric_name)
         if self._apikey:
-            self._tenant = self.tenant(apikey=self._apikey)
+            self._tenant = self.tenant(apikey=self._apikey, skip_tenant=skip_tenant)
             self._fabric = self._tenant.useFabric(self._fabric_name)
         if self._fabric:
             self._search = self._fabric.search()
 
     def __repr__(self):
         return "<C8Client {}>".format(self._url)
 
@@ -188,36 +189,39 @@
         """Return the C8Db base URL.
 
         :returns: C8Db base URL.
         :rtype: str | unicode
         """
         return self._url
 
-    def tenant(self, email="", password="", token=None, apikey=None):
+    def tenant(self, email="", password="", token=None, apikey=None, skip_tenant=False):
         """Connect to a fabric and return the fabric API wrapper.
 
         :param email: Email for basic authentication
         :type email: str | unicode
         :param password: Password for basic authentication.
         :type password: str | unicode
         :param token: Bearer Token for authentication.
         :type token: str
         :param apikey: Api Key for authentication.
         :type apikey: str
+        :param skip_tenant: Whether to fetch tenant name or not.
+        :type skip_tenant: boolean
 
         :returns: Standard fabric API wrapper.
         :type: c8.fabric.StandardFabric
         """
         connection = TenantConnection(
             url=self._url,
             email=email,
             password=password,
             token=token,
             apikey=apikey,
             http_client=self._http_client,
+            skip_tenant=skip_tenant,
         )
         tenant = Tenant(connection)
 
         return tenant
 
     # Reducing steps
```

### Comparing `pyC8-1.0.0/c8/collection.py` & `pyC8-1.0.1/c8/collection.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/connection.py` & `pyC8-1.0.1/c8/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     :param http_client: User-defined HTTP client.
     :type http_client: c8.http.HTTPClient
     :param is_fabric: Whether this a DB or streams call.
                       Anything other than streams is a DB call.
     :type is_fabric: bool
     """
 
-    def __init__(self, url, email, password, token, apikey, http_client):
+    def __init__(self, url, email, password, token, apikey, http_client, skip_tenant=False):
         self.url = url
         self._tenant_name = ""
         self._fabric_name = constants.FABRIC_DEFAULT
         self._email = email
         self._password = password
         self._http_client = http_client or DefaultHTTPClient()
         self._token = token
@@ -56,28 +56,30 @@
             self._tenant_name = body.get("tenant")
             self._header = {"Authorization": "Bearer " + self._auth_token}
 
         if self._tenant_name == "" and self._token is not None:
             headers = {"Authorization": "Bearer " + self._auth_token}
             self._header = headers
 
-            tenurl = self.url + "/_api/user"
-            response = requests.get(url=tenurl, headers=headers)
-            if response.status_code == 200:
-                body = json.loads(response.text)
-                self._tenant_name = body["result"][0]["tenant"]
+            if not skip_tenant:
+                tenurl = self.url + "/_api/user"
+                response = requests.get(url=tenurl, headers=headers)
+                if response.status_code == 200:
+                    body = json.loads(response.text)
+                    self._tenant_name = body["result"][0]["tenant"]
 
         if self._tenant_name == "" and self._apikey is not None:
             headers = {"Authorization": "apikey " + self._auth_token}
             self._header = headers
-            tenurl = self.url + "/_api/user"
-            response = requests.get(url=tenurl, headers=headers)
-            if response.status_code == 200:
-                body = json.loads(response.text)
-                self._tenant_name = body["result"][0]["tenant"]
+            if not skip_tenant:
+                tenurl = self.url + "/_api/user"
+                response = requests.get(url=tenurl, headers=headers)
+                if response.status_code == 200:
+                    body = json.loads(response.text)
+                    self._tenant_name = body["result"][0]["tenant"]
 
         self._url_prefix = "{}/_fabric/{}/_api".format(url, self._fabric_name)
 
         # TODO : Handle the functions side of things
 
     def _get_auth_token(self, email=None, password=None, tenant=None, username=None):
         data = {}
@@ -220,22 +222,23 @@
 class TenantConnection(Connection):
     """Tenant Connection wrapper.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     """
 
-    def __init__(self, url, email, password, token, apikey, http_client):
+    def __init__(self, url, email, password, token, apikey, http_client, skip_tenant=False):
         super(TenantConnection, self).__init__(
             url=url,
             email=email,
             password=password,
             token=token,
             apikey=apikey,
             http_client=http_client,
+            skip_tenant=skip_tenant,
         )
         self._fqfabric_name = self._tenant_name + "." + self._fabric_name
 
     def __repr__(self):
         return "<TenantConnection {}>".format(self._fqfabric_name)
 
     @property
```

### Comparing `pyC8-1.0.0/c8/constants.py` & `pyC8-1.0.1/c8/constants.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/cursor.py` & `pyC8-1.0.1/c8/cursor.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/exceptions.py` & `pyC8-1.0.1/c8/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/executor.py` & `pyC8-1.0.1/c8/executor.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/fabric.py` & `pyC8-1.0.1/c8/fabric.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/function/function_interface.py` & `pyC8-1.0.1/c8/function/function_interface.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/graph.py` & `pyC8-1.0.1/c8/graph.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/http.py` & `pyC8-1.0.1/c8/http.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/job.py` & `pyC8-1.0.1/c8/job.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/keyvalue.py` & `pyC8-1.0.1/c8/keyvalue.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/redis/redis_commands.py` & `pyC8-1.0.1/c8/redis/redis_commands.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/redis/redis_interface.py` & `pyC8-1.0.1/c8/redis/redis_interface.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/request.py` & `pyC8-1.0.1/c8/request.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/response.py` & `pyC8-1.0.1/c8/response.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/search.py` & `pyC8-1.0.1/c8/search.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/stream_apps.py` & `pyC8-1.0.1/c8/stream_apps.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/stream_collection.py` & `pyC8-1.0.1/c8/stream_collection.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/tenant.py` & `pyC8-1.0.1/c8/tenant.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/c8/utils.py` & `pyC8-1.0.1/c8/utils.py`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/pyC8.egg-info/PKG-INFO` & `pyC8-1.0.1/pyC8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyC8
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python SDK for Macrometa Global Data Mesh
 Home-page: https://www.macrometa.com
 Author: Macrometa
 Author-email: product@macrometa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pyC8-1.0.0/pyC8.egg-info/SOURCES.txt` & `pyC8-1.0.1/pyC8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyC8-1.0.0/setup.py` & `pyC8-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md") as fp:
     description = fp.read()
 
 setup(
     name="pyC8",
-    version="1.0.0",
+    version="1.0.1",
     description="Python SDK for Macrometa Global Data Mesh",
     long_description=description,
     long_description_content_type="text/markdown",
     author="Macrometa",
     author_email="product@macrometa.com",
     url="https://www.macrometa.com",
     packages=find_packages(exclude=["tests"]),
```

