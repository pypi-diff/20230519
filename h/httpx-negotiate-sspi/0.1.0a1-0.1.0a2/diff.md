# Comparing `tmp/httpx_negotiate_sspi-0.1.0a1.tar.gz` & `tmp/httpx_negotiate_sspi-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx_negotiate_sspi-0.1.0a1.tar", max compression
+gzip compressed data, was "httpx_negotiate_sspi-0.1.0a2.tar", max compression
```

## Comparing `httpx_negotiate_sspi-0.1.0a1.tar` & `httpx_negotiate_sspi-0.1.0a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      100 2023-05-19 07:47:15.597739 httpx_negotiate_sspi-0.1.0a1/httpx_negotiate_sspi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 06:48:35.954892 httpx_negotiate_sspi-0.1.0a1/httpx_negotiate_sspi/py.typed
--rw-r--r--   0        0        0     9432 2023-05-19 08:09:14.317851 httpx_negotiate_sspi-0.1.0a1/httpx_negotiate_sspi/sspi.py
--rw-r--r--   0        0        0      610 2023-05-19 08:09:28.240811 httpx_negotiate_sspi-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      375 2023-05-19 06:20:48.767290 httpx_negotiate_sspi-0.1.0a1/README.md
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 httpx_negotiate_sspi-0.1.0a1/setup.py
--rw-r--r--   0        0        0     1163 1970-01-01 00:00:00.000000 httpx_negotiate_sspi-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-05-19 07:47:15.597739 httpx_negotiate_sspi-0.1.0a2/httpx_negotiate_sspi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:48:35.954892 httpx_negotiate_sspi-0.1.0a2/httpx_negotiate_sspi/py.typed
+-rw-r--r--   0        0        0     9432 2023-05-19 08:09:14.317851 httpx_negotiate_sspi-0.1.0a2/httpx_negotiate_sspi/sspi.py
+-rw-r--r--   0        0        0      617 2023-05-19 08:19:43.048891 httpx_negotiate_sspi-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      375 2023-05-19 06:20:48.767290 httpx_negotiate_sspi-0.1.0a2/README.md
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 httpx_negotiate_sspi-0.1.0a2/setup.py
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 httpx_negotiate_sspi-0.1.0a2/PKG-INFO
```

### Comparing `httpx_negotiate_sspi-0.1.0a1/httpx_negotiate_sspi/sspi.py` & `httpx_negotiate_sspi-0.1.0a2/httpx_negotiate_sspi/sspi.py`

 * *Files identical despite different names*

### Comparing `httpx_negotiate_sspi-0.1.0a1/pyproject.toml` & `httpx_negotiate_sspi-0.1.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "httpx-negotiate-sspi"
-version = "0.1.0-alpha.1"
+version = "0.1.0-alpha.2"
 description = "SSPI authentication for httpx"
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "httpx_negotiate_sspi" },
 ]
 repository = "https://github.com/rob-blackbourn/httpx-negotiate-sspi"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pypiwin32 = "^223"
-httpx = "^0.24.1"
+httpx = "> 0.16, < 0.25"
 
 [tool.poetry.dev-dependencies]
 autopep8 = "^2.0"
 pylint = "^2.17"
 mypy = "^1.3"
 
 [build-system]
```

### Comparing `httpx_negotiate_sspi-0.1.0a1/setup.py` & `httpx_negotiate_sspi-0.1.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['httpx_negotiate_sspi']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['httpx>=0.24.1,<0.25.0', 'pypiwin32>=223,<224']
+['httpx>0.16,<0.25', 'pypiwin32>=223,<224']
 
 setup_kwargs = {
     'name': 'httpx-negotiate-sspi',
-    'version': '0.1.0a1',
+    'version': '0.1.0a2',
     'description': 'SSPI authentication for httpx',
     'long_description': '# httpx-negotiate-sspi\n\nAn implementation of HTTP Negotiate authentication for httpx. This module provides single-sign-on using Kerberos or NTLM using the Windows SSPI interface.\n\nThis module supports Extended Protection for Authentication (aka Channel Binding Hash), which makes it usable for services that require it, including Active Directory Federation Services.\n\n',
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rob-blackbourn/httpx-negotiate-sspi',
```

### Comparing `httpx_negotiate_sspi-0.1.0a1/PKG-INFO` & `httpx_negotiate_sspi-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: httpx-negotiate-sspi
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: SSPI authentication for httpx
 Home-page: https://github.com/rob-blackbourn/httpx-negotiate-sspi
 License: Apache-2.0
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: httpx (>0.16,<0.25)
 Requires-Dist: pypiwin32 (>=223,<224)
 Project-URL: Repository, https://github.com/rob-blackbourn/httpx-negotiate-sspi
 Description-Content-Type: text/markdown
 
 # httpx-negotiate-sspi
 
 An implementation of HTTP Negotiate authentication for httpx. This module provides single-sign-on using Kerberos or NTLM using the Windows SSPI interface.
```

