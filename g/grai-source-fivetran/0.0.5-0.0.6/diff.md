# Comparing `tmp/grai_source_fivetran-0.0.5.tar.gz` & `tmp/grai_source_fivetran-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.0.5.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.0.6.tar", max compression
```

## Comparing `grai_source_fivetran-0.0.5.tar` & `grai_source_fivetran-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,23 @@
--rw-r--r--   0        0        0      139 2023-04-29 00:58:02.889481 grai_source_fivetran-0.0.5/README.md
--rw-r--r--   0        0        0     1073 2023-04-30 17:37:05.396093 grai_source_fivetran-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.5/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     6644 2023-04-29 00:19:10.366197 grai_source_fivetran-0.0.5/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     1425 2023-02-14 16:39:18.543003 grai_source_fivetran-0.0.5/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    12057 2023-02-14 16:39:18.545562 grai_source_fivetran-0.0.5/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.5/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.5/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.5/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.5/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.5/setup.py
--rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      139 2023-05-19 10:56:28.943431 grai_source_fivetran-0.0.6/README.md
+-rw-r--r--   0        0        0     1073 2023-05-19 10:56:36.009424 grai_source_fivetran-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      441 2023-05-19 09:16:42.851003 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/grai_source_fivetran.iml
+-rw-r--r--   0        0        0     3706 2023-05-19 09:16:42.842120 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-05-19 09:16:42.863792 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      200 2023-05-19 09:16:42.860192 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/misc.xml
+-rw-r--r--   0        0        0      292 2023-05-19 09:16:42.855186 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/modules.xml
+-rw-r--r--   0        0        0     1676 2023-05-19 09:16:42.856457 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/workspace.xml
+-rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.6/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     6644 2023-05-19 10:56:28.944032 grai_source_fivetran-0.0.6/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     1425 2023-02-14 16:39:18.543003 grai_source_fivetran-0.0.6/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0      208 2023-04-10 14:43:24.094047 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0   304385 2023-04-10 14:43:24.142083 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/__pycache__/api_models.cpython-310.pyc
+-rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    13390 2023-05-19 10:56:28.944303 grai_source_fivetran-0.0.6/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.6/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.6/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.6/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.6/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.6/setup.py
+-rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.6/PKG-INFO
```

### Comparing `grai_source_fivetran-0.0.5/pyproject.toml` & `grai_source_fivetran-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_fivetran-0.0.5/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.0.6/src/grai_source_fivetran/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.5/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.0.6/src/grai_source_fivetran/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.5/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.5/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.0.6/src/grai_source_fivetran/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import json
 from itertools import chain
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
@@ -25,15 +26,21 @@
     SchemaMetadataResponse,
     TableMetadataResponse,
     V1ConnectorsConnectorIdSchemasGetResponse,
     V1ConnectorsConnectorIdSchemasSchemaTablesTableColumnsGetResponse,
     V1DestinationsDestinationIdGetResponse,
     V1GroupsGetResponse,
 )
-from grai_source_fivetran.models import Column, Edge, NamespaceIdentifier, Table
+from grai_source_fivetran.models import (
+    Column,
+    Edge,
+    NamespaceIdentifier,
+    NodeTypes,
+    Table,
+)
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 class FiveTranConfig(BaseSettings):
     endpoint: str = "https://api.fivetran.com/v1"
@@ -160,14 +167,19 @@
     def get_source_table_column_metadata(
         self, connector_id: str, schema: str, table: str
     ) -> V1ConnectorsConnectorIdSchemasSchemaTablesTableColumnsGetResponse:
         url = f"{self.config.endpoint}/connectors/{connector_id}/schemas/{schema}/tables/{table}/columns"
         data, response = self.make_request(self.session.get, url)
         return V1ConnectorsConnectorIdSchemasSchemaTablesTableColumnsGetResponse(**data)
 
