# Comparing `tmp/macrometa-source-oracle-0.0.34.tar.gz` & `tmp/macrometa-source-oracle-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-oracle-0.0.34.tar", max compression
+gzip compressed data, was "macrometa-source-oracle-0.0.35.tar", max compression
```

## Comparing `macrometa-source-oracle-0.0.34.tar` & `macrometa-source-oracle-0.0.35.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     9713 2023-05-17 08:51:36.243133 macrometa-source-oracle-0.0.34/LICENSE
--rw-r--r--   0        0        0     1715 2023-05-17 08:51:36.243133 macrometa-source-oracle-0.0.34/README.md
--rw-r--r--   0        0        0    42538 2023-05-17 08:51:36.243133 macrometa-source-oracle-0.0.34/macrometa_source_oracle/__init__.py
--rwxr-xr-x   0        0        0     7417 2023-05-17 08:51:36.243133 macrometa-source-oracle-0.0.34/macrometa_source_oracle/connection.py
--rwxr-xr-x   0        0        0        0 2023-05-17 08:51:36.243133 macrometa-source-oracle-0.0.34/macrometa_source_oracle/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     4779 2023-05-17 08:51:36.243133 macrometa-source-oracle-0.0.34/macrometa_source_oracle/sync_strategies/common.py
--rwxr-xr-x   0        0        0     4874 2023-05-17 08:51:36.243133 macrometa-source-oracle-0.0.34/macrometa_source_oracle/sync_strategies/full_table.py
--rwxr-xr-x   0        0        0    17662 2023-05-17 08:51:36.243133 macrometa-source-oracle-0.0.34/macrometa_source_oracle/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1563 2023-05-17 08:51:36.339135 macrometa-source-oracle-0.0.34/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.34/setup.py
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.34/PKG-INFO
+-rwxr-xr-x   0        0        0     9713 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/LICENSE
+-rw-r--r--   0        0        0     1707 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/README.md
+-rw-r--r--   0        0        0    42821 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/__init__.py
+-rwxr-xr-x   0        0        0     7417 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/connection.py
+-rwxr-xr-x   0        0        0        0 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     4779 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     4874 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/full_table.py
+-rwxr-xr-x   0        0        0    17662 2023-05-19 09:50:52.544616 macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1563 2023-05-19 09:50:52.640616 macrometa-source-oracle-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     2739 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.35/setup.py
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.35/PKG-INFO
```

### Comparing `macrometa-source-oracle-0.0.34/LICENSE` & `macrometa-source-oracle-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.34/README.md` & `macrometa-source-oracle-0.0.35/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
   "host": "dev.oracledb.io",
   "port": 1521,
   "user": "C##HELLO",
   "password": "password",
   "service_name": "ORCLCDB",
   "filter_schema": "C##HELLO",
   "filter_table": "CUSTOMERS",
-  "default_replication_method": "LOG_BASED",
+  "replication_method": "LOG_BASED",
   "pdb_name": "ORCLPDB1",
   "multitenant": true,
   "scn_window_size": 10
 }
 ```
 
 You can run a discover run using the previous `config.json` file to acquire all the tables definition
```

### Comparing `macrometa-source-oracle-0.0.34/macrometa_source_oracle/__init__.py` & `macrometa-source-oracle-0.0.35/macrometa_source_oracle/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,23 +180,23 @@
                            placeholder_value='1521'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='Oracle DB username.',
                            placeholder_value='system'),
             ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='Oracle DB user password.',
                            placeholder_value='password'),
