# Comparing `tmp/patch-cli-0.2.5.tar.gz` & `tmp/patch-cli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patch-cli-0.2.5.tar", last modified: Thu Mar  2 16:10:23 2023, max compression
+gzip compressed data, was "patch-cli-0.2.6.tar", last modified: Wed Apr 26 16:59:15 2023, max compression
```

## Comparing `patch-cli-0.2.5.tar` & `patch-cli-0.2.6.tar`

### file list

```diff
@@ -1,119 +1,133 @@
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.147271 patch-cli-0.2.5/
--rw-r--r--   0 gunner     (501) staff       (20)      655 2023-01-12 18:07:47.000000 patch-cli-0.2.5/.pat-complete.fish
--rw-r--r--   0 gunner     (501) staff       (20)      654 2023-01-12 18:07:47.000000 patch-cli-0.2.5/.pat-complete.sh
--rw-r--r--   0 gunner     (501) staff       (20)      946 2023-01-12 18:07:47.000000 patch-cli-0.2.5/.pat-complete.zsh
--rw-r--r--   0 gunner     (501) staff       (20)     9304 2023-01-12 18:07:47.000000 patch-cli-0.2.5/LICENSE.md
--rw-r--r--   0 gunner     (501) staff       (20)      159 2023-02-13 19:38:49.000000 patch-cli-0.2.5/MANIFEST.in
--rw-r--r--   0 gunner     (501) staff       (20)     3732 2023-03-02 16:10:23.147527 patch-cli-0.2.5/PKG-INFO
--rw-r--r--   0 gunner     (501) staff       (20)     2653 2023-02-27 17:45:34.000000 patch-cli-0.2.5/README.md
--rw-r--r--   0 gunner     (501) staff       (20)        6 2023-03-02 16:10:09.000000 patch-cli-0.2.5/VERSION
--rw-r--r--   0 gunner     (501) staff       (20)       19 2023-01-12 18:07:47.000000 patch-cli-0.2.5/pat.bat
--rw-r--r--   0 gunner     (501) staff       (20)      963 2023-01-12 18:07:47.000000 patch-cli-0.2.5/pat.py
--rw-r--r--   0 gunner     (501) staff       (20)       91 2023-02-13 19:37:47.000000 patch-cli-0.2.5/pyproject.toml
--rw-r--r--   0 gunner     (501) staff       (20)     1580 2023-03-02 16:10:23.147933 patch-cli-0.2.5/setup.cfg
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.124504 patch-cli-0.2.5/src/
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.127440 patch-cli-0.2.5/src/patch/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/__init__.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.128276 patch-cli-0.2.5/src/patch/auth/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/auth/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     5131 2023-02-23 16:39:57.000000 patch-cli-0.2.5/src/patch/auth/auth_client.py
--rw-r--r--   0 gunner     (501) staff       (20)     2853 2023-02-23 16:39:57.000000 patch-cli-0.2.5/src/patch/auth/auth_forms.py
--rw-r--r--   0 gunner     (501) staff       (20)     1762 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/auth/auth_token.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.129471 patch-cli-0.2.5/src/patch/cli/
--rw-r--r--   0 gunner     (501) staff       (20)     1364 2023-02-14 17:40:04.000000 patch-cli-0.2.5/src/patch/cli/__init__.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.132219 patch-cli-0.2.5/src/patch/cli/commands/
--rw-r--r--   0 gunner     (501) staff       (20)     2262 2023-01-17 11:15:41.000000 patch-cli-0.2.5/src/patch/cli/commands/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     4476 2023-02-27 17:45:34.000000 patch-cli-0.2.5/src/patch/cli/commands/access.py
--rw-r--r--   0 gunner     (501) staff       (20)     8682 2023-03-02 16:09:57.000000 patch-cli-0.2.5/src/patch/cli/commands/admin.py
--rw-r--r--   0 gunner     (501) staff       (20)     2818 2023-02-22 23:51:16.000000 patch-cli-0.2.5/src/patch/cli/commands/connector.py
--rw-r--r--   0 gunner     (501) staff       (20)    22544 2023-03-01 17:45:31.000000 patch-cli-0.2.5/src/patch/cli/commands/dataset.py
--rw-r--r--   0 gunner     (501) staff       (20)     1293 2023-02-23 16:39:57.000000 patch-cli-0.2.5/src/patch/cli/commands/login.py
--rw-r--r--   0 gunner     (501) staff       (20)     1783 2023-01-17 11:15:41.000000 patch-cli-0.2.5/src/patch/cli/commands/playground.py
--rw-r--r--   0 gunner     (501) staff       (20)     5732 2023-03-01 17:45:31.000000 patch-cli-0.2.5/src/patch/cli/commands/source.py
--rw-r--r--   0 gunner     (501) staff       (20)      886 2023-01-17 11:15:41.000000 patch-cli-0.2.5/src/patch/cli/commands/token.py
--rw-r--r--   0 gunner     (501) staff       (20)     1901 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/commands/user.py
--rw-r--r--   0 gunner     (501) staff       (20)      232 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/eap.py
--rw-r--r--   0 gunner     (501) staff       (20)     1244 2023-01-17 11:15:41.000000 patch-cli-0.2.5/src/patch/cli/patch_click_context.py
--rw-r--r--   0 gunner     (501) staff       (20)      446 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/phone_number_param_type.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.132741 patch-cli-0.2.5/src/patch/cli/remote/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/remote/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      670 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/remote/dataset_client.py
--rw-r--r--   0 gunner     (501) staff       (20)      542 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/remote/source_client.py
--rw-r--r--   0 gunner     (501) staff       (20)     2122 2023-03-01 17:45:31.000000 patch-cli-0.2.5/src/patch/cli/styled.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.134138 patch-cli-0.2.5/src/patch/cli/tools/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      365 2023-02-28 00:12:05.000000 patch-cli-0.2.5/src/patch/cli/tools/base64_encryption.py
--rw-r--r--   0 gunner     (501) staff       (20)     1217 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/config_spec.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.135195 patch-cli-0.2.5/src/patch/cli/tools/connectors/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/connectors/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     5326 2023-02-28 00:43:51.000000 patch-cli-0.2.5/src/patch/cli/tools/connectors/connector_spec.py
--rw-r--r--   0 gunner     (501) staff       (20)     3874 2023-02-23 22:43:56.000000 patch-cli-0.2.5/src/patch/cli/tools/connectors/source_config.py
--rw-r--r--   0 gunner     (501) staff       (20)     1280 2023-02-22 23:51:16.000000 patch-cli-0.2.5/src/patch/cli/tools/connectors/source_config_interactive.py
--rw-r--r--   0 gunner     (501) staff       (20)     1084 2023-02-22 23:51:16.000000 patch-cli-0.2.5/src/patch/cli/tools/connectors/source_config_non_interactive.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.136128 patch-cli-0.2.5/src/patch/cli/tools/datasets/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/datasets/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     1011 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/datasets/curl_renderer.py
--rw-r--r--   0 gunner     (501) staff       (20)     5153 2023-02-27 17:45:34.000000 patch-cli-0.2.5/src/patch/cli/tools/datasets/endpoint_renderer.py
--rw-r--r--   0 gunner     (501) staff       (20)     2069 2023-03-01 16:12:11.000000 patch-cli-0.2.5/src/patch/cli/tools/datasets/row_table_renderer.py
--rw-r--r--   0 gunner     (501) staff       (20)      729 2023-02-22 23:51:16.000000 patch-cli-0.2.5/src/patch/cli/tools/field_spec.py
--rw-r--r--   0 gunner     (501) staff       (20)      352 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/filters_reader.py
--rw-r--r--   0 gunner     (501) staff       (20)      456 2023-01-13 17:10:04.000000 patch-cli-0.2.5/src/patch/cli/tools/json_reader.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.137564 patch-cli-0.2.5/src/patch/cli/tools/tables/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/__init__.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.140483 patch-cli-0.2.5/src/patch/cli/tools/tables/components/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     1064 2023-01-18 15:21:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/container_panel.py
--rw-r--r--   0 gunner     (501) staff       (20)     2693 2023-02-27 17:45:34.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/hierarchy_renderer.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.140959 patch-cli-0.2.5/src/patch/cli/tools/tables/components/list_tools/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/list_tools/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     1643 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/list_tools/data_list.py
--rw-r--r--   0 gunner     (501) staff       (20)     2093 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_quota.py
--rw-r--r--   0 gunner     (501) staff       (20)      309 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_search.py
--rw-r--r--   0 gunner     (501) staff       (20)     1458 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_summary.py
--rw-r--r--   0 gunner     (501) staff       (20)     3748 2023-02-27 17:45:34.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular.py
--rw-r--r--   0 gunner     (501) staff       (20)      470 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_all_in.py
--rw-r--r--   0 gunner     (501) staff       (20)      904 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_appendable.py
--rw-r--r--   0 gunner     (501) staff       (20)      949 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_positional.py
--rw-r--r--   0 gunner     (501) staff       (20)     1699 2023-01-30 13:11:07.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_positional_hierarchy.py
--rw-r--r--   0 gunner     (501) staff       (20)     1500 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_with_columns.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.141651 patch-cli-0.2.5/src/patch/cli/tools/tables/components/viewport/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/viewport/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     4760 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/viewport/cursor_controller.py
--rw-r--r--   0 gunner     (501) staff       (20)     3321 2023-01-19 15:51:24.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/components/viewport/viewport.py
--rw-r--r--   0 gunner     (501) staff       (20)      462 2023-01-20 14:13:36.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/renders.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.143487 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      962 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/columns_row_collection.py
--rw-r--r--   0 gunner     (501) staff       (20)      431 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/panel_tabular_row.py
--rw-r--r--   0 gunner     (501) staff       (20)      583 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/row_collection.py
--rw-r--r--   0 gunner     (501) staff       (20)     1187 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/table_data_row.py
--rw-r--r--   0 gunner     (501) staff       (20)     1149 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/table_row_collection.py
--rw-r--r--   0 gunner     (501) staff       (20)      266 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/table_row_collection_quota_aware.py
--rw-r--r--   0 gunner     (501) staff       (20)     1371 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py
--rw-r--r--   0 gunner     (501) staff       (20)      423 2023-03-01 17:45:31.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/source_app.css
--rw-r--r--   0 gunner     (501) staff       (20)     4362 2023-03-01 17:45:31.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/source_app.py
--rw-r--r--   0 gunner     (501) staff       (20)      344 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/source_data.py
--rw-r--r--   0 gunner     (501) staff       (20)     3983 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/source_metadata_client.py
--rw-r--r--   0 gunner     (501) staff       (20)     5602 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/cli/tools/tables/state_manager.py
--rw-r--r--   0 gunner     (501) staff       (20)      187 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/debug.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.144227 patch-cli-0.2.5/src/patch/gql/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/gql/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)     3059 2023-02-27 17:45:34.000000 patch-cli-0.2.5/src/patch/gql/client.py
--rw-r--r--   0 gunner     (501) staff       (20)    12020 2023-02-23 16:39:57.000000 patch-cli-0.2.5/src/patch/gql/schema.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.145788 patch-cli-0.2.5/src/patch/storage/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/storage/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      391 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/storage/auth.py
--rw-r--r--   0 gunner     (501) staff       (20)      148 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/storage/generic_payload.py
--rw-r--r--   0 gunner     (501) staff       (20)      955 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/storage/generic_storage_file.py
--rw-r--r--   0 gunner     (501) staff       (20)      398 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/storage/state_file.py
--rw-r--r--   0 gunner     (501) staff       (20)     1471 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/storage/storage.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.146342 patch-cli-0.2.5/src/patch/tp/
--rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/tp/__init__.py
--rw-r--r--   0 gunner     (501) staff       (20)      232 2023-01-12 18:07:47.000000 patch-cli-0.2.5/src/patch/tp/phone_number.py
-drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-03-02 16:10:23.147175 patch-cli-0.2.5/src/patch_cli.egg-info/
--rw-r--r--   0 gunner     (501) staff       (20)     3732 2023-03-02 16:10:23.000000 patch-cli-0.2.5/src/patch_cli.egg-info/PKG-INFO
--rw-r--r--   0 gunner     (501) staff       (20)     3916 2023-03-02 16:10:23.000000 patch-cli-0.2.5/src/patch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 gunner     (501) staff       (20)        1 2023-03-02 16:10:23.000000 patch-cli-0.2.5/src/patch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 gunner     (501) staff       (20)       44 2023-03-02 16:10:23.000000 patch-cli-0.2.5/src/patch_cli.egg-info/entry_points.txt
--rw-r--r--   0 gunner     (501) staff       (20)      236 2023-03-02 16:10:23.000000 patch-cli-0.2.5/src/patch_cli.egg-info/requires.txt
--rw-r--r--   0 gunner     (501) staff       (20)        6 2023-03-02 16:10:23.000000 patch-cli-0.2.5/src/patch_cli.egg-info/top_level.txt
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.893526 patch-cli-0.2.6/
+-rw-r--r--   0 gunner     (501) staff       (20)      655 2023-01-12 18:07:47.000000 patch-cli-0.2.6/.pat-complete.fish
+-rw-r--r--   0 gunner     (501) staff       (20)      654 2023-01-12 18:07:47.000000 patch-cli-0.2.6/.pat-complete.sh
+-rw-r--r--   0 gunner     (501) staff       (20)      946 2023-01-12 18:07:47.000000 patch-cli-0.2.6/.pat-complete.zsh
+-rw-r--r--   0 gunner     (501) staff       (20)     9304 2023-01-12 18:07:47.000000 patch-cli-0.2.6/LICENSE.md
+-rw-r--r--   0 gunner     (501) staff       (20)      159 2023-02-13 19:38:49.000000 patch-cli-0.2.6/MANIFEST.in
+-rw-r--r--   0 gunner     (501) staff       (20)     3732 2023-04-26 16:59:15.893638 patch-cli-0.2.6/PKG-INFO
+-rw-r--r--   0 gunner     (501) staff       (20)     2653 2023-02-27 17:45:34.000000 patch-cli-0.2.6/README.md
+-rw-r--r--   0 gunner     (501) staff       (20)        6 2023-04-26 16:48:54.000000 patch-cli-0.2.6/VERSION
+-rw-r--r--   0 gunner     (501) staff       (20)       19 2023-01-12 18:07:47.000000 patch-cli-0.2.6/pat.bat
+-rw-r--r--   0 gunner     (501) staff       (20)      963 2023-01-12 18:07:47.000000 patch-cli-0.2.6/pat.py
+-rw-r--r--   0 gunner     (501) staff       (20)       91 2023-02-13 19:37:47.000000 patch-cli-0.2.6/pyproject.toml
+-rw-r--r--   0 gunner     (501) staff       (20)     1580 2023-04-26 16:59:15.894014 patch-cli-0.2.6/setup.cfg
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.869123 patch-cli-0.2.6/src/
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.871875 patch-cli-0.2.6/src/patch/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/__init__.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.872773 patch-cli-0.2.6/src/patch/auth/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/auth/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5088 2023-04-06 22:23:48.000000 patch-cli-0.2.6/src/patch/auth/auth_client.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2852 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/auth/auth_forms.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1820 2023-04-12 15:20:57.000000 patch-cli-0.2.6/src/patch/auth/auth_token.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.874080 patch-cli-0.2.6/src/patch/cli/
+-rw-r--r--   0 gunner     (501) staff       (20)     1684 2023-04-19 14:52:13.000000 patch-cli-0.2.6/src/patch/cli/__init__.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.877563 patch-cli-0.2.6/src/patch/cli/commands/
+-rw-r--r--   0 gunner     (501) staff       (20)     2262 2023-01-17 11:15:41.000000 patch-cli-0.2.6/src/patch/cli/commands/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     4476 2023-02-27 17:45:34.000000 patch-cli-0.2.6/src/patch/cli/commands/access.py
+-rw-r--r--   0 gunner     (501) staff       (20)     8684 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/cli/commands/admin.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.878157 patch-cli-0.2.6/src/patch/cli/commands/alpha/
+-rw-r--r--   0 gunner     (501) staff       (20)      231 2023-04-19 14:52:13.000000 patch-cli-0.2.6/src/patch/cli/commands/alpha/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      299 2023-04-19 14:52:13.000000 patch-cli-0.2.6/src/patch/cli/commands/alpha/package.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2821 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/cli/commands/connector.py
+-rw-r--r--   0 gunner     (501) staff       (20)    25166 2023-04-19 14:52:13.000000 patch-cli-0.2.6/src/patch/cli/commands/dataset.py
+-rw-r--r--   0 gunner     (501) staff       (20)     4336 2023-04-26 16:58:27.000000 patch-cli-0.2.6/src/patch/cli/commands/destination.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3058 2023-04-12 15:20:59.000000 patch-cli-0.2.6/src/patch/cli/commands/login.py
+-rw-r--r--   0 gunner     (501) staff       (20)      511 2023-04-12 15:20:57.000000 patch-cli-0.2.6/src/patch/cli/commands/logout.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1800 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/cli/commands/playground.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5838 2023-04-26 16:58:27.000000 patch-cli-0.2.6/src/patch/cli/commands/source.py
+-rw-r--r--   0 gunner     (501) staff       (20)      886 2023-01-17 11:15:41.000000 patch-cli-0.2.6/src/patch/cli/commands/token.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1901 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/commands/user.py
+-rw-r--r--   0 gunner     (501) staff       (20)      232 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/eap.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1244 2023-01-17 11:15:41.000000 patch-cli-0.2.6/src/patch/cli/patch_click_context.py
+-rw-r--r--   0 gunner     (501) staff       (20)      446 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/phone_number_param_type.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.878742 patch-cli-0.2.6/src/patch/cli/remote/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/remote/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      670 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/remote/dataset_client.py
+-rw-r--r--   0 gunner     (501) staff       (20)      542 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/remote/source_client.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2122 2023-03-01 17:45:31.000000 patch-cli-0.2.6/src/patch/cli/styled.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.880662 patch-cli-0.2.6/src/patch/cli/tools/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      368 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/cli/tools/base64_encryption.py
+-rw-r--r--   0 gunner     (501) staff       (20)     4488 2023-04-26 16:58:27.000000 patch-cli-0.2.6/src/patch/cli/tools/config.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1314 2023-04-19 20:57:35.000000 patch-cli-0.2.6/src/patch/cli/tools/config_interactive.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1207 2023-04-19 16:48:56.000000 patch-cli-0.2.6/src/patch/cli/tools/config_spec.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.881246 patch-cli-0.2.6/src/patch/cli/tools/connectors/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/connectors/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5960 2023-04-25 14:24:05.000000 patch-cli-0.2.6/src/patch/cli/tools/connectors/connector_spec.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1054 2023-04-26 16:58:27.000000 patch-cli-0.2.6/src/patch/cli/tools/connectors/source_config_non_interactive.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.882048 patch-cli-0.2.6/src/patch/cli/tools/datasets/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/datasets/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1011 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/datasets/curl_renderer.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5655 2023-04-06 22:16:46.000000 patch-cli-0.2.6/src/patch/cli/tools/datasets/endpoint_renderer.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2069 2023-03-01 16:12:11.000000 patch-cli-0.2.6/src/patch/cli/tools/datasets/row_table_renderer.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.882467 patch-cli-0.2.6/src/patch/cli/tools/destinations/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-04-19 21:08:16.000000 patch-cli-0.2.6/src/patch/cli/tools/destinations/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3383 2023-04-19 19:13:42.000000 patch-cli-0.2.6/src/patch/cli/tools/destinations/destination_spec.py
+-rw-r--r--   0 gunner     (501) staff       (20)      730 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/cli/tools/field_spec.py
+-rw-r--r--   0 gunner     (501) staff       (20)      352 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/filters_reader.py
+-rw-r--r--   0 gunner     (501) staff       (20)      456 2023-01-13 17:10:04.000000 patch-cli-0.2.6/src/patch/cli/tools/json_reader.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.883405 patch-cli-0.2.6/src/patch/cli/tools/state/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-04-12 15:20:57.000000 patch-cli-0.2.6/src/patch/cli/tools/state/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      299 2023-04-12 15:20:59.000000 patch-cli-0.2.6/src/patch/cli/tools/state/auth_state_transfer.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1257 2023-04-12 15:20:57.000000 patch-cli-0.2.6/src/patch/cli/tools/state/bi_directional_state_transfer.py
+-rw-r--r--   0 gunner     (501) staff       (20)      612 2023-04-12 15:20:57.000000 patch-cli-0.2.6/src/patch/cli/tools/state/state_transfer.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.885006 patch-cli-0.2.6/src/patch/cli/tools/tables/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/__init__.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.887508 patch-cli-0.2.6/src/patch/cli/tools/tables/components/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1064 2023-01-18 15:21:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/container_panel.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2693 2023-02-27 17:45:34.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/hierarchy_renderer.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.887796 patch-cli-0.2.6/src/patch/cli/tools/tables/components/list_tools/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/list_tools/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1643 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/list_tools/data_list.py
+-rw-r--r--   0 gunner     (501) staff       (20)     2093 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_quota.py
+-rw-r--r--   0 gunner     (501) staff       (20)      309 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_search.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1458 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_summary.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3748 2023-02-27 17:45:34.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular.py
+-rw-r--r--   0 gunner     (501) staff       (20)      470 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_all_in.py
+-rw-r--r--   0 gunner     (501) staff       (20)      904 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_appendable.py
+-rw-r--r--   0 gunner     (501) staff       (20)      949 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_positional.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1699 2023-01-30 13:11:07.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_positional_hierarchy.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1500 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_with_columns.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.888285 patch-cli-0.2.6/src/patch/cli/tools/tables/components/viewport/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/viewport/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     4760 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/viewport/cursor_controller.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3321 2023-01-19 15:51:24.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/components/viewport/viewport.py
+-rw-r--r--   0 gunner     (501) staff       (20)      478 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/renders.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.889721 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      962 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/columns_row_collection.py
+-rw-r--r--   0 gunner     (501) staff       (20)      431 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/panel_tabular_row.py
+-rw-r--r--   0 gunner     (501) staff       (20)      583 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/row_collection.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1187 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/table_data_row.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1149 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/table_row_collection.py
+-rw-r--r--   0 gunner     (501) staff       (20)      266 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/table_row_collection_quota_aware.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1371 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py
+-rw-r--r--   0 gunner     (501) staff       (20)      423 2023-03-01 17:45:31.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/source_app.css
+-rw-r--r--   0 gunner     (501) staff       (20)     4425 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/source_app.py
+-rw-r--r--   0 gunner     (501) staff       (20)      342 2023-03-22 14:46:09.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/source_data.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3983 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/source_metadata_client.py
+-rw-r--r--   0 gunner     (501) staff       (20)     5602 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/cli/tools/tables/state_manager.py
+-rw-r--r--   0 gunner     (501) staff       (20)      187 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/debug.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.890285 patch-cli-0.2.6/src/patch/gql/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/gql/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)     3024 2023-04-06 22:23:04.000000 patch-cli-0.2.6/src/patch/gql/client.py
+-rw-r--r--   0 gunner     (501) staff       (20)    14467 2023-04-25 14:24:05.000000 patch-cli-0.2.6/src/patch/gql/schema.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.892222 patch-cli-0.2.6/src/patch/storage/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/storage/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      391 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/storage/auth.py
+-rw-r--r--   0 gunner     (501) staff       (20)      163 2023-04-06 22:16:46.000000 patch-cli-0.2.6/src/patch/storage/domain.py
+-rw-r--r--   0 gunner     (501) staff       (20)      148 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/storage/generic_payload.py
+-rw-r--r--   0 gunner     (501) staff       (20)      955 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/storage/generic_storage_file.py
+-rw-r--r--   0 gunner     (501) staff       (20)      398 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/storage/state_file.py
+-rw-r--r--   0 gunner     (501) staff       (20)     1472 2023-04-06 14:53:28.000000 patch-cli-0.2.6/src/patch/storage/storage.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.892592 patch-cli-0.2.6/src/patch/tp/
+-rw-r--r--   0 gunner     (501) staff       (20)        0 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/tp/__init__.py
+-rw-r--r--   0 gunner     (501) staff       (20)      232 2023-01-12 18:07:47.000000 patch-cli-0.2.6/src/patch/tp/phone_number.py
+drwxr-xr-x   0 gunner     (501) staff       (20)        0 2023-04-26 16:59:15.893427 patch-cli-0.2.6/src/patch_cli.egg-info/
+-rw-r--r--   0 gunner     (501) staff       (20)     3732 2023-04-26 16:59:15.000000 patch-cli-0.2.6/src/patch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 gunner     (501) staff       (20)     4348 2023-04-26 16:59:15.000000 patch-cli-0.2.6/src/patch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 gunner     (501) staff       (20)        1 2023-04-26 16:59:15.000000 patch-cli-0.2.6/src/patch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 gunner     (501) staff       (20)       44 2023-04-26 16:59:15.000000 patch-cli-0.2.6/src/patch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 gunner     (501) staff       (20)      236 2023-04-26 16:59:15.000000 patch-cli-0.2.6/src/patch_cli.egg-info/requires.txt
+-rw-r--r--   0 gunner     (501) staff       (20)        6 2023-04-26 16:59:15.000000 patch-cli-0.2.6/src/patch_cli.egg-info/top_level.txt
```

### Comparing `patch-cli-0.2.5/.pat-complete.fish` & `patch-cli-0.2.6/.pat-complete.fish`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/.pat-complete.sh` & `patch-cli-0.2.6/.pat-complete.sh`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/.pat-complete.zsh` & `patch-cli-0.2.6/.pat-complete.zsh`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/LICENSE.md` & `patch-cli-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/PKG-INFO` & `patch-cli-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patch-cli
-Version: 0.2.5
+Version: 0.2.6
 Summary: Spin up analytics APIs over your data in minutes, without writing any code.
 Home-page: https://www.patch.tech/
 Download-URL: https://docs.patch.tech/command-line-interface/installation
 Author: Patch Enterprises
 Author-email: eng@patch.tech
 Project-URL: Changelog, https://patch.releases.live/
 Project-URL: Documentation, https://docs.patch.tech/command-line-interface/basic-usage
```

