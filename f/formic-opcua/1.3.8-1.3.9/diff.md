# Comparing `tmp/formic_opcua-1.3.8.tar.gz` & `tmp/formic_opcua-1.3.9.tar.gz`

## Comparing `formic_opcua-1.3.8.tar` & `formic_opcua-1.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    11780 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/core/parse.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    11780 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/PKG-INFO
```

### Comparing `formic_opcua-1.3.8/.pre-commit-config.yaml` & `formic_opcua-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/examples/opcua_client.py` & `formic_opcua-1.3.9/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.3.9/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.3.9/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.3.9/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.3.9/formic_opcua/client/async_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/formic_opcua/client/opcua_client.py` & `formic_opcua-1.3.9/formic_opcua/client/opcua_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,18 @@
         node_class = node.read_node_class()
         path_to_node = path + '/' + browse_path.Name
         if node_class == NodeClass.Variable and browse_path.NamespaceIndex == self._idx:
             # Remove "/Objects/" since this client is intended for reading only custom nodes
             path_to_node = path_to_node[9:]
             var_type = node.read_data_type_as_variant_type()
             logger.info(f'Found OPCUA variable {path_to_node}, of variant type {var_type}')
-            self._node_map[path_to_node] = (node, var_type)
+            if not path_to_node.startswith('/'):
+                self._node_map['/' + path_to_node] = (node, var_type)
+            else:
+                self._node_map[path_to_node] = (node, var_type)
 
         for child_node in node.get_children():
             self._dfs_mapper(child_node, path_to_node)
 
     def _establish_server_structure(self) -> None:
         try:
             logger.info(f'Mapping namespace using {self._url} and {self._uri}')
```

### Comparing `formic_opcua-1.3.8/formic_opcua/core/parse.py` & `formic_opcua-1.3.9/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/formic_opcua/core/type_conversions.py` & `formic_opcua-1.3.9/formic_opcua/core/type_conversions.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.3.9/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.3.9/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/formic_opcua/server/opcua_server.py` & `formic_opcua-1.3.9/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/hooks/add_issue_prefix.py` & `formic_opcua-1.3.9/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/tests/test_server_config.py` & `formic_opcua-1.3.9/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/.gitignore` & `formic_opcua-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.8/pyproject.toml` & `formic_opcua-1.3.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

