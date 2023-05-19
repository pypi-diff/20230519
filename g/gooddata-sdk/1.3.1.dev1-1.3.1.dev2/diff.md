# Comparing `tmp/gooddata-sdk-1.3.1.dev1.tar.gz` & `tmp/gooddata-sdk-1.3.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-sdk-1.3.1.dev1.tar", last modified: Thu Apr 27 16:08:28 2023, max compression
+gzip compressed data, was "gooddata-sdk-1.3.1.dev2.tar", last modified: Fri May 19 09:30:26 2023, max compression
```

## Comparing `gooddata-sdk-1.3.1.dev1.tar` & `gooddata-sdk-1.3.1.dev2.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.280598 gooddata-sdk-1.3.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-27 16:08:28.280598 gooddata-sdk-1.3.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.268597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.268597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/catalog_service_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.268597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.268597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/responses/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/sql_column.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/entity_model/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/validation/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/validation/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/export/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/export/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/export/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/organization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/organization/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/organization/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/organization/entity_model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/organization/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.272597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/declarative_model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/declarative_model/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/entity_model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/entity_model/user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/content_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.276597 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.280598 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.280598 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/model_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    40057 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.280598 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.280598 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/insight.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.268597 gooddata-sdk-1.3.1.dev1/gooddata_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-27 16:08:28.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-27 16:08:28.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:08:28.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 16:08:28.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 16:08:28.000000 gooddata-sdk-1.3.1.dev1/gooddata_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:08:28.280598 gooddata-sdk-1.3.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-27 16:08:20.000000 gooddata-sdk-1.3.1.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:08:28.280598 gooddata-sdk-1.3.1.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-27 16:08:13.000000 gooddata-sdk-1.3.1.dev1/tests/test_type_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.837524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/catalog_service_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/sql_column.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/entity_model/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/validation/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/export/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/export/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/organization/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/organization/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/organization/entity_model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/organization/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/declarative_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/declarative_model/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/entity_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/entity_model/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/content_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.845523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/model_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.841524 gooddata-sdk-1.3.1.dev2/gooddata_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-19 09:30:26.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-19 09:30:26.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:30:26.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 09:30:26.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 09:30:26.000000 gooddata-sdk-1.3.1.dev2/gooddata_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-19 09:30:19.000000 gooddata-sdk-1.3.1.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:30:26.849523 gooddata-sdk-1.3.1.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-19 09:30:12.000000 gooddata-sdk-1.3.1.dev2/tests/test_type_converter.py
```

### Comparing `gooddata-sdk-1.3.1.dev1/LICENSE.txt` & `gooddata-sdk-1.3.1.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/PKG-INFO` & `gooddata-sdk-1.3.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.3.1.dev1
+Version: 1.3.1.dev2
 Summary: GoodData.CN Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev1
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev2
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-sdk-1.3.1.dev1/README.md` & `gooddata-sdk-1.3.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/__init__.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/base.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/catalog_service_base.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/catalog_service_base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/data_source.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/entity_model/data_source.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/entity_model/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/service.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/data_source/validation/data_source.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/data_source/validation/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/entity.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/entity.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/export/request.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/export/request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/export/service.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/export/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/identifier.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/identifier.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/organization/entity_model/organization.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/organization/entity_model/organization.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/organization/service.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/organization/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/declarative_model/permission.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/declarative_model/permission.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/permission/service.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/permission/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/setting.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/declarative_model/user.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/declarative_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/declarative_model/user_group.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/declarative_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/entity_model/user.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/entity_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/entity_model/user_group.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/entity_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/user/service.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/user/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/content_service.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/content_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import functools
 from pathlib import Path
 from typing import List, Optional, Union
 
 import gooddata_api_client.models as afm_models
