# Comparing `tmp/dbt_superset_lineage-0.3.1.tar.gz` & `tmp/dbt_superset_lineage-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_superset_lineage-0.3.1.tar", max compression
+gzip compressed data, was "dbt_superset_lineage-0.3.2.tar", max compression
```

## Comparing `dbt_superset_lineage-0.3.1.tar` & `dbt_superset_lineage-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2021-12-03 09:02:37.138885 dbt_superset_lineage-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     4774 2023-03-28 19:49:49.244002 dbt_superset_lineage-0.3.1/README.md
--rw-r--r--   0        0        0     6148 2023-03-30 16:32:49.836101 dbt_superset_lineage-0.3.1/dbt_superset_lineage/.DS_Store
--rw-r--r--   0        0        0     4506 2023-04-03 14:26:54.290955 dbt_superset_lineage-0.3.1/dbt_superset_lineage/__init__.py
--rw-r--r--   0        0        0    14162 2023-04-03 20:24:19.463013 dbt_superset_lineage-0.3.1/dbt_superset_lineage/pull_dashboards.py
--rw-r--r--   0        0        0     8842 2023-05-16 14:38:20.272268 dbt_superset_lineage-0.3.1/dbt_superset_lineage/push_descriptions.py
--rw-r--r--   0        0        0     3370 2023-03-21 10:17:38.771099 dbt_superset_lineage-0.3.1/dbt_superset_lineage/superset_api.py
--rw-r--r--   0        0        0      642 2023-05-16 14:38:58.519322 dbt_superset_lineage-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5735 1970-01-01 00:00:00.000000 dbt_superset_lineage-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2021-12-03 09:02:37.138885 dbt_superset_lineage-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     4958 2023-05-19 13:52:56.559857 dbt_superset_lineage-0.3.2/README.md
+-rw-r--r--   0        0        0     6148 2023-03-30 16:32:49.836101 dbt_superset_lineage-0.3.2/dbt_superset_lineage/.DS_Store
+-rw-r--r--   0        0        0     4506 2023-04-03 14:26:54.290955 dbt_superset_lineage-0.3.2/dbt_superset_lineage/__init__.py
+-rw-r--r--   0        0        0    14162 2023-05-19 12:52:18.185188 dbt_superset_lineage-0.3.2/dbt_superset_lineage/pull_dashboards.py
+-rw-r--r--   0        0        0     9120 2023-05-19 13:52:30.622216 dbt_superset_lineage-0.3.2/dbt_superset_lineage/push_descriptions.py
+-rw-r--r--   0        0        0     3370 2023-03-21 10:17:38.771099 dbt_superset_lineage-0.3.2/dbt_superset_lineage/superset_api.py
+-rw-r--r--   0        0        0      642 2023-05-19 13:55:31.884539 dbt_superset_lineage-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5919 1970-01-01 00:00:00.000000 dbt_superset_lineage-0.3.2/PKG-INFO
```

### Comparing `dbt_superset_lineage-0.3.1/LICENSE.md` & `dbt_superset_lineage-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.1/README.md` & `dbt_superset_lineage-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 
 ### Push descriptions
 Push model and column descriptions from your dbt docs to Superset as plain text so that they could be viewed
 in Superset when creating charts.
 
 **N.B.**:
 - Run carefully as this rewrites your datasets using merged metadata from Superset and dbt docs.
