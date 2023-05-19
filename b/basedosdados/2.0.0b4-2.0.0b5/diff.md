# Comparing `tmp/basedosdados-2.0.0b4.tar.gz` & `tmp/basedosdados-2.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basedosdados-2.0.0b4.tar", max compression
+gzip compressed data, was "basedosdados-2.0.0b5.tar", max compression
```

## Comparing `basedosdados-2.0.0b4.tar` & `basedosdados-2.0.0b5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2514 2023-05-17 15:25:36.766063 basedosdados-2.0.0b4/README.md
--rw-r--r--   0        0        0      827 2023-05-17 15:25:36.766653 basedosdados-2.0.0b4/basedosdados/__init__.py
--rw-r--r--   0        0        0      156 2023-05-17 15:25:36.767118 basedosdados-2.0.0b4/basedosdados/__main__.py
--rw-r--r--   0        0        0     9545 2023-05-17 16:26:49.793959 basedosdados-2.0.0b4/basedosdados/backend/__init__.py
--rw-r--r--   0        0        0     6737 2023-05-17 15:25:36.767842 basedosdados-2.0.0b4/basedosdados/cli/cli.py
--rw-r--r--   0        0        0      277 2023-05-17 15:25:36.768671 basedosdados-2.0.0b4/basedosdados/configs/config.toml
--rw-r--r--   0        0        0      469 2022-02-13 03:48:24.650258 basedosdados-2.0.0b4/basedosdados/configs/templates/dataset/README.md
--rw-r--r--   0        0        0      856 2022-02-13 03:48:24.650328 basedosdados-2.0.0b4/basedosdados/configs/templates/dataset/dataset_description.txt
--rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.650411 basedosdados-2.0.0b4/basedosdados/configs/templates/table/publish.sql
--rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.504177 basedosdados-2.0.0b4/basedosdados/configs/templates/table/table_description.txt
--rw-r--r--   0        0        0      895 2023-05-17 15:25:36.768974 basedosdados-2.0.0b4/basedosdados/constants.py
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650584 basedosdados-2.0.0b4/basedosdados/download/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-17 15:25:36.769303 basedosdados-2.0.0b4/basedosdados/download/base.py
--rw-r--r--   0        0        0    17788 2023-05-17 15:25:36.769667 basedosdados-2.0.0b4/basedosdados/download/download.py
--rw-r--r--   0        0        0    13689 2023-05-17 15:25:36.770079 basedosdados-2.0.0b4/basedosdados/download/metadata.py
--rw-r--r--   0        0        0     3903 2023-05-17 15:25:36.770604 basedosdados-2.0.0b4/basedosdados/exceptions.py
--rw-r--r--   0        0        0     6779 2023-05-17 15:25:36.771132 basedosdados-2.0.0b4/basedosdados/schemas/columns_schema.json
--rw-r--r--   0        0        0    65118 2023-05-17 15:25:36.771553 basedosdados-2.0.0b4/basedosdados/schemas/dataset_schema.json
--rw-r--r--   0        0        0    30753 2023-05-17 15:25:36.771686 basedosdados-2.0.0b4/basedosdados/schemas/table_schema.json
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650914 basedosdados-2.0.0b4/basedosdados/upload/__init__.py
--rw-r--r--   0        0        0    15586 2023-05-17 15:25:36.772065 basedosdados-2.0.0b4/basedosdados/upload/base.py
--rw-r--r--   0        0        0     4957 2023-05-17 15:25:36.772254 basedosdados-2.0.0b4/basedosdados/upload/connection.py
--rw-r--r--   0        0        0     9399 2023-05-17 15:25:36.772612 basedosdados-2.0.0b4/basedosdados/upload/dataset.py
--rw-r--r--   0        0        0     3228 2023-05-17 15:25:36.773037 basedosdados-2.0.0b4/basedosdados/upload/datatypes.py
--rw-r--r--   0        0        0    18917 2023-05-17 15:25:36.773769 basedosdados-2.0.0b4/basedosdados/upload/storage.py
--rw-r--r--   0        0        0    30950 2023-05-17 16:21:47.259880 basedosdados-2.0.0b4/basedosdados/upload/table.py
--rw-r--r--   0        0        0     3434 2023-05-17 15:25:36.774605 basedosdados-2.0.0b4/basedosdados/upload/utils.py
--rw-r--r--   0        0        0     1453 2023-05-17 16:27:15.203997 basedosdados-2.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 basedosdados-2.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     2514 2023-05-17 15:25:36.766063 basedosdados-2.0.0b5/README.md
+-rw-r--r--   0        0        0      827 2023-05-17 15:25:36.766653 basedosdados-2.0.0b5/basedosdados/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-17 15:25:36.767118 basedosdados-2.0.0b5/basedosdados/__main__.py
+-rw-r--r--   0        0        0     9545 2023-05-17 16:26:49.793959 basedosdados-2.0.0b5/basedosdados/backend/__init__.py
+-rw-r--r--   0        0        0     6737 2023-05-17 15:25:36.767842 basedosdados-2.0.0b5/basedosdados/cli/cli.py
+-rw-r--r--   0        0        0      277 2023-05-17 15:25:36.768671 basedosdados-2.0.0b5/basedosdados/configs/config.toml
+-rw-r--r--   0        0        0      469 2022-02-13 03:48:24.650258 basedosdados-2.0.0b5/basedosdados/configs/templates/dataset/README.md
+-rw-r--r--   0        0        0      856 2022-02-13 03:48:24.650328 basedosdados-2.0.0b5/basedosdados/configs/templates/dataset/dataset_description.txt
+-rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.650411 basedosdados-2.0.0b5/basedosdados/configs/templates/table/publish.sql
+-rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.504177 basedosdados-2.0.0b5/basedosdados/configs/templates/table/table_description.txt
+-rw-r--r--   0        0        0      895 2023-05-17 15:25:36.768974 basedosdados-2.0.0b5/basedosdados/constants.py
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650584 basedosdados-2.0.0b5/basedosdados/download/__init__.py
+-rw-r--r--   0        0        0     1641 2023-05-17 15:25:36.769303 basedosdados-2.0.0b5/basedosdados/download/base.py
+-rw-r--r--   0        0        0    17788 2023-05-17 15:25:36.769667 basedosdados-2.0.0b5/basedosdados/download/download.py
+-rw-r--r--   0        0        0    13689 2023-05-17 15:25:36.770079 basedosdados-2.0.0b5/basedosdados/download/metadata.py
+-rw-r--r--   0        0        0     3903 2023-05-17 15:25:36.770604 basedosdados-2.0.0b5/basedosdados/exceptions.py
+-rw-r--r--   0        0        0     6779 2023-05-17 15:25:36.771132 basedosdados-2.0.0b5/basedosdados/schemas/columns_schema.json
+-rw-r--r--   0        0        0    65118 2023-05-17 15:25:36.771553 basedosdados-2.0.0b5/basedosdados/schemas/dataset_schema.json
+-rw-r--r--   0        0        0    30753 2023-05-17 15:25:36.771686 basedosdados-2.0.0b5/basedosdados/schemas/table_schema.json
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650914 basedosdados-2.0.0b5/basedosdados/upload/__init__.py
+-rw-r--r--   0        0        0    15586 2023-05-17 15:25:36.772065 basedosdados-2.0.0b5/basedosdados/upload/base.py
+-rw-r--r--   0        0        0     4957 2023-05-17 15:25:36.772254 basedosdados-2.0.0b5/basedosdados/upload/connection.py
+-rw-r--r--   0        0        0     9399 2023-05-17 15:25:36.772612 basedosdados-2.0.0b5/basedosdados/upload/dataset.py
+-rw-r--r--   0        0        0     3228 2023-05-17 15:25:36.773037 basedosdados-2.0.0b5/basedosdados/upload/datatypes.py
+-rw-r--r--   0        0        0    18883 2023-05-19 20:35:33.604737 basedosdados-2.0.0b5/basedosdados/upload/storage.py
+-rw-r--r--   0        0        0    31554 2023-05-19 19:16:17.685574 basedosdados-2.0.0b5/basedosdados/upload/table.py
+-rw-r--r--   0        0        0     3434 2023-05-17 15:25:36.774605 basedosdados-2.0.0b5/basedosdados/upload/utils.py
+-rw-r--r--   0        0        0     1453 2023-05-19 20:37:00.994680 basedosdados-2.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 basedosdados-2.0.0b5/PKG-INFO
```

### Comparing `basedosdados-2.0.0b4/README.md` & `basedosdados-2.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/__init__.py` & `basedosdados-2.0.0b5/basedosdados/__init__.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/backend/__init__.py` & `basedosdados-2.0.0b5/basedosdados/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/cli/cli.py` & `basedosdados-2.0.0b5/basedosdados/cli/cli.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/configs/templates/dataset/dataset_description.txt` & `basedosdados-2.0.0b5/basedosdados/configs/templates/dataset/dataset_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/configs/templates/table/publish.sql` & `basedosdados-2.0.0b5/basedosdados/configs/templates/table/publish.sql`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/configs/templates/table/table_description.txt` & `basedosdados-2.0.0b5/basedosdados/configs/templates/table/table_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/constants.py` & `basedosdados-2.0.0b5/basedosdados/constants.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/download/base.py` & `basedosdados-2.0.0b5/basedosdados/download/base.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/download/download.py` & `basedosdados-2.0.0b5/basedosdados/download/download.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/download/metadata.py` & `basedosdados-2.0.0b5/basedosdados/download/metadata.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/exceptions.py` & `basedosdados-2.0.0b5/basedosdados/exceptions.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/schemas/columns_schema.json` & `basedosdados-2.0.0b5/basedosdados/schemas/columns_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/schemas/dataset_schema.json` & `basedosdados-2.0.0b5/basedosdados/schemas/dataset_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/schemas/table_schema.json` & `basedosdados-2.0.0b5/basedosdados/schemas/table_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/upload/base.py` & `basedosdados-2.0.0b5/basedosdados/upload/base.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/upload/connection.py` & `basedosdados-2.0.0b5/basedosdados/upload/connection.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/upload/dataset.py` & `basedosdados-2.0.0b5/basedosdados/upload/dataset.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/upload/datatypes.py` & `basedosdados-2.0.0b5/basedosdados/upload/datatypes.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/basedosdados/upload/storage.py` & `basedosdados-2.0.0b5/basedosdados/upload/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,14 @@
 
             # replicate folder hierarchy
             savepath = Path(savepath)
             (savepath / blob_folder).mkdir(parents=True, exist_ok=True)
 
             # download blob to savepath
             save_file_path = savepath / blob.name
-            print(save_file_path)
 
             blob.download_to_filename(filename=save_file_path)
 
         logger.success(
             " {object} {object_id}_{mode} was {action} at: {path}!",
             object_id=self.dataset_id,
             mode=mode,
```