+from gooddata_api_client.model.elements_request import ElementsRequest
 from gooddata_sdk.catalog.catalog_service_base import CatalogServiceBase
 from gooddata_sdk.catalog.data_source.validation.data_source import DataSourceValidator
 from gooddata_sdk.catalog.types import ValidObjects
 from gooddata_sdk.catalog.workspace.declarative_model.workspace.analytics_model.analytics_model import (
     CatalogDeclarativeAnalytics,
 )
 from gooddata_sdk.catalog.workspace.declarative_model.workspace.logical_model.ldm import CatalogDeclarativeModel
@@ -23,24 +24,27 @@
 from gooddata_sdk.catalog.workspace.entity_model.graph_objects.graph import (
     CatalogDependentEntitiesRequest,
     CatalogDependentEntitiesResponse,
 )
 from gooddata_sdk.catalog.workspace.model_container import CatalogWorkspaceContent
 from gooddata_sdk.client import GoodDataApiClient
 from gooddata_sdk.compute.model.attribute import Attribute
+from gooddata_sdk.compute.model.base import ObjId
 from gooddata_sdk.compute.model.execution import ExecutionDefinition, compute_model_to_api_model
 from gooddata_sdk.compute.model.filter import Filter
 from gooddata_sdk.compute.model.metric import Metric
 from gooddata_sdk.utils import load_all_entities
 
 ValidObjectTypes = Union[Attribute, Metric, Filter, CatalogLabel, CatalogFact, CatalogMetric]
 
 # Use typing collection types to support python < py3.9
 ValidObjectsInputType = Union[ValidObjectTypes, List[ValidObjectTypes], ExecutionDefinition]
 
+LabelElementsInputType = Union[str, ObjId]
+
 
 class CatalogWorkspaceContentService(CatalogServiceBase):
     # Note on the disabled checking:
     # generated client has issues parsing the vis objects; .. have to avoid return type checks
     #
     # note: the parsing is done lazily so it does not necessarily bomb on the next line but when trying to
     #  access returned object's properties
@@ -517,7 +521,31 @@
                 by_type[_type] = items_of_type
             else:
                 items_of_type = by_type[_type]
 
             items_of_type.add(available["id"])
 
         return by_type
