# Comparing `tmp/jwt_validate-0.3.2.tar.gz` & `tmp/jwt_validate-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwt_validate-0.3.2.tar", max compression
+gzip compressed data, was "jwt_validate-0.3.3.tar", max compression
```

## Comparing `jwt_validate-0.3.2.tar` & `jwt_validate-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.2/index.md
--rw-r--r--   0        0        0     2062 2023-05-19 12:36:58.904101 jwt_validate-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.2/src/__init__.py
--rw-r--r--   0        0        0      773 2023-05-19 12:36:44.634536 jwt_validate-0.3.2/src/config.py
--rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.2/src/constants.py
--rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.2/src/exceptions.py
--rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.3.2/src/generate/generate_jwt.py
--rw-r--r--   0        0        0      432 2023-05-16 22:18:03.768247 jwt_validate-0.3.2/src/main.py
--rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.2/src/utils.py
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.2/src/validate/__init__.py
--rw-r--r--   0        0        0     2984 2023-05-16 20:32:12.173909 jwt_validate-0.3.2/src/validate/validate_jwt.py
--rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 jwt_validate-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.3/index.md
+-rw-r--r--   0        0        0     2112 2023-05-19 13:02:50.110933 jwt_validate-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.3/src/__init__.py
+-rw-r--r--   0        0        0      773 2023-05-19 12:36:44.634536 jwt_validate-0.3.3/src/config.py
+-rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.3/src/constants.py
+-rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.3/src/exceptions.py
+-rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.3.3/src/generate/generate_jwt.py
+-rw-r--r--   0        0        0      432 2023-05-16 22:18:03.768247 jwt_validate-0.3.3/src/main.py
+-rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.3/src/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.3/src/validate/__init__.py
+-rw-r--r--   0        0        0     2984 2023-05-16 20:32:12.173909 jwt_validate-0.3.3/src/validate/validate_jwt.py
+-rw-r--r--   0        0        0     2689 1970-01-01 00:00:00.000000 jwt_validate-0.3.3/PKG-INFO
```

### Comparing `jwt_validate-0.3.2/index.md` & `jwt_validate-0.3.3/index.md`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.2/pyproject.toml` & `jwt_validate-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwt-validate"
-version = "0.3.2"
+version = "0.3.3"
 description = "Library for validation token JWT"
 authors = ["Reinaldo Saraiva do Carmo <reinaldo.carmo@luizalabs.com>"]
 license = "BeerWare"
 readme = "index.md"
 packages = [{include = "src"}]
 
 classifiers = [
@@ -19,14 +19,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.24.0"
 pytest-mock = "^3.10.0"
 pytest-asyncio = "^0.21.0"
+pyjwt = {extras = ["crypto"], version = "^2.7.0"}
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 blue = "^0.9.1"
```

### Comparing `jwt_validate-0.3.2/src/config.py` & `jwt_validate-0.3.3/src/config.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.2/src/exceptions.py` & `jwt_validate-0.3.3/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.2/src/validate/validate_jwt.py` & `jwt_validate-0.3.3/src/validate/validate_jwt.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.2/PKG-INFO` & `jwt_validate-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwt-validate
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library for validation token JWT
 License: Beerware
 Author: Reinaldo Saraiva do Carmo
 Author-email: reinaldo.carmo@luizalabs.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 ![logo do projeto](docs/assets/logo.png){width="100" .center}
 # JWT Validation
```

