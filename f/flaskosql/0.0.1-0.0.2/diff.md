# Comparing `tmp/flaskosql-0.0.1.tar.gz` & `tmp/flaskosql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskosql-0.0.1.tar", last modified: Fri May 19 17:10:36 2023, max compression
+gzip compressed data, was "flaskosql-0.0.2.tar", last modified: Fri May 19 19:11:57 2023, max compression
```

## Comparing `flaskosql-0.0.1.tar` & `flaskosql-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 17:10:36.331962 flaskosql-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-05-19 17:02:17.000000 flaskosql-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      797 2023-05-19 17:10:36.330008 flaskosql-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-19 15:35:29.000000 flaskosql-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 17:10:36.323987 flaskosql-0.0.1/flaskosql.egg-info/
--rw-rw-rw-   0        0        0      797 2023-05-19 17:10:36.000000 flaskosql-0.0.1/flaskosql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-19 17:10:36.000000 flaskosql-0.0.1/flaskosql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 17:10:36.000000 flaskosql-0.0.1/flaskosql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 17:10:36.000000 flaskosql-0.0.1/flaskosql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 17:10:36.000000 flaskosql-0.0.1/flaskosql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 17:10:36.331962 flaskosql-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-05-19 17:10:28.000000 flaskosql-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:11:57.924580 flaskosql-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      799 2023-05-19 19:11:57.921677 flaskosql-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 19:11:57.915557 flaskosql-0.0.2/flaskosql.egg-info/
+-rw-rw-rw-   0        0        0      799 2023-05-19 19:11:57.000000 flaskosql-0.0.2/flaskosql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-05-19 19:11:57.000000 flaskosql-0.0.2/flaskosql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:11:57.000000 flaskosql-0.0.2/flaskosql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 19:11:57.000000 flaskosql-0.0.2/flaskosql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:11:57.000000 flaskosql-0.0.2/flaskosql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 19:11:57.925562 flaskosql-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-05-19 19:11:42.000000 flaskosql-0.0.2/setup.py
```

### Comparing `flaskosql-0.0.1/PKG-INFO` & `flaskosql-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 0.0.1
+Version: 0.0.2
 Summary: ORM for ORACLE DB for FLASK API
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# FLASKOS
+# FLASKOSQL
 <center><img src="./source/flaskos.png"></center><br><br>
 FLASKOS is a ORM for Oracle db for FLASK API, it provides a simple manupilation of database and simple mapiing to simplify interaction with relational database .
```

### Comparing `flaskosql-0.0.1/flaskosql.egg-info/PKG-INFO` & `flaskosql-0.0.2/flaskosql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 0.0.1
+Version: 0.0.2
 Summary: ORM for ORACLE DB for FLASK API
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# FLASKOS
+# FLASKOSQL
 <center><img src="./source/flaskos.png"></center><br><br>
 FLASKOS is a ORM for Oracle db for FLASK API, it provides a simple manupilation of database and simple mapiing to simplify interaction with relational database .
```

### Comparing `flaskosql-0.0.1/setup.py` & `flaskosql-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'ORM for ORACLE DB for FLASK API'
 LONG_DESCRIPTION = 'An ORM that allow us to connect with the ORACLE DB using OOP concept, plus the interaction with the database in order to create a rest API using FLASK framwork '
 
 # Setting up
 setup(
     name="flaskosql",
     version=VERSION,
```