### Comparing `patch-cli-0.2.5/README.md` & `patch-cli-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/pat.py` & `patch-cli-0.2.6/pat.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/setup.cfg` & `patch-cli-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/auth/auth_client.py` & `patch-cli-0.2.6/src/patch/auth/auth_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import requests
 from dataclasses import dataclass, field
 
 from requests import HTTPError
 
 from patch.auth.auth_token import global_access_token
+from patch.storage.domain import get_patch_domain
 
 
 class AuthResponseStatus(Enum):
     Success = 'Success',
     Failure = 'Failure'
     Pending = 'Pending'
 
@@ -50,18 +51,17 @@
     refresh_token: str
 
     def __post_init__(self):
         self.status = AuthResponseStatus.Success
 
 
 class AuthClient:
-    DEFAULT_AUTH_URL: str = 'https://api.patch.tech/v1'
 
     def __init__(self, auth_url=None):
-        self._auth_url = auth_url or os.environ.get('PATCH_AUTH_URL') or AuthClient.DEFAULT_AUTH_URL
+        self._auth_url = auth_url or f"{get_patch_domain()}/v1"
 
     def login_or_signup_phone(self, phone):
         try:
             result = self.call_post('/auth/login', authform=phone, selection="phone")
             body = result.json()
             status = body.get('result', None)
             if status == 'OK':
