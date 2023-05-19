# Comparing `tmp/pgq-3.7.1.tar.gz` & `tmp/pgq-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgq-3.7.1.tar", last modified: Thu Aug 11 12:10:24 2022, max compression
+gzip compressed data, was "pgq-3.7.2.tar", last modified: Fri May 19 07:38:48 2023, max compression
```

## Comparing `pgq-3.7.1.tar` & `pgq-3.7.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 12:10:24.646288 pgq-3.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-11 12:10:21.000000 pgq-3.7.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)    15665 2022-08-11 12:10:21.000000 pgq-3.7.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-08-11 12:10:21.000000 pgq-3.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-08-11 12:10:24.646288 pgq-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-08-11 12:10:21.000000 pgq-3.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 12:10:24.642288 pgq-3.7.1/pgq/
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12074 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/baseconsumer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 12:10:24.642288 pgq-3.7.1/pgq/cascade/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/cascade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    62914 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/cascade/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    10604 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/cascade/consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)    12238 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/cascade/nodeinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)    17878 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/cascade/worker.py
--rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/coopconsumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     7617 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/localconsumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/producer.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     6585 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/remoteconsumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3555 2022-08-11 12:10:21.000000 pgq-3.7.1/pgq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 12:10:24.642288 pgq-3.7.1/pgq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-08-11 12:10:24.000000 pgq-3.7.1/pgq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-08-11 12:10:24.000000 pgq-3.7.1/pgq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 12:10:24.000000 pgq-3.7.1/pgq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-11 12:10:24.000000 pgq-3.7.1/pgq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-11 12:10:24.000000 pgq-3.7.1/pgq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-11 12:10:24.646288 pgq-3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-08-11 12:10:21.000000 pgq-3.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 12:10:24.646288 pgq-3.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-08-11 12:10:21.000000 pgq-3.7.1/tests/test_pgq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-11 12:10:21.000000 pgq-3.7.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:38:48.348418 pgq-3.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 07:38:45.000000 pgq-3.7.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-05-19 07:38:45.000000 pgq-3.7.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-19 07:38:45.000000 pgq-3.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-19 07:38:48.348418 pgq-3.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-19 07:38:45.000000 pgq-3.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:38:48.348418 pgq-3.7.2/pgq/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/baseconsumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:38:48.348418 pgq-3.7.2/pgq/cascade/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/cascade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62910 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/cascade/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/cascade/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/cascade/nodeinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/cascade/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/coopconsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/localconsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/remoteconsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-19 07:38:45.000000 pgq-3.7.2/pgq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:38:48.348418 pgq-3.7.2/pgq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-19 07:38:48.000000 pgq-3.7.2/pgq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-19 07:38:48.000000 pgq-3.7.2/pgq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:38:48.000000 pgq-3.7.2/pgq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 07:38:48.000000 pgq-3.7.2/pgq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 07:38:48.000000 pgq-3.7.2/pgq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 07:38:48.348418 pgq-3.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-19 07:38:45.000000 pgq-3.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:38:48.348418 pgq-3.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-19 07:38:45.000000 pgq-3.7.2/tests/test_pgq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 07:38:45.000000 pgq-3.7.2/tox.ini
```

### Comparing `pgq-3.7.1/.pylintrc` & `pgq-3.7.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/PKG-INFO` & `pgq-3.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgq
-Version: 3.7.1
+Version: 3.7.2
 Summary: PgQ client library for Python
 Home-page: https://github.com/pgq/python-pgq
 Maintainer: Marko Kreen
 Maintainer-email: markokr@gmail.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pgq-3.7.1/pgq/__init__.py` & `pgq-3.7.2/pgq/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     'Event', 'Consumer', 'CoopConsumer', 'LocalConsumer',
     'bulk_insert_events', 'insert_event',
     'RemoteConsumer', 'SerialConsumer', 'PGQStatus',
     'CascadeAdmin', 'CascadedConsumer', 'CascadedWorker',
     'MemberInfo', 'NodeInfo', 'QueueInfo'
 ]
 