-            ConfigProperty('default_replication_method', 'Default Replication Method',
+            ConfigProperty('replication_method', 'Replication Method',
                            ConfigAttributeType.STRING, True, False,
                            description='Choose from LOG_BASED, FULL_TABLE.',
                            default_value='FULL_TABLE'),
             ConfigProperty('filter_schema', 'Source Schema', ConfigAttributeType.STRING, True, False,
                            description='Source Schema to scan.',
                            placeholder_value='C##CUSTOMERS'),
             ConfigProperty('filter_table', 'Source Table', ConfigAttributeType.STRING, True, True,
-                           description='Source Table to scan.',
+                           description='Source Table to scan (Case-sensitive).',
                            placeholder_value='my_table'),
             ConfigProperty('service_name', 'Service Name', ConfigAttributeType.STRING, True, False,
                            description='Oracle DB service name.',
                            placeholder_value='ORCLCDB'),
             ConfigProperty('multitenant', 'Multi-Tenant', ConfigAttributeType.BOOLEAN, False, False,
                            description='Is Oracle DB is multi tenant or not.',
                            default_value='false'),
@@ -245,14 +245,15 @@
                 'host': integration['host'],
                 'user': integration['user'],
                 'password': integration['password'],
                 'port': integration['port'],
                 'service_name': integration['service_name'],
                 'multitenant': integration.get('multitenant', False),
                 'filter_table': integration['filter_table'],
+                'replication_method': integration.get('replication_method', "FULL_TABLE"),
                 # Optional
                 'pdb_name': integration.get('pdb_name', 'CDB$ROOT'),
                 'scn_window_size': integration.get('scn_window_size', log_based.SCN_WINDOW_SIZE),
                 'polling_interval': integration.get('polling_interval', log_based.POLLING_INTERVAL),
                 'ewallet_pem': integration.get('ewallet_pem'),
                 'wallet_password': integration.get('wallet_password'),
             }
@@ -615,14 +616,17 @@
     :return: Catalog containing discovered columns for the given filter criteria.
     :rtype: Catalog
     """
     LOGGER.info("Begin discovering..")
     connection = orc_db.open_connection(conn_config)
     cur = connection.cursor()
 
+    if conn_config['replication_method'] not in ["FULL_TABLE", "LOG_BASED"]:
+        raise Exception('Invalid replication method provided. It should be either FULL_TABLE or LOG_BASED.')
+
     if conn_config['multitenant']:
         LOGGER.info("The database is a multitenant system.")
         # Change session to the anticipated pluggable database (PDB).
         cur.execute(f"ALTER SESSION SET CONTAINER = {conn_config['pdb_name']}")
 
     row_counts = produce_row_counts(cur, filter_schemas, filter_table)
     table_info = {}
@@ -710,29 +714,29 @@
     if last_replication_method is not None and (replication_method != last_replication_method):
         state = singer.reset_stream(state, tap_stream_id)
 
     state = singer.write_bookmark(state, tap_stream_id, 'last_replication_method', replication_method)
     return state
 
 
-def classify_streams(streams, state, default_replication_method):
+def classify_streams(streams, state, replication_method):
     """
     Classifies streams into traditional and logical streams based on their replication method.
 
     :param streams: List of streams
     :param state: State object
-    :param default_replication_method: Default replication method for streams
+    :param replication_method: Default replication method for streams
     :return: Tuple of a dictionary containing the lookup of stream replication method,
              a list of traditional_streams, and a list of logical_streams
     """
     lookup, traditional_streams, logical_streams = {}, [], []
 
     for stream in streams:
         stream_metadata = metadata.to_map(stream.metadata)
-        replication_method = stream_metadata.get((), {}).get('replication-method', default_replication_method)
+        replication_method = stream_metadata.get((), {}).get('replication-method', replication_method)
 
         state = clear_state_on_replication_change(state, stream.tap_stream_id, replication_method)
         md_map, desired_columns = get_metadata_and_desired_columns(stream)
 
         if not is_valid_replication_method(replication_method) or not desired_columns:
             continue
 
@@ -887,42 +891,42 @@
     for stream in traditional_streams:
         sync_method = sync_method_lookup[stream.tap_stream_id]
         state = sync_traditional_stream(conn_config, stream, state, sync_method, end_scn)
 
     return state
 
 
-def do_sync(conn_config, catalog, default_replication_method, state):
+def do_sync(conn_config, catalog, replication_method, state):
     """
     Main synchronization function.
 
     :param conn_config: Connection configuration
     :param catalog: Catalog object