```

### Comparing `patch-cli-0.2.5/src/patch/auth/auth_forms.py` & `patch-cli-0.2.6/src/patch/auth/auth_forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from rich.console import Console
 
 from patch.auth.auth_client import AuthClient, AuthResponseStatus
 from patch.storage.auth import AuthPayload
 from patch.storage.storage import Storage
 from patch.tp.phone_number import PhoneNumber
 
+
 class AuthForm:
     """
     The class is responsible for authentication via phone number or email.
     It is outdated procedure, that involves deprecated DGraph endpoints.
     The procedure will be replaced by a direct FusionAuth calls.
     """
 
-    def __init__(self, authform, type):
+    def __init__(self, authform, auth_type):
         self.console = Console()
         self._ac = AuthClient()
-        self._type = type
-        if type == "sms":
-            authform : PhoneNumber
+        self._type = auth_type
+        if auth_type == "sms":
+            authform: PhoneNumber
         self._authform = authform
-    
+
     def request_validation(self):
         if self._type == "sms":
             result = self._ac.login_or_signup_phone(self._authform.canonical)
             self._handle_response(result)
         elif self._type == "email":
             result = self._ac.login_or_signup_email(self._authform)
             self._handle_response(result)
-    
+
     def _respond_pending_sms(self, result):
         dest_phone = result.verification.to
         self.console.print(f"Check SMS on [blue]{dest_phone}[/blue] for the confirmation code")
         code = self.console.input("[yellow]Code> [/yellow]")
         response = self._ac.validate_phone(self._authform.canonical, code)
         self._handle_response(response)
-    
+
     def _respond_pending_email(self, result):
         dest = result.verification.to
         self.console.print(f"Check inbox at [blue]{dest}[/blue] for the confirmation code")
         code = self.console.input("[yellow]Code> [/yellow]")
         response = self._ac.validate_email(self._authform, code)
         self._handle_response(response)
 
@@ -62,8 +63,7 @@
     def _respond_problem(self, error):
         self.console.print(f"There is a problem: [red]{error}[/red]")
 
     def _respond_success(self, access_token, refresh_token):
         storage = Storage()
         storage.auth.store(AuthPayload(access_token=access_token, refresh_token=refresh_token))
         self.console.print('[green]Authentication succeeded[/green]')
