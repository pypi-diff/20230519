# Comparing `tmp/metis-client-0.0.3.tar.gz` & `tmp/metis_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metis-client-0.0.3.tar", last modified: Thu Mar  2 15:29:20 2023, max compression
+gzip compressed data, was "metis_client-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metis-client-0.0.3.tar` & `metis_client-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,70 @@
--rw-r--r--   0        0        0     1452 2023-01-23 13:58:03.866671 metis-client-0.0.3/LICENSE
--rw-r--r--   0        0        0     2619 2023-03-02 15:19:32.274148 metis-client-0.0.3/README.md
--rw-r--r--   0        0        0      241 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/__init__.py
--rw-r--r--   0        0        0    10748 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/client.py
--rw-r--r--   0        0        0      625 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/const.py
--rw-r--r--   0        0        0      658 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/__init__.py
--rw-r--r--   0        0        0      314 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/auth.py
--rw-r--r--   0        0        0      386 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/base.py
--rw-r--r--   0        0        0      625 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/calculation.py
--rw-r--r--   0        0        0     1355 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/collection.py
--rw-r--r--   0        0        0      796 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/datasource.py
--rw-r--r--   0        0        0      405 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/error.py
--rw-r--r--   0        0        0     2183 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/event.py
--rw-r--r--   0        0        0      282 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/resp.py
--rw-r--r--   0        0        0      683 2023-03-02 15:19:32.274148 metis-client-0.0.3/metis_client/dtos/user.py
--rw-r--r--   0        0        0     1378 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/exc.py
--rw-r--r--   0        0        0     4342 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/helpers.py
--rw-r--r--   0        0        0     6409 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/metis.py
--rw-r--r--   0        0        0     3736 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/metis_async.py
--rw-r--r--   0        0        0      266 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/models/__init__.py
--rw-r--r--   0        0        0     2915 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/models/auth.py
--rw-r--r--   0        0        0      230 2023-01-28 21:31:09.184650 metis-client-0.0.3/metis_client/models/base.py
--rw-r--r--   0        0        0     2410 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/models/event.py
--rw-r--r--   0        0        0     1751 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/models/hub.py
--rw-r--r--   0        0        0     2839 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/models/subscription.py
--rw-r--r--   0        0        0        0 2023-01-23 13:56:27.097113 metis-client-0.0.3/metis_client/namespaces/__init__.py
--rw-r--r--   0        0        0      940 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/namespaces/auth.py
--rw-r--r--   0        0        0      934 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/namespaces/base.py
--rw-r--r--   0        0        0     3058 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/namespaces/calculations.py
--rw-r--r--   0        0        0     3554 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/namespaces/collections.py
--rw-r--r--   0        0        0     2961 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/namespaces/datasources.py
--rw-r--r--   0        0        0     1064 2023-01-28 21:31:09.184650 metis-client-0.0.3/metis_client/namespaces/root.py
--rw-r--r--   0        0        0     2293 2023-03-02 15:19:32.278148 metis-client-0.0.3/metis_client/namespaces/stream.py
--rw-r--r--   0        0        0     1675 2023-02-13 15:30:29.160409 metis-client-0.0.3/metis_client/namespaces/v0.py
--rw-r--r--   0        0        0     3013 2023-03-02 15:19:32.278148 metis-client-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 metis-client-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      372 2023-05-19 14:20:57.706607 metis_client-0.3.0/.flake8
+-rw-r--r--   0        0        0      212 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1396 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/linter.yml
+-rw-r--r--   0        0        0      792 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/pr.yml
+-rw-r--r--   0        0        0     1852 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/push.yml
+-rw-r--r--   0        0        0      867 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1338 2023-05-19 14:20:57.706607 metis_client-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1869 2023-05-19 14:20:57.706607 metis_client-0.3.0/.gitignore
+-rw-r--r--   0        0        0      275 2023-05-19 14:20:57.706607 metis_client-0.3.0/.whitesource
+-rw-r--r--   0        0        0      820 2023-05-19 14:20:57.706607 metis_client-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      492 2023-05-19 14:20:57.706607 metis_client-0.3.0/CITATION.cff
+-rw-r--r--   0        0        0     2819 2023-05-19 14:20:57.706607 metis_client-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1452 2023-05-19 14:20:57.706607 metis_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1746 2023-05-19 14:20:57.706607 metis_client-0.3.0/README.md
+-rw-r--r--   0        0        0      156 2023-05-19 14:20:57.706607 metis_client-0.3.0/examples/data/user_object_one.dat
+-rw-r--r--   0        0        0     2818 2023-05-19 14:20:57.706607 metis_client-0.3.0/examples/example_async.py
+-rw-r--r--   0        0        0     2601 2023-05-19 14:20:57.706607 metis_client-0.3.0/examples/example_sync.py
+-rw-r--r--   0        0        0      241 2023-05-19 14:20:57.706607 metis_client-0.3.0/metis_client/__init__.py
+-rw-r--r--   0        0        0    10756 2023-05-19 14:20:57.706607 metis_client-0.3.0/metis_client/client.py
+-rw-r--r--   0        0        0      625 2023-05-19 14:20:57.706607 metis_client-0.3.0/metis_client/const.py
+-rw-r--r--   0        0        0      691 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/auth.py
+-rw-r--r--   0        0        0      386 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/base.py
+-rw-r--r--   0        0        0      625 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/calculation.py
+-rw-r--r--   0        0        0     1355 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/collection.py
+-rw-r--r--   0        0        0     1002 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/datasource.py
+-rw-r--r--   0        0        0      405 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/error.py
+-rw-r--r--   0        0        0     2183 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/event.py
+-rw-r--r--   0        0        0      282 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/resp.py
+-rw-r--r--   0        0        0      683 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/dtos/user.py
+-rw-r--r--   0        0        0     1474 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/exc.py
+-rw-r--r--   0        0        0     4342 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/helpers.py
+-rw-r--r--   0        0        0     8599 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/metis.py
+-rw-r--r--   0        0        0     3736 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/metis_async.py
+-rw-r--r--   0        0        0      266 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/__init__.py
+-rw-r--r--   0        0        0     2915 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/auth.py
+-rw-r--r--   0        0        0      230 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/base.py
+-rw-r--r--   0        0        0     2410 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/event.py
+-rw-r--r--   0        0        0     1751 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/hub.py
+-rw-r--r--   0        0        0     2839 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/models/subscription.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/auth.py
+-rw-r--r--   0        0        0      934 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/base.py
+-rw-r--r--   0        0        0     7250 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/calculations.py
+-rw-r--r--   0        0        0     3554 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/collections.py
+-rw-r--r--   0        0        0     3847 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/datasources.py
+-rw-r--r--   0        0        0     1064 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/root.py
+-rw-r--r--   0        0        0     2293 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/stream.py
+-rw-r--r--   0        0        0     1675 2023-05-19 14:20:57.710607 metis_client-0.3.0/metis_client/namespaces/v0.py
+-rw-r--r--   0        0        0     3447 2023-05-19 14:20:57.710607 metis_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      217 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/__init__.py
+-rw-r--r--   0        0        0      824 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_auth_no_auth.py
+-rw-r--r--   0        0        0     3139 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_auth_password.py
+-rw-r--r--   0        0        0     1175 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_auth_token.py
+-rw-r--r--   0        0        0      484 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_event.py
+-rw-r--r--   0        0        0      211 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_hub.py
+-rw-r--r--   0        0        0      821 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/models/test_subscription.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/__init__.py
+-rw-r--r--   0        0        0     3761 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/test_auth.py
+-rw-r--r--   0        0        0    12339 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/test_calculations.py
+-rw-r--r--   0        0        0     7952 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/test_collections.py
+-rw-r--r--   0        0        0    10776 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/namespaces/test_datasources.py
+-rw-r--r--   0        0        0    11730 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_client.py
+-rw-r--r--   0        0        0      332 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_exc.py
+-rw-r--r--   0        0        0     1023 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_helpers_convert_dict_items_to_datetime.py
+-rw-r--r--   0        0        0      976 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_helpers_rfc3339.py
+-rw-r--r--   0        0        0      236 2023-05-19 14:20:57.710607 metis_client-0.3.0/tests/test_metis_async.py
+-rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 metis_client-0.3.0/PKG-INFO
```

### Comparing `metis-client-0.0.3/LICENSE` & `metis_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/README.md` & `metis_client-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,59 @@
 # Metis API client
 
