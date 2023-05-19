# Comparing `tmp/peewee-async-0.8.0.tar.gz` & `tmp/peewee-async-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee-async-0.8.0.tar", last modified: Mon Jul 11 10:09:16 2022, max compression
+gzip compressed data, was "peewee-async-0.8.1.tar", last modified: Fri May 19 08:14:31 2023, max compression
```

## Comparing `peewee-async-0.8.0.tar` & `peewee-async-0.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gorshkov_n  (1000) gorshkov_n  (1000)        0 2022-07-11 10:09:16.792853 peewee-async-0.8.0/
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     1096 2021-03-18 05:04:12.000000 peewee-async-0.8.0/LICENSE
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     3753 2022-07-11 10:09:16.792853 peewee-async-0.8.0/PKG-INFO
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     3107 2022-07-11 09:48:18.000000 peewee-async-0.8.0/README.md
-drwxrwxr-x   0 gorshkov_n  (1000) gorshkov_n  (1000)        0 2022-07-11 10:09:16.792853 peewee-async-0.8.0/peewee_async.egg-info/
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     3753 2022-07-11 10:09:16.000000 peewee-async-0.8.0/peewee_async.egg-info/PKG-INFO
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)      285 2022-07-11 10:09:16.000000 peewee-async-0.8.0/peewee_async.egg-info/SOURCES.txt
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)        1 2022-07-11 10:09:16.000000 peewee-async-0.8.0/peewee_async.egg-info/dependency_links.txt
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)        1 2021-03-18 05:13:25.000000 peewee-async-0.8.0/peewee_async.egg-info/not-zip-safe
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)      138 2022-07-11 10:09:16.000000 peewee-async-0.8.0/peewee_async.egg-info/requires.txt
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)       29 2022-07-11 10:09:16.000000 peewee-async-0.8.0/peewee_async.egg-info/top_level.txt
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)    45797 2022-07-11 09:46:36.000000 peewee-async-0.8.0/peewee_async.py
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     2927 2021-10-12 09:39:01.000000 peewee-async-0.8.0/peewee_asyncext.py
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)       73 2022-07-11 10:09:16.792853 peewee-async-0.8.0/setup.cfg
--rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     1600 2022-07-08 10:00:59.000000 peewee-async-0.8.0/setup.py
+drwxrwxr-x   0 gorshkov_n  (1000) gorshkov_n  (1000)        0 2023-05-19 08:14:31.824782 peewee-async-0.8.1/
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     1096 2021-03-18 05:04:12.000000 peewee-async-0.8.1/LICENSE
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     3538 2023-05-19 08:14:31.824782 peewee-async-0.8.1/PKG-INFO
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     2892 2023-05-19 07:55:05.000000 peewee-async-0.8.1/README.md
+drwxrwxr-x   0 gorshkov_n  (1000) gorshkov_n  (1000)        0 2023-05-19 08:14:31.824782 peewee-async-0.8.1/peewee_async.egg-info/
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     3538 2023-05-19 08:14:31.000000 peewee-async-0.8.1/peewee_async.egg-info/PKG-INFO
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)      285 2023-05-19 08:14:31.000000 peewee-async-0.8.1/peewee_async.egg-info/SOURCES.txt
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)        1 2023-05-19 08:14:31.000000 peewee-async-0.8.1/peewee_async.egg-info/dependency_links.txt
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)        1 2023-05-19 08:14:31.000000 peewee-async-0.8.1/peewee_async.egg-info/not-zip-safe
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)      139 2023-05-19 08:14:31.000000 peewee-async-0.8.1/peewee_async.egg-info/requires.txt
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)       29 2023-05-19 08:14:31.000000 peewee-async-0.8.1/peewee_async.egg-info/top_level.txt
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)    45898 2023-05-19 08:08:48.000000 peewee-async-0.8.1/peewee_async.py
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     2927 2021-10-12 09:39:01.000000 peewee-async-0.8.1/peewee_asyncext.py
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)       73 2023-05-19 08:14:31.824782 peewee-async-0.8.1/setup.cfg
+-rw-rw-r--   0 gorshkov_n  (1000) gorshkov_n  (1000)     1603 2023-05-19 07:21:07.000000 peewee-async-0.8.1/setup.py
```

### Comparing `peewee-async-0.8.0/LICENSE` & `peewee-async-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peewee-async-0.8.0/PKG-INFO` & `peewee-async-0.8.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-async
-Version: 0.8.0
+Version: 0.8.1
 Summary: Asynchronous interface for peewee ORM powered by asyncio.
 Home-page: https://github.com/05bit/peewee-async
 Author: Alexey Kinev
 Author-email: rudy@05bit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -23,25 +23,19 @@
 
 Asynchronous interface for **[peewee](https://github.com/coleifer/peewee)**
 ORM powered by **[asyncio](https://docs.python.org/3/library/asyncio.html)**.
 
 ![CI workflow](https://github.com/05bit/peewee-async/actions/workflows/ci.yml/badge.svg) [![PyPi Version](https://img.shields.io/pypi/v/peewee-async.svg)](https://pypi.python.org/pypi/peewee-async)
  [![Documentation Status](https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat)](http://peewee-async.readthedocs.io/en/latest/?badge=latest)
 
-Important notes
----------------
-
-- Since version `0.6.0a` only **peewee 3.5+** is supported
-- If you still need Python 3.5 support use older versions, i.e. `pip install peewee-async==0.7.2`
-
 
 Overview
 --------
 
-* Requires Python 3.6+
+* Requires Python 3.7+
 * Has support for PostgreSQL via [aiopg](https://github.com/aio-libs/aiopg)
 * Has support for MySQL via [aiomysql](https://github.com/aio-libs/aiomysql)
 * Single point for high-level async API
 * Drop-in replacement for sync code, sync will remain sync
 * Basic operations are supported
 * Transactions support is present, yet not heavily tested
 
@@ -66,15 +60,15 @@
 Quickstart
 ----------
 
 Create 'test' PostgreSQL database for running this snippet:
 
     createdb -E utf-8 test
 
-The code below is using new Python 3.6 `async` / `await` syntax
+
 ```python
 import asyncio
 import peewee
 import peewee_async
 
 # Nothing special, just define model and database:
 
@@ -127,19 +121,23 @@
 
 Documentation
 -------------
 
 http://peewee-async.readthedocs.io
 
 Developing
--------------
+----------
 Install dependencies:
 ```pip install -e .[develop]```
 
-Run tests: ``` pytest tests -v -s```
+Run databases:
+```docker-compose up -d```
+
+Run tests:
+```pytest tests -v -s```
 
 Discuss
 -------
 
 You are welcome to add discussion topics or bug reports to tracker on GitHub: https://github.com/05bit/peewee-async/issues
 
 License
```

### Comparing `peewee-async-0.8.0/README.md` & `peewee-async-0.8.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,25 +3,19 @@
 
 Asynchronous interface for **[peewee](https://github.com/coleifer/peewee)**
 ORM powered by **[asyncio](https://docs.python.org/3/library/asyncio.html)**.
 
 ![CI workflow](https://github.com/05bit/peewee-async/actions/workflows/ci.yml/badge.svg) [![PyPi Version](https://img.shields.io/pypi/v/peewee-async.svg)](https://pypi.python.org/pypi/peewee-async)
  [![Documentation Status](https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat)](http://peewee-async.readthedocs.io/en/latest/?badge=latest)
 
-Important notes
----------------
-
-- Since version `0.6.0a` only **peewee 3.5+** is supported
-- If you still need Python 3.5 support use older versions, i.e. `pip install peewee-async==0.7.2`
-
 
 Overview
 --------
 
-* Requires Python 3.6+
+* Requires Python 3.7+
 * Has support for PostgreSQL via [aiopg](https://github.com/aio-libs/aiopg)
 * Has support for MySQL via [aiomysql](https://github.com/aio-libs/aiomysql)
 * Single point for high-level async API
 * Drop-in replacement for sync code, sync will remain sync
 * Basic operations are supported
 * Transactions support is present, yet not heavily tested
 
@@ -46,15 +40,15 @@
 Quickstart
 ----------
 
 Create 'test' PostgreSQL database for running this snippet:
 
     createdb -E utf-8 test
 
-The code below is using new Python 3.6 `async` / `await` syntax
+
 ```python
 import asyncio
 import peewee
 import peewee_async
 
 # Nothing special, just define model and database:
 
@@ -107,19 +101,23 @@
 
 Documentation
 -------------
 
 http://peewee-async.readthedocs.io
 
 Developing
--------------
+----------
 Install dependencies:
 ```pip install -e .[develop]```
 
-Run tests: ``` pytest tests -v -s```
+Run databases:
+```docker-compose up -d```
+
+Run tests:
+```pytest tests -v -s```
 
 Discuss
 -------
 
 You are welcome to add discussion topics or bug reports to tracker on GitHub: https://github.com/05bit/peewee-async/issues
 
 License
```

### Comparing `peewee-async-0.8.0/peewee_async.egg-info/PKG-INFO` & `peewee-async-0.8.1/peewee_async.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-async
-Version: 0.8.0
+Version: 0.8.1
 Summary: Asynchronous interface for peewee ORM powered by asyncio.
 Home-page: https://github.com/05bit/peewee-async
 Author: Alexey Kinev
 Author-email: rudy@05bit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -23,25 +23,19 @@
 
 Asynchronous interface for **[peewee](https://github.com/coleifer/peewee)**
 ORM powered by **[asyncio](https://docs.python.org/3/library/asyncio.html)**.
 
 ![CI workflow](https://github.com/05bit/peewee-async/actions/workflows/ci.yml/badge.svg) [![PyPi Version](https://img.shields.io/pypi/v/peewee-async.svg)](https://pypi.python.org/pypi/peewee-async)
  [![Documentation Status](https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat)](http://peewee-async.readthedocs.io/en/latest/?badge=latest)
 
-Important notes
----------------
-
-- Since version `0.6.0a` only **peewee 3.5+** is supported
-- If you still need Python 3.5 support use older versions, i.e. `pip install peewee-async==0.7.2`
-
 
 Overview
 --------
 
-* Requires Python 3.6+
+* Requires Python 3.7+
 * Has support for PostgreSQL via [aiopg](https://github.com/aio-libs/aiopg)
 * Has support for MySQL via [aiomysql](https://github.com/aio-libs/aiomysql)
 * Single point for high-level async API
 * Drop-in replacement for sync code, sync will remain sync
 * Basic operations are supported
 * Transactions support is present, yet not heavily tested
 
@@ -66,15 +60,15 @@
 Quickstart
 ----------
 
 Create 'test' PostgreSQL database for running this snippet:
 
     createdb -E utf-8 test
 
-The code below is using new Python 3.6 `async` / `await` syntax
+
 ```python
 import asyncio
 import peewee
 import peewee_async
 
 # Nothing special, just define model and database:
 
@@ -127,19 +121,23 @@
 
 Documentation
 -------------
 
 http://peewee-async.readthedocs.io
 
 Developing
--------------
+----------
 Install dependencies:
 ```pip install -e .[develop]```
 
-Run tests: ``` pytest tests -v -s```
+Run databases:
+```docker-compose up -d```
+
+Run tests:
+```pytest tests -v -s```
 
 Discuss
 -------
 
 You are welcome to add discussion topics or bug reports to tracker on GitHub: https://github.com/05bit/peewee-async/issues
 
 License
```

### Comparing `peewee-async-0.8.0/peewee_async.py` & `peewee-async-0.8.1/peewee_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     pymysql = None
 
 try:
     asyncio_current_task = asyncio.current_task
 except AttributeError:
     asyncio_current_task = asyncio.Task.current_task
 
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 __all__ = [
     # High level API ###
 
     'Manager',
     'PostgresqlDatabase',
     'PooledPostgresqlDatabase',
@@ -81,15 +81,15 @@
 
 #################
 # Async manager #
 #################
 
 
 class Manager:
-    """Async peewee models manager.
+    """Async peewee model's manager.
 
     :param loop: (optional) asyncio event loop
     :param database: (optional) async database driver
 
     Example::
 
         class User(peewee.Model):
@@ -267,22 +267,22 @@
 
     async def execute(self, query):
         """Execute query asyncronously.
         """
         query = self._swap_database(query)
         return (await execute(query))
 
-    async def prefetch(self, query, *subqueries):
+    async def prefetch(self, query, *subqueries, prefetch_type=peewee.PREFETCH_TYPE.JOIN):
         """Asynchronous version of the `prefetch()` from peewee.
 
         :return: Query that has already cached data for subqueries
         """
         query = self._swap_database(query)
         subqueries = map(self._swap_database, subqueries)
-        return (await prefetch(query, *subqueries))
+        return (await prefetch(query, *subqueries, prefetch_type=prefetch_type))
 
     async def count(self, query, clear_limit=False):
         """Perform *COUNT* aggregated query asynchronously.
 
         :return: number of objects in ``select()`` query
         """
         query = self._swap_database(query)
@@ -695,22 +695,22 @@
         pass
     finally:
         await cursor.release()
 
     return result
 
 
-async def prefetch(sq, *subqueries):
+async def prefetch(sq, *subqueries, prefetch_type):
     """Asynchronous version of the `prefetch()` from peewee.
     """
     if not subqueries:
         result = await execute(sq)
         return result
 
-    fixed_queries = peewee.prefetch_add_subquery(sq, subqueries)
+    fixed_queries = peewee.prefetch_add_subquery(sq, subqueries, prefetch_type)
     deps = {}
     rel_map = {}
 
     for pq in reversed(fixed_queries):
         query_model = pq.model
         if pq.fields:
             for rel_model in pq.rel_models:
```

### Comparing `peewee-async-0.8.0/peewee_asyncext.py` & `peewee-async-0.8.1/peewee_asyncext.py`

 * *Files identical despite different names*

### Comparing `peewee-async-0.8.0/setup.py` & `peewee-async-0.8.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,32 +30,32 @@
     url='https://github.com/05bit/peewee-async',
     description=__doc__.strip(),
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     license='MIT',
     zip_safe=False,
     install_requires=(
-        'peewee>=3.5.0,<4.0',
+        'peewee>=3.15.4,<4.0',
     ),
     extras_require={
         'develop': [
             'pylint',
             'wheel',
             'twine',
             'aiomysql',
             'aiopg',
             'pytest',
-            'pytest-asyncio'
+            'pytest-asyncio',
         ],
         'aiopg': ['aiopg>=0.14.0'],
         'aiomysql': ['aiomysql>=0.0.19'],
     },
     py_modules=[
         'peewee_async',
-        'peewee_asyncext'
+        'peewee_asyncext',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

