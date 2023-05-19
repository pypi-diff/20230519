# Comparing `tmp/jwt_validate-0.3.1.tar.gz` & `tmp/jwt_validate-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwt_validate-0.3.1.tar", max compression
+gzip compressed data, was "jwt_validate-0.3.2.tar", max compression
```

## Comparing `jwt_validate-0.3.1.tar` & `jwt_validate-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.1/index.md
--rw-r--r--   0        0        0     2062 2023-05-19 12:34:24.336847 jwt_validate-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.1/src/__init__.py
--rw-r--r--   0        0        0      764 2023-05-19 12:34:14.706449 jwt_validate-0.3.1/src/config.py
--rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.1/src/constants.py
--rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.1/src/exceptions.py
--rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.3.1/src/generate/generate_jwt.py
--rw-r--r--   0        0        0      432 2023-05-16 22:18:03.768247 jwt_validate-0.3.1/src/main.py
--rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.1/src/utils.py
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.1/src/validate/__init__.py
--rw-r--r--   0        0        0     2984 2023-05-16 20:32:12.173909 jwt_validate-0.3.1/src/validate/validate_jwt.py
--rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 jwt_validate-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.2/index.md
+-rw-r--r--   0        0        0     2062 2023-05-19 12:36:58.904101 jwt_validate-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.2/src/__init__.py
+-rw-r--r--   0        0        0      773 2023-05-19 12:36:44.634536 jwt_validate-0.3.2/src/config.py
+-rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.2/src/constants.py
+-rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.2/src/exceptions.py
+-rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.3.2/src/generate/generate_jwt.py
+-rw-r--r--   0        0        0      432 2023-05-16 22:18:03.768247 jwt_validate-0.3.2/src/main.py
+-rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.2/src/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.2/src/validate/__init__.py
+-rw-r--r--   0        0        0     2984 2023-05-16 20:32:12.173909 jwt_validate-0.3.2/src/validate/validate_jwt.py
+-rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 jwt_validate-0.3.2/PKG-INFO
```

### Comparing `jwt_validate-0.3.1/index.md` & `jwt_validate-0.3.2/index.md`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.1/pyproject.toml` & `jwt_validate-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwt-validate"
-version = "0.3.1"
+version = "0.3.2"
 description = "Library for validation token JWT"
 authors = ["Reinaldo Saraiva do Carmo <reinaldo.carmo@luizalabs.com>"]
 license = "BeerWare"
 readme = "index.md"
 packages = [{include = "src"}]
 
 classifiers = [
```

### Comparing `jwt_validate-0.3.1/src/config.py` & `jwt_validate-0.3.2/src/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 from src.constants import Environment
 
 
 class Config(BaseSettings):
     env_file = find_dotenv('.secrets/.env')
     env_file_encoding = 'utf-8'
-    # ENVIRONMENT: Environment = Environment.LOCAL
+    ENVIRONMENT: Environment = Environment.LOCAL
     # DEBUG: bool = False
     # CORS_ORIGINS: List[str]
     # CORS_ORIGINS_REGEX: str | None
     # CORS_HEADERS: List[str]
     IDPA_URL: str
     # APP_VERSION: str = '1'
 
 
 settings = Config(_env_file='.env')
 
 app_configs: dict[str, Any] = {'title': 'JWT-Validation - API'}
-if settings.ENVIRONMENT.is_deployed:
-    app_configs['root_path'] = f'/v{settings.APP_VERSION}'
+# if settings.ENVIRONMENT.is_deployed:
+#     app_configs['root_path'] = f'/v{settings.APP_VERSION}'
 
-if not settings.ENVIRONMENT.is_debug:
-    app_configs['openapi_url'] = None  # hide docs
-#
+# if not settings.ENVIRONMENT.is_debug:
+#     app_configs['openapi_url'] = None  # hide docs
+# #
```

### Comparing `jwt_validate-0.3.1/src/exceptions.py` & `jwt_validate-0.3.2/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.1/src/validate/validate_jwt.py` & `jwt_validate-0.3.2/src/validate/validate_jwt.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.1/PKG-INFO` & `jwt_validate-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwt-validate
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for validation token JWT
 License: Beerware
 Author: Reinaldo Saraiva do Carmo
 Author-email: reinaldo.carmo@luizalabs.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
```

