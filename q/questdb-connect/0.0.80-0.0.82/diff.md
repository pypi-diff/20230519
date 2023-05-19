# Comparing `tmp/questdb-connect-0.0.80.tar.gz` & `tmp/questdb-connect-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.80.tar", last modified: Fri May 19 09:01:36 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.82.tar", last modified: Fri May 19 10:00:32 2023, max compression
```

## Comparing `questdb-connect-0.0.80.tar` & `questdb-connect-0.0.82.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 09:01:36.477178 questdb-connect-0.0.80/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.80/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-19 09:01:36.477048 questdb-connect-0.0.80/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.80/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-19 09:00:03.000000 questdb-connect-0.0.80/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-19 09:01:36.477214 questdb-connect-0.0.80/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 09:01:36.471936 questdb-connect-0.0.80/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 09:01:36.474095 questdb-connect-0.0.80/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.80/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.80/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.80/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.80/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.80/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.80/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 09:01:36.475249 questdb-connect-0.0.80/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.80/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11822 2023-05-19 08:48:54.000000 questdb-connect-0.0.80/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.80/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12461 2023-05-19 09:00:47.000000 questdb-connect-0.0.80/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5865 2023-05-19 08:53:49.000000 questdb-connect-0.0.80/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 09:01:36.476137 questdb-connect-0.0.80/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-19 09:01:36.000000 questdb-connect-0.0.80/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-19 09:01:36.000000 questdb-connect-0.0.80/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-19 09:01:36.000000 questdb-connect-0.0.80/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-19 09:01:36.000000 questdb-connect-0.0.80/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-19 09:01:36.000000 questdb-connect-0.0.80/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-19 09:01:36.000000 questdb-connect-0.0.80/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 09:01:36.476775 questdb-connect-0.0.80/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.80/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.80/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.80/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.545717 questdb-connect-0.0.82/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.82/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-19 10:00:32.545580 questdb-connect-0.0.82/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.82/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-19 10:00:05.000000 questdb-connect-0.0.82/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-19 10:00:32.545754 questdb-connect-0.0.82/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.540279 questdb-connect-0.0.82/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.542677 questdb-connect-0.0.82/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.82/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.82/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.82/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.82/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.82/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.82/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.543876 questdb-connect-0.0.82/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.82/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11778 2023-05-19 09:49:25.000000 questdb-connect-0.0.82/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.82/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13615 2023-05-19 09:49:31.000000 questdb-connect-0.0.82/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5865 2023-05-19 08:53:49.000000 questdb-connect-0.0.82/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.544719 questdb-connect-0.0.82/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.545313 questdb-connect-0.0.82/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.82/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.82/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.82/tests/test_types.py
```

### Comparing `questdb-connect-0.0.80/LICENSE` & `questdb-connect-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/PKG-INFO` & `questdb-connect-0.0.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.80
+Version: 0.0.82
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.80/README.md` & `questdb-connect-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/pyproject.toml` & `questdb-connect-0.0.82/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.80'
+version = '0.0.82'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.80/src/examples/__init__.py` & `questdb-connect-0.0.82/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/examples/hello_world.py` & `questdb-connect-0.0.82/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.82/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/examples/server_utilisation.py` & `questdb-connect-0.0.82/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.82/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.82/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/questdb_connect/__init__.py` & `questdb-connect-0.0.82/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/questdb_connect/dialect.py` & `questdb-connect-0.0.82/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,22 +281,22 @@
     def get_schema_names(self, connection, **kw):
         return ['public']
 
     def get_table_names(self, connection, schema=None, **kw):
         return [row.table for row in connection.execute(text('SHOW TABLES'))]
 
     def has_table(self, connection, table_name, schema=None):
-        query = f"tables() WHERE name='{table_name}'"
-        result = connection.execute(text(query))
-        return result.rowcount == 1
+        return connection.execute(text(f"tables() WHERE name='{table_name}'")).rowcount == 1
 
     @cache
     def get_columns(self, connection, table_name, schema=None, **kw):
-        result_set = connection.execute(text(f"table_columns('{table_name}')"))
-        return self.inspector.format_table_columns(table_name, result_set)
+        return self.inspector.format_table_columns(
+            table_name,
+            connection.execute(text(f"table_columns('{table_name}')"))
+        )
 
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
         return []
 
     def get_foreign_keys(self, connection, table_name, schema=None, postgresql_ignore_search_path=False, **kw):
         return []
```

### Comparing `questdb-connect-0.0.80/src/questdb_connect/function_names.py` & `questdb-connect-0.0.82/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.82/src/questdb_connect/superset_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,31 +94,32 @@
     }
     ret_list = []
     for duration, func in _time_grain_expressions.items():
         if duration:
             name = builtin_time_grains[duration]
             ret_list.append(TimeGrain(name, _(name), func, duration))
     _engine_time_grains = tuple(ret_list)