-
```

### Comparing `patch-cli-0.2.5/src/patch/auth/auth_token.py` & `patch-cli-0.2.6/src/patch/auth/auth_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 
     def has_token(self) -> bool:
         return self.get_access_token() is not None
 
     def store(self, new_access_token, new_refresh):
         self.storage.auth.store(AuthPayload(access_token=new_access_token, refresh_token=new_refresh))
 
+    def delete(self):
+        self.storage.auth.delete()
+
     def get_roles(self) -> List[any]:
         if self.has_token():
             options = {'verify_signature': False, 'verify_exp': False}
             jwt_payload = jwt.api_jwt.decode_complete(self.get_access_token(), options=options)
             return jwt_payload.get('payload', {}).get('patch.tech/graphql', {}).get('roles', [])
         return []
```

### Comparing `patch-cli-0.2.5/src/patch/cli/__init__.py` & `patch-cli-0.2.6/src/patch/cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import click
+import os
 import sys
 
+from patch.auth.auth_token import global_is_admin_or_mta
 from patch.cli.patch_click_context import PatchClickContext
 from patch.debug import debug_enabled
+from patch.cli.commands.alpha import alpha
 from patch.cli.commands.connector import connector
 from patch.cli.commands.login import login
+from patch.cli.commands.logout import logout
 from patch.cli.commands.source import source
 from patch.cli.commands.dataset import dataset
 from patch.cli.commands.dataset import edge
+from patch.cli.commands.destination import destination
 from patch.cli.commands.admin import admin
 from patch.cli.commands.playground import playground
 from patch.cli.commands.token import token
 from patch.cli.commands.user import user
 from patch.cli.commands.access import access
 from rich.console import Console
 
@@ -33,17 +38,21 @@
 @click.group(cls=StyledGroup)
 @click.pass_context
 def main(ctx):
     ctx.ensure_object(dict)
     ctx.obj = PatchClickContext(click_ctx=ctx, terminal_width=ctx.terminal_width)
 
 
+if global_is_admin_or_mta:
+    main.add_command(alpha)
 main.add_command(login)
+main.add_command(logout)
 main.add_command(user)
 main.add_command(connector)
 main.add_command(source)
+main.add_command(destination)
 main.add_command(dataset)
 main.add_command(edge)
 main.add_command(admin)
 main.add_command(playground)
 main.add_command(token)
 main.add_command(access)
```

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/__init__.py` & `patch-cli-0.2.6/src/patch/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/access.py` & `patch-cli-0.2.6/src/patch/cli/commands/access.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/admin.py` & `patch-cli-0.2.6/src/patch/cli/commands/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
 @admin.group(cls=StyledGroup, help='Manage datasets')
 def dataset():
     pass
 
 
 @dataset.command(cls=StyledCommand, help='Schedule immediate run for dataset on current source.')
-@click.option('-n','--dataset_name')
+@click.option('-n', '--dataset_name')
 @click.option('-i', '--dataset_id')
 @click.option('-t', '--table_name')
 @with_as_tenant()
 @pass_obj()
 def sync(patch_ctx: PatchClickContext, dataset_name, dataset_id, table_name):
     console = patch_ctx.console
     if dataset_name and dataset_id:
@@ -221,8 +221,8 @@
         elif dataset_name:
             mutation_input['datasetName'] = dataset_name
         if table_name:
             mutation_input['tableName'] = table_name
 
         gql_mutation = client.prepare_mutation('syncDataset', input=mutation_input)
         gql_mutation.execute()
-        console.print(f"[green]Dataset queued for sync[/green]")
+        console.print(f"[green]Dataset queued for sync[/green]")
```

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/connector.py` & `patch-cli-0.2.6/src/patch/cli/commands/connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 @click.group(cls=StyledGroup, help='Review the requirements to connect to supported data sources',
              hidden=not global_access_token.has_token())
 @click.pass_context
 def connector(_ctx, ):
     pass
 
 
-@connector.group(cls=StyledGroup, help='Connectivity commands for Snowflake') # List of sources that Patch can observe
+@connector.group(cls=StyledGroup, help='Connectivity commands for Snowflake')  # List of sources that Patch can observe
 def snowflake():
     pass
 
+
 @connector.group(cls=StyledGroup, help='Connectivity commands for BigQuery')
 def bigquery():
     pass
 
+
 @connector.group(cls=StyledGroup, help='Connectivity commands for Azure Blob Storage')
 def azure_blob():
     pass
 
 
 @azure_blob.command(cls=StyledCommand, help='Fields required for connection to Azure Blob Storage')
 @pass_obj()
```

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/dataset.py` & `patch-cli-0.2.6/src/patch/cli/commands/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,17 @@
 from patch.cli.tools.filters_reader import filters_to_claims
 from patch.cli.tools.tables.source_app import SourceApp
 from patch.cli.tools.tables.source_data import SourceMeta
 from patch.cli.tools.tables.source_metadata_client import SourceMetadataClient
 
 from patch.cli.tools.datasets.row_table_renderer import RowRenderer, RowTableRenderer
 
-DEFAULT_PAXL_GQL_URL = 'https://api.patch.tech/query/graphql'
-
-paxl_gql_url = os.environ.get('PATCH_PAXL_GQL_URL') or DEFAULT_PAXL_GQL_URL
+from patch.storage.domain import get_patch_domain
 
+DOMAIN = get_patch_domain()
 
 @click.group(cls=StyledGroup, help='Create or edit datasets that Patch generates APIs over',
              hidden=not global_access_token.has_token())
 def dataset():
     pass
 
 
@@ -43,15 +42,15 @@
 def create_dataset_interactive(client, console, name, local_state):
     interface = SourceMetadataClient(console, client, local_state)
     meta = SourceMeta(source_data=interface.get_source_metadata())
 
     if not meta.source_data.tables:
         console.print(f"No tables found in active source [blue]{local_state.active_source_name}[/blue].")
         console.print("If the active source is some type of object storage, use " +
-            '\"pat dataset create -c <config.json>\" instead.')
+                      '\"pat dataset create -c <config.json>\" instead.')
         console.print("You can find the config file schema in the docs for the active source's type.")
         return None
 
     source_app = SourceApp(meta=meta)
     source_app.run()
     if meta.source_data.is_ready and interface.confirm_dataset(dataset_name=name,
                                                                tables=meta.source_data.selected_tables):
@@ -59,19 +58,22 @@
 
     console.print(f"Dataset creation [yellow]cancelled![/yellow]")
     return None
 
 
 def create_dataset_from_file(_client, _console, name, source_id, config_file):
     config = json.load(config_file)
-    return {
+    config_vals = {
         'sourceId': source_id,
         'datasetName': name,
         'tables': config["tables"],
     }
+    if "destinations" in config:
+        config_vals["destinations"] = config["destinations"]
+    return config_vals
 
 
 @dataset.command(cls=StyledCommand, help='Configure dataset')
 @click.option('-c', '--config', type=click.File(mode='r'), help='Configuration file')
 @click.argument('name', type=click.STRING)
 @with_as_tenant()
 @pass_obj()
@@ -202,19 +204,40 @@
                                                                            'datasetName': name})
             gql_mutation.execute()
             console.print(f"[green]Dataset queued for deletion[/green]")
         else:
             console.print(f"Command [red]aborted[/red]")
 
 
+@dataset.command(cls=StyledCommand, help='Pause syncs of a dataset')
+@click.argument('name', type=click.STRING)
+@click.option('-y', '--assume-yes', '--yes', help='Skip confirmation', is_flag=True)
+@with_as_tenant()
+@pass_obj()
+def pause(patch_ctx: PatchClickContext, name, assume_yes):
+    console = patch_ctx.console
+    with active_source(patch_ctx, show_state=True) as local_state:
+        confirmation = assume_yes or Confirm.ask(f"Would you like to pause the Dataset [cyan]{name}[/cyan] " +
+                                                 f"from Source [cyan]{local_state.active_source_name}[/cyan]? ",
+                                                 console=console)
+        if confirmation:
+            client = patch_ctx.gql_client
+            gql_mutation = client.prepare_mutation('pauseDataset', input={'sourceId': local_state.active_source_id,
+                                                                          'datasetName': name})
+            gql_mutation.execute()
+            console.print(f"[green]Dataset will be paused.[/green]")
+        else:
+            console.print(f"Command [red]aborted[/red]")
+
+
 @dataset.command(cls=StyledCommand, help='Endpoints for the dataset')
 @click.argument('name', type=click.STRING)
 @click.option('-o', '--output',
-    type=click.Choice(['json', 'table']), default='table', show_default=True,
-    help='Output format (choices: json, table)')
+              type=click.Choice(['json', 'table']), default='table', show_default=True,
+              help='Output format (choices: json, table)')
 @with_as_tenant()
 @pass_obj()
 def endpoints(patch_ctx: PatchClickContext, name, output):
     if output == 'json':
         console = patch_ctx.switch_to_data_output()
     else:
         console = patch_ctx.console
@@ -225,15 +248,15 @@
         source_id = local_state.active_source_id
         client = patch_ctx.gql_client
         gql_query = client.prepare_query('datasetByName', input={
             'sourceId': source_id,
             'datasetName': name
         })
         with gql_query as q:
-            q.__fields__('id', 'name', 'tables')
+            q.__fields__('id', 'name', 'tables', 'destinations')
 
         result = gql_query.execute()
         eh = EndpointRenderer(console, local_state, name, output)
         eh.render_query_result(result)
 
 
 def match_primary_keys(table_pk, input_pk):
@@ -339,50 +362,80 @@
             'filters': filters_to_claims(filter_scope)
         })
         with gql_mutation as m:
             m.__fields__('accessToken')
 
         return gql_mutation.execute()
 
+def get_dataset_destinations(patch_ctx: PatchClickContext, name):
+    with active_source(patch_ctx) as local_state:
+        source_id = local_state.active_source_id
+        client = patch_ctx.gql_client
+        gql_query = client.prepare_query('datasetByName', input={
+            'sourceId': source_id,
+            'datasetName': name,
+        })
+        with gql_query as q:
+            q.__fields__('destinations')
 
+        return gql_query.execute()
 
 @dataset.command(cls=StyledCommand, help='Bearer tokens for endpoints.')
 @click.argument('name', type=click.STRING)
 @click.option('-f', '--filter', 'filter_scope', type=str, help='Filter of the authorization scope', multiple=True)
 @with_as_tenant()
 @pass_obj()
 def bearer(patch_ctx: PatchClickContext, name, filter_scope):
     result = generate_query_auth(patch_ctx, name, filter_scope)
     print(result.accessToken)
 
 
-@dataset.command(cls=StyledCommand, help='Launch GraphQL Playground.')
+@dataset.command(cls=StyledCommand, help='Launch the GraphQL or Batch Playground.')
 @click.argument('name', type=click.STRING)
 @click.option('-f', '--filter', 'filter_scope', type=str, help='Filter of the authorization scope', multiple=True)
 @with_as_tenant()
 @pass_obj()
 def playground(patch_ctx: PatchClickContext, name, filter_scope):
     mutation_result = generate_query_auth(patch_ctx, name, filter_scope)
     token = mutation_result.accessToken
+    destinations = get_dataset_destinations(patch_ctx, name)
+    has_batch = any(d.destination.type == "BATCH_API" for d in destinations.destinations)
+    has_dataset = any(d.destination.type == "DATASET_API" for d in destinations.destinations)
 
     console = patch_ctx.console
-    console.print("You are about to open GraphQL Playground.")
+    if has_batch:
+        console.print("You are about to open the Batch Playground.")
+    if has_dataset:
+        console.print("You are about to open the GraphQL Playground.")
     console.print(
-        "The configuration below will be copied to your clipboard. You can paste it in [yellow]HTTP HEADERS[/yellow] tab in the Playground console.\n")
+        "The configuration below will be copied to your clipboard. You can paste it in [yellow]HTTP HEADERS[/yellow] " +
+        "tab in the Playground console.\n")
     headers = json.dumps({'Authorization': token})
     console.out(headers)
 
     console.input("\nPress Enter to continue...")
-    paxl_gql_prompt_url = f"{paxl_gql_url}#prompt"
-    result = click.launch(paxl_gql_prompt_url)
+    batch_playground_url = f"{DOMAIN}/batch/playground/#prompt"
+    gql_playground_url = f"{DOMAIN}/query/graphql#prompt"
+    playground_url = gql_playground_url #backwards compatibility (datasets without destinations)
+    if has_batch:
+        playground_url =  batch_playground_url
+    if has_dataset:
+        playground_url =   gql_playground_url
+    result = 0
+    if has_batch ^ has_dataset:
+        result = click.launch(playground_url)
     if result != 0:
-        console.input(f"Now, open [magenta]{paxl_gql_url}#prompt[/magenta]")
+        if has_dataset:
+            console.input(f"Open [magenta]{gql_playground_url}[/magenta]for the dataset playground")
+        if has_batch:
+            console.input(f"Open [magenta]{batch_playground_url}[/magenta]for the batch playground")
     else:
         console.print(
-            f"If your default browser hasn't loaded it, open this url in your browser: [magenta]{paxl_gql_url}#prompt[/magenta]")
+            f"If your default browser hasn't loaded it, open this url in your browser: " +
+            f"[magenta]{playground_url}[/magenta]")
     pyperclip.copy(headers)
 
 
 @click.group(cls=StyledGroup, help='Create, edit, or delete edges between tables of a dataset',
              hidden=not global_access_token.has_token())
 def edge():
     pass
@@ -403,15 +456,16 @@
     '-c',
     '--on-columns',
     multiple=True,
     nargs=2,
     required=True,
     type=click.STRING,
     help='Pairs of columns used to join table1 and table2, e.g. -c <table1-cola> <table2-colb>')
-@click.option('-u', '--is-unique', is_flag=True, required=False, default=False, show_default=True, help='Is this a 1:1 relationship?')
+@click.option('-u', '--is-unique', is_flag=True, required=False, default=False, show_default=True,
+              help='Is this a 1:1 relationship?')
 @with_as_tenant()
 @pass_obj()
 def create(patch_ctx: PatchClickContext, name, dataset_name, from_table_name, to_table_name, on_columns, is_unique):
     console = patch_ctx.console
     eap_warning(console)
     with active_source(patch_ctx, show_state=True) as local_state:
         source_id = local_state.active_source_id
```

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/playground.py` & `patch-cli-0.2.6/src/patch/cli/commands/playground.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     if not token:
         console.print("[red]Error[/red] You need to log-in before you use GraphQL")
         patch_ctx.exit(1)
     else:
         gql_url = patch_ctx.gql_client.get_url()
         console.print("You are about to open GraphQL Playground.")
         console.print(
-            "The configuration below will be copied to your clipboard. You can paste it in [yellow]HTTP HEADERS[/yellow] tab in the Playground console.\n")
+            "The configuration below will be copied to your clipboard. " +
+            "You can paste it in [yellow]HTTP HEADERS[/yellow] tab in the Playground console.\n")
         headers = json.dumps({'Authorization': token})
         console.out(headers)
         console.print("\nExample query:")
         console.print("[blue]query[/blue] {")
         console.print("    [yellow]getSourceList[/yellow]([magenta]input[/magenta]:{}) { ")
         console.print("        [yellow]id [/yellow]")
         console.print("        [yellow]name[/yellow]")
