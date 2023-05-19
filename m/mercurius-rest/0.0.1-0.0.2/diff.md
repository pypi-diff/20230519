# Comparing `tmp/mercurius-rest-0.0.1.tar.gz` & `tmp/mercurius-rest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercurius-rest-0.0.1.tar", last modified: Fri May 19 16:32:51 2023, max compression
+gzip compressed data, was "mercurius-rest-0.0.2.tar", last modified: Fri May 19 16:34:32 2023, max compression
```

## Comparing `mercurius-rest-0.0.1.tar` & `mercurius-rest-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      434 2023-05-19 15:37:22.900100 mercurius-rest-0.0.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0     1807 2023-05-19 16:32:03.182026 mercurius-rest-0.0.1/.gitignore
--rw-r--r--   0        0        0      107 2023-05-19 16:30:47.503911 mercurius-rest-0.0.1/.pypirc
--rw-r--r--   0        0        0     1075 2023-05-10 15:30:50.430013 mercurius-rest-0.0.1/LICENCE
--rw-r--r--   0        0        0      336 2023-05-19 15:48:06.811404 mercurius-rest-0.0.1/README.md
--rw-r--r--   0        0        0       43 2023-05-14 17:29:50.540410 mercurius-rest-0.0.1/mercurius/rest/__init__.py
--rw-r--r--   0        0        0      132 2023-05-11 10:55:27.667332 mercurius-rest-0.0.1/mercurius/rest/constants.py
--rw-r--r--   0        0        0      862 2023-05-19 15:24:53.531952 mercurius-rest-0.0.1/mercurius/rest/controllers.py
--rw-r--r--   0        0        0    17078 2023-05-15 16:38:37.548685 mercurius-rest-0.0.1/mercurius/rest/datastructures.py
--rw-r--r--   0        0        0      603 2023-05-19 15:29:54.013412 mercurius-rest-0.0.1/mercurius/rest/decorators.py
--rw-r--r--   0        0        0    10481 2023-05-19 14:21:46.753389 mercurius-rest-0.0.1/mercurius/rest/formparsers.py
--rw-r--r--   0        0        0     2547 2023-05-19 15:30:57.235509 mercurius-rest-0.0.1/mercurius/rest/integration.py
--rw-r--r--   0        0        0     8584 2023-05-19 15:33:04.714704 mercurius-rest-0.0.1/mercurius/rest/requests.py
--rw-r--r--   0        0        0    11458 2023-05-14 17:45:30.463971 mercurius-rest-0.0.1/mercurius/rest/responses.py
--rw-r--r--   0        0        0      413 2023-05-19 15:17:20.251279 mercurius-rest-0.0.1/mercurius/rest/router.py
--rw-r--r--   0        0        0    29168 2023-05-19 12:25:51.606473 mercurius-rest-0.0.1/mercurius/rest/test_client.py
--rw-r--r--   0        0        0      502 2023-05-19 12:25:39.508457 mercurius-rest-0.0.1/mercurius/rest/types.py
--rw-r--r--   0        0        0     1286 2023-05-19 15:23:36.808836 mercurius-rest-0.0.1/mercurius/rest/utils/aio.py
--rw-r--r--   0        0        0      155 2023-05-11 11:58:20.486090 mercurius-rest-0.0.1/mercurius/rest/utils/crypto.py
--rw-r--r--   0        0        0      796 2023-05-13 16:02:41.940644 mercurius-rest-0.0.1/mercurius/rest/utils/fallback_handlers.py
--rw-r--r--   0        0        0      868 2023-05-14 17:29:50.517410 mercurius-rest-0.0.1/mercurius/rest/utils/http.py
--rw-r--r--   0        0        0      841 2023-05-19 15:36:44.449041 mercurius-rest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 15:43:14.490951 mercurius-rest-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      307 2023-05-19 14:27:15.468870 mercurius-rest-0.0.1/tests/fixtures.py
--rw-r--r--   0        0        0       23 2023-05-19 14:04:58.429903 mercurius-rest-0.0.1/tests/pytest.ini
--rw-r--r--   0        0        0      439 2023-05-19 15:04:22.389129 mercurius-rest-0.0.1/tests/test_controllers.py
--rw-r--r--   0        0        0    11049 2023-05-19 12:10:08.946359 mercurius-rest-0.0.1/tests/test_datastructures.py
--rw-r--r--   0        0        0      282 2023-05-19 14:57:44.796539 mercurius-rest-0.0.1/tests/test_decorators.py
--rw-r--r--   0        0        0    16344 2023-05-19 14:27:57.911932 mercurius-rest-0.0.1/tests/test_requests.py
--rw-r--r--   0        0        0    12791 2023-05-19 14:53:54.766198 mercurius-rest-0.0.1/tests/test_responses.py
--rw-r--r--   0        0        0     1081 2023-05-19 15:16:53.708240 mercurius-rest-0.0.1/tests/test_router.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 mercurius-rest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-05-19 15:37:22.900100 mercurius-rest-0.0.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1807 2023-05-19 16:32:03.182026 mercurius-rest-0.0.2/.gitignore
+-rw-r--r--   0        0        0      107 2023-05-19 16:30:47.503911 mercurius-rest-0.0.2/.pypirc
+-rw-r--r--   0        0        0     1075 2023-05-10 15:30:50.430013 mercurius-rest-0.0.2/LICENCE
+-rw-r--r--   0        0        0      336 2023-05-19 15:48:06.811404 mercurius-rest-0.0.2/README.md
+-rw-r--r--   0        0        0       43 2023-05-14 17:29:50.540410 mercurius-rest-0.0.2/mercurius/rest/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-11 10:55:27.667332 mercurius-rest-0.0.2/mercurius/rest/constants.py
+-rw-r--r--   0        0        0      862 2023-05-19 15:24:53.531952 mercurius-rest-0.0.2/mercurius/rest/controllers.py
+-rw-r--r--   0        0        0    17078 2023-05-15 16:38:37.548685 mercurius-rest-0.0.2/mercurius/rest/datastructures.py
+-rw-r--r--   0        0        0      603 2023-05-19 15:29:54.013412 mercurius-rest-0.0.2/mercurius/rest/decorators.py
+-rw-r--r--   0        0        0    10481 2023-05-19 14:21:46.753389 mercurius-rest-0.0.2/mercurius/rest/formparsers.py
+-rw-r--r--   0        0        0     2547 2023-05-19 15:30:57.235509 mercurius-rest-0.0.2/mercurius/rest/integration.py
+-rw-r--r--   0        0        0     8584 2023-05-19 15:33:04.714704 mercurius-rest-0.0.2/mercurius/rest/requests.py
+-rw-r--r--   0        0        0    11458 2023-05-14 17:45:30.463971 mercurius-rest-0.0.2/mercurius/rest/responses.py
+-rw-r--r--   0        0        0      413 2023-05-19 15:17:20.251279 mercurius-rest-0.0.2/mercurius/rest/router.py
+-rw-r--r--   0        0        0    29168 2023-05-19 12:25:51.606473 mercurius-rest-0.0.2/mercurius/rest/test_client.py
+-rw-r--r--   0        0        0      502 2023-05-19 12:25:39.508457 mercurius-rest-0.0.2/mercurius/rest/types.py
+-rw-r--r--   0        0        0     1286 2023-05-19 15:23:36.808836 mercurius-rest-0.0.2/mercurius/rest/utils/aio.py
+-rw-r--r--   0        0        0      155 2023-05-11 11:58:20.486090 mercurius-rest-0.0.2/mercurius/rest/utils/crypto.py
+-rw-r--r--   0        0        0      796 2023-05-13 16:02:41.940644 mercurius-rest-0.0.2/mercurius/rest/utils/fallback_handlers.py
+-rw-r--r--   0        0        0      868 2023-05-14 17:29:50.517410 mercurius-rest-0.0.2/mercurius/rest/utils/http.py
+-rw-r--r--   0        0        0      841 2023-05-19 16:34:25.585130 mercurius-rest-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 15:43:14.490951 mercurius-rest-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      307 2023-05-19 14:27:15.468870 mercurius-rest-0.0.2/tests/fixtures.py
+-rw-r--r--   0        0        0       23 2023-05-19 14:04:58.429903 mercurius-rest-0.0.2/tests/pytest.ini
+-rw-r--r--   0        0        0      439 2023-05-19 15:04:22.389129 mercurius-rest-0.0.2/tests/test_controllers.py
+-rw-r--r--   0        0        0    11049 2023-05-19 12:10:08.946359 mercurius-rest-0.0.2/tests/test_datastructures.py
+-rw-r--r--   0        0        0      282 2023-05-19 14:57:44.796539 mercurius-rest-0.0.2/tests/test_decorators.py
+-rw-r--r--   0        0        0    16344 2023-05-19 14:27:57.911932 mercurius-rest-0.0.2/tests/test_requests.py
+-rw-r--r--   0        0        0    12791 2023-05-19 14:53:54.766198 mercurius-rest-0.0.2/tests/test_responses.py
+-rw-r--r--   0        0        0     1081 2023-05-19 15:16:53.708240 mercurius-rest-0.0.2/tests/test_router.py
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 mercurius-rest-0.0.2/PKG-INFO
```

### Comparing `mercurius-rest-0.0.1/.gitignore` & `mercurius-rest-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/LICENCE` & `mercurius-rest-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/controllers.py` & `mercurius-rest-0.0.2/mercurius/rest/controllers.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/datastructures.py` & `mercurius-rest-0.0.2/mercurius/rest/datastructures.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/decorators.py` & `mercurius-rest-0.0.2/mercurius/rest/decorators.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/formparsers.py` & `mercurius-rest-0.0.2/mercurius/rest/formparsers.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/integration.py` & `mercurius-rest-0.0.2/mercurius/rest/integration.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/requests.py` & `mercurius-rest-0.0.2/mercurius/rest/requests.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/responses.py` & `mercurius-rest-0.0.2/mercurius/rest/responses.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/test_client.py` & `mercurius-rest-0.0.2/mercurius/rest/test_client.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/utils/aio.py` & `mercurius-rest-0.0.2/mercurius/rest/utils/aio.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/utils/fallback_handlers.py` & `mercurius-rest-0.0.2/mercurius/rest/utils/fallback_handlers.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/mercurius/rest/utils/http.py` & `mercurius-rest-0.0.2/mercurius/rest/utils/http.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/pyproject.toml` & `mercurius-rest-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mercurius-rest"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Nicholas Lamprecht", email = "nicholas@lamprecht.me" }
 ]
 description = "HTTP Module for the Mercurius Framework"
 readme = "README.md"
 requires-python=">=3.11"
 classifiers = [
@@ -27,12 +27,12 @@
     "trio"
 ]
 
 [tool.flit.module]
 name = "mercurius.rest"
 
 [project.urls]