+- Running with `--superset-refresh-columns` overrides `columns.filterable` and `columns.groupby` to `true`,
+  because of [this issue](https://github.com/apache/superset/issues/24136).
 - Descriptions are rendered as plain text, hence no markdown syntax, incl. links, will be displayed.
 - Avoid special characters and strings in your dbt docs, e.g. `→` or `<null>`.
 
 ```console
 $ cd jaffle_shop
 $ dbt compile  # Compile project to create manifest.json
 $ export SUPERSET_ACCESS_TOKEN=<TOKEN>
```

#### html2text {}

```diff
@@ -44,15 +44,18 @@
 mysuperset.mycompany.com # Pull dashboards from Superset to /models/exposures/
 superset_dashboards.yml $ dbt docs generate # Generate dbt docs $ dbt docs
 serve # Serve dbt docs ``` ![Separate exposure in dbt docs](assets/
 exposures_1.png) ![Referenced exposure in dbt docs](assets/exposures_2.png) ###
 Push descriptions Push model and column descriptions from your dbt docs to
 Superset as plain text so that they could be viewed in Superset when creating
 charts. **N.B.**: - Run carefully as this rewrites your datasets using merged
-metadata from Superset and dbt docs. - Descriptions are rendered as plain text,
-hence no markdown syntax, incl. links, will be displayed. - Avoid special
-characters and strings in your dbt docs, e.g. `â` or ``. ```console $ cd
-jaffle_shop $ dbt compile # Compile project to create manifest.json $ export
-SUPERSET_ACCESS_TOKEN= $ dbt-superset-lineage push-descriptions https://
-mysuperset.mycompany.com # Push descrptions from dbt docs to Superset ``` !
-[Column descriptions in Superset](assets/descriptions.png) ## License Licensed
-under the MIT license (see [LICENSE.md](LICENSE.md) file for more details).
+metadata from Superset and dbt docs. - Running with `--superset-refresh-
+columns` overrides `columns.filterable` and `columns.groupby` to `true`,
+because of [this issue](https://github.com/apache/superset/issues/24136). -
+Descriptions are rendered as plain text, hence no markdown syntax, incl. links,
+will be displayed. - Avoid special characters and strings in your dbt docs,
+e.g. `â` or ``. ```console $ cd jaffle_shop $ dbt compile # Compile project
+to create manifest.json $ export SUPERSET_ACCESS_TOKEN= $ dbt-superset-lineage
+push-descriptions https://mysuperset.mycompany.com # Push descrptions from dbt
+docs to Superset ``` ![Column descriptions in Superset](assets/
+descriptions.png) ## License Licensed under the MIT license (see [LICENSE.md]
+(LICENSE.md) file for more details).
```

### Comparing `dbt_superset_lineage-0.3.1/dbt_superset_lineage/.DS_Store` & `dbt_superset_lineage-0.3.2/dbt_superset_lineage/.DS_Store`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.1/dbt_superset_lineage/__init__.py` & `dbt_superset_lineage-0.3.2/dbt_superset_lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.1/dbt_superset_lineage/pull_dashboards.py` & `dbt_superset_lineage-0.3.2/dbt_superset_lineage/pull_dashboards.py`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.1/dbt_superset_lineage/push_descriptions.py` & `dbt_superset_lineage-0.3.2/dbt_superset_lineage/push_descriptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     logging.info("Pulling fresh columns info from Superset.")
 
     res = superset.request('GET', f"/dataset/{dataset['id']}")
     result = res['result']
 
     dataset['columns'] = result['columns']
     dataset['description'] = result['description']
+    dataset['owners'] = result['owners']
 
     return dataset
 
 
 def convert_markdown_to_plain_text(md_string):
     """Converts a markdown string to plaintext.
 
@@ -147,14 +148,16 @@
     key = dataset['key']
     sst_columns = dataset['columns']
     dbt_columns = tables.get(key, {}).get('columns', {})
 
     sst_description = dataset['description']
     dbt_description = tables.get(key, {}).get('description')
 
+    sst_owners = dataset['owners']
+
     columns_new = []
     for sst_column in sst_columns:
 
         column_name = sst_column['column_name']
 
         # add the mandatory fields
         column_new = {
@@ -179,37 +182,41 @@
 
     # add dataset description
     if dbt_description is None:
         dataset['description_new'] = sst_description
     else:
         dataset['description_new'] = convert_markdown_to_plain_text(dbt_description)
 
+    # add dataset owner IDs (otherwise Superset empties the owners list)
+    dataset['owners_new'] = [owner['id'] for owner in sst_owners]
+
     return dataset
 
 
 def check_columns_equal(lst1, lst2):
     return sorted(lst1, key=lambda c: c["id"]) == sorted(lst2, key=lambda c: c["id"])
 
 
 def put_descriptions_to_superset(superset, dataset):
     logging.info("Putting model and column descriptions into Superset.")
 
     description_new = dataset['description_new']
     columns_new = dataset['columns_new']
+    owners_new = dataset['owners_new']
 
     description_old = dataset['description']
     columns_old = [{
         'column_name': col['column_name'],
         'id': col['id'],
         'description': col['description']
     } for col in dataset['columns']]
 
     if description_new != description_old or \
        not check_columns_equal(columns_new, columns_old):
-        payload = {'description': description_new, 'columns': columns_new}
+        payload = {'description': description_new, 'columns': columns_new, 'owners': owners_new}
         superset.request('PUT', f"/dataset/{dataset['id']}?override_columns=false", json=payload)
     else:
         logging.info("Skipping PUT execute request as nothing would be updated.")
 
 
 def main(dbt_project_dir, dbt_db_name,
          superset_url, superset_db_id, superset_refresh_columns,
```

### Comparing `dbt_superset_lineage-0.3.1/dbt_superset_lineage/superset_api.py` & `dbt_superset_lineage-0.3.2/dbt_superset_lineage/superset_api.py`

 * *Files identical despite different names*

### Comparing `dbt_superset_lineage-0.3.1/pyproject.toml` & `dbt_superset_lineage-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-superset-lineage"
-version = "0.3.1"
+version = "0.3.2"
 description = "Make dbt docs and Apache Superset talk to one another"
 authors = ["Michal Kolacek <mkolacek@slido.com>"]
 readme = "README.md"
 repository = "https://github.com/slidoapp/dbt-superset-lineage"
 
 [tool.poetry.scripts]
 dbt-superset-lineage = "dbt_superset_lineage.__init__:app"
```

### Comparing `dbt_superset_lineage-0.3.1/PKG-INFO` & `dbt_superset_lineage-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-superset-lineage
-Version: 0.3.1
+Version: 0.3.2
 Summary: Make dbt docs and Apache Superset talk to one another
 Home-page: https://github.com/slidoapp/dbt-superset-lineage
 Author: Michal Kolacek
 Author-email: mkolacek@slido.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -101,14 +101,16 @@
 
 ### Push descriptions
 Push model and column descriptions from your dbt docs to Superset as plain text so that they could be viewed
 in Superset when creating charts.
 
 **N.B.**:
 - Run carefully as this rewrites your datasets using merged metadata from Superset and dbt docs.
+- Running with `--superset-refresh-columns` overrides `columns.filterable` and `columns.groupby` to `true`,
+  because of [this issue](https://github.com/apache/superset/issues/24136).
 - Descriptions are rendered as plain text, hence no markdown syntax, incl. links, will be displayed.
 - Avoid special characters and strings in your dbt docs, e.g. `→` or `<null>`.
 
 ```console
 $ cd jaffle_shop
 $ dbt compile  # Compile project to create manifest.json
 $ export SUPERSET_ACCESS_TOKEN=<TOKEN>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-superset-lineage Version: 0.3.1 Summary: Make
+Metadata-Version: 2.1 Name: dbt-superset-lineage Version: 0.3.2 Summary: Make
 dbt docs and Apache Superset talk to one another Home-page: https://github.com/
 slidoapp/dbt-superset-lineage Author: Michal Kolacek Author-email:
 mkolacek@slido.com Requires-Python: >=3.8,<4.0 Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: Markdown (>=3.3.6,<4.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-
@@ -57,15 +57,18 @@
 mysuperset.mycompany.com # Pull dashboards from Superset to /models/exposures/
 superset_dashboards.yml $ dbt docs generate # Generate dbt docs $ dbt docs
 serve # Serve dbt docs ``` ![Separate exposure in dbt docs](assets/
 exposures_1.png) ![Referenced exposure in dbt docs](assets/exposures_2.png) ###
 Push descriptions Push model and column descriptions from your dbt docs to
 Superset as plain text so that they could be viewed in Superset when creating
 charts. **N.B.**: - Run carefully as this rewrites your datasets using merged
-metadata from Superset and dbt docs. - Descriptions are rendered as plain text,
-hence no markdown syntax, incl. links, will be displayed. - Avoid special
-characters and strings in your dbt docs, e.g. `â` or ``. ```console $ cd
-jaffle_shop $ dbt compile # Compile project to create manifest.json $ export
-SUPERSET_ACCESS_TOKEN= $ dbt-superset-lineage push-descriptions https://
-mysuperset.mycompany.com # Push descrptions from dbt docs to Superset ``` !
-[Column descriptions in Superset](assets/descriptions.png) ## License Licensed
-under the MIT license (see [LICENSE.md](LICENSE.md) file for more details).
+metadata from Superset and dbt docs. - Running with `--superset-refresh-
+columns` overrides `columns.filterable` and `columns.groupby` to `true`,
+because of [this issue](https://github.com/apache/superset/issues/24136). -
+Descriptions are rendered as plain text, hence no markdown syntax, incl. links,
+will be displayed. - Avoid special characters and strings in your dbt docs,
+e.g. `â` or ``. ```console $ cd jaffle_shop $ dbt compile # Compile project
+to create manifest.json $ export SUPERSET_ACCESS_TOKEN= $ dbt-superset-lineage
+push-descriptions https://mysuperset.mycompany.com # Push descrptions from dbt
+docs to Superset ``` ![Column descriptions in Superset](assets/
+descriptions.png) ## License Licensed under the MIT license (see [LICENSE.md]
+(LICENSE.md) file for more details).
```

