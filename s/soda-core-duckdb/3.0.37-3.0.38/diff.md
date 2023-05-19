# Comparing `tmp/soda-core-duckdb-3.0.37.tar.gz` & `tmp/soda-core-duckdb-3.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-duckdb-3.0.37.tar", last modified: Fri May 12 02:09:12 2023, max compression
+gzip compressed data, was "soda-core-duckdb-3.0.38.tar", last modified: Fri May 19 03:35:02 2023, max compression
```

## Comparing `soda-core-duckdb-3.0.37.tar` & `soda-core-duckdb-3.0.38.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 02:09:12.759980 soda-core-duckdb-3.0.37/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-12 02:09:12.759980 soda-core-duckdb-3.0.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 02:09:12.759980 soda-core-duckdb-3.0.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-12 02:07:04.000000 soda-core-duckdb-3.0.37/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 02:09:12.759980 soda-core-duckdb-3.0.37/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 02:09:12.759980 soda-core-duckdb-3.0.37/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-05-12 02:07:04.000000 soda-core-duckdb-3.0.37/soda/data_sources/duckdb_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 02:09:12.759980 soda-core-duckdb-3.0.37/soda_core_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-12 02:09:12.000000 soda-core-duckdb-3.0.37/soda_core_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-12 02:09:12.000000 soda-core-duckdb-3.0.37/soda_core_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 02:09:12.000000 soda-core-duckdb-3.0.37/soda_core_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-12 02:09:12.000000 soda-core-duckdb-3.0.37/soda_core_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-12 02:09:12.000000 soda-core-duckdb-3.0.37/soda_core_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 02:09:12.759980 soda-core-duckdb-3.0.37/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-05-12 02:07:04.000000 soda-core-duckdb-3.0.37/tests/test_duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:02.937940 soda-core-duckdb-3.0.38/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-19 03:35:02.937940 soda-core-duckdb-3.0.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-19 03:35:02.937940 soda-core-duckdb-3.0.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-19 03:34:25.000000 soda-core-duckdb-3.0.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:02.937940 soda-core-duckdb-3.0.38/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:02.937940 soda-core-duckdb-3.0.38/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5504 2023-05-19 03:34:25.000000 soda-core-duckdb-3.0.38/soda/data_sources/duckdb_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:02.937940 soda-core-duckdb-3.0.38/soda_core_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-19 03:35:02.000000 soda-core-duckdb-3.0.38/soda_core_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-19 03:35:02.000000 soda-core-duckdb-3.0.38/soda_core_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 03:35:02.000000 soda-core-duckdb-3.0.38/soda_core_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-19 03:35:02.000000 soda-core-duckdb-3.0.38/soda_core_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-19 03:35:02.000000 soda-core-duckdb-3.0.38/soda_core_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 03:35:02.937940 soda-core-duckdb-3.0.38/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-05-19 03:34:25.000000 soda-core-duckdb-3.0.38/tests/test_duckdb.py
```

### Comparing `soda-core-duckdb-3.0.37/setup.py` & `soda-core-duckdb-3.0.38/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-duckdb"
-package_version = "3.0.37"
+package_version = "3.0.38"
 description = "Soda Core Duckdb Package"
 
-requires = [f"soda-core=={package_version}", "duckdb==0.6.1"]
+requires = [f"soda-core=={package_version}", "duckdb<=0.8"]
 
 setup(
     name=package_name,
     version=package_version,
     install_requires=requires,
     packages=find_namespace_packages(include=["soda*"]),
 )
```

### Comparing `soda-core-duckdb-3.0.37/soda/data_sources/duckdb_data_source.py` & `soda-core-duckdb-3.0.38/soda/data_sources/duckdb_data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     TEXT_TYPES_FOR_PROFILING = ["char", "varchar"]
 
     def __init__(self, logs: Logs, data_source_name: str, data_source_properties: dict):
         super().__init__(logs, data_source_name, data_source_properties)
         self.path = data_source_properties.get("path")
         self.read_only = data_source_properties.get("read_only", False)
         self.duckdb_connection = data_source_properties.get("duckdb_connection")
-        self.configuration = data_source_properties.get("configuration")
+        self.configuration = data_source_properties.get("configuration", dict())
 
     def connect(self):
         import duckdb
 
         try:
             if self.duckdb_connection:
                 self.connection = DuckDBDataSourceConnectionWrapper(self.duckdb_connection)
```

### Comparing `soda-core-duckdb-3.0.37/tests/test_duckdb.py` & `soda-core-duckdb-3.0.38/tests/test_duckdb.py`

 * *Files identical despite different names*