-    _column_type_to_generic_type_mapping = {
-        types.Boolean.__visit_name__: GenericDataType.BOOLEAN,
-        types.Byte.__visit_name__: GenericDataType.NUMERIC,
-        types.Short.__visit_name__: GenericDataType.NUMERIC,
-        types.Int.__visit_name__: GenericDataType.NUMERIC,
-        types.Long.__visit_name__: GenericDataType.NUMERIC,
-        types.Float.__visit_name__: GenericDataType.NUMERIC,
-        types.Double.__visit_name__: GenericDataType.NUMERIC,
-        types.Symbol.__visit_name__: GenericDataType.STRING,
-        types.String.__visit_name__: GenericDataType.STRING,
-        types.Char.__visit_name__: GenericDataType.STRING,
-        types.Long256.__visit_name__: GenericDataType.STRING,
-        types.UUID.__visit_name__: GenericDataType.STRING,
-        types.Timestamp.__visit_name__: GenericDataType.TEMPORAL,
-        types.Date.__visit_name__: GenericDataType.TEMPORAL,
-        # GEOHASH (GenericDataType.STRING) is treated separately
-    }
+    _default_column_type_mappings = (
+        (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
+        (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
+        (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
+        (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
+        (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
+        (re.compile("^LONG", re.IGNORECASE), types.Long, GenericDataType.NUMERIC),
+        (re.compile("^FLOAT", re.IGNORECASE), types.Float, GenericDataType.NUMERIC),
+        (re.compile("^DOUBLE'", re.IGNORECASE), types.Double, GenericDataType.NUMERIC),
+        (re.compile("^SYMBOL", re.IGNORECASE), types.Symbol, GenericDataType.STRING),
+        (re.compile("^STRING", re.IGNORECASE), types.String, GenericDataType.STRING),
+        (re.compile("^UUID", re.IGNORECASE), types.UUID, GenericDataType.STRING),
+        (re.compile("^CHAR", re.IGNORECASE), types.Char, GenericDataType.STRING),
+        (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp, GenericDataType.TEMPORAL),
+        (re.compile("^DATE", re.IGNORECASE), types.Date, GenericDataType.TEMPORAL),
+        (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), types.GeohashLong, GenericDataType.STRING)
+    )
+    column_type_mappings = _default_column_type_mappings
 
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
     ) -> str:
@@ -130,22 +131,14 @@
             parameters.get("database"))
 
     @classmethod
     def get_default_schema_for_query(cls, database, query) -> Optional[str]:
         return 'public'
 
     @classmethod
-    def get_allow_cost_estimate(cls, extra: Dict[str, Any]) -> bool:
-        return False
-
-    @classmethod
-    def get_view_names(cls, database, inspector, schema: Optional[str]):
-        return []
-
-    @classmethod
     def get_text_clause(cls, clause):
         """SQLAlchemy wrapper to ensure text clauses are escaped properly
         :param clause: string clause with potentially unescaped characters
         :return: text clause with escaped characters
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
@@ -207,16 +200,54 @@
         """Return a sqlalchemy native column type and generic data type that
         corresponds to the column type defined in the data source (return None
         to use default type inferred by SQLAlchemy). Override `column_type_mappings`
         for specific needs (see MSSQL for example of NCHAR/NVARCHAR handling).
         :param column_type: Column type returned by inspector
         :return: SQLAlchemy and generic Superset column types
         """
-        column_spec = cls.get_column_spec()
-        return column_spec.sqla_type, column_spec.generic_type
+        if not column_type:
+            return None
+        for regex, sqla_type, generic_type in cls._default_column_type_mappings:
+            matching_name = regex.search(column_type)
+            if matching_name:
+                return (
+                    types.resolve_type_from_name(sqla_type.__visit_name__).impl,
+                    generic_type
+                )
+        return None
+
+    @classmethod
+    def get_column_spec(
+            cls,
+            native_type: Optional[str],
+            db_extra: Optional[Dict[str, Any]] = None,
+            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
+    ) -> Optional[utils.ColumnSpec]:
+        """Get generic type related specs regarding a native column type.
+        :param native_type: Native database type
+        :param db_extra: The database extra object
+        :param source: Type coming from the database table or cursor description
+        :return: ColumnSpec object
+        """
+        if not native_type:
+            return None
+        sqla_type = types.resolve_type_from_name(native_type)
+        name_u = sqla_type.__visit_name__
+        generic_type = None
+        if name_u == 'BOOLEAN':
+            generic_type = GenericDataType.BOOLEAN
+        elif name_u in ('BYTE', 'SHORT', 'INT', 'LONG', 'FLOAT', 'DOUBLE'):
+            generic_type = GenericDataType.NUMERIC
+        elif name_u in ('SYMBOL', 'STRING', 'CHAR', 'LONG256', 'UUID'):
+            generic_type = GenericDataType.STRING
+        elif name_u in ('DATE', 'TIMESTAMP'):
+            generic_type = GenericDataType.TEMPORAL
+        elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
+            generic_type = GenericDataType.STRING
+        return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
 
     @classmethod
     def get_sqla_column_type(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
             source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
@@ -273,24 +304,13 @@
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
         :return: A list of function names usable in the database
         """
         return FUNCTION_NAMES
 
     @classmethod
-    def get_column_spec(
-            cls,
-            native_type: Optional[str],
-            db_extra: Optional[Dict[str, Any]] = None,
-            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
-    ) -> Optional[utils.ColumnSpec]:
-        """Get generic type related specs regarding a native column type.
-        :param native_type: Native database type
-        :param db_extra: The database extra object
-        :param source: Type coming from the database table or cursor description
-        :return: ColumnSpec object
-        """
-        sqla_type = types.resolve_type_from_name(native_type)
-        generic_type = cls._column_type_to_generic_type_mapping.get(native_type)
-        if not generic_type and 'GEOHASH' in native_type and '(' in native_type and ')' in native_type:
-            generic_type = GenericDataType.STRING
-        return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
+    def get_allow_cost_estimate(cls, extra: Dict[str, Any]) -> bool:
+        return False
+
+    @classmethod
+    def get_view_names(cls, database, inspector, schema: Optional[str]):
+        return []
```

### Comparing `questdb-connect-0.0.80/src/questdb_connect/types.py` & `questdb-connect-0.0.82/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.82/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.80
+Version: 0.0.82
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.80/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.82/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/tests/test_dialect.py` & `questdb-connect-0.0.82/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/tests/test_superset.py` & `questdb-connect-0.0.82/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.80/tests/test_types.py` & `questdb-connect-0.0.82/tests/test_types.py`

 * *Files identical despite different names*

