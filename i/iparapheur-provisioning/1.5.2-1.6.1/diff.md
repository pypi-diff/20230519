# Comparing `tmp/iparapheur-provisioning-1.5.2.tar.gz` & `tmp/iparapheur-provisioning-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.5.2.tar", last modified: Fri May  5 12:31:31 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.6.1.tar", last modified: Fri May 19 18:25:52 2023, max compression
```

## Comparing `iparapheur-provisioning-1.5.2.tar` & `iparapheur-provisioning-1.6.1.tar`

### file list

```diff
@@ -1,116 +1,290 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13664 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.022544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.026544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.026544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.026544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.030544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-05-05 12:30:15.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    30122 2023-05-05 12:30:17.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3694 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     4284 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-05-05 12:30:21.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-05-05 12:30:21.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.030544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     1937 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.030544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)      699 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.030544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13625 2023-05-05 12:30:23.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.030544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-05-05 12:30:23.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11315 2023-05-05 12:30:23.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.030544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-05-05 12:30:21.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.030544 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11335 2023-05-05 12:30:21.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.026544 iparapheur-provisioning-1.5.2/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-05 12:31:30.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5222 2023-05-05 12:31:31.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 12:31:30.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-05 12:31:30.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-05 12:31:30.000000 iparapheur-provisioning-1.5.2/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.022544 iparapheur-provisioning-1.5.2/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-05 12:30:15.000000 iparapheur-provisioning-1.5.2/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-05 12:30:18.000000 iparapheur-provisioning-1.5.2/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-05 12:30:19.000000 iparapheur-provisioning-1.5.2/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-05 12:30:20.000000 iparapheur-provisioning-1.5.2/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-05 12:30:21.000000 iparapheur-provisioning-1.5.2/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-05 12:30:21.000000 iparapheur-provisioning-1.5.2/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-05-05 12:30:21.000000 iparapheur-provisioning-1.5.2/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-05 12:30:24.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:31:31.034544 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-05 12:30:22.000000 iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18951 2023-05-19 18:23:31.000000 iparapheur-provisioning-1.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.645561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.649561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7708 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.649561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks.py
+-rw-r--r--   0 root         (0) root         (0)      284 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-19 18:23:23.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-19 18:23:23.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.653561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-05-19 18:22:59.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/composite_id.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-05-19 18:23:00.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    30318 2023-05-19 18:23:01.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3807 2023-05-19 18:23:02.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-05-19 18:23:02.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_config.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5803 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9051 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_layer.py
+-rw-r--r--   0 root         (0) root         (0)     9078 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    25904 2023-05-19 18:23:09.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2023-05-19 18:23:09.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9363 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4042 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4434 2023-05-19 18:23:12.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-05-19 18:23:12.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-05-19 18:23:13.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     4236 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-05-19 18:23:29.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-05-19 18:23:20.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-05-19 18:23:20.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-05-19 18:23:20.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-19 18:23:18.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-05-19 18:23:17.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-19 18:23:18.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-05-19 18:23:17.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-05-19 18:23:18.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-05-19 18:23:18.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17482 2023-05-19 18:23:26.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-05-19 18:23:29.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-05-19 18:23:25.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-05-19 18:23:26.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-05-19 18:23:29.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-05-19 18:23:28.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-05-19 18:23:25.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-05-19 18:23:25.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-05-19 18:23:29.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/
+-rw-r--r--   0 root         (0) root         (0)      521 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15568 2023-05-19 18:23:26.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15504 2023-05-19 18:23:27.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/
+-rw-r--r--   0 root         (0) root         (0)      483 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15478 2023-05-19 18:23:27.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-05-19 18:23:28.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.669561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-05-19 18:23:15.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-05-19 18:23:15.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.645561 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17214 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.645561 iparapheur-provisioning-1.6.1/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.673561 iparapheur-provisioning-1.6.1/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-19 18:22:59.000000 iparapheur-provisioning-1.6.1/test/test_models/test_composite_id.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-05-19 18:23:00.000000 iparapheur-provisioning-1.6.1/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-19 18:23:01.000000 iparapheur-provisioning-1.6.1/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-19 18:23:02.000000 iparapheur-provisioning-1.6.1/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_config.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_layer.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-19 18:23:09.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-19 18:23:09.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-19 18:23:12.000000 iparapheur-provisioning-1.6.1/test/test_models/test_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-19 18:23:12.000000 iparapheur-provisioning-1.6.1/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-19 18:23:13.000000 iparapheur-provisioning-1.6.1/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.673561 iparapheur-provisioning-1.6.1/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.673561 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.5.2/LICENSE.md` & `iparapheur-provisioning-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.5.2"
+__version__ = "1.6.1"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.5.2/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.5.2".\
+               "SDK Package Version: 1.6.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/desk_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
     body
     """
 
 
     class MetaOapg:
         required = {
+            "ownerIds",
             "name",
             "shortName",
         }
         
         class properties:
             
             
@@ -49,44 +50,38 @@
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
+                    regex=[{
+                        'pattern': r'^[^
+ ]+$',  # noqa: E501
+                    }]
             
             
             class shortName(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
-            id = schemas.StrSchema
-            tenantId = schemas.StrSchema
-            description = schemas.StrSchema
-            folderCreationAllowed = schemas.BoolSchema
-            actionAllowed = schemas.BoolSchema
-            archivingAllowed = schemas.BoolSchema
-            chainAllowed = schemas.BoolSchema
-            parentDeskId = schemas.StrSchema
-        
-            @staticmethod
-            def parentDesk() -> typing.Type['DeskRepresentation']:
-                return DeskRepresentation
             
             
             class ownerIds(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
+                    max_items = 256
+                    min_items = 0
                     items = schemas.StrSchema
             
                 def __new__(
                     cls,
                     _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'ownerIds':
@@ -94,14 +89,26 @@
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
+            id = schemas.StrSchema
+            tenantId = schemas.StrSchema
+            description = schemas.StrSchema
+            folderCreationAllowed = schemas.BoolSchema
+            actionAllowed = schemas.BoolSchema
+            archivingAllowed = schemas.BoolSchema
+            chainAllowed = schemas.BoolSchema
+            parentDeskId = schemas.StrSchema
+        
+            @staticmethod
+            def parentDesk() -> typing.Type['DeskRepresentation']:
+                return DeskRepresentation
             
             
             class owners(
                 schemas.ListSchema
             ):
             
             
@@ -417,24 +424,24 @@
                     )
             
                 def __getitem__(self, i: int) -> 'UserRepresentation':
                     return super().__getitem__(i)
             __annotations__ = {
                 "name": name,
                 "shortName": shortName,
+                "ownerIds": ownerIds,
                 "id": id,
                 "tenantId": tenantId,
                 "description": description,
                 "folderCreationAllowed": folderCreationAllowed,
                 "actionAllowed": actionAllowed,
                 "archivingAllowed": archivingAllowed,
                 "chainAllowed": chainAllowed,
                 "parentDeskId": parentDeskId,
                 "parentDesk": parentDesk,
-                "ownerIds": ownerIds,
                 "owners": owners,
                 "associatedDeskIds": associatedDeskIds,
                 "associatedDesks": associatedDesks,
                 "filterableMetadataIds": filterableMetadataIds,
                 "filterableMetadata": filterableMetadata,
                 "filterableSubtypeIds": filterableSubtypeIds,
                 "filterableSubtypes": filterableSubtypes,
@@ -442,24 +449,28 @@
                 "availableSubtypes": availableSubtypes,
                 "supervisorIds": supervisorIds,
                 "supervisors": supervisors,
                 "delegationManagerIds": delegationManagerIds,
                 "delegationManagers": delegationManagers,
             }
     
+    ownerIds: MetaOapg.properties.ownerIds
     name: MetaOapg.properties.name
     shortName: MetaOapg.properties.shortName
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["shortName"]) -> MetaOapg.properties.shortName: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["ownerIds"]) -> MetaOapg.properties.ownerIds: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["tenantId"]) -> MetaOapg.properties.tenantId: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
@@ -479,17 +490,14 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parentDeskId"]) -> MetaOapg.properties.parentDeskId: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parentDesk"]) -> 'DeskRepresentation': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ownerIds"]) -> MetaOapg.properties.ownerIds: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["owners"]) -> MetaOapg.properties.owners: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["associatedDeskIds"]) -> MetaOapg.properties.associatedDeskIds: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["associatedDesks"]) -> MetaOapg.properties.associatedDesks: ...
@@ -523,26 +531,29 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["delegationManagers"]) -> MetaOapg.properties.delegationManagers: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "shortName", "id", "tenantId", "description", "folderCreationAllowed", "actionAllowed", "archivingAllowed", "chainAllowed", "parentDeskId", "parentDesk", "ownerIds", "owners", "associatedDeskIds", "associatedDesks", "filterableMetadataIds", "filterableMetadata", "filterableSubtypeIds", "filterableSubtypes", "availableSubtypeIds", "availableSubtypes", "supervisorIds", "supervisors", "delegationManagerIds", "delegationManagers", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "shortName", "ownerIds", "id", "tenantId", "description", "folderCreationAllowed", "actionAllowed", "archivingAllowed", "chainAllowed", "parentDeskId", "parentDesk", "owners", "associatedDeskIds", "associatedDesks", "filterableMetadataIds", "filterableMetadata", "filterableSubtypeIds", "filterableSubtypes", "availableSubtypeIds", "availableSubtypes", "supervisorIds", "supervisors", "delegationManagerIds", "delegationManagers", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["shortName"]) -> MetaOapg.properties.shortName: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["ownerIds"]) -> MetaOapg.properties.ownerIds: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["tenantId"]) -> typing.Union[MetaOapg.properties.tenantId, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
@@ -562,17 +573,14 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parentDeskId"]) -> typing.Union[MetaOapg.properties.parentDeskId, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parentDesk"]) -> typing.Union['DeskRepresentation', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ownerIds"]) -> typing.Union[MetaOapg.properties.ownerIds, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["owners"]) -> typing.Union[MetaOapg.properties.owners, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["associatedDeskIds"]) -> typing.Union[MetaOapg.properties.associatedDeskIds, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["associatedDesks"]) -> typing.Union[MetaOapg.properties.associatedDesks, schemas.Unset]: ...
@@ -606,33 +614,33 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["delegationManagers"]) -> typing.Union[MetaOapg.properties.delegationManagers, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "shortName", "id", "tenantId", "description", "folderCreationAllowed", "actionAllowed", "archivingAllowed", "chainAllowed", "parentDeskId", "parentDesk", "ownerIds", "owners", "associatedDeskIds", "associatedDesks", "filterableMetadataIds", "filterableMetadata", "filterableSubtypeIds", "filterableSubtypes", "availableSubtypeIds", "availableSubtypes", "supervisorIds", "supervisors", "delegationManagerIds", "delegationManagers", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "shortName", "ownerIds", "id", "tenantId", "description", "folderCreationAllowed", "actionAllowed", "archivingAllowed", "chainAllowed", "parentDeskId", "parentDesk", "owners", "associatedDeskIds", "associatedDesks", "filterableMetadataIds", "filterableMetadata", "filterableSubtypeIds", "filterableSubtypes", "availableSubtypeIds", "availableSubtypes", "supervisorIds", "supervisors", "delegationManagerIds", "delegationManagers", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
+        ownerIds: typing.Union[MetaOapg.properties.ownerIds, list, tuple, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         shortName: typing.Union[MetaOapg.properties.shortName, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
         tenantId: typing.Union[MetaOapg.properties.tenantId, str, schemas.Unset] = schemas.unset,
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         folderCreationAllowed: typing.Union[MetaOapg.properties.folderCreationAllowed, bool, schemas.Unset] = schemas.unset,
         actionAllowed: typing.Union[MetaOapg.properties.actionAllowed, bool, schemas.Unset] = schemas.unset,
         archivingAllowed: typing.Union[MetaOapg.properties.archivingAllowed, bool, schemas.Unset] = schemas.unset,
         chainAllowed: typing.Union[MetaOapg.properties.chainAllowed, bool, schemas.Unset] = schemas.unset,
         parentDeskId: typing.Union[MetaOapg.properties.parentDeskId, str, schemas.Unset] = schemas.unset,
         parentDesk: typing.Union['DeskRepresentation', schemas.Unset] = schemas.unset,
-        ownerIds: typing.Union[MetaOapg.properties.ownerIds, list, tuple, schemas.Unset] = schemas.unset,
         owners: typing.Union[MetaOapg.properties.owners, list, tuple, schemas.Unset] = schemas.unset,
         associatedDeskIds: typing.Union[MetaOapg.properties.associatedDeskIds, list, tuple, schemas.Unset] = schemas.unset,
         associatedDesks: typing.Union[MetaOapg.properties.associatedDesks, list, tuple, schemas.Unset] = schemas.unset,
         filterableMetadataIds: typing.Union[MetaOapg.properties.filterableMetadataIds, list, tuple, schemas.Unset] = schemas.unset,
         filterableMetadata: typing.Union[MetaOapg.properties.filterableMetadata, list, tuple, schemas.Unset] = schemas.unset,
         filterableSubtypeIds: typing.Union[MetaOapg.properties.filterableSubtypeIds, list, tuple, schemas.Unset] = schemas.unset,
         filterableSubtypes: typing.Union[MetaOapg.properties.filterableSubtypes, list, tuple, schemas.Unset] = schemas.unset,
@@ -644,26 +652,26 @@
         delegationManagers: typing.Union[MetaOapg.properties.delegationManagers, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'DeskDto':
         return super().__new__(
             cls,
             *_args,
+            ownerIds=ownerIds,
             name=name,
             shortName=shortName,
             id=id,
             tenantId=tenantId,
             description=description,
             folderCreationAllowed=folderCreationAllowed,
             actionAllowed=actionAllowed,
             archivingAllowed=archivingAllowed,
             chainAllowed=chainAllowed,
             parentDeskId=parentDeskId,
             parentDesk=parentDesk,
-            ownerIds=ownerIds,
             owners=owners,
             associatedDeskIds=associatedDeskIds,
             associatedDesks=associatedDesks,
             filterableMetadataIds=filterableMetadataIds,
             filterableMetadata=filterableMetadata,
             filterableSubtypeIds=filterableSubtypeIds,
             filterableSubtypes=filterableSubtypes,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class DeskRepresentation(
+class TenantDto(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    body
     """
 
 
     class MetaOapg:
         required = {
             "name",
         }
