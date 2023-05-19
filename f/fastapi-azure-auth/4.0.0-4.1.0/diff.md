# Comparing `tmp/fastapi_azure_auth-4.0.0.tar.gz` & `tmp/fastapi_azure_auth-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_azure_auth-4.0.0.tar", max compression
+gzip compressed data, was "fastapi_azure_auth-4.1.0.tar", max compression
```

## Comparing `fastapi_azure_auth-4.0.0.tar` & `fastapi_azure_auth-4.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-04-04 11:49:48.140700 fastapi_azure_auth-4.0.0/LICENSE
--rw-r--r--   0        0        0     6468 2023-04-04 11:49:48.140700 fastapi_azure_auth-4.0.0/README.md
--rw-r--r--   0        0        0      339 2023-04-04 11:49:48.160700 fastapi_azure_auth-4.0.0/fastapi_azure_auth/__init__.py
--rw-r--r--   0        0        0    19735 2023-04-04 11:49:48.160700 fastapi_azure_auth-4.0.0/fastapi_azure_auth/auth.py
--rw-r--r--   0        0        0      337 2023-04-04 11:49:48.160700 fastapi_azure_auth-4.0.0/fastapi_azure_auth/exceptions.py
--rw-r--r--   0        0        0     4451 2023-04-04 11:49:48.160700 fastapi_azure_auth-4.0.0/fastapi_azure_auth/openid_config.py
--rw-r--r--   0        0        0        0 2023-04-04 11:49:48.160700 fastapi_azure_auth-4.0.0/fastapi_azure_auth/py.typed
--rw-r--r--   0        0        0      733 2023-04-04 11:49:48.160700 fastapi_azure_auth-4.0.0/fastapi_azure_auth/user.py
--rw-r--r--   0        0        0      457 2023-04-04 11:49:48.160700 fastapi_azure_auth-4.0.0/fastapi_azure_auth/utils.py
--rw-r--r--   0        0        0     2365 2023-04-04 11:49:48.160700 fastapi_azure_auth-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     8084 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-19 15:56:38.807537 fastapi_azure_auth-4.1.0/LICENSE
+-rw-r--r--   0        0        0     6468 2023-05-19 15:56:38.807537 fastapi_azure_auth-4.1.0/README.md
+-rw-r--r--   0        0        0      339 2023-05-19 15:56:38.823537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/__init__.py
+-rw-r--r--   0        0        0    19735 2023-05-19 15:56:38.823537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/auth.py
+-rw-r--r--   0        0        0      337 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/exceptions.py
+-rw-r--r--   0        0        0     4451 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/openid_config.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/py.typed
+-rw-r--r--   0        0        0     9000 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/user.py
+-rw-r--r--   0        0        0      457 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/utils.py
+-rw-r--r--   0        0        0     2365 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8033 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.1.0/PKG-INFO
```

### Comparing `fastapi_azure_auth-4.0.0/LICENSE` & `fastapi_azure_auth-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.0.0/README.md` & `fastapi_azure_auth-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.0.0/fastapi_azure_auth/auth.py` & `fastapi_azure_auth-4.1.0/fastapi_azure_auth/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.0.0/fastapi_azure_auth/openid_config.py` & `fastapi_azure_auth-4.1.0/fastapi_azure_auth/openid_config.py`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.0.0/pyproject.toml` & `fastapi_azure_auth-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-azure-auth"
-version = "4.0.0"  # Remember to change in __init__.py as well
+version = "4.1.0"  # Remember to change in __init__.py as well
 description = "Easy and secure implementation of Azure AD for your FastAPI APIs"
 authors = ["Jonas Krüger Svensson <jonas.svensson@intility.no>"]
 readme = "README.md"
 homepage = "https://github.com/intility/fastapi-azure-auth"
 repository = "https://github.com/intility/fastapi-azure-auth"
 documentation = "https://github.com/intility/fastapi-azure-auth"
 keywords = [
```

### Comparing `fastapi_azure_auth-4.0.0/PKG-INFO` & `fastapi_azure_auth-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-azure-auth
-Version: 4.0.0
+Version: 4.1.0
 Summary: Easy and secure implementation of Azure AD for your FastAPI APIs
 Home-page: https://github.com/intility/fastapi-azure-auth
 Keywords: ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi tenant,oauth2,oidc,security,single tenant,starlette,trio
 Author: Jonas Krüger Svensson
 Author-email: jonas.svensson@intility.no
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cryptography (>=40.0.1)
 Requires-Dist: fastapi (>0.68.0)
 Requires-Dist: httpx (>0.18.2)
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.0.0 Summary: Easy and
+Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.1.0 Summary: Easy and
 secure implementation of Azure AD for your FastAPI APIs Home-page: https://
 github.com/intility/fastapi-azure-auth Keywords:
 ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi
 tenant,oauth2,oidc,security,single tenant,starlette,trio Author: Jonas KrÃ¼ger
 Svensson Author-email: jonas.svensson@intility.no Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Software Development Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Dist: cryptography (>=40.0.1) Requires-Dist: fastapi (>0.68.0)
-Requires-Dist: httpx (>0.18.2) Requires-Dist: python-jose[cryptography]
-(>=3.3.0,<4.0.0) Project-URL: Documentation, https://github.com/intility/
-fastapi-azure-auth Project-URL: Repository, https://github.com/intility/
-fastapi-azure-auth Description-Content-Type: text/markdown
+Classifier: Topic :: Software Development Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Application Frameworks Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Dist: cryptography (>=40.0.1) Requires-
+Dist: fastapi (>0.68.0) Requires-Dist: httpx (>0.18.2) Requires-Dist: python-
+jose[cryptography] (>=3.3.0,<4.0.0) Project-URL: Documentation, https://
+github.com/intility/fastapi-azure-auth Project-URL: Repository, https://
+github.com/intility/fastapi-azure-auth Description-Content-Type: text/markdown
       ****** [https://avatars.githubusercontent.com/u/35199565] [https://
   raw.githubusercontent.com/Intility/fastapi-azure-auth/main/docs/static/img/
                               global/fastad.png]
                            FastAPI-Azure-Auth ******
               Azure AD Authentication for FastAPI apps made easy.
              [Python_version] [FastAPI_Version] [Package_version]
                 [Codecov] [Pre-commit] [Black] [mypy] [isort]
```