+    def get_connectors(self) -> List[ConnectorResponse]:
+        groups = {group.id: group for group in self.get_all_groups() if group.id is not None}
+        connectors = [conn for group_id in groups.keys() for conn in self.get_group_connectors(group_id)]
+        return connectors
+
 
 async def caller(semaphore: asyncio.Semaphore, func: Callable[..., T], *args, **kwargs) -> T:
     result = func(*args, **kwargs)
 
     async with semaphore:
         if semaphore.locked():
             await asyncio.sleep(1)
@@ -197,86 +209,101 @@
 
 
 class SourceDestinationDict(TypedDict):
     source: str
     destination: str
 
 
-NamespaceTypes = Union[Dict[str, str], SourceDestinationDict]
+NamespaceTypes = Union[Dict[str, Union[str, SourceDestinationDict]], str]
 
 
 class FivetranConnector(FivetranAPI):
     def __init__(
         self,
         namespaces: Optional[NamespaceTypes] = None,
         default_namespace: Optional[str] = None,
         parallelization: int = 10,
         *args,
         **kwargs,
     ):
-        if namespaces is None and default_namespace is None:
-            message = (
-                f"The FivetranGraiMapper requires a not null value for `default_namespace` and/or `namespaces. "
-                f"These values are used to identify which Fivetran connection id's belong to which associated "
-                f"Grai namespace. `default_namespace` will map a single namespace to ALL connection id's."
-                "This behavior can be overridden by `namespaces` which maps {connection_id -> "
-                "namespace} or {connection_id -> {source: namespace, destination: namespace}}"
-            )
-            raise ValueError(message)
-        elif namespaces is not None:
-            assert all(isinstance(v, (dict, str)) for v in namespaces.values())
-            assert all(isinstance(v, SourceDestinationDict) for v in namespaces.values() if isinstance(v, dict))
-        else:
-            namespaces = {}
-
         super().__init__(*args, **kwargs)
         self.parallelization = parallelization
         self.semaphore = asyncio.Semaphore(self.parallelization)
         self.http_runner = parallelize_http(self.semaphore)
+        self.default_namespace = default_namespace
 
-        self.groups = {group.id: group for group in self.get_all_groups() if group.id is not None}
-        self.connectors = {
-            conn.id: conn
-            for group_id in self.groups.keys()
-            for conn in self.get_group_connectors(group_id)
-            if conn.id is not None
-        }
-
-        if default_namespace is None:
-            self.connectors = {k: v for k, v in self.connectors.items() if v in namespaces}
-        else:
-            namespaces = {**namespaces}  # avoid modifying the users original argument
-            for k in self.connectors.keys():
-                namespaces.setdefault(k, default_namespace)
-
-        self.namespace_map = {
-            k: NamespaceIdentifier(source=v, destination=v) if isinstance(v, str) else NamespaceIdentifier(**v)
-            for k, v in namespaces.items()
-        }
+        self.connectors = {conn.id: conn for conn in self.get_connectors() if conn.id is not None}
+        self.namespace_map = self._build_namespace_map(namespaces)
+        if self.default_namespace is None:
+            self.connectors = {k: v for k, v in self.connectors.items() if k in self.namespace_map}
+
+        self.table_to_conn_map: Dict[str, str] = {}
+        self.column_to_conn_map: Dict[str, str] = {}
+        self.schemas: Dict[str, SchemaMetadataResponse] = {}
+        self.tables: Dict[str, TableMetadataResponse] = {}
+        self.columns: Dict[str, ColumnMetadataResponse] = {}
 
+    def build_lineage(self):
         connector_ids = [[conn_id] for conn_id in self.connectors.keys()]
         schemas = self.http_runner(self.get_schemas, arg_list=connector_ids)
         tables = self.http_runner(self.get_tables, arg_list=connector_ids)
         columns = self.http_runner(self.get_columns, arg_list=connector_ids)
 
-        self.table_to_conn_map = {}
-        self.column_to_conn_map = {}
         for conn_id, t_res, c_res in zip(self.connectors.keys(), tables, columns):
             for table in t_res:
                 self.table_to_conn_map.setdefault(table.id, conn_id)
             for column in c_res:
                 self.column_to_conn_map.setdefault(column.id, conn_id)
 
