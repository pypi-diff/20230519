# Comparing `tmp/flaskosql-1.0.0.tar.gz` & `tmp/flaskosql-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskosql-1.0.0.tar", last modified: Fri May 19 19:37:09 2023, max compression
+gzip compressed data, was "flaskosql-1.0.1.tar", last modified: Fri May 19 19:53:30 2023, max compression
```

## Comparing `flaskosql-1.0.0.tar` & `flaskosql-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:37:09.352413 flaskosql-1.0.0/
--rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      799 2023-05-19 19:37:09.350401 flaskosql-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 19:37:09.344400 flaskosql-1.0.0/flaskosql.egg-info/
--rw-rw-rw-   0        0        0      799 2023-05-19 19:37:09.000000 flaskosql-1.0.0/flaskosql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-19 19:37:09.000000 flaskosql-1.0.0/flaskosql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:37:09.000000 flaskosql-1.0.0/flaskosql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 19:37:09.000000 flaskosql-1.0.0/flaskosql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:37:09.000000 flaskosql-1.0.0/flaskosql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 19:37:09.352413 flaskosql-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-05-19 19:35:58.000000 flaskosql-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:53:30.654758 flaskosql-1.0.1/
+-rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      799 2023-05-19 19:53:30.652829 flaskosql-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 19:53:30.627762 flaskosql-1.0.1/flaskosql/
+-rw-rw-rw-   0        0        0        0 2023-05-19 19:34:12.000000 flaskosql-1.0.1/flaskosql/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.1/flaskosql/db.py
+-rw-rw-rw-   0        0        0      887 2023-05-19 18:59:18.000000 flaskosql-1.0.1/flaskosql/field.py
+-rw-rw-rw-   0        0        0     6475 2023-05-19 19:08:41.000000 flaskosql-1.0.1/flaskosql/model.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:53:30.648763 flaskosql-1.0.1/flaskosql.egg-info/
+-rw-rw-rw-   0        0        0      799 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:53:30.654758 flaskosql-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-05-19 19:52:56.000000 flaskosql-1.0.1/setup.py
```

### Comparing `flaskosql-1.0.0/PKG-INFO` & `flaskosql-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.0
+Version: 1.0.1
 Summary: ORM for ORACLE DB for FLASK API
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.0/flaskosql.egg-info/PKG-INFO` & `flaskosql-1.0.1/flaskosql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.0
+Version: 1.0.1
 Summary: ORM for ORACLE DB for FLASK API
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.0/setup.py` & `flaskosql-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'ORM for ORACLE DB for FLASK API'
 LONG_DESCRIPTION = 'An ORM that allow us to connect with the ORACLE DB using OOP concept, plus the interaction with the database in order to create a rest API using FLASK framwork '
 
 # Setting up
 setup(
     name="flaskosql",
     version=VERSION,
```

