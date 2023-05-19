# Comparing `tmp/flaskosql-1.0.1.tar.gz` & `tmp/flaskosql-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskosql-1.0.1.tar", last modified: Fri May 19 19:53:30 2023, max compression
+gzip compressed data, was "flaskosql-1.0.2.tar", last modified: Fri May 19 21:19:30 2023, max compression
```

## Comparing `flaskosql-1.0.1.tar` & `flaskosql-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:53:30.654758 flaskosql-1.0.1/
--rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      799 2023-05-19 19:53:30.652829 flaskosql-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 19:53:30.627762 flaskosql-1.0.1/flaskosql/
--rw-rw-rw-   0        0        0        0 2023-05-19 19:34:12.000000 flaskosql-1.0.1/flaskosql/__init__.py
--rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.1/flaskosql/db.py
--rw-rw-rw-   0        0        0      887 2023-05-19 18:59:18.000000 flaskosql-1.0.1/flaskosql/field.py
--rw-rw-rw-   0        0        0     6475 2023-05-19 19:08:41.000000 flaskosql-1.0.1/flaskosql/model.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:53:30.648763 flaskosql-1.0.1/flaskosql.egg-info/
--rw-rw-rw-   0        0        0      799 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 19:53:30.000000 flaskosql-1.0.1/flaskosql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 19:53:30.654758 flaskosql-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-05-19 19:52:56.000000 flaskosql-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:19:30.388600 flaskosql-1.0.2/
+-rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      799 2023-05-19 21:19:30.386598 flaskosql-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 21:19:30.359602 flaskosql-1.0.2/flaskosql/
+-rw-rw-rw-   0        0        0        0 2023-05-19 19:34:12.000000 flaskosql-1.0.2/flaskosql/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.2/flaskosql/db.py
+-rw-rw-rw-   0        0        0      887 2023-05-19 18:59:18.000000 flaskosql-1.0.2/flaskosql/field.py
+-rw-rw-rw-   0        0        0     6467 2023-05-19 21:18:24.000000 flaskosql-1.0.2/flaskosql/model.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:19:30.381604 flaskosql-1.0.2/flaskosql.egg-info/
+-rw-rw-rw-   0        0        0      799 2023-05-19 21:19:29.000000 flaskosql-1.0.2/flaskosql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-19 21:19:30.000000 flaskosql-1.0.2/flaskosql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 21:19:29.000000 flaskosql-1.0.2/flaskosql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 21:19:29.000000 flaskosql-1.0.2/flaskosql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 21:19:29.000000 flaskosql-1.0.2/flaskosql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 21:19:30.389603 flaskosql-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-05-19 21:17:27.000000 flaskosql-1.0.2/setup.py
```

### Comparing `flaskosql-1.0.1/PKG-INFO` & `flaskosql-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.1
+Version: 1.0.2
 Summary: ORM for ORACLE DB for FLASK API
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.1/flaskosql/db.py` & `flaskosql-1.0.2/flaskosql/db.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.1/flaskosql/field.py` & `flaskosql-1.0.2/flaskosql/field.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.1/flaskosql/model.py` & `flaskosql-1.0.2/flaskosql/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cx_Oracle
-from __db__ import Connect
-from __field__ import Field
+from db import Connect
+from field import Field
 
 class Model:
     _connection = None
     
     # Constructor : it takes two arguments (self ("this" in other languages and *kwargs wich can be translated to string of values))
     def __init__(self, **kwargs):
         # Initialize the object with provided attributes
```

### Comparing `flaskosql-1.0.1/flaskosql.egg-info/PKG-INFO` & `flaskosql-1.0.2/flaskosql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.1
+Version: 1.0.2
 Summary: ORM for ORACLE DB for FLASK API
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.1/setup.py` & `flaskosql-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'ORM for ORACLE DB for FLASK API'
 LONG_DESCRIPTION = 'An ORM that allow us to connect with the ORACLE DB using OOP concept, plus the interaction with the database in order to create a rest API using FLASK framwork '
 
 # Setting up
 setup(
     name="flaskosql",
     version=VERSION,
```