+
+    def get_label_elements(self, workspace_id: str, label_id: LabelElementsInputType) -> List[str]:
+        """
+        Get existing values for a label.
+        Under-the-hood, it basically executes SELECT DISTINCT <label_column_name> from corresponding table.
+        Values are automatically sorted lexicographically.
+
+        Args:
+            workspace_id (str):
+                Workspace identification string e.g. "demo".
+            label_id (str):
+                Label ID. We support string or ObjId types.
+                String may not contain "label/" prefix, we append it if necessary.
+        Returns:
+            list of label values
+        """
+        # API expects ID without type prefix
+        parts = str(label_id).split("/")
+        if len(parts) == 2:
+            label_id = parts[1]
+        request = ElementsRequest(label=label_id)
+        # TODO - fix return type of Paging.next in Backend + add support for this API to SDK
+        values = self._actions_api.compute_label_elements_post(workspace_id, request, _check_return_type=False)
+        return [v["title"] for v in values["elements"]]
```

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/entity_model/workspace.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/entity_model/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/model_container.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/model_container.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/catalog/workspace/service.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/catalog/workspace/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,21 @@
     CatalogDeclarativeWorkspaces,
     get_workspace_folder,
 )
 from gooddata_sdk.catalog.workspace.entity_model.content_objects.workspace_setting import CatalogWorkspaceSetting
 from gooddata_sdk.catalog.workspace.entity_model.user_data_filter import CatalogUserDataFilterDocument
 from gooddata_sdk.catalog.workspace.entity_model.workspace import CatalogWorkspace
 from gooddata_sdk.client import GoodDataApiClient
-from gooddata_sdk.utils import load_all_entities, load_all_entities_dict, read_layout_from_file, write_layout_to_file
+from gooddata_sdk.utils import (
+    create_directory,
+    load_all_entities,
+    load_all_entities_dict,
+    read_layout_from_file,
+    write_layout_to_file,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class CatalogWorkspaceService(CatalogServiceBase):
     def __init__(self, api_client: GoodDataApiClient) -> None:
         super(CatalogWorkspaceService, self).__init__(api_client)
@@ -157,14 +163,23 @@
             pass
 
     def get_workspace_setting(self, workspace_id: str, workspace_setting_id: str) -> CatalogWorkspaceSetting:
         return CatalogWorkspaceSetting.from_api(
             self._entities_api.get_entity_workspace_settings(workspace_id, workspace_setting_id).data
         )
 
+    def list_workspace_settings(self, workspace_id: str) -> List[CatalogWorkspaceSetting]:
+        get_workspace_settings = functools.partial(
+            self._entities_api.get_all_entities_workspace_settings,
+            workspace_id,
+            _check_return_type=False,
+        )
+        workspace_settings = load_all_entities(get_workspace_settings).data
+        return [CatalogWorkspaceSetting.from_api(ws) for ws in workspace_settings]
+
     # Declarative methods - workspaces
 
     def get_declarative_workspaces(self) -> CatalogDeclarativeWorkspaces:
         """Get all workspaces in the current organization in a declarative form.
 
         Args:
             None
@@ -394,16 +409,17 @@
     def generate_localized_workspaces(
         self,
         workspace_id: str,
         to_lang: str,
         to_locale: str,
         from_lang: str = "en",
         translator_func: Optional[Callable] = None,
-        layout_root_path: Path = Path.cwd(),
-        provision_workspace: bool = False,
+        layout_root_path: Optional[Path] = None,
+        provision_workspace: Optional[bool] = False,
+        store_layouts: Optional[bool] = False,
     ) -> None:
         """
         Generate layouts of new workspaces based on the source workspace.
         All texts (titles, ...) will be translated to different languages if requested.
         Translation YAML files are created for each language containing pairs of source and target texts.
         If translation is not requested, source and target texts are identical. Users must translate it manually.
         We recommend to translate using a third party service and polish the result manually.
@@ -411,44 +427,61 @@
         :param workspace_id: ID of source workspace which we clone and translate all texts in it
         :param to_lang: ISO lang name (IETF BCP 47)
         :param to_locale: ISO lang code and country code (IETF BCP 47, e.g. en-US, cs-CZ, ...).
                           Check GoodData documentation for what codes are supported.
         :param from_lang: from which language we are going to translate
         :param translator_func: 3rd party service capable of translating a batch of strings to various languages
         :param layout_root_path: folder, where to store all layout YAML files (of new translated workspaces)
+                                 if empty, they are stored to:
+                                 <CURRENT_DIR>/<LAYOUT_ROOT_FOLDER>/<organization_id>/
+                                   <LAYOUT_WORKSPACES_DIR>/<workspace_id>
+                                 else they are stored to <layout_root_path>/<workspace_id>
+                                 If not empty, the caller is responsible to create the whole directory structure
         :param provision_workspace: Should new workspace for the target language be provisioned?
                                      Including setting of corresponding locales.
+        :param store_layouts: Store declarative layouts of all workspaces to disk
         :return: None
         """
         logger.info(f"generate_localized_workspaces START from_lang={from_lang} to_lang={to_lang}")
-        layout_organization_folder = self.layout_organization_folder(layout_root_path)
-        workspace_folder = get_workspace_folder(workspace_id, layout_organization_folder)
+        workspace_folder = self.create_custom_workspace_folder(workspace_id, layout_root_path)
         translation_file_path = workspace_folder / f"translations_{to_lang}.yml"
         already_translated = self.read_translation_file(translation_file_path)
         # Get current WS and its content definitions
         workspace = self.get_workspace(workspace_id)
         workspace_content = self.get_declarative_workspace(workspace_id)
         # Get all texts from WS definition to be translated. Skip already translated.
         to_translate = self.get_texts_to_translate(workspace, workspace_content, already_translated)
-        # Backup current workspace
-        workspace_content.store_to_disk(workspace_folder)
+        if store_layouts:
+            # Backup current workspace
+            workspace_content.store_to_disk(workspace_folder)
         # Translate, if requested, otherwise fill in already translated or 1:1 copy of original texts
         translated = self.translate_if_requested(
             to_translate, translator_func, to_lang, from_lang, already_translated, translation_file_path
         )
+
         # Create new workspace definition with translated texts
         new_workspace = deepcopy(workspace)
         new_workspace_content = deepcopy(workspace_content)
         self.set_translated_texts(workspace, new_workspace, new_workspace_content, to_lang, translated)
-        workspace_new_folder = get_workspace_folder(new_workspace.id, layout_organization_folder)
-        # Store layouts of new workspace to disk
-        new_workspace_content.store_to_disk(workspace_new_folder)
+        workspace_new_folder = self.create_custom_workspace_folder(new_workspace.id, layout_root_path)
+        if store_layouts:
+            # Store layouts of new workspace to disk
+            new_workspace_content.store_to_disk(workspace_new_folder)
         # Provision new WS if requested
         if provision_workspace:
-            self.provision_workspace_with_locales(new_workspace, new_workspace_content, to_locale)
+            self.provision_workspace_with_locales(workspace_id, new_workspace, new_workspace_content, to_locale)
+
+    def create_custom_workspace_folder(self, workspace_id: str, layout_root_path: Optional[Path]) -> Path:
+        if layout_root_path:
+            workspace_folder = layout_root_path / workspace_id
+        else:
+            layout_organization_folder = self.layout_organization_folder(Path.cwd())
+            workspace_folder = get_workspace_folder(workspace_id, layout_organization_folder)
+        create_directory(workspace_folder)
+        return workspace_folder
 
     @staticmethod
     def translate_in_batches(
         to_translate: Set[str], to_lang: str, from_lang: str, translator_func: Callable, batch_size: int = 100
     ) -> Dict[str, str]:
         start = time()
         # Group the values into batches
@@ -480,22 +513,35 @@
         # Read already existing translation file, if it exists
         already_translated = {}
         if translation_file_path.is_file():
             already_translated = read_layout_from_file(translation_file_path)
         return already_translated
 
     def provision_workspace_with_locales(
-        self, new_workspace: CatalogWorkspace, new_workspace_content: CatalogDeclarativeWorkspaceModel, to_locale: str
+        self,
+        source_workspace_id: str,
+        new_workspace: CatalogWorkspace,
+        new_workspace_content: CatalogDeclarativeWorkspaceModel,
+        to_locale: str,
     ) -> None:
         logger.info(f"Provision workspace with locales workspace_id={new_workspace.id}")
         self.create_or_update(new_workspace)
         self.put_declarative_workspace(new_workspace.id, new_workspace_content)
-        # TODO - remove deletes after the fix is delivered to dev_latest
+        # TODO - uncomment the copy after the fix is fully released
+        #      - list_workspace_settings is failing with 500 error too :-(
+        # Copy settings from source workspace
+        # current_settings = self.list_workspace_settings(source_workspace_id)
+        # for setting in current_settings:
+        #     # TODO - remove delete after the fix is fully released
+        #     self.delete_workspace_setting(new_workspace.id, setting.id)
+        #     self.create_or_update_workspace_setting(new_workspace.id, setting)
+        # TODO - remove deletes after the fix is fully released
         self.delete_workspace_setting(new_workspace.id, "locale")
         self.delete_workspace_setting(new_workspace.id, "formatLocale")
+        # Create/update locale settings to target language
         self.create_or_update_workspace_setting(
             new_workspace.id, CatalogWorkspaceSetting(id="locale", content={"value": to_locale})
         )
         self.create_or_update_workspace_setting(
             new_workspace.id, CatalogWorkspaceSetting(id="formatLocale", content={"value": to_locale})
         )
 
@@ -584,23 +630,26 @@
             for insight in workspace_content.analytics.visualization_objects or []:
                 self.add_title_description(to_translate, insight.title, insight.description)
                 for bucket in insight.content["buckets"]:
                     for item in bucket["items"]:
                         if "measure" in item:
                             if "alias" in item["measure"]:
                                 to_translate.add(item["measure"]["alias"])
-        if workspace_content.analytics:
             for dashboard in workspace_content.analytics.analytical_dashboards or []:
                 self.add_title_description(to_translate, dashboard.title, dashboard.description)
                 # Hack: translate titles in free-form, which is not processed intentionally by this SDK
                 for section in dashboard.content["layout"]["sections"]:
                     for item in section["items"]:
                         title = item["widget"]["title"]
                         description = item["widget"]["description"]
                         self.add_title_description(to_translate, title, description)
+                    if "header" in section:
+                        title = section["header"]["title"]
+                        description = section["header"]["description"]
+                        self.add_title_description(to_translate, title, description)
 
         # Translate texts, which have not been translated yet
         if already_translated:
             to_translate = to_translate - set(already_translated.keys())
         return to_translate
 
     def set_translated_texts(
@@ -635,23 +684,26 @@
             for insight in new_workspace_content.analytics.visualization_objects or []:
                 self.set_title_description(insight, translated)
                 for bucket in insight.content["buckets"]:
                     for item in bucket["items"]:
                         if "measure" in item:
                             if "alias" in item["measure"]:
                                 item["measure"]["alias"] = translated[item["measure"]["alias"]]
-        if new_workspace_content.analytics:
             for dashboard in new_workspace_content.analytics.analytical_dashboards or []:
                 self.set_title_description(dashboard, translated)
                 # Hack: translate titles in free-form, which is not processed intentionally by this SDK
                 for section in dashboard.content["layout"]["sections"]:
                     for item in section["items"]:
                         item["widget"]["title"] = translated[item["widget"]["title"]]
                         if item["widget"]["description"]:
                             item["widget"]["description"] = translated[item["widget"]["description"]]
+                    if "header" in section:
+                        section["header"]["title"] = translated[section["header"]["title"]]
+                        if section["header"]["description"]:
+                            section["header"]["description"] = translated[section["header"]["description"]]
 
     # Declarative methods - workspace data filters
 
     def get_declarative_workspace_data_filters(self) -> CatalogDeclarativeWorkspaceDataFilters:
         """Retrieve a workspace data filers layout.
 
         Args:
```

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/client.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/attribute.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/attribute.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/base.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/execution.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/execution.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/filter.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/model/metric.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/model/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/compute/service.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/compute/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/insight.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/insight.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/sdk.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/support.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/support.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/table.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/type_converter.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/type_converter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk/utils.py` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk.egg-info/PKG-INFO` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.3.1.dev1
+Version: 1.3.1.dev2
 Summary: GoodData.CN Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev1
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.3.1.dev2
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-sdk-1.3.1.dev1/gooddata_sdk.egg-info/SOURCES.txt` & `gooddata-sdk-1.3.1.dev2/gooddata_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.3.1.dev1/setup.py` & `gooddata-sdk-1.3.1.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-api-client~=1.3.1.dev1",
+    "gooddata-api-client~=1.3.1.dev2",
     'importlib-metadata >= 1.0 ; python_version >= "3.7"',
     "python-dateutil>=2.5.3",
     "pyyaml>=5.1",
     "attrs==21.4.0",
     "cattrs==22.1.0",
     "brotli==1.0.9",
 ]
 
 
 setup(
     name="gooddata-sdk",
     description="GoodData.CN Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.3.1.dev1",
+    version="1.3.1.dev2",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
     python_requires=">=3.7.0",
     project_urls={
-        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.3.1.dev1",
+        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.3.1.dev2",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```

### Comparing `gooddata-sdk-1.3.1.dev1/tests/test_type_converter.py` & `gooddata-sdk-1.3.1.dev2/tests/test_type_converter.py`

 * *Files identical despite different names*