-    :param default_replication_method: Default replication method for streams
+    :param replication_method: Default replication method for streams
     :param state: State object
     :return: Updated state
     """
     currently_syncing = singer.get_currently_syncing(state)
     streams = sorted(filter(is_selected_via_metadata, catalog.streams), key=lambda s: s.tap_stream_id)
     LOGGER.info("Streams which were sleected: %s ", [s.tap_stream_id for s in streams])
 
-    end_scn = log_based.get_current_scn(conn_config) if any_logical_streams(streams, default_replication_method) else None
+    end_scn = log_based.get_current_scn(conn_config) if any_logical_streams(streams, replication_method) else None
     LOGGER.info("End SCN: %s ", end_scn)
 
-    sync_method_lookup, traditional_streams, logical_streams = classify_streams(streams, state, default_replication_method)
+    sync_method_lookup, traditional_streams, logical_streams = classify_streams(streams, state, replication_method)
 
     if currently_syncing:
         LOGGER.info("Stream found to be currently syncing: %s", currently_syncing)
         traditional_streams = reorder_traditional_streams(traditional_streams, currently_syncing)
     else:
         LOGGER.info("No stream found to be currently syncing")
 
     state = sync_traditional_streams(conn_config, traditional_streams, state, sync_method_lookup, end_scn)
 
-    _, _, logical_streams = classify_streams(streams, state, default_replication_method)
+    _, _, logical_streams = classify_streams(streams, state, replication_method)
     LOGGER.info(f"Logical (LogBased) streams after: {logical_streams}")
 
     state = sync_log_based_streams(conn_config, list(logical_streams), state, end_scn)
     return state
 
 
 def reorder_traditional_streams(traditional_streams, currently_syncing):
@@ -966,42 +970,43 @@
     if log_based_streams:
         log_based_streams = list(map(log_based.add_schema_properties, log_based_streams))
         state = log_based.sync_tables(conn_config, log_based_streams, state, end_scn)
 
     return state
 
 
-def any_logical_streams(streams, default_replication_method):
+def any_logical_streams(streams, replication_method):
     """
     Determine if there are any logical streams in the provided list of streams.
 
     :param streams: List of streams to check for logical streams.
     :type streams: list
