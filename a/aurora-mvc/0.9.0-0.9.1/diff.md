# Comparing `tmp/aurora-mvc-0.9.0.tar.gz` & `tmp/aurora-mvc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora-mvc-0.9.0.tar", last modified: Sun Apr  2 13:42:56 2023, max compression
+gzip compressed data, was "aurora-mvc-0.9.1.tar", last modified: Fri May 19 16:52:02 2023, max compression
```

## Comparing `aurora-mvc-0.9.0.tar` & `aurora-mvc-0.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 13:42:56.654485 aurora-mvc-0.9.0/
--rw-rw-rw-   0        0        0     1067 2023-03-17 15:11:50.000000 aurora-mvc-0.9.0/LICENSE
--rw-rw-rw-   0        0        0       35 2022-01-03 08:02:19.000000 aurora-mvc-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4217 2023-04-02 13:42:56.654485 aurora-mvc-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2981 2023-03-28 10:40:36.000000 aurora-mvc-0.9.0/README.md
--rw-rw-rw-   0        0        0      174 2022-10-02 11:48:51.000000 aurora-mvc-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0     1222 2023-04-02 13:42:56.663478 aurora-mvc-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-02 13:42:56.415216 aurora-mvc-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-02 13:42:56.458190 aurora-mvc-0.9.0/src/aurora/
--rw-rw-rw-   0        0        0    12294 2022-11-09 08:26:56.000000 aurora-mvc-0.9.0/src/aurora/Aurora.py
--rw-rw-rw-   0        0        0   117091 2023-03-28 08:41:58.000000 aurora-mvc-0.9.0/src/aurora/CLI.py
--rw-rw-rw-   0        0        0     4786 2023-03-28 12:07:59.000000 aurora-mvc-0.9.0/src/aurora/Controller.py
--rw-rw-rw-   0        0        0      813 2022-07-07 06:08:51.000000 aurora-mvc-0.9.0/src/aurora/Forms.py
--rw-rw-rw-   0        0        0    26256 2023-03-29 19:33:24.000000 aurora-mvc-0.9.0/src/aurora/Model.py
--rw-rw-rw-   0        0        0   134167 2023-03-29 19:42:59.000000 aurora-mvc-0.9.0/src/aurora/SQL.py
--rw-rw-rw-   0        0        0     1605 2023-03-17 15:00:46.000000 aurora-mvc-0.9.0/src/aurora/Template.py
--rw-rw-rw-   0        0        0      328 2023-03-28 08:29:41.000000 aurora-mvc-0.9.0/src/aurora/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-02 13:42:56.614509 aurora-mvc-0.9.0/src/aurora/blueprints/
--rw-rw-rw-   0        0        0        0 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/__init__.py
--rw-rw-rw-   0        0        0      255 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/controller.zip
--rw-rw-rw-   0        0        0      393 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/controllers.zip
--rw-rw-rw-   0        0        0      240 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/form.zip
--rw-rw-rw-   0        0        0      374 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/forms.zip
--rw-rw-rw-   0        0        0   117070 2023-04-02 13:33:56.000000 aurora-mvc-0.9.0/src/aurora/blueprints/init.zip
--rw-rw-rw-   0        0        0      407 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/model.zip
--rw-rw-rw-   0        0        0      410 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/model_safe.zip
--rw-rw-rw-   0        0        0      286 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/statics.zip
--rw-rw-rw-   0        0        0      451 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/users_model.zip
--rw-rw-rw-   0        0        0      451 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/users_model_safe.zip
--rw-rw-rw-   0        0        0      227 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/view.zip
--rw-rw-rw-   0        0        0      584 2022-07-01 07:40:04.000000 aurora-mvc-0.9.0/src/aurora/blueprints/views.zip
--rw-rw-rw-   0        0        0     1809 2023-03-28 08:10:35.000000 aurora-mvc-0.9.0/src/aurora/connector.py
--rw-rw-rw-   0        0        0    39136 2023-03-29 23:47:00.000000 aurora-mvc-0.9.0/src/aurora/helpers.py
--rw-rw-rw-   0        0        0     2356 2023-03-28 08:31:17.000000 aurora-mvc-0.9.0/src/aurora/init.py
--rw-rw-rw-   0        0        0    12764 2023-03-29 20:43:53.000000 aurora-mvc-0.9.0/src/aurora/security.py
-drwxrwxrwx   0        0        0        0 2023-04-02 13:42:56.652485 aurora-mvc-0.9.0/src/aurora_mvc.egg-info/
--rw-rw-rw-   0        0        0     4217 2023-04-02 13:42:56.000000 aurora-mvc-0.9.0/src/aurora_mvc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2023-04-02 13:42:56.000000 aurora-mvc-0.9.0/src/aurora_mvc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 13:42:56.000000 aurora-mvc-0.9.0/src/aurora_mvc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-02 13:42:56.000000 aurora-mvc-0.9.0/src/aurora_mvc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 16:52:02.005756 aurora-mvc-0.9.1/
+-rw-rw-rw-   0        0        0     1067 2023-03-17 15:11:50.000000 aurora-mvc-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0       35 2022-01-03 08:02:19.000000 aurora-mvc-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4217 2023-05-19 16:52:02.005756 aurora-mvc-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2981 2023-05-19 16:42:37.000000 aurora-mvc-0.9.1/README.md
+-rw-rw-rw-   0        0        0      174 2022-10-02 11:48:51.000000 aurora-mvc-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1222 2023-05-19 16:52:02.015753 aurora-mvc-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 16:52:01.848142 aurora-mvc-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 16:52:01.882910 aurora-mvc-0.9.1/src/aurora/
+-rw-rw-rw-   0        0        0    12294 2022-11-09 08:26:56.000000 aurora-mvc-0.9.1/src/aurora/Aurora.py
+-rw-rw-rw-   0        0        0   118964 2023-05-19 16:40:42.000000 aurora-mvc-0.9.1/src/aurora/CLI.py
+-rw-rw-rw-   0        0        0     4786 2023-03-28 12:07:59.000000 aurora-mvc-0.9.1/src/aurora/Controller.py
+-rw-rw-rw-   0        0        0      813 2022-07-07 06:08:51.000000 aurora-mvc-0.9.1/src/aurora/Forms.py
+-rw-rw-rw-   0        0        0    26256 2023-03-29 19:33:24.000000 aurora-mvc-0.9.1/src/aurora/Model.py
+-rw-rw-rw-   0        0        0   134167 2023-03-29 19:42:59.000000 aurora-mvc-0.9.1/src/aurora/SQL.py
+-rw-rw-rw-   0        0        0     1605 2023-03-17 15:00:46.000000 aurora-mvc-0.9.1/src/aurora/Template.py
+-rw-rw-rw-   0        0        0      328 2023-05-19 16:41:51.000000 aurora-mvc-0.9.1/src/aurora/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:52:01.987828 aurora-mvc-0.9.1/src/aurora/blueprints/
+-rw-rw-rw-   0        0        0        0 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/__init__.py
+-rw-rw-rw-   0        0        0      255 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/controller.zip
+-rw-rw-rw-   0        0        0      393 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/controllers.zip
+-rw-rw-rw-   0        0        0      240 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/form.zip
+-rw-rw-rw-   0        0        0      374 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/forms.zip
+-rw-rw-rw-   0        0        0   117070 2023-04-02 13:33:56.000000 aurora-mvc-0.9.1/src/aurora/blueprints/init.zip
+-rw-rw-rw-   0        0        0      407 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/model.zip
+-rw-rw-rw-   0        0        0      410 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/model_safe.zip
+-rw-rw-rw-   0        0        0      286 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/statics.zip
+-rw-rw-rw-   0        0        0      451 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/users_model.zip
+-rw-rw-rw-   0        0        0      451 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/users_model_safe.zip
+-rw-rw-rw-   0        0        0      227 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/view.zip
+-rw-rw-rw-   0        0        0      584 2022-07-01 07:40:04.000000 aurora-mvc-0.9.1/src/aurora/blueprints/views.zip
+-rw-rw-rw-   0        0        0     1809 2023-03-28 08:10:35.000000 aurora-mvc-0.9.1/src/aurora/connector.py
+-rw-rw-rw-   0        0        0    39954 2023-05-19 16:40:38.000000 aurora-mvc-0.9.1/src/aurora/helpers.py
+-rw-rw-rw-   0        0        0     2356 2023-03-28 08:31:17.000000 aurora-mvc-0.9.1/src/aurora/init.py
+-rw-rw-rw-   0        0        0    12764 2023-03-29 20:43:53.000000 aurora-mvc-0.9.1/src/aurora/security.py
+drwxrwxrwx   0        0        0        0 2023-05-19 16:52:02.004359 aurora-mvc-0.9.1/src/aurora_mvc.egg-info/
+-rw-rw-rw-   0        0        0     4217 2023-05-19 16:52:01.000000 aurora-mvc-0.9.1/src/aurora_mvc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2023-05-19 16:52:01.000000 aurora-mvc-0.9.1/src/aurora_mvc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 16:52:01.000000 aurora-mvc-0.9.1/src/aurora_mvc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-19 16:52:01.000000 aurora-mvc-0.9.1/src/aurora_mvc.egg-info/top_level.txt
```

### Comparing `aurora-mvc-0.9.0/LICENSE` & `aurora-mvc-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/PKG-INFO` & `aurora-mvc-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-mvc
-Version: 0.9.0
+Version: 0.9.1
 Summary: Aurora is an MVC web framework for creating RESTFUL CRUD applications quickly and simply
 Home-page: https://github.com/heminsatya/aurora
 Author: Hemin Satya
 Author-email: heminsatya@gmail.com
 License: MIT
 Project-URL: source, https://github.com/heminsatya/aurora
 Project-URL: Documentation, https://github.com/heminsatya/aurora/tree/main/docs
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Aurora Framework (v0.9.0 beta)
+# Aurora Framework (v0.9.1 beta)
 
 Aurora is an MVC web framework for creating CRUD applications quickly and simply.
 
 It is based on REST architecture. In another word it is a RESTFUL web framework.
 
 Aurora is written in [Python](https://www.python.org/), and partially used [Flask](https://flask.palletsprojects.com/).
```

### Comparing `aurora-mvc-0.9.0/README.md` & `aurora-mvc-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Aurora Framework (v0.9.0 beta)
+# Aurora Framework (v0.9.1 beta)
 
 Aurora is an MVC web framework for creating CRUD applications quickly and simply.
 
 It is based on REST architecture. In another word it is a RESTFUL web framework.
 
 Aurora is written in [Python](https://www.python.org/), and partially used [Flask](https://flask.palletsprojects.com/).
```

### Comparing `aurora-mvc-0.9.0/setup.cfg` & `aurora-mvc-0.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7572 6f72 612d 6d76 630d 0a76   = aurora-mvc..v
-00000020: 6572 7369 6f6e 203d 2030 2e39 2e30 0d0a  ersion = 0.9.0..
+00000020: 6572 7369 6f6e 203d 2030 2e39 2e31 0d0a  ersion = 0.9.1..
 00000030: 6175 7468 6f72 203d 2048 656d 696e 2053  author = Hemin S
 00000040: 6174 7961 0d0a 6175 7468 6f72 5f65 6d61  atya..author_ema
 00000050: 696c 203d 2068 656d 696e 7361 7479 6140  il = heminsatya@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 7572 6f72 6120  iption = Aurora 
 00000080: 6973 2061 6e20 4d56 4320 7765 6220 6672  is an MVC web fr
 00000090: 616d 6577 6f72 6b20 666f 7220 6372 6561  amework for crea
```

### Comparing `aurora-mvc-0.9.0/src/aurora/Aurora.py` & `aurora-mvc-0.9.1/src/aurora/Aurora.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/CLI.py` & `aurora-mvc-0.9.1/src/aurora/CLI.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,26 +448,48 @@
 
                         # Exit the program
                         exit()
 
                 # Database is OK
                 else:
                     db_changed = False
+                    miss_module = False
                     
                     # Fetch migration models data
                     try:
                         m_version = db.read(table="_migrations", cols=['version'], where={"current":True}).first()['version']
+
+                        # Missing migration module
+                        if not file_exist(app_path + sep + f'_migrations{sep + m_version}.py'):
+                            miss_module = True
+
                         m_module = importlib.import_module(f'_migrations.{m_version}')
                         m_models = m_module._models
                         m_db_system =  m_module.DB_SYSTEM
+
+                    # Unknown database system
                     except:
                         m_db_system = 'Unknown'
 
+                    # Missing migration module
+                    if miss_module:
+                        alert = '''----------------------------------------------------------\n'''
+                        alert += '''ERROR!\n'''
+                        alert += '''The migration module is missed!\n'''
+                        alert += '''----------------------------------------------------------'''
+                        
+                        # Alert the user
+                        print(alert)
+                        time.sleep(0.1)
+
+                        # Exit the program
+                        exit()
+
                     # Unknown database system
-                    if not m_db_system in db_systems:
+                    elif not m_db_system in db_systems:
                         alert = '''----------------------------------------------------------\n'''
                         alert += '''WARNING!\n'''
                         alert += '''Unknown database system has been selected!\n'''
                         alert += f'''Supported database systems are: {', '.join(db_systems)}\n'''
                         alert += '''----------------------------------------------------------'''
                         
                         # Alert the user
@@ -516,35 +538,36 @@
         time.sleep(0.1)
 
         # Global placeholders
         tables   = []
         m_tables = []
         f_tables = []
 
-        # Find migration tables
-        for model in m_models:
-            m_tables.append(getattr(m_module, model)['table'])
+        # Not "init" pattern
+        if not pattern == "init":
+            # Find migration tables
+            for model in m_models:
+                m_tables.append(getattr(m_module, model)['table'])
 
-            for x in getattr(m_module, model)['foreign_key']:
-                if not getattr(m_module, model)['foreign_key'][x]['r_table'] in f_tables:
-                    f_tables.append(getattr(m_module, model)['foreign_key'][x]['r_table'])
+                for x in getattr(m_module, model)['foreign_key']:
+                    if not getattr(m_module, model)['foreign_key'][x]['r_table'] in f_tables:
+                        f_tables.append(getattr(m_module, model)['foreign_key'][x]['r_table'])
 
         # Loop models
         for model in models:
+            # Local placeholders
+            cols    = []
+            attrs   = {}
+            m_attrs = {}
+
             # Not "init" pattern & not database changed & not database corrupted
             if not pattern == "init" and not db_changed and not db_corrupted:
                 # Migration model attributes
                 if model in m_models:
                     m_attrs = getattr(m_module, model)
-                else:
-                    m_attrs = {}
-
-            # Local placeholders
-            cols = []
-            attrs = {}
 
             # Model class
             Model = importlib.import_module(f'models.{model}')
             Class = getattr(Model, model)
 
             # Model meta data
             table = Class().table
@@ -1634,25 +1657,39 @@
                 # Search for temporary tables
                 if db._exist_table(f"{table}__temp"):
                     table_repair = True
 
                     print(f'- Corrupted "{table}" table for "{model}" model detected!')
                     time.sleep(0.1)
 
-                    # For only the repair pattern
+                    # Repair pattern
                     if pattern == "repair":
                         print(f'Repairing "{table}" table in the database...')
                         time.sleep(0.1)
 
-                        db._delete_table(f"{table}__temp", True)
+                        # Main table exists
+                        if db._exist_table(f"{table}"):
+                            db._delete_table(f"{table}__temp", True)
+                            
+                        # Main table not exists
+                        else:
+                            db._update_table(f"{table}__temp", f"{table}")
+
+                # Search for temporary columns
+                for col in m_attrs['col_type']:
+                    if db._exist_column(table, f"{col}__temp"):
+                        print(f'- Corrupted "{col}" column of "{table}" table for "{model}" model detected!')
+                        time.sleep(0.1)
+
+                        # Repair pattern
+                        if pattern == "repair":
+                            print(f'Repairing "{col}" column of "{table}" table in the database...')
 
-                        # Search for temporary columns
-                        for col in m_attrs['col_type']:
-                            if db._exist_column(table, f"{col}__temp"):
-                                db._delete_column(table, f"{col}__temp", True)
+                            time.sleep(0.1)
+                            db._delete_column(table, f"{col}__temp", True)
 
                 # Find the current model repair attribute
                 c_model = importlib.import_module(f'models.{model}')
                 c_class = getattr(c_model, model)
                 repair = c_class().repair
 
                 # Produce repairing model attributes
@@ -1785,37 +1822,43 @@
 
                             # Repair the column
                             try:
                                 db._update_column(table, col, repair[col], m_datatype, m_constraints)
                             
                             # On error
                             except:
-                                # Rename table to a temporary table
-                                db._update_table(table, f"{table}__temp")
-
-                                # Create a new table with latest constraints (renamed)
-                                db._create_table(table, r_attrs['col_type'], r_attrs['primary_key'], r_attrs['unique'], 
-                                    r_attrs['not_null'], r_attrs['default'], r_attrs['check'], r_attrs['foreign_key'])
+                                try:
+                                    # Rename table to a temporary table
+                                    db._update_table(table, f"{table}__temp")
+
+                                    # Create a new table with latest constraints (renamed)
+                                    db._create_table(table, r_attrs['col_type'], r_attrs['primary_key'], r_attrs['unique'], 
+                                        r_attrs['not_null'], r_attrs['default'], r_attrs['check'], r_attrs['foreign_key'])
 
-                                # Insert the temp table data into the new table
-                                db.query(f"INSERT INTO {table}({r_cols}) SELECT {c_cols} FROM {table}__temp;")
-                                
-                                # Remove the temp table
-                                db._delete_table(f"{table}__temp", True)
+                                    # Insert the temp table data into the new table
+                                    db.query(f"INSERT INTO {table}({r_cols}) SELECT {c_cols} FROM {table}__temp;")
+                                    
+                                    # Remove the temp table
+                                    db._delete_table(f"{table}__temp", True)
+                                except NameError as e:
+                                    print(e)
+                                    exit()
                             
                             model_file = f'{app_path + sep}models{sep + model}.py'
 
+                            ##
                             # Update the model file
+                            ##
+                            # Update the columns
                             old_str = rf"^[ ]*{col}+[ ]*[=]+[ ]*Model+\.+"
                             new_str = f"    {repair[col]} = Model."
                             replace_file_string(model_file, old_str, new_str, True)
 
-                            old_line = rf"^[ ]*'{col}'+[ ]*[:]+[ ]*'{repair[col]}'+\,*"
-                            new_line = ""
-                            replace_file_line(model_file, old_line, new_line, True)
+                            # Update the map
+                            replace_file_lines(model_file, "{", "}", "")
 
             # Column repair detected
             if column_repair and pattern == "repair":
                 # Produce the migration content
                 content = CLI.migration_data(models, True)
 
                 # Prompt the user for migration comment
@@ -2952,16 +2995,18 @@
         # Confirmed
         if confirm.lower() == 'yes':
             # Begin the process
             try:
                 print('Reseting the database...')
                 time.sleep(0.1)
 
-                # Delete the migrations
+                # Fetch the migrations
                 migrations = db.read(table="_migrations").all()
+
+                # Delete the migrations
                 for migration in migrations:
                     # Delete the migration files
                     delete_file(f"""{app_path + sep}_migrations{sep + migration['version']}.py""")
 
                 # Drop the database
                 db._delete_database(database, True)
```

### Comparing `aurora-mvc-0.9.0/src/aurora/Controller.py` & `aurora-mvc-0.9.1/src/aurora/Controller.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/Forms.py` & `aurora-mvc-0.9.1/src/aurora/Forms.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/Model.py` & `aurora-mvc-0.9.1/src/aurora/Model.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/SQL.py` & `aurora-mvc-0.9.1/src/aurora/SQL.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/Template.py` & `aurora-mvc-0.9.1/src/aurora/Template.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/blueprints/init.zip` & `aurora-mvc-0.9.1/src/aurora/blueprints/init.zip`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/blueprints/views.zip` & `aurora-mvc-0.9.1/src/aurora/blueprints/views.zip`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/connector.py` & `aurora-mvc-0.9.1/src/aurora/connector.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/helpers.py` & `aurora-mvc-0.9.1/src/aurora/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1228,14 +1228,43 @@
                 # Write other lines
                 else:
                     f.write(line)
 
         # Resize the file to the current file stream position
         f.truncate()
 
+    # Close file
+    return f.close()
+
+
+##
+# @desc Replaces multiple lines in a file between two strings with new data
+#
+# @param {str}  starting_str -- The starting string
+# @param {str}  ending_str   -- The ending string
+# @param {str}  replace_to   -- The new data to replace
+#
+# @retun {bool} -- True (on success), False (on error)
+##
+def replace_file_lines(file_path:str, starting_str, ending_str, replace_to):
+    # Read the file
+    content = read_file(file_path)
+
+    # Write the file
+    with open(file_path, 'w') as f:
+        # Find lines
+        replace_from = content[content.find(starting_str)+len(starting_str):content.rfind(ending_str)]
+
+        # Replace lines
+        content = content.replace(replace_from, replace_to)
+
+        # Rewrite the file
+        f.writelines(content)
+
+    # Close the file
     return f.close()
 
 
 ######################
 # Directory Handling #
 ######################
 ##
```

### Comparing `aurora-mvc-0.9.0/src/aurora/init.py` & `aurora-mvc-0.9.1/src/aurora/init.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora/security.py` & `aurora-mvc-0.9.1/src/aurora/security.py`

 * *Files identical despite different names*

### Comparing `aurora-mvc-0.9.0/src/aurora_mvc.egg-info/PKG-INFO` & `aurora-mvc-0.9.1/src/aurora_mvc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-mvc
-Version: 0.9.0
+Version: 0.9.1
 Summary: Aurora is an MVC web framework for creating RESTFUL CRUD applications quickly and simply
 Home-page: https://github.com/heminsatya/aurora
 Author: Hemin Satya
 Author-email: heminsatya@gmail.com
 License: MIT
 Project-URL: source, https://github.com/heminsatya/aurora
 Project-URL: Documentation, https://github.com/heminsatya/aurora/tree/main/docs
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Aurora Framework (v0.9.0 beta)
+# Aurora Framework (v0.9.1 beta)
 
 Aurora is an MVC web framework for creating CRUD applications quickly and simply.
 
 It is based on REST architecture. In another word it is a RESTFUL web framework.
 
 Aurora is written in [Python](https://www.python.org/), and partially used [Flask](https://flask.palletsprojects.com/).
```

### Comparing `aurora-mvc-0.9.0/src/aurora_mvc.egg-info/SOURCES.txt` & `aurora-mvc-0.9.1/src/aurora_mvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

