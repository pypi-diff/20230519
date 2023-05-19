# Comparing `tmp/jwt_validate-0.2.0.tar.gz` & `tmp/jwt_validate-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwt_validate-0.2.0.tar", max compression
+gzip compressed data, was "jwt_validate-0.3.0.tar", max compression
```

## Comparing `jwt_validate-0.2.0.tar` & `jwt_validate-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.2.0/index.md
--rw-r--r--   0        0        0     2062 2023-05-19 12:15:04.332279 jwt_validate-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.2.0/src/__init__.py
--rw-r--r--   0        0        0      751 2023-05-16 20:05:04.152366 jwt_validate-0.2.0/src/config.py
--rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.2.0/src/constants.py
--rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.2.0/src/exceptions.py
--rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.2.0/src/generate/generate_jwt.py
--rw-r--r--   0        0        0      432 2023-05-16 22:18:03.768247 jwt_validate-0.2.0/src/main.py
--rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.2.0/src/utils.py
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.2.0/src/validate/__init__.py
--rw-r--r--   0        0        0     2984 2023-05-16 20:32:12.173909 jwt_validate-0.2.0/src/validate/validate_jwt.py
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 jwt_validate-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.0/index.md
+-rw-r--r--   0        0        0     2062 2023-05-19 12:29:47.767403 jwt_validate-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.0/src/__init__.py
+-rw-r--r--   0        0        0      800 2023-05-19 12:28:52.132461 jwt_validate-0.3.0/src/config.py
+-rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.0/src/constants.py
+-rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.0/src/exceptions.py
+-rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.3.0/src/generate/generate_jwt.py
+-rw-r--r--   0        0        0      432 2023-05-16 22:18:03.768247 jwt_validate-0.3.0/src/main.py
+-rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.0/src/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.0/src/validate/__init__.py
+-rw-r--r--   0        0        0     2984 2023-05-16 20:32:12.173909 jwt_validate-0.3.0/src/validate/validate_jwt.py
+-rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 jwt_validate-0.3.0/PKG-INFO
```

### Comparing `jwt_validate-0.2.0/index.md` & `jwt_validate-0.3.0/index.md`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.2.0/pyproject.toml` & `jwt_validate-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwt-validate"
-version = "0.2.0"
+version = "0.3.0"
 description = "Library for validation token JWT"
 authors = ["Reinaldo Saraiva do Carmo <reinaldo.carmo@luizalabs.com>"]
 license = "BeerWare"
 readme = "index.md"
 packages = [{include = "src"}]
 
 classifiers = [
@@ -15,15 +15,15 @@
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 httpx = "^0.24.0"
 pytest-mock = "^3.10.0"
 pytest-asyncio = "^0.21.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
```

### Comparing `jwt_validate-0.2.0/src/exceptions.py` & `jwt_validate-0.3.0/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.2.0/src/validate/validate_jwt.py` & `jwt_validate-0.3.0/src/validate/validate_jwt.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.2.0/PKG-INFO` & `jwt_validate-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: jwt-validate
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library for validation token JWT
 License: Beerware
 Author: Reinaldo Saraiva do Carmo
 Author-email: reinaldo.carmo@luizalabs.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Description-Content-Type: text/markdown
```

