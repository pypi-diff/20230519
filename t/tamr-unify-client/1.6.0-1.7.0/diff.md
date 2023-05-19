# Comparing `tmp/tamr-unify-client-1.6.0.tar.gz` & `tmp/tamr_unify_client-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamr-unify-client-1.6.0.tar", last modified: Thu Oct 27 18:44:48 2022, max compression
+gzip compressed data, was "tamr_unify_client-1.7.0.tar", max compression
```

## Comparing `tamr-unify-client-1.6.0.tar` & `tamr_unify_client-1.7.0.tar`

### file list

```diff
@@ -1,96 +1,95 @@
--rw-r--r--   0        0        0    11334 2022-10-27 18:44:04.153097 tamr-unify-client-1.6.0/LICENSE
--rw-r--r--   0        0        0     1766 2022-10-27 18:44:04.153097 tamr-unify-client-1.6.0/README.md
--rw-r--r--   0        0        0     1403 2022-10-27 18:44:41.341325 tamr-unify-client-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     1407 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/__init__.py
--rw-r--r--   0        0        0      652 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_beta.py
--rw-r--r--   0        0        0     1002 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/__init__.py
--rw-r--r--   0        0        0     3632 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/attribute.py
--rw-r--r--   0        0        0     1983 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/auth.py
--rw-r--r--   0        0        0      354 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/backup.py
--rw-r--r--   0        0        0      958 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/dataset.py
--rw-r--r--   0        0        0      310 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/instance.py
--rw-r--r--   0        0        0      113 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/json.py
--rw-r--r--   0        0        0      430 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/operation.py
--rw-r--r--   0        0        0     2016 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/project.py
--rw-r--r--   0        0        0      370 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/restore.py
--rw-r--r--   0        0        0     2179 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/session.py
--rw-r--r--   0        0        0      421 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/transformations.py
--rw-r--r--   0        0        0      381 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/_types/url.py
--rw-r--r--   0        0        0      332 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/attribute/__init__.py
--rw-r--r--   0        0        0     7981 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/attribute/_attribute.py
--rw-r--r--   0        0        0      868 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/attribute/sub.py
--rw-r--r--   0        0        0     2567 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/attribute/type.py
--rw-r--r--   0        0        0     3944 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/backup.py
--rw-r--r--   0        0        0      340 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/categorization/__init__.py
--rw-r--r--   0        0        0     2694 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/categorization/_categorization.py
--rw-r--r--   0        0        0     1532 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/categorization/project.py
--rw-r--r--   0        0        0      279 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/dataset/__init__.py
--rw-r--r--   0        0        0     7205 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/dataset/_dataset.py
--rw-r--r--   0        0        0     6534 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/dataset/dataframe.py
--rw-r--r--   0        0        0     5982 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/dataset/record.py
--rw-r--r--   0        0        0     2743 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/dataset/unified.py
--rw-r--r--   0        0        0      100 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/exception.py
--rw-r--r--   0        0        0      255 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/golden_records/__init__.py
--rw-r--r--   0        0        0     1470 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/golden_records/_golden_records.py
--rw-r--r--   0        0        0      416 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/golden_records/project.py
--rw-r--r--   0        0        0      882 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/instance.py
--rw-r--r--   0        0        0      581 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/mastering/__init__.py
--rw-r--r--   0        0        0     4751 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/mastering/_mastering.py
--rw-r--r--   0        0        0     1486 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/mastering/project.py
--rw-r--r--   0        0        0     5616 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/operation.py
--rw-r--r--   0        0        0      326 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/primary_key.py
--rw-r--r--   0        0        0     6601 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/project.py
--rw-r--r--   0        0        0        0 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/py.typed
--rw-r--r--   0        0        0     1655 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/response.py
--rw-r--r--   0        0        0     2569 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/restore.py
--rw-r--r--   0        0        0      233 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/schema_mapping/__init__.py
--rw-r--r--   0        0        0      826 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/schema_mapping/_schema_mapping.py
--rw-r--r--   0        0        0     6112 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/schema_mapping/attribute_mapping.py
--rw-r--r--   0        0        0     1547 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/schema_mapping/project.py
--rw-r--r--   0        0        0      557 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/session.py
--rw-r--r--   0        0        0     3952 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_client/transformations.py
--rw-r--r--   0        0        0       76 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/__init__.py
--rw-r--r--   0        0        0     2083 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/_ignore_nan_encoder.py
--rw-r--r--   0        0        0     3945 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/attribute/collection.py
--rw-r--r--   0        0        0     6070 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/attribute/resource.py
--rw-r--r--   0        0        0     1271 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/attribute/subattribute.py
--rw-r--r--   0        0        0     4230 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/attribute/type.py
--rw-r--r--   0        0        0      199 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/auth/__init__.py
--rw-r--r--   0        0        0      882 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/auth/jwt_token.py
--rw-r--r--   0        0        0      406 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/auth/token.py
--rw-r--r--   0        0        0     1320 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/auth/username_password.py
--rw-r--r--   0        0        0     4688 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/base_collection.py
--rw-r--r--   0        0        0     1736 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/base_model.py
--rw-r--r--   0        0        0     1403 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/base_resource.py
--rw-r--r--   0        0        0     3979 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/categorization/category/collection.py
--rw-r--r--   0        0        0     4708 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/categorization/category/resource.py
--rw-r--r--   0        0        0     2057 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/categorization/project.py
--rw-r--r--   0        0        0     1003 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/categorization/taxonomy.py
--rw-r--r--   0        0        0     6992 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/client.py
--rw-r--r--   0        0        0     8539 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/dataset/collection.py
--rw-r--r--   0        0        0     2952 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/dataset/profile.py
--rw-r--r--   0        0        0    23440 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/dataset/resource.py
--rw-r--r--   0        0        0     1257 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/dataset/status.py
--rw-r--r--   0        0        0     1083 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/dataset/uri.py
--rw-r--r--   0        0        0     1117 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/dataset/usage.py
--rw-r--r--   0        0        0     1906 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/dataset/use.py
--rw-r--r--   0        0        0     1661 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/binning_model.py
--rw-r--r--   0        0        0     3021 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/estimated_pair_counts.py
--rw-r--r--   0        0        0    10995 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/project.py
--rw-r--r--   0        0        0     4821 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/configuration.py
--rw-r--r--   0        0        0      688 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/metric.py
--rw-r--r--   0        0        0     1691 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/record.py
--rw-r--r--   0        0        0      900 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/record_version.py
--rw-r--r--   0        0        0     1090 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/resource.py
--rw-r--r--   0        0        0     1274 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/version.py
--rw-r--r--   0        0        0     7940 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/operation.py
--rw-r--r--   0        0        0     3699 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/project/attribute_configuration/collection.py
--rw-r--r--   0        0        0     7891 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/project/attribute_configuration/resource.py
--rw-r--r--   0        0        0     3163 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/project/attribute_mapping/collection.py
--rw-r--r--   0        0        0     9294 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/project/attribute_mapping/resource.py
--rw-r--r--   0        0        0     3475 2022-10-27 18:44:04.157097 tamr-unify-client-1.6.0/tamr_unify_client/project/collection.py
--rw-r--r--   0        0        0    10418 2022-10-27 18:44:04.161097 tamr-unify-client-1.6.0/tamr_unify_client/project/resource.py
--rw-r--r--   0        0        0     2197 2022-10-27 18:44:04.161097 tamr-unify-client-1.6.0/tamr_unify_client/project/step.py
--rw-r--r--   0        0        0      722 2022-10-27 18:44:04.161097 tamr-unify-client-1.6.0/tamr_unify_client/response.py
--rw-r--r--   0        0        0     3200 2022-10-27 18:44:48.245280 tamr-unify-client-1.6.0/setup.py
--rw-r--r--   0        0        0     2817 2022-10-27 18:44:48.245740 tamr-unify-client-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-05-19 06:44:34.203274 tamr_unify_client-1.7.0/LICENSE
+-rw-r--r--   0        0        0     1719 2023-05-19 06:44:34.203274 tamr_unify_client-1.7.0/README.md
+-rw-r--r--   0        0        0     1359 2023-05-19 06:45:36.250232 tamr_unify_client-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1407 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/__init__.py
+-rw-r--r--   0        0        0      652 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_beta.py
+-rw-r--r--   0        0        0     1002 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/__init__.py
+-rw-r--r--   0        0        0     3632 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/attribute.py
+-rw-r--r--   0        0        0     1983 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/auth.py
+-rw-r--r--   0        0        0      354 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/backup.py
+-rw-r--r--   0        0        0      958 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/dataset.py
+-rw-r--r--   0        0        0      310 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/instance.py
+-rw-r--r--   0        0        0      113 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/json.py
+-rw-r--r--   0        0        0      430 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/operation.py
+-rw-r--r--   0        0        0     2016 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/project.py
+-rw-r--r--   0        0        0      370 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/restore.py
+-rw-r--r--   0        0        0     2179 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/session.py
+-rw-r--r--   0        0        0      421 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/transformations.py
+-rw-r--r--   0        0        0      381 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/_types/url.py
+-rw-r--r--   0        0        0      332 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/attribute/__init__.py
+-rw-r--r--   0        0        0     7981 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/attribute/_attribute.py
+-rw-r--r--   0        0        0      868 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/attribute/sub.py
+-rw-r--r--   0        0        0     2567 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/attribute/type.py
+-rw-r--r--   0        0        0     3934 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/backup.py
+-rw-r--r--   0        0        0      340 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/categorization/__init__.py
+-rw-r--r--   0        0        0     2694 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/categorization/_categorization.py
+-rw-r--r--   0        0        0     1532 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/categorization/project.py
+-rw-r--r--   0        0        0      279 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/dataset/__init__.py
+-rw-r--r--   0        0        0     7204 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/dataset/_dataset.py
+-rw-r--r--   0        0        0     6529 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/dataset/dataframe.py
+-rw-r--r--   0        0        0     5982 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/dataset/record.py
+-rw-r--r--   0        0        0     2743 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/dataset/unified.py
+-rw-r--r--   0        0        0      100 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/exception.py
+-rw-r--r--   0        0        0      255 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/golden_records/__init__.py
+-rw-r--r--   0        0        0     1470 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/golden_records/_golden_records.py
+-rw-r--r--   0        0        0      416 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/golden_records/project.py
+-rw-r--r--   0        0        0      882 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/instance.py
+-rw-r--r--   0        0        0      581 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/mastering/__init__.py
+-rw-r--r--   0        0        0     4751 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/mastering/_mastering.py
+-rw-r--r--   0        0        0     1486 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/mastering/project.py
+-rw-r--r--   0        0        0     5601 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/operation.py
+-rw-r--r--   0        0        0      326 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/primary_key.py
+-rw-r--r--   0        0        0     6601 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/project.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/py.typed
+-rw-r--r--   0        0        0     1655 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/response.py
+-rw-r--r--   0        0        0     2559 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/restore.py
+-rw-r--r--   0        0        0      233 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/schema_mapping/__init__.py
+-rw-r--r--   0        0        0      826 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/schema_mapping/_schema_mapping.py
+-rw-r--r--   0        0        0     6110 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/schema_mapping/attribute_mapping.py
+-rw-r--r--   0        0        0     1547 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/schema_mapping/project.py
+-rw-r--r--   0        0        0      557 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/session.py
+-rw-r--r--   0        0        0     3952 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_client/transformations.py
+-rw-r--r--   0        0        0       76 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/__init__.py
+-rw-r--r--   0        0        0     2060 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/_ignore_nan_encoder.py
+-rw-r--r--   0        0        0     3945 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/attribute/collection.py
+-rw-r--r--   0        0        0     6070 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/attribute/resource.py
+-rw-r--r--   0        0        0     1271 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/attribute/subattribute.py
+-rw-r--r--   0        0        0     4230 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/attribute/type.py
+-rw-r--r--   0        0        0      199 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/auth/__init__.py
+-rw-r--r--   0        0        0      882 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/auth/jwt_token.py
+-rw-r--r--   0        0        0      406 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/auth/token.py
+-rw-r--r--   0        0        0     1320 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/auth/username_password.py
+-rw-r--r--   0        0        0     4688 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/base_collection.py
+-rw-r--r--   0        0        0     1736 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/base_model.py
+-rw-r--r--   0        0        0     1403 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/base_resource.py
+-rw-r--r--   0        0        0     3978 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/categorization/category/collection.py
+-rw-r--r--   0        0        0     4708 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/categorization/category/resource.py
+-rw-r--r--   0        0        0     2057 2023-05-19 06:44:34.211274 tamr_unify_client-1.7.0/tamr_unify_client/categorization/project.py
+-rw-r--r--   0        0        0     1003 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/categorization/taxonomy.py
+-rw-r--r--   0        0        0     6956 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/client.py
+-rw-r--r--   0        0        0     8539 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/dataset/collection.py
+-rw-r--r--   0        0        0     2952 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/dataset/profile.py
+-rw-r--r--   0        0        0    23445 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/dataset/resource.py
+-rw-r--r--   0        0        0     1257 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/dataset/status.py
+-rw-r--r--   0        0        0     1083 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/dataset/uri.py
+-rw-r--r--   0        0        0     1117 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/dataset/usage.py
+-rw-r--r--   0        0        0     1906 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/dataset/use.py
+-rw-r--r--   0        0        0     1660 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/binning_model.py
+-rw-r--r--   0        0        0     3021 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/estimated_pair_counts.py
+-rw-r--r--   0        0        0    10995 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/project.py
+-rw-r--r--   0        0        0     4821 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/configuration.py
+-rw-r--r--   0        0        0      687 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/metric.py
+-rw-r--r--   0        0        0     1691 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/record.py
+-rw-r--r--   0        0        0      900 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/record_version.py
+-rw-r--r--   0        0        0     1090 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/resource.py
+-rw-r--r--   0        0        0     1274 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/version.py
+-rw-r--r--   0        0        0     7940 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/operation.py
+-rw-r--r--   0        0        0     3695 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/project/attribute_configuration/collection.py
+-rw-r--r--   0        0        0     7889 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/project/attribute_configuration/resource.py
+-rw-r--r--   0        0        0     3167 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/project/attribute_mapping/collection.py
+-rw-r--r--   0        0        0     9294 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/project/attribute_mapping/resource.py
+-rw-r--r--   0        0        0     3475 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/project/collection.py
+-rw-r--r--   0        0        0    10421 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/project/resource.py
+-rw-r--r--   0        0        0     2197 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/project/step.py
+-rw-r--r--   0        0        0      722 2023-05-19 06:44:34.215274 tamr_unify_client-1.7.0/tamr_unify_client/response.py
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 tamr_unify_client-1.7.0/PKG-INFO
```

### Comparing `tamr-unify-client-1.6.0/LICENSE` & `tamr_unify_client-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/README.md` & `tamr_unify_client-1.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -34,9 +34,8 @@
   - Generate predictions from trained models
 - 🔒 Authenticate with Tamr
 
 For more see the [official docs](https://tamr-client.readthedocs.io/en/stable/).
 
 ## Maintainers
 
-- [Pedro Cattori](https://github.com/pcattori)
 - [Samuel Kalish](https://github.com/skalish)
```

### Comparing `tamr-unify-client-1.6.0/pyproject.toml` & `tamr_unify_client-1.7.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 [tool.poetry]
 name = "tamr-unify-client"
-version = "1.6.0"
+version = "1.7.0"
 description = "Python Client for the Tamr API"
 license = "Apache-2.0"
-authors = ["Pedro Cattori <pedro.cattori@tamr.com>"]
+authors = ["Samuel Kalish <samuel.kalish@tamr.com>"]
 readme = "README.md"
 homepage = "https://tamr-client.readthedocs.io/en/stable/"
 repository = "https://github.com/Datatamer/tamr-client"
 keywords = ["tamr"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9"
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
 ]
 packages = [
     { include = "tamr_client" },
     { include = "tamr_unify_client" },
 ]
 include = ["tamr_client/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.6.1"
+python = "^3.7.1"
 requests = "^2.22"
-dataclasses = { version = "^0.6.0", python = "<3.7"}
+urllib3 = "<2"
 
 [tool.poetry.dev-dependencies]
 responses = "^0.10.6"
 flake8-import-order = "^0.18.1"
-flake8 = "^3.7"
-pytest = "^5.3.2"
-nox = "^2020.5.24"
+flake8 = "^5.0.0"
+pytest = "^7.2.0"
+nox = "^2022.11.21"
 pandas = "^1.0.5"
-black = {version = "^19.10b0", allow-prereleases = true}
-mypy = "^0.782"
+black = "^22.12.0"
+mypy = "^1.2.0"
+types-requests = "^2.30.0"
 
 [build-system]
-requires = ["poetry>=1.0"]
+requires = ["poetry>=1.4"]
 build-backend = "poetry.masonry.api"
```

### Comparing `tamr-unify-client-1.6.0/tamr_client/__init__.py` & `tamr_unify_client-1.7.0/tamr_client/__init__.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/_beta.py` & `tamr_unify_client-1.7.0/tamr_client/_beta.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/_types/__init__.py` & `tamr_unify_client-1.7.0/tamr_client/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/_types/attribute.py` & `tamr_unify_client-1.7.0/tamr_client/_types/attribute.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/_types/auth.py` & `tamr_unify_client-1.7.0/tamr_client/_types/auth.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/_types/dataset.py` & `tamr_unify_client-1.7.0/tamr_client/_types/dataset.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/_types/project.py` & `tamr_unify_client-1.7.0/tamr_client/_types/project.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/_types/session.py` & `tamr_unify_client-1.7.0/tamr_client/_types/session.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/attribute/_attribute.py` & `tamr_unify_client-1.7.0/tamr_client/attribute/_attribute.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/attribute/sub.py` & `tamr_unify_client-1.7.0/tamr_client/attribute/sub.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/attribute/type.py` & `tamr_unify_client-1.7.0/tamr_client/attribute/type.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/backup.py` & `tamr_unify_client-1.7.0/tamr_client/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 
 from tamr_client import Backup, response
 from tamr_client._types import Instance, JsonDict, Session, URL
 from tamr_client.exception import TamrClientException
 
 
 class InvalidOperation(TamrClientException):
-    """Raised when attempting an invalid operation.
-    """
+    """Raised when attempting an invalid operation."""
 
     pass
 
 
 class NotFound(TamrClientException):
-    """Raised when referencing a backup that does not exist on the server.
-    """
+    """Raised when referencing a backup that does not exist on the server."""
 
     pass
 
 
 def _from_json(url: URL, data: JsonDict) -> Backup:
     """Make backup from JSON data (deserialize).
```

### Comparing `tamr-unify-client-1.6.0/tamr_client/categorization/_categorization.py` & `tamr_unify_client-1.7.0/tamr_client/categorization/_categorization.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/categorization/project.py` & `tamr_unify_client-1.7.0/tamr_client/categorization/project.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/dataset/_dataset.py` & `tamr_unify_client-1.7.0/tamr_client/dataset/_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         dataset: A Tamr dataset which will be materialized
     """
     op = _materialize_async(session, dataset)
     return operation.wait(session, op)
 
 
 def _materialize_async(session: Session, dataset: Dataset) -> Operation:
-    r = session.post(str(dataset.url) + ":refresh",)
+    r = session.post(str(dataset.url) + ":refresh")
     return operation._from_response(dataset.url.instance, r)
 
 
 def delete(session: Session, dataset: Dataset, *, cascade: bool = False):
     """Deletes an existing dataset
 
     Sends a deletion request to the Tamr server
```

### Comparing `tamr-unify-client-1.6.0/tamr_client/dataset/dataframe.py` & `tamr_unify_client-1.7.0/tamr_client/dataset/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 BUILDING_DOCS = os.environ.get("TAMR_CLIENT_DOCS") == "1"
 if TYPE_CHECKING or BUILDING_DOCS:
     import pandas as pd
 
 
 class CreationFailure(TamrClientException):
-    """Raised when a dataset could not be created from a pandas DataFrame
-    """
+    """Raised when a dataset could not be created from a pandas DataFrame"""
 
     pass
 
 
 def upsert(
     session: Session,
     dataset: Dataset,
```

### Comparing `tamr-unify-client-1.6.0/tamr_client/dataset/record.py` & `tamr_unify_client-1.7.0/tamr_client/dataset/record.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/dataset/unified.py` & `tamr_unify_client-1.7.0/tamr_client/dataset/unified.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/golden_records/_golden_records.py` & `tamr_unify_client-1.7.0/tamr_client/golden_records/_golden_records.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/instance.py` & `tamr_unify_client-1.7.0/tamr_client/instance.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/mastering/__init__.py` & `tamr_unify_client-1.7.0/tamr_client/mastering/__init__.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/mastering/_mastering.py` & `tamr_unify_client-1.7.0/tamr_client/mastering/_mastering.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/mastering/project.py` & `tamr_unify_client-1.7.0/tamr_client/mastering/project.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/operation.py` & `tamr_unify_client-1.7.0/tamr_client/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 
 from tamr_client import response
 from tamr_client._types import Instance, JsonDict, Operation, Session, URL
 from tamr_client.exception import TamrClientException
 
 
 class NotFound(TamrClientException):
-    """Raised when referencing an operation that does not exist on the server.
-    """
+    """Raised when referencing an operation that does not exist on the server."""
 
     pass
 
 
 class Failed(TamrClientException):
-    """Raised when checking a failed operation.
-    """
+    """Raised when checking a failed operation."""
 
     pass
 
 
 def check(session: Session, operation: Operation):
     """Waits for the operation to finish and raises an exception if the operation was not successful.
 
@@ -82,16 +80,15 @@
         operation = poll(session, operation)
     raise TimeoutError(
         f"Waiting for operation took longer than {timeout_seconds} seconds."
     )
 
 
 def succeeded(operation: Operation) -> bool:
-    """Convenience method for checking if operation was successful.
-    """
+    """Convenience method for checking if operation was successful."""
     return operation.status is not None and operation.status["state"] == "SUCCEEDED"
 
 
 def by_resource_id(session: Session, instance: Instance, resource_id: str) -> Operation:
     """Get operation by ID
 
     Args:
```

### Comparing `tamr-unify-client-1.6.0/tamr_client/project.py` & `tamr_unify_client-1.7.0/tamr_client/project.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/response.py` & `tamr_unify_client-1.7.0/tamr_client/response.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/restore.py` & `tamr_unify_client-1.7.0/tamr_client/restore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from tamr_client import response, Restore
 from tamr_client._types import Instance, JsonDict, Session, URL
 from tamr_client.exception import TamrClientException
 
 
 class InvalidOperation(TamrClientException):
-    """Raised when attempting an invalid operation.
-    """
+    """Raised when attempting an invalid operation."""
 
     pass
 
 
 class NotFound(TamrClientException):
-    """Raised when referencing a restore that does not exist on the server.
-    """
+    """Raised when referencing a restore that does not exist on the server."""
 
     pass
 
 
 def _from_json(url: URL, data: JsonDict) -> Restore:
     """Make restore from JSON data (deserialize).
```

### Comparing `tamr-unify-client-1.6.0/tamr_client/schema_mapping/_schema_mapping.py` & `tamr_unify_client-1.7.0/tamr_client/schema_mapping/_schema_mapping.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/schema_mapping/attribute_mapping.py` & `tamr_unify_client-1.7.0/tamr_client/schema_mapping/attribute_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,18 +76,18 @@
 
     data = response.successful(r).json()
     instance = project.url.instance
     url = URL(instance=instance, path=data["relativeId"])
     return AttributeMapping(
         url,
         input_attribute=attribute._attribute._by_url(
-            session, URL(instance=instance, path=data["relativeInputAttributeId"]),
+            session, URL(instance=instance, path=data["relativeInputAttributeId"])
         ),
         unified_attribute=attribute._attribute._by_url(
-            session, URL(instance=instance, path=data["relativeUnifiedAttributeId"]),
+            session, URL(instance=instance, path=data["relativeUnifiedAttributeId"])
         ),
     )
 
 
 def get_all(session: Session, tamr_project: Project) -> List[AttributeMapping]:
     """Get all attribute mappings of a Tamr project
```

### Comparing `tamr-unify-client-1.6.0/tamr_client/schema_mapping/project.py` & `tamr_unify_client-1.7.0/tamr_client/schema_mapping/project.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/session.py` & `tamr_unify_client-1.7.0/tamr_client/session.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_client/transformations.py` & `tamr_unify_client-1.7.0/tamr_client/transformations.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/_ignore_nan_encoder.py` & `tamr_unify_client-1.7.0/tamr_unify_client/_ignore_nan_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         else:
             markers = None
         if self.ensure_ascii:
             _encoder = encode_basestring_ascii
         else:
             _encoder = encode_basestring
 
-        def floatstr(
-            o, _repr=float.__repr__, _inf=INFINITY, _neginf=-INFINITY,
-        ):
+        def floatstr(o, _repr=float.__repr__, _inf=INFINITY, _neginf=-INFINITY):
             if o != o or o == _inf or o == _neginf:
                 return "null"
             else:
                 return _repr(o)
 
         _iterencode = _make_iterencode(
             markers,
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/attribute/collection.py` & `tamr_unify_client-1.7.0/tamr_unify_client/attribute/collection.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/attribute/resource.py` & `tamr_unify_client-1.7.0/tamr_unify_client/attribute/resource.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/attribute/subattribute.py` & `tamr_unify_client-1.7.0/tamr_unify_client/attribute/subattribute.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/attribute/type.py` & `tamr_unify_client-1.7.0/tamr_unify_client/attribute/type.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/auth/jwt_token.py` & `tamr_unify_client-1.7.0/tamr_unify_client/auth/jwt_token.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/auth/username_password.py` & `tamr_unify_client-1.7.0/tamr_unify_client/auth/username_password.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/base_collection.py` & `tamr_unify_client-1.7.0/tamr_unify_client/base_collection.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/base_model.py` & `tamr_unify_client-1.7.0/tamr_unify_client/base_model.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/base_resource.py` & `tamr_unify_client-1.7.0/tamr_unify_client/base_resource.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/categorization/category/collection.py` & `tamr_unify_client-1.7.0/tamr_unify_client/categorization/category/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             >>>     do_stuff(category)
             >>> for category in collection: # implicit
             >>>     do_stuff(category)
         """
         return super().stream(Category)
 
     def create(self, creation_spec):
-        """ Creates a new category.
+        """Creates a new category.
 
         :param creation_spec: Category creation specification, formatted as specified in the
             `Public Docs for Creating a Category <https://docs.tamr.com/reference#create-a-category>`_.
         :type creation_spec: dict
         :return: The newly created category.
         :rtype: :class:`~tamr_unify_client.categorization.category.resource.Category`
         """
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/categorization/category/resource.py` & `tamr_unify_client-1.7.0/tamr_unify_client/categorization/category/resource.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/categorization/project.py` & `tamr_unify_client-1.7.0/tamr_unify_client/categorization/project.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/categorization/taxonomy.py` & `tamr_unify_client-1.7.0/tamr_unify_client/categorization/taxonomy.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/client.py` & `tamr_unify_client-1.7.0/tamr_unify_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,31 +116,27 @@
 
         logger.info(
             f"{response.request.method} {response.url} : {response.status_code}"
         )
         return response
 
     def get(self, endpoint, **kwargs):
-        """Calls :func:`~tamr_unify_client.Client.request` with the ``"GET"`` method.
-        """
+        """Calls :func:`~tamr_unify_client.Client.request` with the ``"GET"`` method."""
         return self.request("GET", endpoint, **kwargs)
 
     def post(self, endpoint, **kwargs):
-        """Calls :func:`~tamr_unify_client.Client.request` with the ``"POST"`` method.
-        """
+        """Calls :func:`~tamr_unify_client.Client.request` with the ``"POST"`` method."""
         return self.request("POST", endpoint, **kwargs)
 
     def put(self, endpoint, **kwargs):
-        """Calls :func:`~tamr_unify_client.Client.request` with the ``"PUT"`` method.
-        """
+        """Calls :func:`~tamr_unify_client.Client.request` with the ``"PUT"`` method."""
         return self.request("PUT", endpoint, **kwargs)
 
     def delete(self, endpoint, **kwargs):
-        """Calls :func:`~tamr_unify_client.Client.request` with the ``"DELETE"`` method.
-        """
+        """Calls :func:`~tamr_unify_client.Client.request` with the ``"DELETE"`` method."""
         return self.request("DELETE", endpoint, **kwargs)
 
     def set_auth_cookie(self):
         """Fetch and store an auth token for the given client configuration"""
         # Fetch auth token and store as cookie
         if not isinstance(self.auth, UsernamePasswordAuth):
             raise TypeError(
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/dataset/collection.py` & `tamr_unify_client-1.7.0/tamr_unify_client/dataset/collection.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/dataset/profile.py` & `tamr_unify_client-1.7.0/tamr_unify_client/dataset/profile.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/dataset/resource.py` & `tamr_unify_client-1.7.0/tamr_unify_client/dataset/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,19 +589,19 @@
         :rtype: :class:`~tamr_unify_client.dataset.resource.DatasetSpec`
         """
         return self.from_data({**self._data, "description": new_description})
 
     def with_key_attribute_names(self, new_key_attribute_names):
         """Creates a new spec with the same properties, updating key attribute names.
 
-       :param new_key_attribute_names: The new key attribute names.
-       :type new_key_attribute_names: list[str]
-       :return: A new spec.
-       :rtype: :class:`~tamr_unify_client.dataset.resource.DatasetSpec`
-       """
+        :param new_key_attribute_names: The new key attribute names.
+        :type new_key_attribute_names: list[str]
+        :return: A new spec.
+        :rtype: :class:`~tamr_unify_client.dataset.resource.DatasetSpec`
+        """
         return self.from_data(
             {**self._data, "keyAttributeNames": new_key_attribute_names}
         )
 
     def with_tags(self, new_tags):
         """Creates a new spec with the same properties, updating tags.
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/dataset/status.py` & `tamr_unify_client-1.7.0/tamr_unify_client/dataset/status.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/dataset/uri.py` & `tamr_unify_client-1.7.0/tamr_unify_client/dataset/uri.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/dataset/usage.py` & `tamr_unify_client-1.7.0/tamr_unify_client/dataset/usage.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/dataset/use.py` & `tamr_unify_client-1.7.0/tamr_unify_client/dataset/use.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/binning_model.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/binning_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 from tamr_unify_client.base_resource import BaseResource
 
 
 class BinningModel(BaseResource):
-    """ A binning model object."""
+    """A binning model object."""
 
     @classmethod
     def from_json(cls, client, resource_json, api_path=None):
         return super().from_data(client, resource_json, api_path)
 
     def records(self):
         """Stream this object's records as Python dictionaries.
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/estimated_pair_counts.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/estimated_pair_counts.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/project.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/project.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/configuration.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/configuration.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/metric.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 class Metric:
-    """ A metric for a published cluster.
+    """A metric for a published cluster.
 
     This is not a `BaseResource` because it does not have its own API endpoint.
 
     :param data: The JSON entity representing this cluster.
     """
 
     def __init__(self, data):
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/record.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/record.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/record_version.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/record_version.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/resource.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/resource.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/mastering/published_cluster/version.py` & `tamr_unify_client-1.7.0/tamr_unify_client/mastering/published_cluster/version.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/operation.py` & `tamr_unify_client-1.7.0/tamr_unify_client/operation.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/project/attribute_configuration/collection.py` & `tamr_unify_client-1.7.0/tamr_unify_client/project/attribute_configuration/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,19 @@
         :rtype: :class:`~tamr_unify_client.project.attribute_configuration.resource.AttributeConfiguration`
         """
         return super().by_resource_id(self.api_path, resource_id)
 
     def by_relative_id(self, relative_id):
         """Retrieve an attribute configuration by relative ID.
 
-       :param relative_id: The relative ID.
-       :type relative_id: str
-       :returns: The specified attribute configuration.
-       :rtype: :class:`~tamr_unify_client.project.attribute_configuration.resource.AttributeConfiguration`
-       """
+        :param relative_id: The relative ID.
+        :type relative_id: str
+        :returns: The specified attribute configuration.
+        :rtype: :class:`~tamr_unify_client.project.attribute_configuration.resource.AttributeConfiguration`
+        """
         return super().by_relative_id(AttributeConfiguration, relative_id)
 
     def by_external_id(self, external_id):
         """Retrieve an attribute configuration by external ID.
 
         Since attributes do not have external IDs, this method is not supported and will
         raise a :class:`NotImplementedError` .
@@ -48,25 +48,25 @@
         :raises LookupError: If multiple attributes with the specified external_id are found
         :raises NotImplementedError: AttributeConfiguration does not support external_id
         """
         raise NotImplementedError("AttributeConfiguration does not support external_id")
 
     def stream(self):
         """Stream attribute configurations in this collection. Implicitly called when iterating
-         over this collection.
+        over this collection.
 
-         :returns: Stream of attribute configurations.
-         :rtype: Python generator yielding :class:`~tamr_unify_client.project.attribute_configuration.resource.AttributeConfiguration`
+        :returns: Stream of attribute configurations.
+        :rtype: Python generator yielding :class:`~tamr_unify_client.project.attribute_configuration.resource.AttributeConfiguration`
 
-         Usage:
-             >>> for attributeConfiguration in collection.stream(): # explicit
-             >>>     do_stuff(attributeConfiguration)
-             >>> for attributeConfiguration in collection: # implicit
-             >>>     do_stuff(attributeConfiguration)
-         """
+        Usage:
+            >>> for attributeConfiguration in collection.stream(): # explicit
+            >>>     do_stuff(attributeConfiguration)
+            >>> for attributeConfiguration in collection: # implicit
+            >>>     do_stuff(attributeConfiguration)
+        """
 
         return super().stream(AttributeConfiguration)
 
     def create(self, creation_spec):
         """Create an Attribute configuration in this collection
 
         :param creation_spec: Attribute configuration creation specification should be formatted as specified in the
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/project/attribute_configuration/resource.py` & `tamr_unify_client-1.7.0/tamr_unify_client/project/attribute_configuration/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from tamr_unify_client.base_resource import BaseResource
 
 
 class AttributeConfiguration(BaseResource):
     """The configurations of Tamr Attributes.
 
-   See https://docs.tamr.com/reference#the-attribute-configuration-object
-   """
+    See https://docs.tamr.com/reference#the-attribute-configuration-object
+    """
 
     @classmethod
     def from_json(
         cls, client, resource_json, api_path=None
     ) -> "AttributeConfiguration":
         return super().from_data(client, resource_json, api_path)
 
@@ -48,28 +48,28 @@
     @property
     def tokenizer(self):
         """:type: str"""
         return self._data.get("tokenizer")
 
     @property
     def numeric_field_resolution(self):
-        """:type: list """
+        """:type: list"""
         return self._data.get("numericFieldResolution")
 
     @property
     def attribute_name(self):
         """:type: str"""
         return self._data.get("attributeName")
 
     def spec(self):
         """Returns this attribute configuration's spec.
 
-         :return: The spec of this attribute configuration.
-         :rtype: :class:`~tamr_unify_client.project.attribute_configuration.resource.AttributeConfigurationSpec`
-         """
+        :return: The spec of this attribute configuration.
+        :rtype: :class:`~tamr_unify_client.project.attribute_configuration.resource.AttributeConfigurationSpec`
+        """
         return AttributeConfigurationSpec.of(self)
 
     def __repr__(self):
         return (
             f"{self.__class__.__module__}."
             f"{self.__class__.__qualname__}("
             f"relative_id={self.relative_id!r}, "
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/project/attribute_mapping/collection.py` & `tamr_unify_client-1.7.0/tamr_unify_client/project/attribute_mapping/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,19 +39,19 @@
             if resource_id == split_id:
                 return mapping
         raise LookupError("cannot locate mapping from resource ID")
 
     def by_relative_id(self, relative_id):
         """Retrieve an item in this collection by relative ID.
 
-       :param relative_id: The relative ID.
-       :type relative_id: str
-       :returns: The specified attribute mapping.
-       :rtype: :class:`~tamr_unify_client.project.attribute_mapping.resource.AttributeMapping`
-       """
+        :param relative_id: The relative ID.
+        :type relative_id: str
+        :returns: The specified attribute mapping.
+        :rtype: :class:`~tamr_unify_client.project.attribute_mapping.resource.AttributeMapping`
+        """
         resource_id = relative_id.split("attributeMappings/")[1]
         return self.by_resource_id(resource_id)
 
     def create(self, creation_spec):
         """Create an Attribute mapping in this collection
 
         :param creation_spec: Attribute mapping creation specification should be formatted as specified in the
@@ -66,11 +66,11 @@
     def delete_by_resource_id(self, resource_id):
         """Delete an attribute mapping using its Resource ID.
 
         :param resource_id: the resource ID of the mapping to be deleted.
         :type resource_id: str
         :returns: HTTP response from the server
         :rtype: :class:`requests.Response`
-         """
+        """
         path = self.api_path + "/" + resource_id
         response = self.client.delete(path).successful()
         return response
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/project/attribute_mapping/resource.py` & `tamr_unify_client-1.7.0/tamr_unify_client/project/attribute_mapping/resource.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/project/collection.py` & `tamr_unify_client-1.7.0/tamr_unify_client/project/collection.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/project/resource.py` & `tamr_unify_client-1.7.0/tamr_unify_client/project/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,17 +144,17 @@
         alias = self.api_path + "/attributeConfigurations"
         info = AttributeConfigurationCollection(self.client, api_path=alias)
         return info
 
     def attribute_mappings(self):
         """Project's attribute's mappings.
 
-       :returns: The attribute mappings of a project.
-       :rtype: :class:`~tamr_unify_client.project.attribute_mapping.collection.AttributeMappingCollection`
-       """
+        :returns: The attribute mappings of a project.
+        :rtype: :class:`~tamr_unify_client.project.attribute_mapping.collection.AttributeMappingCollection`
+        """
         alias = self.api_path + "/attributeMappings"
         info = AttributeMappingCollection(self.client, alias)
         return info
 
     def spec(self):
         """Returns this project's spec.
```

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/project/step.py` & `tamr_unify_client-1.7.0/tamr_unify_client/project/step.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/tamr_unify_client/response.py` & `tamr_unify_client-1.7.0/tamr_unify_client/response.py`

 * *Files identical despite different names*

### Comparing `tamr-unify-client-1.6.0/PKG-INFO` & `tamr_unify_client-1.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: tamr-unify-client
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python Client for the Tamr API
 Home-page: https://tamr-client.readthedocs.io/en/stable/
 License: Apache-2.0
 Keywords: tamr
-Author: Pedro Cattori
-Author-email: pedro.cattori@tamr.com
-Requires-Python: >=3.6.1,<4.0.0
+Author: Samuel Kalish
+Author-email: samuel.kalish@tamr.com
+Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: dataclasses (>=0.6.0,<0.7.0); python_version < "3.7"
 Requires-Dist: requests (>=2.22,<3.0)
+Requires-Dist: urllib3 (<2)
 Project-URL: Repository, https://github.com/Datatamer/tamr-client
 Description-Content-Type: text/markdown
 
 # Python Client
 Programmatically 💻 interact with Tamr using Python 🐍
 
 [![Version](https://img.shields.io/pypi/v/tamr-unify-client.svg?style=flat-square)](https://pypi.org/project/tamr-unify-client/)
@@ -60,10 +65,9 @@
   - Generate predictions from trained models
 - 🔒 Authenticate with Tamr
 
 For more see the [official docs](https://tamr-client.readthedocs.io/en/stable/).
 
 ## Maintainers
 
-- [Pedro Cattori](https://github.com/pcattori)
 - [Samuel Kalish](https://github.com/skalish)
```