```

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/source.py` & `patch-cli-0.2.6/src/patch/cli/commands/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import click
 
 from patch.auth.auth_token import global_access_token
 from patch.cli import PatchClickContext
 from patch.cli.remote.source_client import SourceClient
 from patch.cli.styled import StyledGroup, StyledCommand
 from patch.cli.commands import pass_obj, with_as_tenant
-from patch.cli.tools.connectors.source_config_interactive import SourceConfigInteractive
+from patch.cli.tools.config_interactive import ConfigInteractive
+from patch.cli.tools.connectors.connector_spec import field_specs, ConnectorConfigSpec
 from patch.cli.tools.connectors.source_config_non_interactive import SourceConfigNonInteractive
 
 from rich import box
 from rich.table import Table
 from rich.prompt import Confirm
 
 from patch.storage.state_file import StatePayload
@@ -31,27 +32,28 @@
 @pass_obj()
 def connect(patch_ctx: PatchClickContext, config, interactive, staging_db):
     console = patch_ctx.console
     if not config and not interactive:
         console.print("[red]Provide either configuration file or interactive mode[/red]")
         patch_ctx.exit(1)
     if interactive:
-        source_config = SourceConfigInteractive(console, config, staging_db)
+        source_config = ConfigInteractive(console, config, staging_db)
     else:
         source_config = SourceConfigNonInteractive(config, staging_db)
-    config_values = source_config.resolve_config()
+    config_values = source_config.resolve_config(field_specs)
 
-    result_source = source_config.send_to_gql(patch_ctx, config_values)
+    result_source = source_config.send_to_gql(patch_ctx, config_values, spec=ConnectorConfigSpec)
     console.print(f"[green]Succeeded[/green]")
     console.print(f"Source Name: [yellow]{result_source.name}[/yellow], ID [yellow]{result_source.id}[/yellow]")
 
 
 @source.command(cls=StyledCommand, help='Disconnect source from Patch')
 @click.argument('name', type=click.STRING)
-@click.option('-y', '--assume-yes', '--yes', help='Skip confirmation, will fail if datasets are still attached to source',  is_flag=True)
+@click.option('-y', '--assume-yes', '--yes',
+              help='Skip confirmation, will fail if datasets are still attached to source', is_flag=True)
 @with_as_tenant()
 @pass_obj()
 def disconnect(patch_ctx: PatchClickContext, name, assume_yes):
     console = patch_ctx.console
     confirmation = assume_yes or Confirm.ask(f"Would you like to remove Source [cyan]{name}[/cyan]? ", console=console)
     if confirmation:
         client = patch_ctx.gql_client
@@ -104,15 +106,15 @@
         for source_elem in sorted_sources:
             table.add_row(source_elem.name, source_elem.id)
         console.print(table)
 
 
 @source.command(cls=StyledCommand, help='Select this source as default one')
 @click.argument('name', type=click.STRING)
-@click.option('-f', '--force', help='Select this source as default even if connection fails ',  is_flag=True)
+@click.option('-f', '--force', help='Select this source as default even if connection fails ', is_flag=True)
 @with_as_tenant()
 @pass_obj()
 def use(patch_ctx: PatchClickContext, name, force):
     console = patch_ctx.console
     client = SourceClient(patch_ctx.gql_client)
     result_q = client.get_sources_by_name(name)
     result_q_len = len(result_q)
```

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/token.py` & `patch-cli-0.2.6/src/patch/cli/commands/token.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/commands/user.py` & `patch-cli-0.2.6/src/patch/cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/patch_click_context.py` & `patch-cli-0.2.6/src/patch/cli/patch_click_context.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/remote/dataset_client.py` & `patch-cli-0.2.6/src/patch/cli/remote/dataset_client.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/remote/source_client.py` & `patch-cli-0.2.6/src/patch/cli/remote/source_client.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/styled.py` & `patch-cli-0.2.6/src/patch/cli/styled.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/config_spec.py` & `patch-cli-0.2.6/src/patch/cli/tools/config_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def set_type_from_str(self, str_type: Optional[str]) -> None:
         self._type = None
         if str_type:
             if str_type in self._spec.keys():
                 self._type = str_type
             else:
-                raise ConfigSpecError("Unknown connector type")
+                raise ConfigSpecError("Unknown type")
 
     def get_spec(self) -> Optional[InputSpec]:
         return self._spec[self._type]
 
     def get_spec_fields(self) -> List[FieldSpec]:
         return self.get_spec().fields
