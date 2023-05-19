# Comparing `tmp/pyliteadmin-0.0.8.tar.gz` & `tmp/pyliteadmin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyliteadmin-0.0.8.tar", last modified: Thu May 11 18:30:40 2023, max compression
+gzip compressed data, was "pyliteadmin-0.0.9.tar", last modified: Fri May 19 16:37:39 2023, max compression
```

## Comparing `pyliteadmin-0.0.8.tar` & `pyliteadmin-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:30:40.165773 pyliteadmin-0.0.8/
--rw-rw-rw-   0        0        0    11545 2023-05-04 19:06:23.000000 pyliteadmin-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2199 2023-05-11 18:30:40.164774 pyliteadmin-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1648 2023-05-04 19:06:17.000000 pyliteadmin-0.0.8/README.md
--rw-rw-rw-   0        0        0      752 2023-05-11 18:30:13.000000 pyliteadmin-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 18:30:40.165773 pyliteadmin-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 18:30:40.131509 pyliteadmin-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 18:30:40.144016 pyliteadmin-0.0.8/src/pyliteadmin/
--rw-rw-rw-   0        0        0        0 2023-05-11 18:27:32.000000 pyliteadmin-0.0.8/src/pyliteadmin/__init__.py
--rw-rw-rw-   0        0        0     3937 2023-05-11 18:27:32.000000 pyliteadmin-0.0.8/src/pyliteadmin/db.py
--rw-rw-rw-   0        0        0    16760 2023-05-11 18:30:22.000000 pyliteadmin-0.0.8/src/pyliteadmin/pyliteadmin.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:30:40.163772 pyliteadmin-0.0.8/src/pyliteadmin.egg-info/
--rw-rw-rw-   0        0        0     2199 2023-05-11 18:30:40.000000 pyliteadmin-0.0.8/src/pyliteadmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-05-11 18:30:40.000000 pyliteadmin-0.0.8/src/pyliteadmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:30:40.000000 pyliteadmin-0.0.8/src/pyliteadmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-11 18:30:40.000000 pyliteadmin-0.0.8/src/pyliteadmin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 18:30:40.000000 pyliteadmin-0.0.8/src/pyliteadmin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-11 18:30:40.000000 pyliteadmin-0.0.8/src/pyliteadmin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 16:37:39.432708 pyliteadmin-0.0.9/
+-rw-rw-rw-   0        0        0    11545 2023-05-04 19:06:23.000000 pyliteadmin-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2199 2023-05-19 16:37:39.431709 pyliteadmin-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1648 2023-05-04 19:06:17.000000 pyliteadmin-0.0.9/README.md
+-rw-rw-rw-   0        0        0      752 2023-05-19 16:37:18.000000 pyliteadmin-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 16:37:39.432708 pyliteadmin-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 16:37:39.396664 pyliteadmin-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 16:37:39.411186 pyliteadmin-0.0.9/src/pyliteadmin/
+-rw-rw-rw-   0        0        0        0 2023-05-11 18:27:32.000000 pyliteadmin-0.0.9/src/pyliteadmin/__init__.py
+-rw-rw-rw-   0        0        0     3953 2023-05-19 16:37:22.000000 pyliteadmin-0.0.9/src/pyliteadmin/db.py
+-rw-rw-rw-   0        0        0    16760 2023-05-11 18:30:22.000000 pyliteadmin-0.0.9/src/pyliteadmin/pyliteadmin.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:37:39.429709 pyliteadmin-0.0.9/src/pyliteadmin.egg-info/
+-rw-rw-rw-   0        0        0     2199 2023-05-19 16:37:39.000000 pyliteadmin-0.0.9/src/pyliteadmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-05-19 16:37:39.000000 pyliteadmin-0.0.9/src/pyliteadmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:37:39.000000 pyliteadmin-0.0.9/src/pyliteadmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-19 16:37:39.000000 pyliteadmin-0.0.9/src/pyliteadmin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 16:37:39.000000 pyliteadmin-0.0.9/src/pyliteadmin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 16:37:39.000000 pyliteadmin-0.0.9/src/pyliteadmin.egg-info/top_level.txt
```

### Comparing `pyliteadmin-0.0.8/LICENSE` & `pyliteadmin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.8/PKG-INFO` & `pyliteadmin-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyliteadmin
-Version: 0.0.8
+Version: 0.0.9
 Summary: A TUI for viewing and CRUDing sqlite databases.
 Author-email: Brandon Demelo <brandon@brandondemelo.com>
 Project-URL: Homepage, https://github.com/The-Bush/pyliteadmin
 Project-URL: Bug Tracker, https://github.com/The-Bush/pyliteadmin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyliteadmin-0.0.8/README.md` & `pyliteadmin-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.8/pyproject.toml` & `pyliteadmin-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyliteadmin"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Brandon Demelo", email="brandon@brandondemelo.com" },
 ]
 description = "A TUI for viewing and CRUDing sqlite databases."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyliteadmin-0.0.8/src/pyliteadmin/db.py` & `pyliteadmin-0.0.9/src/pyliteadmin/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import sqlite3
 
-# Import the path to the database
-from pyliteadmin import db_path
+
 
 def get_columns(table:str) -> list:
     """ Returns a list of column names and types for a given table """
     conn = sqlite3.connect(db_path)
     cursor = conn.cursor()
     cursor.execute(f"SELECT * FROM {table}")
     columns = [description[0] for description in cursor.description]
     conn.close()
     return columns
 
 def get_table(table:str) -> tuple[list[tuple], list[str]]:
     """ Returns a list of rows as tuples and a list of column names for a given table """
+    # Import the path to the database
+    from pyliteadmin import db_path
+    
     conn = sqlite3.connect(db_path)
     cursor = conn.cursor()
     cursor.execute(f"SELECT * FROM {table}")
 
     # Get all items in this table
     rows = cursor.fetchall()
```

### Comparing `pyliteadmin-0.0.8/src/pyliteadmin/pyliteadmin.py` & `pyliteadmin-0.0.9/src/pyliteadmin/pyliteadmin.py`

 * *Files identical despite different names*

### Comparing `pyliteadmin-0.0.8/src/pyliteadmin.egg-info/PKG-INFO` & `pyliteadmin-0.0.9/src/pyliteadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyliteadmin
-Version: 0.0.8
+Version: 0.0.9
 Summary: A TUI for viewing and CRUDing sqlite databases.
 Author-email: Brandon Demelo <brandon@brandondemelo.com>
 Project-URL: Homepage, https://github.com/The-Bush/pyliteadmin
 Project-URL: Bug Tracker, https://github.com/The-Bush/pyliteadmin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

