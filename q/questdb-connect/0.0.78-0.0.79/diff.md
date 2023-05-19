# Comparing `tmp/questdb-connect-0.0.78.tar.gz` & `tmp/questdb-connect-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.78.tar", last modified: Thu May 18 19:44:39 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.79.tar", last modified: Thu May 18 20:09:44 2023, max compression
```

## Comparing `questdb-connect-0.0.78.tar` & `questdb-connect-0.0.79.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.381457 questdb-connect-0.0.78/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.78/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 19:44:39.381321 questdb-connect-0.0.78/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.78/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 19:43:35.000000 questdb-connect-0.0.78/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 19:44:39.381496 questdb-connect-0.0.78/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.376042 questdb-connect-0.0.78/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.377991 questdb-connect-0.0.78/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.78/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.78/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.78/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.78/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.78/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.78/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.379637 questdb-connect-0.0.78/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.78/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11793 2023-05-18 19:29:38.000000 questdb-connect-0.0.78/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.78/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12639 2023-05-18 19:43:05.000000 questdb-connect-0.0.78/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)    10129 2023-05-18 19:43:05.000000 questdb-connect-0.0.78/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.380505 questdb-connect-0.0.78/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.381127 questdb-connect-0.0.78/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.78/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.78/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.78/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 20:09:44.330582 questdb-connect-0.0.79/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.79/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 20:09:44.330412 questdb-connect-0.0.79/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.79/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 20:09:10.000000 questdb-connect-0.0.79/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 20:09:44.330624 questdb-connect-0.0.79/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 20:09:44.323475 questdb-connect-0.0.79/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 20:09:44.326082 questdb-connect-0.0.79/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.79/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.79/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.79/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.79/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.79/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.79/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 20:09:44.327926 questdb-connect-0.0.79/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.79/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11793 2023-05-18 19:29:38.000000 questdb-connect-0.0.79/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.79/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12639 2023-05-18 19:43:05.000000 questdb-connect-0.0.79/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10016 2023-05-18 20:08:46.000000 questdb-connect-0.0.79/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 20:09:44.329178 questdb-connect-0.0.79/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 20:09:44.000000 questdb-connect-0.0.79/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 20:09:44.000000 questdb-connect-0.0.79/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 20:09:44.000000 questdb-connect-0.0.79/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 20:09:44.000000 questdb-connect-0.0.79/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 20:09:44.000000 questdb-connect-0.0.79/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 20:09:44.000000 questdb-connect-0.0.79/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 20:09:44.329919 questdb-connect-0.0.79/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.79/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.79/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.79/tests/test_types.py
```

### Comparing `questdb-connect-0.0.78/LICENSE` & `questdb-connect-0.0.79/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/PKG-INFO` & `questdb-connect-0.0.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.78
+Version: 0.0.79
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.78/README.md` & `questdb-connect-0.0.79/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/pyproject.toml` & `questdb-connect-0.0.79/pyproject.toml`

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
-version = '0.0.78'
+version = '0.0.79'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.78/src/examples/__init__.py` & `questdb-connect-0.0.79/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/examples/hello_world.py` & `questdb-connect-0.0.79/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.79/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/examples/server_utilisation.py` & `questdb-connect-0.0.79/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.79/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.79/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/questdb_connect/__init__.py` & `questdb-connect-0.0.79/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/questdb_connect/dialect.py` & `questdb-connect-0.0.79/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/questdb_connect/function_names.py` & `questdb-connect-0.0.79/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.79/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/src/questdb_connect/types.py` & `questdb-connect-0.0.79/src/questdb_connect/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,17 @@
     @classmethod
     def matches_type_name(cls, type_name):
         return cls if type_name == cls.__visit_name__ else None
 
     def column_spec(self, column_name):
         return f"{quote_identifier(column_name)} {self.__visit_name__}"
 
+    def _compiler_dispatch(cls, _visitor, **_kw) -> str:
+        return cls.__visit_name__
+
 
 class Boolean(QDBTypeMixin):
     __visit_name__ = 'BOOLEAN'
     impl = sqla.types.Boolean
     type_code = 1
 
 
@@ -248,52 +251,14 @@
         raise ArgumentError(f'unsupported type: {type_name}')
     return type_class
 
 
 class QDBTypeCompiler(GenericTypeCompiler):
     ensure_kwarg = None
 
-    def visit_GEOHASHINT(self, type_, **kw):
-        return GeohashInt.__visit_name__
-
-    def visit_GeohashInt(self, type_, **kw):
-        return GeohashInt.__visit_name__
-
-    def visit_GEOHASHLONG(self, type_, **kw):
-        return GeohashLong.__visit_name__
-
-    def visit_GeohashLong(self, type_, **kw):
-        return GeohashLong.__visit_name__
-
-    def visit_GEOHASHBYTE(self, type_, **kw):
-        return GeohashByte.__visit_name__
-
-    def visit_GeohashByte(self, type_, **kw):
-        return GeohashByte.__visit_name__
-
-    def visit_GEOHASHSHORT(self, type_, **kw):
-        return GeohashShort.__visit_name__
-
-    def visit_GeohashShort(self, type_, **kw):
-        return GeohashShort.__visit_name__
-
-    def visit_unsupported_compilation(self, element, err, **kw):
-        if isinstance(element, GeohashLong):
-            return GeohashLong.__visit_name__
-        if isinstance(element, GeohashInt):
-            return GeohashInt.__visit_name__
-        if isinstance(element, GeohashShort):
-            return GeohashShort.__visit_name__
-        if isinstance(element, GeohashByte):
-            return GeohashByte.__visit_name__
-        raise_(
-            UnsupportedCompilationError(self, element),
-            replace_context=err,
-        )
-
     def visit_BOOLEAN(self, type_, **kw):
         return Boolean.__visit_name__
 
     def visit_boolean(self, type_, **kw):
         return Boolean.__visit_name__
 
     def visit_BOOL(self, type_, **kw):
@@ -385,15 +350,47 @@
 
     def visit_symbol(self, type_, **kw):
         return Symbol.__visit_name__
 
     def _render_string_type(self, type_, name):
         return name
 
-    def visit_null(self, type_, **kw):
-        raise CompileError(f'cannot generate DDL for type: {type_}')
+    def visit_GEOHASHINT(self, type_, **kw):
+        return GeohashInt.__visit_name__
+
+    def visit_GeohashInt(self, type_, **kw):
+        return GeohashInt.__visit_name__
+
+    def visit_GEOHASHLONG(self, type_, **kw):
+        return GeohashLong.__visit_name__
+
+    def visit_GeohashLong(self, type_, **kw):
+        return GeohashLong.__visit_name__
+
+    def visit_GEOHASHBYTE(self, type_, **kw):
+        return GeohashByte.__visit_name__
 
-    def visit_type_decorator(self, type_, **kw):
-        return self.process(type_.type_engine(self.dialect), **kw)
+    def visit_GeohashByte(self, type_, **kw):
+        return GeohashByte.__visit_name__
+
+    def visit_GEOHASHSHORT(self, type_, **kw):
+        return GeohashShort.__visit_name__
 
-    def visit_user_defined(self, type_, **kw):
-        return type_.get_col_spec(**kw)
+    def visit_GeohashShort(self, type_, **kw):
+        return GeohashShort.__visit_name__
+
+    def visit_unsupported_compilation(self, element, err, **kw):
+        if isinstance(element, GeohashLong):
+            return GeohashLong.__visit_name__
+        if isinstance(element, GeohashInt):
+            return GeohashInt.__visit_name__
+        if isinstance(element, GeohashShort):
+            return GeohashShort.__visit_name__
+        if isinstance(element, GeohashByte):
+            return GeohashByte.__visit_name__
+        raise_(
+            UnsupportedCompilationError(self, element),
+            replace_context=err,
+        )
+
+    def visit_null(self, type_, **kw):
+        raise CompileError(f'cannot generate DDL for type: {type_}')
```

### Comparing `questdb-connect-0.0.78/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.79/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.78
+Version: 0.0.79
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.78/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.79/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/tests/test_dialect.py` & `questdb-connect-0.0.79/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/tests/test_superset.py` & `questdb-connect-0.0.79/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.78/tests/test_types.py` & `questdb-connect-0.0.79/tests/test_types.py`

 * *Files identical despite different names*

