# Comparing `tmp/latch_postgres-0.1.7.tar.gz` & `tmp/latch_postgres-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_postgres-0.1.7.tar", max compression
+gzip compressed data, was "latch_postgres-0.1.8.tar", max compression
```

## Comparing `latch_postgres-0.1.7.tar` & `latch_postgres-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.7/LICENSE
--rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-10 16:20:18.720567 latch_postgres-0.1.7/latch_postgres/__init__.py
--rw-r--r--   0        0        0    24469 2023-05-17 01:55:18.986327 latch_postgres-0.1.7/latch_postgres/postgres.py
--rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.7/latch_postgres/py.typed
--rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.7/latch_postgres/retries.py
--rw-r--r--   0        0        0     1018 2023-05-17 01:55:35.995411 latch_postgres-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.7/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.8/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 16:20:18.720567 latch_postgres-0.1.8/latch_postgres/__init__.py
+-rw-r--r--   0        0        0    24455 2023-05-19 02:39:34.353217 latch_postgres-0.1.8/latch_postgres/postgres.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.8/latch_postgres/py.typed
+-rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.8/latch_postgres/retries.py
+-rw-r--r--   0        0        0     1735 2023-05-19 02:39:36.113871 latch_postgres-0.1.8/latch_postgres/transactions.py
+-rw-r--r--   0        0        0     1018 2023-05-19 02:40:06.887265 latch_postgres-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.8/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.8/PKG-INFO
```

### Comparing `latch_postgres-0.1.7/LICENSE` & `latch_postgres-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.7/latch_postgres/postgres.py` & `latch_postgres-0.1.8/latch_postgres/postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,17 +211,15 @@
             return None
 
         if len(results) > 1:
             raise RuntimeError(f"received too many rows: '{len(results)}' > 1")
 
         return results[0]
 
-    async def query_void(
-        self, query: sql.SQL, **kwargs: Any
-    ) -> None:
+    async def query_void(self, query: sql.SQL, **kwargs: Any) -> None:
         await self.queryn(type(None), query, **kwargs)
 
 
 @dataclass(frozen=True)
 class EnumInfoQueryResponse:
     nspname: str
     name: str
```

### Comparing `latch_postgres-0.1.7/latch_postgres/retries.py` & `latch_postgres-0.1.8/latch_postgres/retries.py`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.7/pyproject.toml` & `latch_postgres-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-postgres"
-version = "0.1.7"
+version = "0.1.8"
 description = "Postges wrapper for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_postgres"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_postgres-0.1.7/setup.py` & `latch_postgres-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'latch-postgres',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Postges wrapper for latch python backend services',
     'long_description': '# python-postgres\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_postgres-0.1.7/PKG-INFO` & `latch_postgres-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-postgres
-Version: 0.1.7
+Version: 0.1.8
 Summary: Postges wrapper for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