-__version__ = '3.7.1'
+__version__ = '3.7.2'
```

### Comparing `pgq-3.7.1/pgq/baseconsumer.py` & `pgq-3.7.2/pgq/baseconsumer.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/cascade/admin.py` & `pgq-3.7.2/pgq/cascade/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,16 +485,16 @@
 
     def load_node_status(self, name: str, location: str) -> NodeInfo:
         """ Load node info & status """
         # must be thread-safe (!)
         if not self.node_alive(name):
             node = NodeInfo(self.queue_name or '', None, node_name=name, location=location)
             return node
+        db = None
         try:
-            db = None
             db = skytools.connect_database(location)
             db.set_isolation_level(skytools.I_AUTOCOMMIT)
             curs = db.cursor()
             curs.execute("select * from pgq_node.get_node_info(%s)", [self.queue_name])
             node = NodeInfo(self.queue_name or '', curs.fetchone(), location=location)
             node.load_status(curs)
             self.load_extra_status(curs, node)
```

### Comparing `pgq-3.7.1/pgq/cascade/consumer.py` & `pgq-3.7.2/pgq/cascade/consumer.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/cascade/nodeinfo.py` & `pgq-3.7.2/pgq/cascade/nodeinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         self._info_lines = []
         self.cascaded_consumer_map = {}
         self.node_attrs = {}
         self.child_list = []
         self.total_childs = 0
         self.levels = 0
         self.service = None
+        self.provider_node = None
 
         self._row = row
 
         if location:
             m = re.search(r'service=(\S+)', location)
             if m:
                 self.service = m.group(1)
```

### Comparing `pgq-3.7.1/pgq/cascade/worker.py` & `pgq-3.7.2/pgq/cascade/worker.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/consumer.py` & `pgq-3.7.2/pgq/consumer.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/coopconsumer.py` & `pgq-3.7.2/pgq/coopconsumer.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/event.py` & `pgq-3.7.2/pgq/event.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/localconsumer.py` & `pgq-3.7.2/pgq/localconsumer.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/producer.py` & `pgq-3.7.2/pgq/producer.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/remoteconsumer.py` & `pgq-3.7.2/pgq/remoteconsumer.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq/status.py` & `pgq-3.7.2/pgq/status.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/pgq.egg-info/PKG-INFO` & `pgq-3.7.2/pgq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgq
-Version: 3.7.1
+Version: 3.7.2
 Summary: PgQ client library for Python
 Home-page: https://github.com/pgq/python-pgq
 Maintainer: Marko Kreen
 Maintainer-email: markokr@gmail.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pgq-3.7.1/setup.py` & `pgq-3.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/tests/test_pgq.py` & `pgq-3.7.2/tests/test_pgq.py`

 * *Files identical despite different names*

### Comparing `pgq-3.7.1/tox.ini` & `pgq-3.7.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 [tox]
-envlist = lint,py38
+envlist = lint,py3
 
 [package]
 name = pgq
 deps =
-    psycopg2-binary==2.9.3
-    skytools==3.8
+    psycopg2-binary==2.9.5
+    skytools==3.8.1
 test_deps =
-    coverage==6.4.1
-    pytest==7.1.2
-    pytest-cov==3.0.0
+    coverage==6.5.0
+    pytest==7.2.0
+    pytest-cov==4.0.0
 lint_deps =
-    pylint==2.14.4
-    flake8==4.0.1
-    mypy==0.961
-    pytype==2022.6.30
+    pylint==2.15.6
+    flake8==5.0.4
+    mypy==0.991
+    pytype==2022.11.18
 
 [testenv]
 changedir = {envsitepackagesdir}
 deps =
     {[package]deps}
     {[package]test_deps}
 passenv =
```