### Comparing `basedosdados-2.0.0b4/basedosdados/upload/table.py` & `basedosdados-2.0.0b5/basedosdados/upload/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,14 +288,29 @@
 
     def _get_cross_columns_from_bq_api(self):
         bq = self._get_columns_from_bq(mode="staging")
         bq_columns = bq.get("partition_columns") + bq.get("columns")
 
         api = self._get_columns_metadata_from_api()
         api_columns = api.get("partition_columns") + api.get("columns")
+
+        # bq_columns_list = [col.get("name") for col in bq_columns]
+        # api_columns_list = [col.get("name") for col in api_columns]
+
+        # not_in_api_columns = [
+        #     col for col in bq_columns_list if col not in api_columns_list
+        # ]
+        # not_in_bq_columns = [
+        #     col for col in api_columns_list if col not in bq_columns_list
+        # ]
+        # print("bq_columns_list", len(bq_columns_list))
+        # print("api_columns_list", len(api_columns_list))
+        # print("not_in_api_columns", not_in_api_columns)
+        # print("not_in_bq_columns", not_in_bq_columns)
+
         if api_columns != []:
             for bq_col in bq_columns:
                 for api_col in api_columns:
                     if bq_col.get("name") == api_col.get("name"):
                         bq_col["type"] = api_col.get("type")
                         bq_col["description"] = api_col.get("description")
 