-"Homepage" = "https://gitlab.com/mercurius-framework/mercurius-core"
+"Homepage" = "https://github.com/mercurius-framework/mercurius-core"
 
 [build-system]
 requires = ["flit>=3.8"]
 build-backend = "flit_core.buildapi"
```

### Comparing `mercurius-rest-0.0.1/tests/test_datastructures.py` & `mercurius-rest-0.0.2/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/tests/test_requests.py` & `mercurius-rest-0.0.2/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/tests/test_responses.py` & `mercurius-rest-0.0.2/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/tests/test_router.py` & `mercurius-rest-0.0.2/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `mercurius-rest-0.0.1/PKG-INFO` & `mercurius-rest-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mercurius-rest
-Version: 0.0.1
+Version: 0.0.2
 Summary: HTTP Module for the Mercurius Framework
 Author-email: Nicholas Lamprecht <nicholas@lamprecht.me>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Dist: anyio==3.6.2
 Requires-Dist: python-multipart==0.2.4
 Requires-Dist: sanic-routing==22.8.0
 Requires-Dist: pytest == 7.3.1 ; extra == "test"
 Requires-Dist: pytest-asyncio==0.21.0 ; extra == "test"
 Requires-Dist: trio ; extra == "test"
-Project-URL: Homepage, https://gitlab.com/mercurius-framework/mercurius-core
+Project-URL: Homepage, https://github.com/mercurius-framework/mercurius-core
 Provides-Extra: test
 
 # Mercurius REST
 [![build](https://github.com/mercurius-framework/mercurius-rest/actions/workflows/build.yaml/badge.svg)](https://github.com/mercurius-framework/mercurius-rest/actions/workflows/build.yaml)
 
 The REST module of the mercurius framework
```