@@ -46,68 +48,62 @@
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
+                    regex=[{
+                        'pattern': r'^[^
+ ]+$',  # noqa: E501
+                    }]
             id = schemas.StrSchema
-            tenantId = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
-                "tenantId": tenantId,
             }
     
     name: MetaOapg.properties.name
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["tenantId"]) -> MetaOapg.properties.tenantId: ...
-    
-    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "tenantId", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["tenantId"]) -> typing.Union[MetaOapg.properties.tenantId, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "tenantId", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        tenantId: typing.Union[MetaOapg.properties.tenantId, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DeskRepresentation':
+    ) -> 'TenantDto':
         return super().__new__(
             cls,
             *_args,
             name=name,
             id=id,
-            tenantId=tenantId,
             _configuration=_configuration,
             **kwargs,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,147 +20,137 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class MetadataRepresentation(
+class Metadata(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         
         class properties:
             id = schemas.StrSchema
+            key = schemas.StrSchema
+            name = schemas.StrSchema
+            index = schemas.Int32Schema
+        
+            @staticmethod
+            def type() -> typing.Type['MetadataType']:
+                return MetadataType
             
             
-            class name(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 255
-                    min_length = 2
-            
-            
-            class key(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 128
-                    min_length = 1
-            
-            
-            class index(
-                schemas.Int32Base,
-                schemas.IntBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneDecimalMixin
+            class restrictedValues(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
-                    format = 'int32'
-            
+                    items = schemas.StrSchema
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[None, decimal.Decimal, int, ],
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'index':
+                ) -> 'restrictedValues':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
-        
-            @staticmethod
-            def type() -> typing.Type['MetadataType']:
-                return MetadataType
+            
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
             __annotations__ = {
                 "id": id,
-                "name": name,
                 "key": key,
+                "name": name,
                 "index": index,
                 "type": type,
+                "restrictedValues": restrictedValues,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def __getitem__(self, name: typing_extensions.Literal["key"]) -> MetaOapg.properties.key: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["key"]) -> MetaOapg.properties.key: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["index"]) -> MetaOapg.properties.index: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> 'MetadataType': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["restrictedValues"]) -> MetaOapg.properties.restrictedValues: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", "key", "index", "type", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "key", "name", "index", "type", "restrictedValues", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["key"]) -> typing.Union[MetaOapg.properties.key, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["key"]) -> typing.Union[MetaOapg.properties.key, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["index"]) -> typing.Union[MetaOapg.properties.index, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> typing.Union['MetadataType', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["restrictedValues"]) -> typing.Union[MetaOapg.properties.restrictedValues, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", "key", "index", "type", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "key", "name", "index", "type", "restrictedValues", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
         key: typing.Union[MetaOapg.properties.key, str, schemas.Unset] = schemas.unset,
-        index: typing.Union[MetaOapg.properties.index, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
+        index: typing.Union[MetaOapg.properties.index, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         type: typing.Union['MetadataType', schemas.Unset] = schemas.unset,
+        restrictedValues: typing.Union[MetaOapg.properties.restrictedValues, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'MetadataRepresentation':
+    ) -> 'Metadata':
         return super().__new__(
             cls,
             *_args,
             id=id,
-            name=name,
             key=key,
+            name=name,
             index=index,
             type=type,
+            restrictedValues=restrictedValues,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.metadata_type import MetadataType
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_representation.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,21 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class TenantDto(
+class TenantRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-
-    body
     """
 
 
     class MetaOapg:
         required = {
             "name",
         }
@@ -48,14 +46,18 @@
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
+                    regex=[{
+                        'pattern': r'^[^
+ ]+$',  # noqa: E501
+                    }]
             id = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
             }
     
     name: MetaOapg.properties.name
@@ -90,15 +92,15 @@
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'TenantDto':
+    ) -> 'TenantRepresentation':
         return super().__new__(
             cls,
             *_args,
             name=name,
             id=id,
             _configuration=_configuration,
             **kwargs,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/typology_representation.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/typology_representation.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,88 +31,97 @@
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
+        required = {
+            "name",
+        }
         
         class properties:
-            id = schemas.StrSchema
             
             
             class name(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
+                    regex=[{
+                        'pattern': r'^[^
+ ]+$',  # noqa: E501
+                    }]
+            id = schemas.StrSchema
             parentId = schemas.StrSchema
             childrenCount = schemas.Int32Schema
             __annotations__ = {
-                "id": id,
                 "name": name,
+                "id": id,
                 "parentId": parentId,
                 "childrenCount": childrenCount,
             }
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    name: MetaOapg.properties.name
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parentId"]) -> MetaOapg.properties.parentId: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["childrenCount"]) -> MetaOapg.properties.childrenCount: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", "parentId", "childrenCount", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "parentId", "childrenCount", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parentId"]) -> typing.Union[MetaOapg.properties.parentId, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["childrenCount"]) -> typing.Union[MetaOapg.properties.childrenCount, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", "parentId", "childrenCount", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "parentId", "childrenCount", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
+        name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
         parentId: typing.Union[MetaOapg.properties.parentId, str, schemas.Unset] = schemas.unset,
         childrenCount: typing.Union[MetaOapg.properties.childrenCount, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'TypologyRepresentation':
         return super().__new__(
             cls,
             *_args,
-            id=id,
             name=name,
+            id=id,
             parentId=parentId,
             childrenCount=childrenCount,
             _configuration=_configuration,
             **kwargs,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,69 +40,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -136,17 +136,17 @@
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '401': _response_for_401,
     '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
     '201': _response_for_201,
     '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
@@ -210,15 +210,15 @@
         content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Create a tenant
+        Create a new tenant
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
 
         _headers = HTTPHeaderDict()
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,88 +54,88 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
-    '204': _response_for_204,
     '404': _response_for_404,
+    '204': _response_for_204,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,95 +55,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '404': _response_for_404,
-    '200': _response_for_200,
     '401': _response_for_401,
+    '403': _response_for_403,
+    '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
@@ -187,15 +187,15 @@
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Get a tenant
+        Get a full tenant description
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
+    '401': _response_for_401,
     '403': _response_for_403,
     '400': _response_for_400,
-    '404': _response_for_404,
     '200': _response_for_200,
-    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,69 +66,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -142,59 +142,59 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '201': _response_for_201,
-    '507': _response_for_507,
     '409': _response_for_409,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,88 +62,88 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
-    '204': _response_for_204,
     '404': _response_for_404,
+    '204': _response_for_204,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
@@ -187,15 +187,15 @@
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Delete desk
+        Delete a desk
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,95 +63,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '404': _response_for_404,
-    '200': _response_for_200,
     '401': _response_for_401,
+    '403': _response_for_403,
+    '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,135 +74,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '404': _response_for_404,
-    '200': _response_for_200,
     '401': _response_for_401,
-    '507': _response_for_507,
+    '403': _response_for_403,
+    '200': _response_for_200,
     '409': _response_for_409,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.6.1/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/setup.py` & `iparapheur-provisioning-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.5.2"
+VERSION = "1.6.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_typology_representation.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_typology_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_models/test_workflow_definition_sort_by.py` & `iparapheur-provisioning-1.6.1/test/test_models/test_workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/__init__.py` & `iparapheur-provisioning-1.6.1/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenant unit test stubs
-        Create a tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Delete a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
-
-
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Get a tenant  # noqa: E501
+        Edit a tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Edit a tenant  # noqa: E501
+    ApiProvisioningV1AdminTenant unit test stubs
+        Create a new tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Delete desk  # noqa: E501
+        Get a full desk description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Get a full desk description  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Get a full user description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.5.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