-    :param default_replication_method: The default replication method to use when stream metadata does not specify one.
-    :type default_replication_method: str
+    :param replication_method: The default replication method to use when stream metadata does not specify one.
+    :type replication_method: str
     :return: True if any logical streams are found, False otherwise.
     :rtype: bool
     """
     for stream in streams:
         stream_metadata = metadata.to_map(stream.metadata)
-        replication_method = stream_metadata.get((), {}).get('replication-method', default_replication_method)
+        replication_method = stream_metadata.get((), {}).get('replication-method', replication_method)
         if replication_method == 'LOG_BASED':
             return True
 
     return False
 
 
 def main_impl():
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     conn_config = {'user': args.config['user'],
                    'password': args.config['password'],
                    'host': args.config['host'],
                    'port': args.config['port'],
                    'service_name': args.config['service_name'],
                    'multitenant': args.config.get('multitenant', False),
+                   'replication_method': args.config.get('replication_method', "FULL_TABLE"),
                    # If PDB name is not specified then we will use CDB$ROOT as the default container 
                    'pdb_name': args.config.get('pdb_name', 'CDB$ROOT'), 
                    'ewallet_pem': args.config.get('ewallet_pem'),
                    'wallet_password': args.config.get('wallet_password'), }
 
     log_based.SCN_WINDOW_SIZE = int(args.config.get('scn_window_size', log_based.SCN_WINDOW_SIZE))
     log_based.POLLING_INTERVAL = int(args.config.get('polling_interval', log_based.POLLING_INTERVAL))
@@ -1010,15 +1015,15 @@
         if args.discover:
             filter_schemas = [args.config.get('filter_schema')]
             filter_table = args.config.get('filter_table')
             do_discovery(conn_config, filter_schemas, filter_table)
 
         elif args.catalog:
             state = args.state
-            do_sync(conn_config, args.catalog, args.config.get('default_replication_method'), state)
+            do_sync(conn_config, args.catalog, args.config.get('replication_method', "FULL_TABLE"), state)
         else:
             LOGGER.info("No properties were selected")
     except Exception as e:
         LOGGER.info('Exception raised: %s', e)
         orc_db.delete_wallet_file(conn_config)
         raise e
     orc_db.delete_wallet_file(conn_config)
```

### Comparing `macrometa-source-oracle-0.0.34/macrometa_source_oracle/connection.py` & `macrometa-source-oracle-0.0.35/macrometa_source_oracle/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.34/macrometa_source_oracle/sync_strategies/common.py` & `macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.34/macrometa_source_oracle/sync_strategies/full_table.py` & `macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.34/macrometa_source_oracle/sync_strategies/log_based.py` & `macrometa-source-oracle-0.0.35/macrometa_source_oracle/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.34/pyproject.toml` & `macrometa-source-oracle-0.0.35/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-oracle"
-version='0.0.34'
+version='0.0.35'
 description = "Macrometa source oracle connector for reading from oracle databases."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 readme = "README.md"
 homepage = "https://www.macrometa.com/"
 keywords = [
     "ELT",
```

### Comparing `macrometa-source-oracle-0.0.34/setup.py` & `macrometa-source-oracle-0.0.35/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'strict-rfc3339>=0.7,<0.8']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-oracle = macrometa_source_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-oracle',
-    'version': '0.0.34',
+    'version': '0.0.35',
     'description': 'Macrometa source oracle connector for reading from oracle databases.',
-    'long_description': '# macrometa-source-oracle\n\nMacrometa source connector that extracts data from a [Oracle](https://www.oracle.com/database/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).\n\n## How to use it\n\n### Install and Run\n\nFirst, make sure Python 3 is installed on your system or follow these\ninstallation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or\n[Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).\n\n\nIt\'s recommended to use a virtualenv:\n\n```bash\n  python3 -m venv venv\n  pip install macrometa-source-oracle\n```\n\nor from source using,\n1. Install poetry using https://python-poetry.org/docs/#installation\n2. Run \n    ```bash\n    poetry build\n    pip install dist/macrometa_source_oracle-<version>*.whl\n    ```\n\n### Configuration\n\nRunning the the macrometa source connector independently requires a `config.json` file. \n\nExample configuration:\n\n```json\n{\n  "host": "dev.oracledb.io",\n  "port": 1521,\n  "user": "C##HELLO",\n  "password": "password",\n  "service_name": "ORCLCDB",\n  "filter_schema": "C##HELLO",\n  "filter_table": "CUSTOMERS",\n  "default_replication_method": "LOG_BASED",\n  "pdb_name": "ORCLPDB1",\n  "multitenant": true,\n  "scn_window_size": 10\n}\n```\n\nYou can run a discover run using the previous `config.json` file to acquire all the tables definition\n \n```\nmacrometa-source-oracle --config /tmp/config.json --discover >> /tmp/catalog.json\n```\n\nThen use the catalog.json to run a full export:\n\n```\nmacrometa-source-oracle --config /tmp/config.json --catalog /tmp/catalog.json\n```\n\n',
+    'long_description': '# macrometa-source-oracle\n\nMacrometa source connector that extracts data from a [Oracle](https://www.oracle.com/database/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).\n\n## How to use it\n\n### Install and Run\n\nFirst, make sure Python 3 is installed on your system or follow these\ninstallation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or\n[Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).\n\n\nIt\'s recommended to use a virtualenv:\n\n```bash\n  python3 -m venv venv\n  pip install macrometa-source-oracle\n```\n\nor from source using,\n1. Install poetry using https://python-poetry.org/docs/#installation\n2. Run \n    ```bash\n    poetry build\n    pip install dist/macrometa_source_oracle-<version>*.whl\n    ```\n\n### Configuration\n\nRunning the the macrometa source connector independently requires a `config.json` file. \n\nExample configuration:\n\n```json\n{\n  "host": "dev.oracledb.io",\n  "port": 1521,\n  "user": "C##HELLO",\n  "password": "password",\n  "service_name": "ORCLCDB",\n  "filter_schema": "C##HELLO",\n  "filter_table": "CUSTOMERS",\n  "replication_method": "LOG_BASED",\n  "pdb_name": "ORCLPDB1",\n  "multitenant": true,\n  "scn_window_size": 10\n}\n```\n\nYou can run a discover run using the previous `config.json` file to acquire all the tables definition\n \n```\nmacrometa-source-oracle --config /tmp/config.json --discover >> /tmp/catalog.json\n```\n\nThen use the catalog.json to run a full export:\n\n```\nmacrometa-source-oracle --config /tmp/config.json --catalog /tmp/catalog.json\n```\n\n',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.macrometa.com/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `macrometa-source-oracle-0.0.34/PKG-INFO` & `macrometa-source-oracle-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-oracle
-Version: 0.0.34
+Version: 0.0.35
 Summary: Macrometa source oracle connector for reading from oracle databases.
 Home-page: https://www.macrometa.com/
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Oracle,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8
@@ -62,15 +62,15 @@
   "host": "dev.oracledb.io",
   "port": 1521,
   "user": "C##HELLO",
   "password": "password",
   "service_name": "ORCLCDB",
   "filter_schema": "C##HELLO",
   "filter_table": "CUSTOMERS",
-  "default_replication_method": "LOG_BASED",
+  "replication_method": "LOG_BASED",
   "pdb_name": "ORCLPDB1",
   "multitenant": true,
   "scn_window_size": 10
 }
 ```
 
 You can run a discover run using the previous `config.json` file to acquire all the tables definition
```

