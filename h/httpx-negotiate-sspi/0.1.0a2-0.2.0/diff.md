# Comparing `tmp/httpx_negotiate_sspi-0.1.0a2.tar.gz` & `tmp/httpx_negotiate_sspi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx_negotiate_sspi-0.1.0a2.tar", max compression
+gzip compressed data, was "httpx_negotiate_sspi-0.2.0.tar", max compression
```

## Comparing `httpx_negotiate_sspi-0.1.0a2.tar` & `httpx_negotiate_sspi-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      100 2023-05-19 07:47:15.597739 httpx_negotiate_sspi-0.1.0a2/httpx_negotiate_sspi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 06:48:35.954892 httpx_negotiate_sspi-0.1.0a2/httpx_negotiate_sspi/py.typed
--rw-r--r--   0        0        0     9432 2023-05-19 08:09:14.317851 httpx_negotiate_sspi-0.1.0a2/httpx_negotiate_sspi/sspi.py
--rw-r--r--   0        0        0      617 2023-05-19 08:19:43.048891 httpx_negotiate_sspi-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      375 2023-05-19 06:20:48.767290 httpx_negotiate_sspi-0.1.0a2/README.md
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 httpx_negotiate_sspi-0.1.0a2/setup.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 httpx_negotiate_sspi-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-05-19 07:47:15.597739 httpx_negotiate_sspi-0.2.0/httpx_negotiate_sspi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:48:35.954892 httpx_negotiate_sspi-0.2.0/httpx_negotiate_sspi/py.typed
+-rw-r--r--   0        0        0     9477 2023-05-19 09:34:55.786407 httpx_negotiate_sspi-0.2.0/httpx_negotiate_sspi/sspi.py
+-rw-r--r--   0        0        0      609 2023-05-19 09:34:34.606935 httpx_negotiate_sspi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      375 2023-05-19 06:20:48.767290 httpx_negotiate_sspi-0.2.0/README.md
+-rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 httpx_negotiate_sspi-0.2.0/setup.py
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 httpx_negotiate_sspi-0.2.0/PKG-INFO
```

### Comparing `httpx_negotiate_sspi-0.1.0a2/httpx_negotiate_sspi/sspi.py` & `httpx_negotiate_sspi-0.2.0/httpx_negotiate_sspi/sspi.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,16 @@
         self._delegate = delegate
 
     def auth_flow(
             self,
             request: Request
     ) -> Generator[Request, Response, None]:
         response = yield request
-        yield from self._handle_response(response)
+        if response.status_code == 401:
+            yield from self._handle_response(response)
 
     def _handle_response(
             self,
             response: Response
     ) -> Generator[Request, Response, None]:
         if 'Authorization' in response.request.headers:
             return
```

### Comparing `httpx_negotiate_sspi-0.1.0a2/pyproject.toml` & `httpx_negotiate_sspi-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "httpx-negotiate-sspi"
-version = "0.1.0-alpha.2"
+version = "0.2.0"
 description = "SSPI authentication for httpx"
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "httpx_negotiate_sspi" },
 ]
```

### Comparing `httpx_negotiate_sspi-0.1.0a2/setup.py` & `httpx_negotiate_sspi-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>0.16,<0.25', 'pypiwin32>=223,<224']
 
 setup_kwargs = {
     'name': 'httpx-negotiate-sspi',
-    'version': '0.1.0a2',
+    'version': '0.2.0',
     'description': 'SSPI authentication for httpx',
     'long_description': '# httpx-negotiate-sspi\n\nAn implementation of HTTP Negotiate authentication for httpx. This module provides single-sign-on using Kerberos or NTLM using the Windows SSPI interface.\n\nThis module supports Extended Protection for Authentication (aka Channel Binding Hash), which makes it usable for services that require it, including Active Directory Federation Services.\n\n',
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rob-blackbourn/httpx-negotiate-sspi',
```

### Comparing `httpx_negotiate_sspi-0.1.0a2/PKG-INFO` & `httpx_negotiate_sspi-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-negotiate-sspi
-Version: 0.1.0a2
+Version: 0.2.0
 Summary: SSPI authentication for httpx
 Home-page: https://github.com/rob-blackbourn/httpx-negotiate-sspi
 License: Apache-2.0
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