```

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/connectors/connector_spec.py` & `patch-cli-0.2.6/src/patch/cli/tools/connectors/connector_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,29 +43,39 @@
         name='Azure Blob Storage',
         create_mutation_name='sourceConnectAzureBlob', fields=[
             FieldSpec(key="containerName", desc="The name of the Blob Storage container", required=True),
             FieldSpec(key="accountName", desc="The name of the storage account that owns the container", required=True),
             FieldSpec(key="sasToken", desc="A SAS token that grants access to the container (or a directory within)",
                       required=True),
         ]),
+    'databricks': InputSpec(
+        name='Databricks',
+        create_mutation_name='sourceConnectDatabricks', fields=[
+            FieldSpec(key="hostname", desc="Hostname for your Databricks SQL endpoint", required=True),
+            FieldSpec(key="httpPath", desc="httpPath for your Databricks SQL endpoint", required=True),
+            FieldSpec(key="token", desc="Access token for your Databricks SQL endpoint", required=True),
+        ])
 }
 
 field_specs: List[FieldSpec] = [
     FieldSpec(key="name", desc="Source name", required=True),
     FieldSpec(key="type", desc="Connector type", required=True, choices=[
         FieldChoice(key='snowflake', gql_value='snowflake'),
         FieldChoice(key='bigquery', gql_value='bigquery'),
         FieldChoice(key='azure-blob', gql_value='azure-blob'),
+        FieldChoice(key='databricks', gql_value='databricks'),
     ], conditions=[
         FieldSpecCondition(if_value='snowflake',
                            then_fields=conn_spec['snowflake'].fields),
         FieldSpecCondition(if_value='bigquery',
                            then_fields=conn_spec['bigquery'].fields),
         FieldSpecCondition(if_value='azure-blob',
                            then_fields=conn_spec['azure-blob'].fields),
+        FieldSpecCondition(if_value='databricks',
+                           then_fields=conn_spec['databricks'].fields),
     ])
 ]
 
 
 def render_bool(value: bool):
     return "True" if value else "False"
 
@@ -78,19 +88,19 @@
     return result
 
 
 class ConnectorConfigSpec(ConfigSpec):
 
     def __init__(self, str_connector_type):
         super().__init__(conn_spec, name_spec, str_connector_type)
-        largestKey = 0
+        largest_key = 0
         for line in self.get_spec_fields():
-            if len(line.key) > largestKey:
-                largestKey = len(line.key)
-        self._largest_key = largestKey
+            if len(line.key) > largest_key:
+                largest_key = len(line.key)
+        self._largest_key = largest_key
 
     def render_line(self, table: Table, field: FieldSpec, required_desc: str, applicable_desc: str):
         table.add_row(field.key, field.desc, required_desc, applicable_desc)
         key_map = map_values(field)
         if field.conditions is not None:
             for condition in field.conditions:
                 required = render_bool(field.required)
```

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/connectors/source_config.py` & `patch-cli-0.2.6/src/patch/cli/tools/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import ABC, abstractmethod
 from collections import deque
 from typing import Optional, TextIO, Any, List
 
-from patch.cli.tools.connectors.connector_spec import field_specs, ConnectorConfigSpec
+from patch.cli.tools.destinations.destination_spec import DestinationConfigSpec
+from patch.cli.tools.connectors.connector_spec import ConnectorConfigSpec
+
 from patch.cli.tools.field_spec import FieldSpec, FieldChoice
 from patch.cli.tools.json_reader import read_json
 
 
 def choices_to_gql_value(field_name: str, choices: List[FieldChoice], key_val: str) -> str:
     for choice in choices:
         if choice.key == key_val:
@@ -15,15 +17,15 @@
     raise SpecVerificationError(f"Unknown value for field: {field_name}. Accepted values: {accepted_choices}")
 
 
 class SpecVerificationError(Exception):
     pass
 
 