-![PyPI](https://img.shields.io/pypi/v/metis_client.svg?style=flat)
+[![DOI](https://zenodo.org/badge/563802198.svg)](https://doi.org/10.5281/zenodo.7693569)
+[![PyPI](https://img.shields.io/pypi/v/metis_client.svg?style=flat)](https://pypi.org/project/metis-client)
 
 <p align="center"><img src="https://github.com/tilde-lab/metis.science/blob/master/src/assets/img/metis.svg" width="300" height="300" /></p>
 
 This library allows for programmatic interactions with the [Metis infrastructure](https://metis.science).
 
 ## Installation
 
 `pip install metis_client`
 
 ## Usage
 
-There are two client flavors - asyncronous `asyncio` client
-and simplified synchronous client.
+There are two client flavors: **asyncronous** `asyncio` client
+and simplified **synchronous** client.
 
 ### Asynchronous client
 
-There is a asynchronous client `MetisAPIAsync`. Example of usage:
+An asynchronous client is `MetisAPIAsync`. Example of usage:
 
 ```python
 from metis_client import MetisAPIAsync, MetisTokenAuth
 
 async def main():
-    async with MetisAPIAsync(API_URL, auth=MetisTokenAuth("admin@test.com")) as client:
+    async with MetisAPIAsync(API_URL, auth=MetisTokenAuth("VERY_SECRET_TOKEN")) as client:
         print(await client.v0.auth.whoami())
         data = await client.v0.datasources.create(content)
-        calc = await client.v0.calculations.create(data["id"])
-        print(calc)
-
-        # There is also a low level interface
-        from metis_client.models import MetisDataSourcesEventModel, MetisCalculationsEventModel
-        async with client.stream.subscribe() as sub:
-            req = await client.v0.datasources.create_event(content)
-            async for msg in sub:
-                if msg["type"] == "datasources" and msg.get("data", {}).get(
-                    "reqId"
-                ) == req.get("reqId"):
-                    answer = msg.get("data")
-                    break
-            if not answer:
-                return None
-
-            data_id = sorted(
-                answer.get("data", []),
-                key=lambda x: x.get("createdAt", datetime.fromordinal(1)),
-            )[-1].get("id")
-            req = await client.v0.calculations.create_event(data_id)
-            answer = None
-            async for msg in sub:
-                if msg["type"] == "calculations" and msg.get("data", {}).get(
-                    "reqId"
-                ) == req.get("reqId"):
-                    data = msg.get("data", {}).get("data", [])
-                    if data:
-                        answer = data[-1]
-                    break
-            print(answer)
+        results = await client.v0.calculations.create_get_results(data["id"])
+        print(resuls)
 ```
 
 See `examples` directory for more examples.
 
 ### Synchronous client
 
-There is a synchronous client `MetisAPI`. Example of usage:
+A synchronous client is `MetisAPI`. Example of usage:
 
 ```python
 from metis_client import MetisAPI, MetisTokenAuth
 
-client = MetisAPI(API_URL, auth=MetisTokenAuth("admin@test.com"))
+client = MetisAPI(API_URL, auth=MetisTokenAuth("VERY_SECRET_TOKEN"))
 data = client.v0.datasources.create(content)
-calc = client.v0.calculations.create(data.get("id"))
-print(calc)
+results = client.v0.calculations.create_get_results(data["id"])
+print(results)
 ```
 
+NB in development one can replace a `VERY_SECRET_TOKEN` string with the development user email, e.g.
+`admin@test.com` (refer to **users_emails** BFF table).
+
 ## License
 
 Author Sergey Korolev, Tilde Materials Informatics
 
 Copyright 2023 BASF SE
 
 BSD 3-Clause
+  * [ ]
```

### Comparing `metis-client-0.0.3/metis_client/client.py` & `metis_client-0.3.0/metis_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     timeout: NotRequired[float]
     auth_required: NotRequired[bool]
 
 
 class MetisClient(MetisBase):
     """
     Client to handle API calls.
-    Don't use this directly, use `metis_client.metis.Metis` to get the client.
+    Don't use this directly, use `metis_client.metis.Metis` instead to get the client.
     """
 
     _auth: BaseAuthenticator
     _base_url: URL
 
     def __init__(
         self,
```

### Comparing `metis-client-0.0.3/metis_client/const.py` & `metis_client-0.3.0/metis_client/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Constants for metis_client."""
 
 from __future__ import annotations
 
 from logging import Logger, getLogger
 from typing import Literal, Union
 
-PROJECT_VERSION = "0.0.3"
+PROJECT_VERSION = "0.3.0"
 PROJECT_NAME = "metis_client"
 
 # This is the default user agent,
 # but it is adviced to use your own when building out your application
 DEFAULT_USER_AGENT = f"metis_client/{PROJECT_VERSION}"
```

### Comparing `metis-client-0.0.3/metis_client/dtos/calculation.py` & `metis_client-0.3.0/metis_client/dtos/calculation.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 
 class MetisCalculationDTO(MetisTimestampsDTO):
     "Calculation DTO"
     id: int
     name: str
     userId: int
-    status: int
     progress: int
+    parent: int
     result: NotRequired[Sequence[MetisDataSourceDTO]]
```

### Comparing `metis-client-0.0.3/metis_client/dtos/collection.py` & `metis_client-0.3.0/metis_client/dtos/collection.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/dtos/datasource.py` & `metis_client-0.3.0/metis_client/dtos/datasource.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Data sources DTOs"""
 
 import sys
+from enum import Enum
 
 from .base import MetisTimestampsDTO
 from .collection import MetisCollectionDTO
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Sequence
 else:  # pragma: no cover
@@ -12,25 +13,35 @@
 
 if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import TypedDict
 else:  # pragma: no cover
     from typing import TypedDict
 
 
+class DataSourceType(int, Enum):
+    "Data source types"
+    STRUCTURE = 1
+    CALCULATION = 2
+    PROPERTY = 3
+    WORKFLOW = 4
+    PATTERN = 5
+
+
 class MetisDataSourceDTO(MetisTimestampsDTO):
     "Data source DTO"
 
     id: int
+    parents: Sequence[int]
+    children: Sequence[int]
     userId: int
     userFirstName: str
     userLastName: str
     userEmail: str
     name: str
     content: str
     type: int
     collections: Sequence[MetisCollectionDTO]
-    progress: int
 
 
 class MetisDataSourceContentOnlyDTO(TypedDict):
     "Data source content only DTO"
     content: str
```

### Comparing `metis-client-0.0.3/metis_client/dtos/event.py` & `metis_client-0.3.0/metis_client/dtos/event.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/dtos/user.py` & `metis_client-0.3.0/metis_client/dtos/user.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/exc.py` & `metis_client-0.3.0/metis_client/exc.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     ):
         super().__init__(*args, **kwargs)
         if status:
             self.status = status
         if message:
             self.message = message
 
+    def __str__(self) -> str:
+        return f"status: {self.status}, message: {self.message}"
+
 
 class MetisNotFoundException(MetisError):
     """This is raised when the requested resource is not found."""
 
 
 class MetisPayloadException(MetisError):
     """This is raised when the payload is invalid."""
```

### Comparing `metis-client-0.0.3/metis_client/helpers.py` & `metis_client-0.3.0/metis_client/helpers.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/metis.py` & `metis_client-0.3.0/metis_client/metis.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Metis API synchronous client"""
 
 import sys
 from functools import partial
-from typing import Any, TypeVar, cast
+from typing import Any, Optional, Sequence, TypeVar, cast
 
 from aiohttp.typedefs import StrOrURL
 from asgiref.sync import async_to_sync
 
+from metis_client.dtos.datasource import MetisDataSourceDTO
+
 from .metis_async import MetisAPIAsync, MetisAPIKwargs
 from .models.base import MetisBase
+from .namespaces.calculations import MetisCalculationOnProgressT
 from .namespaces.collections import MetisCollectionsCreateKwargs
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Awaitable, Callable
 else:  # pragma: no cover
     from collections.abc import Awaitable, Callable
 
 if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import Concatenate, ParamSpec, Unpack
 else:  # pragma: no cover
     from typing import Concatenate, ParamSpec, Unpack
 
+
 AsyncClientGetter = Callable[[], MetisAPIAsync]
 ReturnT_co = TypeVar("ReturnT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 
 
 # pylint: disable=too-few-public-methods
 class MetisNamespaceSyncBase:
@@ -70,80 +74,142 @@
         return await client.v0.auth.whoami()
 
 
 class MetisDatasourcesNamespaceSync(MetisNamespaceSyncBase):
     """Datasources endpoints namespace"""
 
     @to_sync_with_metis_client
-    async def create(self, client: MetisAPIAsync, content: str):
-        "Create data source and wait for result"
-        return await client.v0.datasources.create(content)
+    async def create(
+        self,
+        client: MetisAPIAsync,
+        content: str,
+        fmt: Optional[str] = None,
+        name: Optional[str] = None,
+    ):
+        "Create data source and wait for the result"
+        return await client.v0.datasources.create(content, fmt, name)
 
     @to_sync_with_metis_client
     async def delete(self, client: MetisAPIAsync, data_id: int):
-        "Delete data source by id and wait for result"
+        "Delete data source by id and wait for the result"
         return await client.v0.datasources.delete(data_id)
 
     @to_sync_with_metis_client
     async def list(self, client: MetisAPIAsync):
-        "List data sources and wait for result"
+        "List data sources and wait for the result"
         return await client.v0.datasources.list()
 
     @to_sync_with_metis_client
-    async def get(self, client: MetisAPIAsync, data_id: int):
+    async def get(
+        self, client: MetisAPIAsync, data_id: int
+    ) -> Optional[MetisDataSourceDTO]:
         "Get data source by id"
         return await client.v0.datasources.get(data_id)
 
+    @to_sync_with_metis_client
+    async def get_parents(
+        self, client: MetisAPIAsync, data_id: int
+    ) -> Sequence[MetisDataSourceDTO]:
+        "Get parent data sources by id"
+        return await client.v0.datasources.get_parents(data_id)
+
+    @to_sync_with_metis_client
+    async def get_children(
+        self, client: MetisAPIAsync, data_id: int
+    ) -> Sequence[MetisDataSourceDTO]:
+        "Get children data sources by id"
+        return await client.v0.datasources.get_children(data_id)
+
+    @to_sync_with_metis_client
+    async def get_content(self, client: MetisAPIAsync, data_id: int):
+        "Get data source by id"
+        return await client.v0.datasources.get_content(data_id)
+
 
 class MetisCalculationsNamespaceSync(MetisNamespaceSyncBase):
     """Calculations endpoints namespace"""
 
     @to_sync_with_metis_client
     async def cancel(self, client: MetisAPIAsync, calc_id: int):
-        "Cancel calculation and wait for result"
+        "Cancel calculation and wait for the result"
         return await client.v0.calculations.cancel(calc_id)
 
     @to_sync_with_metis_client
-    async def create(self, client: MetisAPIAsync, data_id: int, engine: str = "dummy"):
-        "Create calculation and wait for result"
-        return await client.v0.calculations.create(data_id, engine)
+    async def create(
+        self,
+        client: MetisAPIAsync,
+        data_id: int,
+        engine: str = "dummy",
+        input: Optional[str] = None,  # pylint: disable=redefined-builtin
+    ):
+        "Create calculation and wait for the result"
+        return await client.v0.calculations.create(data_id, engine, input)
+
+    @to_sync_with_metis_client
+    async def get_results(
+        self,
+        client: MetisAPIAsync,
+        calc_id: int,
+        on_progress: Optional[MetisCalculationOnProgressT] = None,
+    ):
+        "Waits for the end of the calculation and returns the results"
+        return await client.v0.calculations.get_results(calc_id, on_progress)
+
+    @to_sync_with_metis_client
+    async def create_get_results(
+        self,
+        client: MetisAPIAsync,
+        data_id: int,
+        engine: str = "dummy",
+        input: Optional[str] = None,  # pylint: disable=redefined-builtin
+        on_progress: Optional[MetisCalculationOnProgressT] = None,
+    ):
+        "Create calculation, wait done and get results"
+        return await client.v0.calculations.create_get_results(
+            data_id, engine, input, on_progress
+        )
 
     @to_sync_with_metis_client
     async def get_engines(self, client: MetisAPIAsync):
         "Get supported calculation engines"
         return await client.v0.calculations.get_engines()
 
     @to_sync_with_metis_client
     async def list(self, client: MetisAPIAsync):
-        "List all user's calculations and wait for result"
+        "List all user's calculations and wait for the result"
         return await client.v0.calculations.list()
 
+    @to_sync_with_metis_client
+    async def get(self, client: MetisAPIAsync, calc_id: int):
+        "Get calculation by id"
+        return await client.v0.calculations.get(calc_id)
+
 
 class MetisCollectionsNamespaceSync(MetisNamespaceSyncBase):
     """Collections endpoints namespace"""
 
     @to_sync_with_metis_client
     async def create(
         self,
         client: MetisAPIAsync,
         type_id: int,
         title: str,
         **opts: Unpack[MetisCollectionsCreateKwargs],
     ):
-        "Create collection and wait for result"
+        "Create collection and wait for the result"
         return await client.v0.collections.create(type_id, title, **opts)
 
     @to_sync_with_metis_client
     async def list(self, client: MetisAPIAsync):
-        "List user's collections by criteria and wait for result"
+        "List user's collections by criteria and wait for the result"
         return await client.v0.collections.list()
 
     @to_sync_with_metis_client
     async def delete(self, client: MetisAPIAsync, collection_id: int):
-        "Remove a collection by id and wait for result"
+        "Remove a collection by id and wait for the result"
         return await client.v0.collections.delete(collection_id)
 
 
 # pylint: disable=too-few-public-methods
 class MetisV0NamespaceSync(MetisNamespaceSyncBase):
     """v0 namespace"""
```

### Comparing `metis-client-0.0.3/metis_client/metis_async.py` & `metis_client-0.3.0/metis_client/metis_async.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/models/auth.py` & `metis_client-0.3.0/metis_client/models/auth.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/models/event.py` & `metis_client-0.3.0/metis_client/models/event.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/models/hub.py` & `metis_client-0.3.0/metis_client/models/hub.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/models/subscription.py` & `metis_client-0.3.0/metis_client/models/subscription.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/namespaces/auth.py` & `metis_client-0.3.0/metis_client/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/namespaces/base.py` & `metis_client-0.3.0/metis_client/namespaces/base.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/namespaces/collections.py` & `metis_client-0.3.0/metis_client/namespaces/collections.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/namespaces/datasources.py` & `metis_client-0.3.0/metis_client/namespaces/datasources.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 else:  # pragma: no cover
     from collections.abc import Sequence
 
 
 class MetisDatasourcesNamespace(BaseNamespace):
     """Datasources endpoints namespace"""
 
-    async def create_event(self, content: str) -> MetisRequestIdDTO:
+    async def create_event(
+        self, content: str, fmt: Optional[str] = None, name: Optional[str] = None
+    ) -> MetisRequestIdDTO:
         "Create data source"
         async with self._client.request(
             method="POST",
             url=self._base_url,
-            json={"content": content},
+            json={"content": content, "fmt": fmt, "name": name},
             auth_required=True,
         ) as resp:
             return await resp.json()
 
-    async def create(self, content: str) -> Optional[MetisDataSourceDTO]:
-        "Create data source and wait for result"
+    async def create(
+        self, content: str, fmt: Optional[str] = None, name: Optional[str] = None
+    ) -> Optional[MetisDataSourceDTO]:
+        "Create data source and wait for the result"
         evt = await act_and_get_result_from_stream(
-            self._root.stream.subscribe, partial(self.create_event, content)
+            self._root.stream.subscribe, partial(self.create_event, content, fmt, name)
         )
         if evt["type"] == "datasources":
             data = sorted(
                 evt.get("data", {}).get("data", []),
                 key=lambda x: x.get("createdAt", datetime.fromordinal(1)),
             )
             return data[-1] if data else None
@@ -47,39 +51,56 @@
             method="DELETE",
             url=self._base_url / str(data_id),
             auth_required=True,
         ) as resp:
             return await resp.json()
 
     async def delete(self, data_id: int) -> None:
-        "Delete data source by id and wait for result"
+        "Delete data source by id and wait for the result"
         await act_and_get_result_from_stream(
             self._root.stream.subscribe, partial(self.delete_event, data_id)
         )
 
     async def list_event(self) -> MetisRequestIdDTO:
         "List data sources"
         async with self._client.request(
             method="GET",
             url=self._base_url,
             auth_required=True,
         ) as resp:
             return await resp.json()
 
     async def list(self) -> Sequence[MetisDataSourceDTO]:
-        "List data sources and wait for result"
+        "List data sources and wait for the result"
         evt = await act_and_get_result_from_stream(
             self._root.stream.subscribe, partial(self.list_event)
         )
         if evt["type"] == "datasources":
             return evt.get("data", {}).get("data", [])
         return []  # pragma: no cover
 
+    async def get(self, data_id: int) -> Optional[MetisDataSourceDTO]:
+        "Get data source by id"
+        data = list(filter(lambda x: x["id"] == data_id, await self.list()))
+        return data[-1] if data else None
+
+    async def get_parents(self, data_id: int) -> Sequence[MetisDataSourceDTO]:
+        "Get parent data sources by id"
+        return list(
+            filter(lambda x: data_id in x.get("children", []), await self.list())
+        )
+
+    async def get_children(self, data_id: int) -> Sequence[MetisDataSourceDTO]:
+        "Get children data sources by id"
+        return list(
+            filter(lambda x: data_id in x.get("parents", []), await self.list())
+        )
+
     @raise_on_metis_error
-    async def get(self, data_id: int) -> MetisDataSourceContentOnlyDTO:
+    async def get_content(self, data_id: int) -> MetisDataSourceContentOnlyDTO:
         "Get data source by id"
         async with self._client.request(
             method="GET",
             url=self._base_url / str(data_id),
             auth_required=True,
         ) as resp:
             return await resp.json()
```

### Comparing `metis-client-0.0.3/metis_client/namespaces/root.py` & `metis_client-0.3.0/metis_client/namespaces/root.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/namespaces/stream.py` & `metis_client-0.3.0/metis_client/namespaces/stream.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/metis_client/namespaces/v0.py` & `metis_client-0.3.0/metis_client/namespaces/v0.py`

 * *Files identical despite different names*

### Comparing `metis-client-0.0.3/pyproject.toml` & `metis_client-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # build the package with [flit](https://flit.readthedocs.io)
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "metis-client"
-dynamic = ["version"]  # read from metis_client/__init__.py
+version = "0.3.0"
 description = """Metis infra API client in Python"""
 authors = [{name = "Sergei Korolev", email = "knopki@duck.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: BSD License",
@@ -37,30 +37,37 @@
 
 [project.optional-dependencies]
 debug = [
       "wdb"
 ]
 lint = [
      "autoflake",
-     "black",
+     "black >= 23.1",
      "flake8",
      "flake8-bugbear",
      "isort",
      "mypy >= 1.0.0, <2",
      "pylint",
      "pylint-per-file-ignores >= 1",
      "pyupgrade",
 ]
 test = [
     "freezegun",
     "pytest-aiohttp >= 1.0.4, <2",
     "pytest-cov",
 ]
+release = [
+    "commitizen",
+    "flit",
+]
 
 [project.urls]
+Home = "https://github.com/tilde-lab/metis-client"
+Changelog = "https://github.com/tilde-lab/metis-client/blob/master/CHANGELOG.md"
+Issues = "https://github.com/tilde-lab/metis-client/issues"
 Source = "https://github.com/tilde-lab/metis-client"
 
 [tool.flit.module]
 name = "metis_client"
 
 [tool.autoflake]
 expand-star-imports = true
@@ -118,8 +125,19 @@
 score = "no"
 
 [tool.pylint-per-file-ignores]
 "/tests/" = "redefined-outer-name"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
-addopts = "--cov=metis_client --cov-report=term --cov-report=html --no-cov-on-fail --cov-fail-under=99"
+addopts = "--cov=metis_client --cov-report=term --no-cov-on-fail --cov-fail-under=99"
+
+[tool.commitizen]
+name = "cz_conventional_commits"
+version = "0.3.0"
+tag_format = "v$version"
+major_version_zero = true
+version_files = [
+    "pyproject.toml:^version",
+    "metis_client/const.py:^PROJECT_VERSION",
+]
+update_changelog_on_bump = true
```

### Comparing `metis-client-0.0.3/PKG-INFO` & `metis_client-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metis-client
-Version: 0.0.3
+Version: 0.3.0
 Summary: Metis infra API client in Python
 Keywords: metis,client
 Author-email: Sergei Korolev <knopki@duck.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -22,107 +22,89 @@
 Requires-Dist: aiohttp >= 3.7.4
 Requires-Dist: aiohttp-sse-client >= 0.2.1
 Requires-Dist: asgiref >= 3.5.2
 Requires-Dist: typing-extensions >= 4.2.0; python_version < '3.11'
 Requires-Dist: yarl >= 1.6.3
 Requires-Dist: wdb ; extra == "debug"
 Requires-Dist: autoflake ; extra == "lint"
-Requires-Dist: black ; extra == "lint"
+Requires-Dist: black >= 23.1 ; extra == "lint"
 Requires-Dist: flake8 ; extra == "lint"
 Requires-Dist: flake8-bugbear ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: mypy >= 1.0.0, <2 ; extra == "lint"
 Requires-Dist: pylint ; extra == "lint"
 Requires-Dist: pylint-per-file-ignores >= 1 ; extra == "lint"
 Requires-Dist: pyupgrade ; extra == "lint"
+Requires-Dist: commitizen ; extra == "release"
+Requires-Dist: flit ; extra == "release"
 Requires-Dist: freezegun ; extra == "test"
 Requires-Dist: pytest-aiohttp >= 1.0.4, <2 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
+Project-URL: Changelog, https://github.com/tilde-lab/metis-client/blob/master/CHANGELOG.md
+Project-URL: Home, https://github.com/tilde-lab/metis-client
+Project-URL: Issues, https://github.com/tilde-lab/metis-client/issues
 Project-URL: Source, https://github.com/tilde-lab/metis-client
 Provides-Extra: debug
 Provides-Extra: lint
+Provides-Extra: release
 Provides-Extra: test
 
 # Metis API client
 
-![PyPI](https://img.shields.io/pypi/v/metis_client.svg?style=flat)
+[![DOI](https://zenodo.org/badge/563802198.svg)](https://doi.org/10.5281/zenodo.7693569)
+[![PyPI](https://img.shields.io/pypi/v/metis_client.svg?style=flat)](https://pypi.org/project/metis-client)
 
 <p align="center"><img src="https://github.com/tilde-lab/metis.science/blob/master/src/assets/img/metis.svg" width="300" height="300" /></p>
 
 This library allows for programmatic interactions with the [Metis infrastructure](https://metis.science).
 
 ## Installation
 
 `pip install metis_client`
 
 ## Usage
 
-There are two client flavors - asyncronous `asyncio` client
-and simplified synchronous client.
+There are two client flavors: **asyncronous** `asyncio` client
+and simplified **synchronous** client.
 
 ### Asynchronous client
 
-There is a asynchronous client `MetisAPIAsync`. Example of usage:
+An asynchronous client is `MetisAPIAsync`. Example of usage:
 
 ```python
 from metis_client import MetisAPIAsync, MetisTokenAuth
 
 async def main():
-    async with MetisAPIAsync(API_URL, auth=MetisTokenAuth("admin@test.com")) as client:
+    async with MetisAPIAsync(API_URL, auth=MetisTokenAuth("VERY_SECRET_TOKEN")) as client:
         print(await client.v0.auth.whoami())
         data = await client.v0.datasources.create(content)
-        calc = await client.v0.calculations.create(data["id"])
-        print(calc)
-
-        # There is also a low level interface
-        from metis_client.models import MetisDataSourcesEventModel, MetisCalculationsEventModel
-        async with client.stream.subscribe() as sub:
-            req = await client.v0.datasources.create_event(content)
-            async for msg in sub:
-                if msg["type"] == "datasources" and msg.get("data", {}).get(
-                    "reqId"
-                ) == req.get("reqId"):
-                    answer = msg.get("data")
-                    break
-            if not answer:
-                return None
-
-            data_id = sorted(
-                answer.get("data", []),
-                key=lambda x: x.get("createdAt", datetime.fromordinal(1)),
-            )[-1].get("id")
-            req = await client.v0.calculations.create_event(data_id)
-            answer = None
-            async for msg in sub:
-                if msg["type"] == "calculations" and msg.get("data", {}).get(
-                    "reqId"
-                ) == req.get("reqId"):
-                    data = msg.get("data", {}).get("data", [])
-                    if data:
-                        answer = data[-1]
-                    break
-            print(answer)
+        results = await client.v0.calculations.create_get_results(data["id"])
+        print(resuls)
 ```
 
 See `examples` directory for more examples.
 
 ### Synchronous client
 
-There is a synchronous client `MetisAPI`. Example of usage:
+A synchronous client is `MetisAPI`. Example of usage:
 
 ```python
 from metis_client import MetisAPI, MetisTokenAuth
 
-client = MetisAPI(API_URL, auth=MetisTokenAuth("admin@test.com"))
+client = MetisAPI(API_URL, auth=MetisTokenAuth("VERY_SECRET_TOKEN"))
 data = client.v0.datasources.create(content)
-calc = client.v0.calculations.create(data.get("id"))
-print(calc)
+results = client.v0.calculations.create_get_results(data["id"])
+print(results)
 ```
 
+NB in development one can replace a `VERY_SECRET_TOKEN` string with the development user email, e.g.
+`admin@test.com` (refer to **users_emails** BFF table).
+
 ## License
 
 Author Sergey Korolev, Tilde Materials Informatics
 
 Copyright 2023 BASF SE
 
 BSD 3-Clause
+  * [ ]
```

