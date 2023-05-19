# Comparing `tmp/flaskosql-1.0.3.tar.gz` & `tmp/flaskosql-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskosql-1.0.3.tar", last modified: Fri May 19 21:35:27 2023, max compression
+gzip compressed data, was "flaskosql-1.0.4.tar", last modified: Fri May 19 21:42:14 2023, max compression
```

## Comparing `flaskosql-1.0.3.tar` & `flaskosql-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 21:35:27.268700 flaskosql-1.0.3/
--rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      799 2023-05-19 21:35:27.266692 flaskosql-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 21:35:27.237698 flaskosql-1.0.3/flaskosql/
--rw-rw-rw-   0        0        0        0 2023-05-19 19:34:12.000000 flaskosql-1.0.3/flaskosql/__init__.py
--rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.3/flaskosql/db.py
--rw-rw-rw-   0        0        0      887 2023-05-19 18:59:18.000000 flaskosql-1.0.3/flaskosql/field.py
--rw-rw-rw-   0        0        0     6445 2023-05-19 21:27:54.000000 flaskosql-1.0.3/flaskosql/model.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:35:27.262686 flaskosql-1.0.3/flaskosql.egg-info/
--rw-rw-rw-   0        0        0      799 2023-05-19 21:35:26.000000 flaskosql-1.0.3/flaskosql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-19 21:35:27.000000 flaskosql-1.0.3/flaskosql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 21:35:26.000000 flaskosql-1.0.3/flaskosql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 21:35:26.000000 flaskosql-1.0.3/flaskosql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 21:35:26.000000 flaskosql-1.0.3/flaskosql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 21:35:27.269692 flaskosql-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-05-19 21:35:20.000000 flaskosql-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:42:14.857229 flaskosql-1.0.4/
+-rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      799 2023-05-19 21:42:14.854210 flaskosql-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 21:42:14.831228 flaskosql-1.0.4/flaskosql/
+-rw-rw-rw-   0        0        0        0 2023-05-19 19:34:12.000000 flaskosql-1.0.4/flaskosql/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.4/flaskosql/db.py
+-rw-rw-rw-   0        0        0      887 2023-05-19 18:59:18.000000 flaskosql-1.0.4/flaskosql/field.py
+-rw-rw-rw-   0        0        0     6418 2023-05-19 21:41:17.000000 flaskosql-1.0.4/flaskosql/model.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:42:14.850209 flaskosql-1.0.4/flaskosql.egg-info/
+-rw-rw-rw-   0        0        0      799 2023-05-19 21:42:14.000000 flaskosql-1.0.4/flaskosql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-19 21:42:14.000000 flaskosql-1.0.4/flaskosql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 21:42:14.000000 flaskosql-1.0.4/flaskosql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 21:42:14.000000 flaskosql-1.0.4/flaskosql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 21:42:14.000000 flaskosql-1.0.4/flaskosql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 21:42:14.858213 flaskosql-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-05-19 21:41:26.000000 flaskosql-1.0.4/setup.py
```

### Comparing `flaskosql-1.0.3/PKG-INFO` & `flaskosql-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.3
+Version: 1.0.4
 Summary: ORM for ORACLE DB for FLASK API
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.3/flaskosql/db.py` & `flaskosql-1.0.4/flaskosql/db.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.3/flaskosql/field.py` & `flaskosql-1.0.4/flaskosql/field.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.3/flaskosql/model.py` & `flaskosql-1.0.4/flaskosql/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import cx_Oracle
-from field import Field
-
 
 class Model:
     _connection = None
     
     # Constructor : it takes two arguments (self ("this" in other languages and *kwargs wich can be translated to string of values))
     def __init__(self, **kwargs):
         # Initialize the object with provided attributes
```

### Comparing `flaskosql-1.0.3/flaskosql.egg-info/PKG-INFO` & `flaskosql-1.0.4/flaskosql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.3
+Version: 1.0.4
 Summary: ORM for ORACLE DB for FLASK API
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.3/setup.py` & `flaskosql-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'ORM for ORACLE DB for FLASK API'
 LONG_DESCRIPTION = 'An ORM that allow us to connect with the ORACLE DB using OOP concept, plus the interaction with the database in order to create a rest API using FLASK framwork '
 
 # Setting up
 setup(
     name="flaskosql",
     version=VERSION,
```