-class SourceConfig(ABC):
+class Config(ABC):
     """The source config.
 
     This class manages collecting and interpreting source configuration.
     There are two possible sources of the configuration:
     - configuration JSON file
     - the function resolve_missing_config_field from subclasses
                (for example, in the interactive subclass, it asks user for the value)
@@ -49,15 +51,15 @@
     def finalize_key_resolution(self) -> None:
         """
         Finalization function for field resolvers.
         For example, can say "thank you" to the user, or throws exception with all missing fields.
         """
         pass
 
-    def resolve_config(self):
+    def resolve_config(self, field_specs):
         """
         The function tries to resolve values for all fields from the specification.
         If values can't be resolved, it throws an exception.
         If there are excessive values, it throws an exception.
         :return:
         """
         input_values: dict = self.config.copy()
@@ -82,16 +84,28 @@
             if len(keys) == 1:
                 raise SpecVerificationError(f"Unknown key: {keys[0]}")
             else:
                 key_values = ", ".join(keys)
                 raise SpecVerificationError(f"Unknown keys: {key_values}")
         return result_values
 
-    def send_to_gql(self, patch_ctx, values: dict):
+    def send_to_gql(self, patch_ctx, values: dict, spec):
         client = patch_ctx.gql_client
         config = values.copy()
-        connector_type = config.pop('type', None)
-        connector_spec = ConnectorConfigSpec(connector_type)
-        if self.staging_db:
-            config['stagingDatabase'] = self.staging_db
-        mut = client.prepare_mutation(connector_spec.mutation_name, input=config)
+        if spec == ConnectorConfigSpec:
+            type = config.pop('type', None)
+            final_spec = spec(type)
+            if self.staging_db:
+                config['stagingDatabase'] = self.staging_db
+        if spec == DestinationConfigSpec:
+            retention = int(config.pop('retentionDays', None))
+            batch_size = config.pop('maxBatchSize', None)
+            if retention or batch_size:
+                config['batchApi'] = {}
+                if retention:
+                    config['batchApi']['retentionDays'] = int(retention)
+                if batch_size:
+                    config['batchApi']['maxBatchSize'] = int(batch_size)
+            type = config['type']
+            final_spec = spec(type)
+        mut = client.prepare_mutation(final_spec.mutation_name, input=config)
         return mut.execute()
```

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/connectors/source_config_interactive.py` & `patch-cli-0.2.6/src/patch/cli/tools/config_interactive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import TextIO, Optional
 
-from patch.cli.tools.connectors.source_config import SourceConfig
+from patch.cli.tools.config import Config
+
 from rich.prompt import Prompt
 
 from patch.cli.tools.field_spec import FieldSpec
 from patch.cli.tools.base64_encryption import b64_encryption
 
 
-class SourceConfigInteractive(SourceConfig):
+class ConfigInteractive(Config):
 
-    def __init__(self, console, file_config: Optional[TextIO], staging_db: Optional[str]):
+    def __init__(self, console, file_config: Optional[TextIO], staging_db: Optional[str] = None):
         super().__init__(file_config, staging_db)
         self.console = console
 
     def resolve_missing_config_field(self, field: FieldSpec):
         """Resolves the given field by prompting the user for a value."""
         choices = None
         if field.choices:
@@ -29,7 +30,11 @@
                     return value
             elif not field.required:
                 return None
             self.console.print("[prompt.invalid]Value cannot be empty")
 
     def finalize_key_resolution(self) -> None:
         pass
+
+    def finalize_key_resolution(self) -> None:
+        pass
+
```

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/connectors/source_config_non_interactive.py` & `patch-cli-0.2.6/src/patch/cli/tools/connectors/source_config_non_interactive.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, TextIO, List
 
-from patch.cli.tools.connectors.source_config import SourceConfig, SpecVerificationError
+from patch.cli.tools.config import Config, SpecVerificationError
 from patch.cli.tools.field_spec import FieldSpec
 
 
-class SourceConfigNonInteractive(SourceConfig):
+class SourceConfigNonInteractive(Config):
     missing_fields: List[FieldSpec]
 
     def __init__(self, file_config: Optional[TextIO], staging_db: Optional[str]):
         super().__init__(file_config, staging_db)
         self.missing_fields = []
 
     def resolve_missing_config_field(self, field: FieldSpec):
```

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/datasets/curl_renderer.py` & `patch-cli-0.2.6/src/patch/cli/tools/datasets/curl_renderer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/datasets/endpoint_renderer.py` & `patch-cli-0.2.6/src/patch/cli/tools/datasets/endpoint_renderer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
+import os
 from typing import List, Optional
 
 from rich.console import Console
 from rich.table import Table
 
 from patch.cli.styled import NONE_BOX
 from patch.cli.tools.datasets.curl_renderer import has_curl, CurlRenderer
 from patch.gql.schema import Dataset
 from patch.storage.state_file import StatePayload
+from patch.storage.domain import get_patch_domain
 
 
 def table_route(name, primary_keys: List[str]):
     keys_path = ",".join(["{" + pk.lower() + "}" for pk in primary_keys])
     return f"/{name.lower()}/[yellow]{keys_path}[/yellow]"
 
 
@@ -61,15 +63,15 @@
             self.table.add_row(column_1, column_2)
 
     def render(self):
         self.console.print(self.table)
 
 
 class EndpointRenderer:
-    DOMAIN = 'https://api.patch.tech/query'
+    DOMAIN = f'{get_patch_domain()}/query'
 
     def __init__(self, console: Console, source_state: StatePayload, name: str, output: str):
         self.console = console
         self.source_state = source_state
         self.source_id = source_state.active_source_id
         self.name = name
         self.table = EndpointTableRenderer(self.console)
@@ -77,21 +79,23 @@
 
     def render_base_url(self, suffix):
         return ''.join([self.DOMAIN, c('yellow', suffix)])
 
     def render_base_url_text(self, suffix):
         return ''.join([self.DOMAIN, suffix])
 
-    def render_bases(self):
-        self.table.header("Base URLs")
-        self.table.row('SQL', self.render_base_url('/sql'), is_dimmed=True)
+    def render_dataset_bases(self):
         self.table.row('GraphQL',
                        f"{self.render_base_url('/graphql')} (try [cyan]pat dataset playground {self.name}[/cyan])")
         self.table.row('REST', self.render_base_url('/rest/{route}'))
 
+    def render_batch_bases(self):
+        self.table.row('Batch', self.render_base_url('/batch/consume'))
+        self.table.row('Batch Schema', self.render_base_url('/batch/schema.json'))
+
     def render_query_result(self, result: Optional[Dataset]):
         if self.output == 'table':
             self.render_query_result_table(result)
         if self.output == 'json':
             self.render_query_result_json(result)
 
     def render_query_result_json(self, result: Optional[Dataset]):
@@ -116,17 +120,24 @@
                     'base': self.render_base_url_text('/rest'),
                     'resources': rest_routes
                 }
             }
         }))
 
     def render_query_result_table(self, result: Optional[Dataset]):
+        has_batch = any(r.destination.type == "BATCH_API" for r in result.destinations)
+        has_default = any(r.destination.type == "DATASET_API" for r in result.destinations)
+
         if result:
-            self.render_bases()
-            if result.tables:
+            self.table.header("Base URLs")
+            if has_default:
+                self.render_dataset_bases()
+            if has_batch:
+                self.render_batch_bases()
+            if has_default and result.tables:
                 self.table.newline()
                 self.table.header("Routes")
                 for result_table in result.tables:
                     primary_key = [k.name for k in result_table.primaryKey]
                     self.table.simple_row(table_route(result_table.name, primary_key))
                 if has_curl():
                     self.table.newline()
@@ -134,14 +145,14 @@
                     self.table.simple_row(f"export BEARER_TOKEN=$(pat dataset bearer {self.name})")
                     curl = CurlRenderer()
                     limit = 10
                     for result_table in result.tables:
                         rendered_command = curl.render_url(self.render_base_url('/rest/' + result_table.name.lower()),
                                                            limit=limit)
                         self.table.simple_row(rendered_command)
-            else:
-                self.table.newline()
-                self.table.header("No routes")
+                else:
+                    self.table.newline()
+                    self.table.header("No routes")
             self.table.render()
         else:
             self.console.print(f"Dataset {c('cyan', self.name)} "
                                f"for source ID {c('yellow', self.source_id)} has not been found.")
```

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/datasets/row_table_renderer.py` & `patch-cli-0.2.6/src/patch/cli/tools/datasets/row_table_renderer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/field_spec.py` & `patch-cli-0.2.6/src/patch/cli/tools/field_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 @dataclass
 class FieldChoice:
     gql_value: Any
     key: str
 
+
 @dataclass
 class FieldSpec:
     key: str
     desc: str
     required: bool
     is_password: bool = False
     type: str = "str"
```

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/container_panel.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/container_panel.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/hierarchy_renderer.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/hierarchy_renderer.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/list_tools/data_list.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/list_tools/data_list.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_quota.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_quota.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_summary.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_summary.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_appendable.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_appendable.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_positional.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_positional.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_positional_hierarchy.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_positional_hierarchy.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/panel_tabular_with_columns.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/panel_tabular_with_columns.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/viewport/cursor_controller.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/viewport/cursor_controller.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/components/viewport/viewport.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/components/viewport/viewport.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/rows/columns_row_collection.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/rows/columns_row_collection.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/rows/row_collection.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/rows/row_collection.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/rows/table_data_row.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/rows/table_data_row.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/rows/table_row_collection.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/rows/table_row_collection.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/source_app.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/source_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,41 +32,44 @@
         self.selected_tables = PanelTabularWithColumns.instance(
             'Zero tables selected', TableWithPkRowCollection([]))
         self.primary_keys = PanelTabularAllIn.instance(
             'No Columns', ColumnsRowCollection([]))
         super().__init__()
 
     def compose(self) -> ComposeResult:
-
         self.panel_quota.initialize(self.source_data.quota, self.source_data.quota_used, self.tables_quota_aware)
 
         self.panel_summary.initialize(self.panel_quota)
 
         self.state_mngr = StateManager(
             self,
             self.panel_search, self.panel_summary, self.panel_quota,
             self.all_tables, self.selected_tables, self.primary_keys,
             self.tables_quota_aware)
         top_help_container = Container(
-            Label("[yellow]Select tables for your dataset by scrolling or searching. Then, select a unique column as a Primary Key.\nIf none are unique, select multiple columns to form a composite key.[yellow]", id="help-text"),
+            Label(
+                "[yellow]Select tables for your dataset by scrolling or searching. Then, select a unique column " +
+                "as a Primary Key.\nIf none are unique, select multiple columns to form a composite key.[yellow]",
+                id="help-text"),
             id="top-help-container"
         )
         bottom_help_container = Container(
-            Label("[yellow]When you are finished, submit the dataset using CTRL+S. Press CTRL+C to cancel.[yellow]", id="help-text"),
+            Label("[yellow]When you are finished, submit the dataset using CTRL+S. Press CTRL+C to cancel.[yellow]",
+                  id="help-text"),
             id="bottom-help-container"
         )
         main_container = Container(
             ContainerPanel(self.panel_search, title='Search Tables'),
             ContainerPanel(self.panel_summary, title='Summary'),
             ContainerPanel(self.panel_quota, title='Quota'),
             ContainerPanel(self.all_tables, title='All Tables'),
             ContainerPanel(self.selected_tables, title='Selected Tables'),
             ContainerPanel(self.primary_keys, title='Primary Key Columns'),
             id="app-grid")
-        
+
         yield top_help_container
         yield main_container
         yield bottom_help_container
 
     def startup(self):
         pass
```

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/source_metadata_client.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/source_metadata_client.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/cli/tools/tables/state_manager.py` & `patch-cli-0.2.6/src/patch/cli/tools/tables/state_manager.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/gql/client.py` & `patch-cli-0.2.6/src/patch/gql/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from sgqlc.operation import Operation
 
 from sgqlc.endpoint.http import HTTPEndpoint
 
 from patch.auth.auth_client import AuthClient
 from patch.debug import debug_log
 from patch.gql.schema import Query, Mutation
+from patch.storage.domain import get_patch_domain
 
 
 class GqlExecutionError(Exception):
 
     def __init__(self, errors):
         self.errors = errors
         messages = [e.get('message') for e in errors]
@@ -34,19 +35,18 @@
 
     def execute(self):
         result = self._client.execute(self._op)
         return getattr(result, self._query_name)
 
 
 class Client:
-    DEFAULT_GQL_URL: str = 'https://api.patch.tech/graphql'
-    DEFAULT_TIMEOUT: int = 300 # 5 minutes
+    DEFAULT_TIMEOUT: int = 300  # 5 minutes
 
     def __init__(self, gql_url=None, as_tenant=None):
-        self._gql_url = gql_url or os.environ.get('PATCH_GQL_URL') or Client.DEFAULT_GQL_URL
+        self._gql_url = gql_url or f"{get_patch_domain()}/graphql"
         self.auth_client = AuthClient()
         self._as_tenant = as_tenant
 
     def execute(self, operation, variables=None):
         gql_result = self._call_operation(operation, variables)
         errors = gql_result.get('errors')
         if errors:
```

### Comparing `patch-cli-0.2.5/src/patch/gql/schema.py` & `patch-cli-0.2.6/src/patch/gql/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     type = non_null(str)
     nullable = non_null(bool)
     index = int
     extra = non_null(list_of(non_null(TableColumnInfo)))
 
 
 class TableStateEnum(Enum):
-    __choices__ = ("INIT", "LOADING", "READY", "ERROR", "DELETING")
+    __choices__ = ("INIT", "LOADING", "READY", "ERROR", "DELETING", "PAUSED")
 
 
 class TableDescription(Type):
     id = non_null(str)
     name = non_null(str)
     database = non_null(str)
     schema = non_null(str)
@@ -86,43 +86,110 @@
 
 
 class Source(Type):
     id = non_null(str)
     name = non_null(str)
 
 
+class HttpMethod(Enum):
+    __choices__ = ("POST", "PUT")
+
+
+class HttpHeader(Type):
+    name = non_null(str)
+
+
+class DestinationType(Enum):
+    __choices__ = ("DATASET_API", "BATCH_API")
+
+
+class BatchApiDestination(Type):
+    retentionDays = non_null(int)
+
+
+class BatchApiDestinationInput(Input):
+    retentionDays = int
+
+
+class WebhookDestination(Type):
+    url = non_null(str)
+    method = non_null(HttpMethod)
+    headers = non_null(list_of(non_null(HttpHeader)))
+    maxBatchSize = non_null(int)
+    retentionDays = non_null(int)
+
+
+class Destination(Type):
+    name = non_null(str)
+    type = non_null(DestinationType)
+    batchApi = BatchApiDestination
+
+
 class DatasetTableColumn(Type):
     name = non_null(str)
 
+
 class TableEdgeOnColumns(Type):
     fromColumnName = non_null(str)
     toColumnName = non_null(str)
 
+
 class TableEdge(Type):
     name = non_null(str)
     fromTableId = non_null(str)
     toTableId = non_null(str)
     onColumns = non_null(list_of(non_null(TableEdgeOnColumns)))
     unique = bool
 
+
+class ColumnMappingInput(Input):
+    sourceColumn = non_null(str)
+    destinationField = non_null(str)
+
+
+class TableMappingInput(Input):
+    tableId = non_null(str)
+    mappedTableName = str
+    columnMappings = list_of(non_null(ColumnMappingInput))
+
+
+class TableMapping(Type):
+    tableId = non_null(str)
+    mappedTableName = str
+    mapping = list_of(non_null(TableMappingInput))
+
+
 class DatasetTable(Type):
     id = non_null(str)
     qualifiedTableIdentifier = non_null(str)
     name = non_null(str)
     primaryKey = non_null(list_of(non_null(DatasetTableColumn)))
     tableState = non_null(TableStateEnum)
     lastRowCount = int
     edges = list_of(non_null(TableEdge))
     lastSyncAt = DateTime
     lastCdcSuccessTimeAgo = str
 
+
+class DatasetDestination(Type):
+    name = non_null(str)
+    mapping = list_of(non_null(TableMapping))
+    destination = non_null(Destination)
+
+
+class DatasetDestinationInput(Input):
+    name = non_null(str)
+    mapping = list_of(non_null(TableMappingInput))
+
+
 class Dataset(Type):
     id = non_null(str)
     name = non_null(str)
     tables = non_null(list_of(non_null('DatasetTable')))
+    destinations = non_null(list_of(non_null(DatasetDestination)))
 
 
 class QueryAuth(Type):
     accessToken = non_null(str)
 
 
 class DataAccessKey(Type):
@@ -173,14 +240,25 @@
     objectStorage = CreateObjectStorageTableInput
 
 
 class CreateDatasetInput(Input):
     sourceId = non_null(str)
     datasetName = non_null(str)
     tables = non_null(list_of(non_null(CreateDatasetTableInput)))
+    destinations = list_of(non_null(DatasetDestinationInput))
+
+
+class DestinationInput(Input):
+    name = non_null(str)
+    type = non_null(DestinationType)
+    batchApi = BatchApiDestinationInput
+
+
+class RemoveDestinationInput(Input):
+    name = non_null(str)
 
 
 class TableEdgeOnColumnsInput(Input):
     fromColumnName = non_null(str)
     toColumnName = non_null(str)
 
 
@@ -219,14 +297,21 @@
 class SourceConnectionAzureBlobInput(Input):
     name = non_null(str)
     containerName = non_null(str)
     accountName = non_null(str)
     sasToken = str
 
 
+class SourceConnectionDatabricksInput(Input):
+    name = non_null(str)
+    hostname = non_null(str)
+    httpPath = non_null(str)
+    token = non_null(str)
+
+
 class SourceConnectionBigQueryInput(Input):
     name = non_null(str)
     credentialsKey = non_null(str)
     projectId = non_null(str)
     location = str
     dataset = str
     stagingProjectId = non_null(str)
@@ -291,14 +376,19 @@
 
 
 class RemoveDatasetInput(Input):
     sourceId = non_null(str)
     datasetName = non_null(str)
 
 
+class PauseDatasetInput(Input):
+    sourceId = non_null(str)
+    datasetName = non_null(str)
+
+
 class GenerateQueryAuthFilterInput(Input):
     tableName = non_null(str)
     columnName = non_null(str)
     value = non_null(str)
 
 
 class GenerateQueryAuthInput(Input):
@@ -398,14 +488,15 @@
     }))
     datasetByName = Field('Dataset', args=ArgDict({
         'input': 'DatasetByNameInput'
     }))
     datasets = Field(non_null(list_of(non_null('Dataset'))), args=ArgDict({
         'input': 'DatasetsInput'
     }))
+    destinations = Field(non_null(list_of(non_null(Destination))))
     user = Field(non_null('User'), args=ArgDict({
         'id': non_null(str)
     }))
     currentUser = Field(non_null('CurrentUser'))
     recordInspection = Field(non_null('RecordInspection'), args=ArgDict({
         'input': non_null('RecordInspectionInput')
     }))
@@ -423,23 +514,32 @@
 class Mutation(Type):
     sourceConnectAzureBlob = Field(non_null(Source), args=ArgDict({
         'input': non_null(SourceConnectionAzureBlobInput)
     }))
     sourceConnectBigQuery = Field(non_null(Source), args=ArgDict({
         'input': non_null(SourceConnectionBigQueryInput)
     }))
+    sourceConnectDatabricks = Field(non_null(Source), args=ArgDict({
+        'input': non_null(SourceConnectionDatabricksInput)
+    }))
     sourceConnectSnowflake = Field(non_null(Source), args=ArgDict({
         'input': non_null(SourceConnectionSnowflakeInput)
     }))
     sourceDisconnect = Field(non_null(bool), args=ArgDict({
         'input': non_null(SourceDisconnectInput)
     }))
     createDataset = Field(non_null(bool), args=ArgDict({
         'input': non_null(CreateDatasetInput)
     }))
+    createDestination = Field(non_null(Destination), args=ArgDict({
+        'input': non_null(DestinationInput)
+    }))
+    removeDestination = Field(non_null(bool), args=ArgDict({
+        'input': non_null(DestinationInput)
+    }))
     createTableEdge = Field(non_null(bool), args=ArgDict({
         'input': non_null(TableEdgeInput)
     }))
     registerUser = Field(non_null('User'), args=ArgDict({
         'input': non_null('RegisterUserInput')
     }))
     unregisterUser = Field(non_null('User'), args=ArgDict({
@@ -447,14 +547,17 @@
     }))
     updateUser = Field(non_null('User'), args=ArgDict({
         'input': non_null('UpdateUserInput')
     }))
     updateTenant = Field(non_null('Tenant'), args=ArgDict({
         'input': non_null('UpdateTenantInput')
     }))
+    pauseDataset = Field(non_null(bool), args=ArgDict({
+        'input': non_null('PauseDatasetInput')
+    }))
     removeDataset = Field(non_null(bool), args=ArgDict({
         'input': non_null('RemoveDatasetInput')
     }))
     generateQueryAuth = Field(non_null(QueryAuth), args=ArgDict({
         'input': non_null('GenerateQueryAuthInput')
     }))
     generateDataAccessKey = Field(non_null(DataAccessKey), args=ArgDict({
```

### Comparing `patch-cli-0.2.5/src/patch/storage/generic_storage_file.py` & `patch-cli-0.2.6/src/patch/storage/generic_storage_file.py`

 * *Files identical despite different names*

### Comparing `patch-cli-0.2.5/src/patch/storage/storage.py` & `patch-cli-0.2.6/src/patch/storage/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 from appdirs import user_data_dir
 from pathlib import Path
 
 from patch.storage.auth import AuthFileGeneric
 from patch.storage.state_file import StateFile
 
+
 def _require_patch_home(data_dir=None):
     migrate = False
 
     if data_dir is None:
         data_dir = os.environ.get('PATCH_HOME', None)
 
     if data_dir is None or data_dir == "":
@@ -25,14 +26,15 @@
             path = os.path.join(deprecated_data_dir, file)
             if os.path.exists(path):
                 os.rename(path, os.path.join(data_dir, file))
         os.rmdir(deprecated_data_dir)
 
     return data_dir
 
+
 class Storage:
     VENDOR = "patch.tech"
     APPLICATION = "patch-cli"
     DEPRECATED_PATCH_HOME = ".patch-tech"
 
     def __init__(self, location=None):
         self._data_dir = _require_patch_home(location)
@@ -42,8 +44,7 @@
     @property
     def auth(self):
         return self._auth_file
 
     @property
     def source_state(self):
         return self._state_file
-
```

### Comparing `patch-cli-0.2.5/src/patch_cli.egg-info/PKG-INFO` & `patch-cli-0.2.6/src/patch_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patch-cli
-Version: 0.2.5
+Version: 0.2.6
 Summary: Spin up analytics APIs over your data in minutes, without writing any code.
 Home-page: https://www.patch.tech/
 Download-URL: https://docs.patch.tech/command-line-interface/installation
 Author: Patch Enterprises
 Author-email: eng@patch.tech
 Project-URL: Changelog, https://patch.releases.live/
 Project-URL: Documentation, https://docs.patch.tech/command-line-interface/basic-usage
```

### Comparing `patch-cli-0.2.5/src/patch_cli.egg-info/SOURCES.txt` & `patch-cli-0.2.6/src/patch_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,37 +22,47 @@
 src/patch/cli/phone_number_param_type.py
 src/patch/cli/styled.py
 src/patch/cli/commands/__init__.py
 src/patch/cli/commands/access.py
 src/patch/cli/commands/admin.py
 src/patch/cli/commands/connector.py
 src/patch/cli/commands/dataset.py
+src/patch/cli/commands/destination.py
 src/patch/cli/commands/login.py
+src/patch/cli/commands/logout.py
 src/patch/cli/commands/playground.py
 src/patch/cli/commands/source.py
 src/patch/cli/commands/token.py
 src/patch/cli/commands/user.py
+src/patch/cli/commands/alpha/__init__.py
+src/patch/cli/commands/alpha/package.py
 src/patch/cli/remote/__init__.py
 src/patch/cli/remote/dataset_client.py
 src/patch/cli/remote/source_client.py
 src/patch/cli/tools/__init__.py
 src/patch/cli/tools/base64_encryption.py
+src/patch/cli/tools/config.py
+src/patch/cli/tools/config_interactive.py
 src/patch/cli/tools/config_spec.py
 src/patch/cli/tools/field_spec.py
 src/patch/cli/tools/filters_reader.py
 src/patch/cli/tools/json_reader.py
 src/patch/cli/tools/connectors/__init__.py
 src/patch/cli/tools/connectors/connector_spec.py
-src/patch/cli/tools/connectors/source_config.py
-src/patch/cli/tools/connectors/source_config_interactive.py
 src/patch/cli/tools/connectors/source_config_non_interactive.py
 src/patch/cli/tools/datasets/__init__.py
 src/patch/cli/tools/datasets/curl_renderer.py
 src/patch/cli/tools/datasets/endpoint_renderer.py
 src/patch/cli/tools/datasets/row_table_renderer.py
+src/patch/cli/tools/destinations/__init__.py
+src/patch/cli/tools/destinations/destination_spec.py
+src/patch/cli/tools/state/__init__.py
+src/patch/cli/tools/state/auth_state_transfer.py
+src/patch/cli/tools/state/bi_directional_state_transfer.py
+src/patch/cli/tools/state/state_transfer.py
 src/patch/cli/tools/tables/__init__.py
 src/patch/cli/tools/tables/renders.py
 src/patch/cli/tools/tables/source_app.css
 src/patch/cli/tools/tables/source_app.py
 src/patch/cli/tools/tables/source_data.py
 src/patch/cli/tools/tables/source_metadata_client.py
 src/patch/cli/tools/tables/state_manager.py
@@ -82,14 +92,15 @@
 src/patch/cli/tools/tables/rows/table_row_collection_quota_aware.py
 src/patch/cli/tools/tables/rows/table_with_pk_row_collection.py
 src/patch/gql/__init__.py
 src/patch/gql/client.py
 src/patch/gql/schema.py
 src/patch/storage/__init__.py
 src/patch/storage/auth.py
+src/patch/storage/domain.py
 src/patch/storage/generic_payload.py
 src/patch/storage/generic_storage_file.py
 src/patch/storage/state_file.py
 src/patch/storage/storage.py
 src/patch/tp/__init__.py
 src/patch/tp/phone_number.py
 src/patch_cli.egg-info/PKG-INFO
```