-        self.schemas: Dict[str, SchemaMetadataResponse] = {item.id: item for seq in schemas for item in seq}
-        self.tables: Dict[str, TableMetadataResponse] = {item.id: item for seq in tables for item in seq}
-        self.columns: Dict[str, ColumnMetadataResponse] = {item.id: item for seq in columns for item in seq}
+        self.schemas.update({item.id: item for seq in schemas for item in seq})
+        self.tables.update({item.id: item for seq in tables for item in seq})
+        self.columns.update({item.id: item for seq in columns for item in seq})
+
+    def _build_namespace_map(self, namespace_map: Optional[NamespaceTypes]) -> Dict[str, NamespaceIdentifier]:
+        if namespace_map is None and self.default_namespace is None:
+            message = (
+                f"The FivetranGraiMapper requires a not null value for `default_namespace` and/or `namespaces. "
+                f"These values are used to identify which Fivetran connection id's belong to which associated "
+                f"Grai namespace. `default_namespace` will map a single namespace to ALL connection id's."
+                "This behavior can be overridden by `namespaces` which maps {connection_id -> "
+                "namespace} or {connection_id -> {source: namespace, destination: namespace}}"
+            )
+            raise ValueError(message)
+        elif isinstance(namespace_map, str):
+            namespace_map = json.loads(namespace_map)
+
+        if namespace_map is None:
+            namespace_map = {}
+        else:
+            message = (
+                "The namespaces object should be a dictionary whose id's are Fivetran connector id's and whose values "
+                "identify the Grai namespace associated with either the source or destination of the connector. "
+                "The values can either be provided as a dictionary with the keys 'source' and 'destination' or ",
+                "as strings identifying the Grai namespace you'd like to associate with both the source "
+                "and destination.",
+            )
+            assert all(isinstance(v, (dict, str)) for v in namespace_map.values()), message
+            assert all(
+                isinstance(v, SourceDestinationDict) for v in namespace_map.values() if isinstance(v, dict)
+            ), message
+
+        if self.default_namespace is not None:
+            namespace_map = namespace_map.copy()  # avoid modifying the users original argument
+            for k in self.connectors.keys():
+                namespace_map.setdefault(k, self.default_namespace)
+
+        return {
+            k: NamespaceIdentifier(source=v, destination=v) if isinstance(v, str) else NamespaceIdentifier(**v)
+            for k, v in namespace_map.items()
+        }
 
-    def get_nodes_and_edges(self):
+    def get_nodes_and_edges(self) -> Tuple[List[NodeTypes], List[Edge]]:
         # table.parent_id -> schema.id
         # column.parent_id -> table.id
+        self.build_lineage()
         tables = {
             table.id: Table.from_fivetran_models(
                 self.schemas[table.parent_id],
                 table,
                 self.namespace_map[self.table_to_conn_map[table.id]],
             )
             for table in self.tables.values()
```

### Comparing `grai_source_fivetran-0.0.5/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.0.6/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.5/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.0.6/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.5/setup.py` & `grai_source_fivetran-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['grai_source_fivetran', 'grai_source_fivetran.fivetran_api']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'grai_source_fivetran': ['.idea/*', '.idea/inspectionProfiles/*']}
 
 install_requires = \
 ['fivetran>=0.7.0,<0.8.0',
  'grai-client>=0.2.0,<0.3.0',
  'grai-schemas>=0.1.10,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic>=1.9.1,<2.0.0',
  'python-dotenv>=0.21.1,<0.22.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-fivetran',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': '',
     'long_description': '# Grai Fivetran Integration\n\nThe Fivetran integration synchronizes metadata from your Fivetran instance into your Grai data lineage graph.\n',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.grai.io/',
```

### Comparing `grai_source_fivetran-0.0.5/PKG-INFO` & `grai_source_fivetran-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-fivetran
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
```