@@ -740,15 +755,15 @@
 
         if mode == "all":
             for m, n in self.table_full_name[mode].items():
                 self.client[f"bigquery_{m}"].delete_table(n, not_found_ok=True)
                 logger.info(
                     " {object} {object_id}_{mode} was {action}!",
                     object_id=self.table_id,
-                    mode=m["mode"],
+                    mode=m,
                     object="Table",
                     action="deleted",
                 )
         else:
             self.client[f"bigquery_{mode}"].delete_table(
                 self.table_full_name[mode], not_found_ok=True
             )
```

### Comparing `basedosdados-2.0.0b4/basedosdados/upload/utils.py` & `basedosdados-2.0.0b5/basedosdados/upload/utils.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b4/pyproject.toml` & `basedosdados-2.0.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 license = "MIT"
 name = "basedosdados"
 packages = [
   {include = "basedosdados"},
 ]
 readme = "README.md"
 repository = "https://github.com/base-dos-dados/bases"
-version = "2.0.0-beta.4"
+version = "2.0.0-beta.5"
 
 [tool.poetry.scripts]
 basedosdados = 'basedosdados.cli.cli:cli'
 
 [tool.poetry.dependencies]
 google-api-python-client = "^2.86.0"
 google-cloud-bigquery = "^3.10.0"
```

### Comparing `basedosdados-2.0.0b4/PKG-INFO` & `basedosdados-2.0.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basedosdados
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: Organizar e facilitar o acesso a dados brasileiros através de tabelas públicas no BigQuery.
 Home-page: https://github.com/base-dos-dados/bases
 License: MIT
 Author: Joao Carabetta
 Author-email: joao.carabetta@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

