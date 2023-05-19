# Comparing `tmp/duckdb_engine-0.7.2.tar.gz` & `tmp/duckdb_engine-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdb_engine-0.7.2.tar", max compression
+gzip compressed data, was "duckdb_engine-0.7.3.tar", max compression
```

## Comparing `duckdb_engine-0.7.2.tar` & `duckdb_engine-0.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0     5953 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/README.md
--rw-r--r--   0        0        0        4 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
--rw-r--r--   0        0        0        1 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
--rw-r--r--   0        0        0    20688 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
--rw-r--r--   0        0        0    11629 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/__init__.py
--rw-r--r--   0        0        0      985 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/config.py
--rw-r--r--   0        0        0        0 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/conftest.py
--rw-r--r--   0        0        0     2291 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/datatypes.py
--rw-r--r--   0        0        0        0 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/py.typed
--rw-r--r--   0        0        0        0 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/snapshots/__init__.py
--rw-r--r--   0        0        0      338 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/snapshots/snap_test_basic.py
--rw-r--r--   0        0        0    10426 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_basic.py
--rw-r--r--   0        0        0     3015 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_datatypes.py
--rw-r--r--   0        0        0      948 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_ibis.py
--rw-r--r--   0        0        0      455 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_integration.py
--rw-r--r--   0        0        0     3946 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/test_pandas.py
--rw-r--r--   0        0        0      257 2023-05-17 10:30:48.303976 duckdb_engine-0.7.2/duckdb_engine/tests/util.py
--rw-r--r--   0        0        0     1370 2023-05-17 10:30:48.307976 duckdb_engine-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/LICENSE.txt
+-rw-r--r--   0        0        0     5953 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/README.md
+-rw-r--r--   0        0        0        4 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
+-rw-r--r--   0        0        0        1 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
+-rw-r--r--   0        0        0    20688 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
+-rw-r--r--   0        0        0    11629 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/config.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/conftest.py
+-rw-r--r--   0        0        0     2198 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/datatypes.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/py.typed
+-rw-r--r--   0        0        0        0 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/snapshots/snap_test_basic.py
+-rw-r--r--   0        0        0    10426 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_basic.py
+-rw-r--r--   0        0        0     3185 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_datatypes.py
+-rw-r--r--   0        0        0      948 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_ibis.py
+-rw-r--r--   0        0        0      455 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_integration.py
+-rw-r--r--   0        0        0     3946 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_pandas.py
+-rw-r--r--   0        0        0      257 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/util.py
+-rw-r--r--   0        0        0     1370 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.7.3/PKG-INFO
```

### Comparing `duckdb_engine-0.7.2/LICENSE.txt` & `duckdb_engine-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.2/README.md` & `duckdb_engine-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.2/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz` & `duckdb_engine-0.7.3/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.2/duckdb_engine/__init__.py` & `duckdb_engine-0.7.3/duckdb_engine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.engine.url import URL
 
 from .config import apply_config, get_core_config
 from .datatypes import ISCHEMA_NAMES, register_extension_types
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 if TYPE_CHECKING:
     from sqlalchemy.base import Connection
     from sqlalchemy.engine.interfaces import _IndexDict
 
 
 register_extension_types()
```

### Comparing `duckdb_engine-0.7.2/duckdb_engine/config.py` & `duckdb_engine-0.7.3/duckdb_engine/config.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.2/duckdb_engine/datatypes.py` & `duckdb_engine-0.7.3/duckdb_engine/datatypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,16 +100,13 @@
     "usmallint": USmallInteger,
     "uinteger": UInt8,
     "ubigint": UBigInteger,
     "timestamp_s": sqltypes.TIMESTAMP,
     "timestamp_ms": sqltypes.TIMESTAMP,
     "timestamp_ns": sqltypes.TIMESTAMP,
     "enum": sqltypes.Enum,
-    "list": lambda: sqltypes.ARRAY(sqltypes.NULLTYPE),
-    "struct": Struct,
-    "map": Map,
 }
 
 
 def register_extension_types() -> None:
     for subclass in types:
         compiles(subclass, "duckdb")(compile_uint)
```

### Comparing `duckdb_engine-0.7.2/duckdb_engine/tests/conftest.py` & `duckdb_engine-0.7.3/duckdb_engine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.2/duckdb_engine/tests/test_basic.py` & `duckdb_engine-0.7.3/duckdb_engine/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.2/duckdb_engine/tests/test_datatypes.py` & `duckdb_engine-0.7.3/duckdb_engine/tests/test_datatypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,11 +102,15 @@
     importorskip("sqlalchemy", "1.4.0")
     importorskip("duckdb", "0.5.1")
 
     with warnings.catch_warnings() as capture, engine.connect() as conn:
         conn.execute(text("create table t2 as select * from test_all_types()"))
         table = Table("t2", MetaData(), autoload_with=conn)
         for col in table.columns:
-            if col.name.endswith("_enum") and duckdb.__version__ < "0.7.1":  # type: ignore[attr-defined]
+            name = col.name
+            if name.endswith("_enum") and duckdb.__version__ < "0.7.1":  # type: ignore[attr-defined]
                 continue
-            assert col.type != sqltypes.NULLTYPE, col.name
+            if "array" in name or "struct" in name or "map" in name:
+                assert col.type == sqltypes.NULLTYPE, name
+            else:
+                assert col.type != sqltypes.NULLTYPE, name
         assert not capture
```

### Comparing `duckdb_engine-0.7.2/duckdb_engine/tests/test_ibis.py` & `duckdb_engine-0.7.3/duckdb_engine/tests/test_ibis.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.2/duckdb_engine/tests/test_pandas.py` & `duckdb_engine-0.7.3/duckdb_engine/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.2/pyproject.toml` & `duckdb_engine-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duckdb_engine"
-version = "0.7.2"
+version = "0.7.3"
 description = "SQLAlchemy driver for duckdb"
 authors = ["Elliana <me@mause.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Mause/duckdb_engine"
 
 [tool.poetry.urls]
```

### Comparing `duckdb_engine-0.7.2/PKG-INFO` & `duckdb_engine-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckdb-engine
-Version: 0.7.2
+Version: 0.7.3
 Summary: SQLAlchemy driver for duckdb
 Home-page: https://github.com/Mause/duckdb_engine
 License: MIT
 Author: Elliana
 Author-email: me@mause.me
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

