# Comparing `tmp/prodvana-0.1.0.tar.gz` & `tmp/prodvana-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.1.0.tar", max compression
+gzip compressed data, was "prodvana-0.1.1.tar", max compression
```

## Comparing `prodvana-0.1.0.tar` & `prodvana-0.1.1.tar`

### file list

```diff
@@ -1,335 +1,336 @@
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.0/prodvana/__init__.py
--rw-r--r--   0        0        0     2708 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.0/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.0/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.0/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0    19183 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    18983 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-05-19 18:33:14.531273 prodvana-0.1.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.0/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     4200 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     4693 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    24873 2023-05-19 18:33:14.691273 prodvana-0.1.0/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16394 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-05-19 18:33:14.531273 prodvana-0.1.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2801 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2294 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.0/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0    13908 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     5071 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.535273 prodvana-0.1.0/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2876 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.535273 prodvana-0.1.0/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     6823 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.535273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2659 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2017 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     3634 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/external_config_pb2.py
--rw-r--r--   0        0        0     4163 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/external_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     5630 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5448 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     1890 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     2541 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     2516 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0    10776 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0     8692 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    13928 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15915 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     1837 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/ref_pb2.py
--rw-r--r--   0        0        0      743 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/ref_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
--rw-r--r--   0        0        0     3229 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2192 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     1490 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     1929 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/version_push_pb2.py
--rw-r--r--   0        0        0     1782 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/version_push_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3576 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4132 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/__init__.py
--rw-r--r--   0        0        0     6840 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/config_pb2.py
--rw-r--r--   0        0        0     6043 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11266 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/manager_pb2.py
--rw-r--r--   0        0        0     7072 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi
--rw-r--r--   0        0        0    10633 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3123 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2566 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/object_pb2.py
--rw-r--r--   0        0        0     1823 2023-05-19 18:33:14.683273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    33432 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    28076 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    18226 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     5259 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    36449 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    61730 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     3895 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     7903 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    17651 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    23424 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    18211 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    14932 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    17792 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     5195 2023-05-19 18:33:14.539273 prodvana-0.1.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     6416 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3627 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    15940 2023-05-19 18:33:14.679273 prodvana-0.1.0/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     3041 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0    14774 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     5507 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1844 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0    16162 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2859 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     7494 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0    10914 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    10003 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2828 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1859 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1425 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     8400 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0     8865 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10471 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     6767 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    10450 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3113 2023-05-19 18:33:14.543273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     6255 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4847 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     3574 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    12153 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12710 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11989 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0     7509 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    13099 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4150 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     2441 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1559 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/extensions_pb2.py
--rw-r--r--   0        0        0     1360 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.pyi
--rw-r--r--   0        0        0     7542 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6671 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1265 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0    10074 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     5498 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     5760 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2655 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-05-19 18:33:14.671273 prodvana-0.1.0/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    30923 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    42140 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    48527 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38025 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    41143 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0    12424 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2934 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     8509 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1530 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/prodvana/template/__init__.py
--rw-r--r--   0        0        0     2429 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/template/service_pb2.py
--rw-r--r--   0        0        0     1768 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/template/service_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/template/service_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     2099 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2255 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     5412 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-05-19 18:33:14.667273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    69010 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    50096 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    55859 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16155 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    21204 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.0/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     4095 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7188 2023-05-19 18:33:14.663273 prodvana-0.1.0/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      562 2023-05-19 18:33:14.663273 prodvana-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 prodvana-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-05-19 18:55:20.232080 prodvana-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.1/prodvana/__init__.py
+-rw-r--r--   0        0        0     2708 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.1/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.1/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.1/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0    19183 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    18983 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-05-19 18:33:14.531273 prodvana-0.1.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.1/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     4200 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     4693 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24873 2023-05-19 18:33:14.691273 prodvana-0.1.1/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16394 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-05-19 18:33:14.531273 prodvana-0.1.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2801 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2294 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.531273 prodvana-0.1.1/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0    13908 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5071 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.535273 prodvana-0.1.1/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2876 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.535273 prodvana-0.1.1/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     6823 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.535273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2659 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2017 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3634 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/external_config_pb2.py
+-rw-r--r--   0        0        0     4163 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/external_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5630 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5448 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1890 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.687273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2541 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2516 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10776 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0     8692 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13928 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15915 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1837 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/ref_pb2.py
+-rw-r--r--   0        0        0      743 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/ref_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3229 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2192 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     1490 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1929 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/version_push_pb2.py
+-rw-r--r--   0        0        0     1782 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/version_push_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3576 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4132 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/__init__.py
+-rw-r--r--   0        0        0     6840 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/config_pb2.py
+-rw-r--r--   0        0        0     6043 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11266 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/manager_pb2.py
+-rw-r--r--   0        0        0     7072 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi
+-rw-r--r--   0        0        0    10633 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3123 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2566 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/object_pb2.py
+-rw-r--r--   0        0        0     1823 2023-05-19 18:33:14.683273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    33432 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    28076 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    18226 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5259 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    36449 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    61730 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3895 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     7903 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    17651 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    23424 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18211 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    14932 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    17792 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5195 2023-05-19 18:33:14.539273 prodvana-0.1.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     6416 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3627 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15940 2023-05-19 18:33:14.679273 prodvana-0.1.1/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     3041 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0    14774 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     5507 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1844 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0    16162 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2859 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     7494 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0    10914 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10003 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2828 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1859 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1425 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8400 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0     8865 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.675273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10471 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     6767 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    10450 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3113 2023-05-19 18:33:14.543273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6255 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4847 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     3574 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12153 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12710 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11989 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0     7509 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    13099 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4150 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     2441 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1559 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/extensions_pb2.py
+-rw-r--r--   0        0        0     1360 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7542 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6671 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1265 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0    10074 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     5498 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     5760 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2655 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-05-19 18:33:14.671273 prodvana-0.1.1/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    30923 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    42140 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    48527 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38025 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    41143 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    12424 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2934 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.547273 prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     8509 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1530 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/prodvana/template/__init__.py
+-rw-r--r--   0        0        0     2429 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/template/service_pb2.py
+-rw-r--r--   0        0        0     1768 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/template/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/template/service_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     2099 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2255 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     4805 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     5412 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-05-19 18:33:14.667273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    69010 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    50096 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    55859 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16155 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    21204 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-05-19 18:33:14.551273 prodvana-0.1.1/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     4095 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7188 2023-05-19 18:33:14.663273 prodvana-0.1.1/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      583 2023-05-19 18:55:43.501187 prodvana-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 prodvana-0.1.1/PKG-INFO
```

### Comparing `prodvana-0.1.0/prodvana/client.py` & `prodvana-0.1.1/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/external_config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/external_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/external_config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/external_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/ref_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/ref_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/version_push_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/version_push_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/common_config/version_push_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/common_config/version_push_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/object_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/delivery_module/object_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/delivery_module/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/runtimes/extensions_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/runtimes/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/template/service_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/template/service_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/template/service_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/template/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/version/source_metadata_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.1.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.1.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.1.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.1.1/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.1.1/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/utils/desired_states.py` & `prodvana-0.1.1/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/utils/service_config.py` & `prodvana-0.1.1/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/prodvana/utils/tests/test_service_config.py` & `prodvana-0.1.1/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.0/pyproject.toml` & `prodvana-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.1.0"
+version = "0.1.1"
 description = "Prodvana's client libraries"
+readme = "README.md"
 authors = []
 
 [tool.poetry.dependencies]
 python = "^3.10"
 protobuf = ">=4.21.0,<5.0"
 types-protobuf = ">=3.20.0,<5.0"
 grpcio = ">=1.48.0,<2.0"
```

### Comparing `prodvana-0.1.0/PKG-INFO` & `prodvana-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prodvana's client libraries
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpc-stubs (>=1.24.0,<2.0)
 Requires-Dist: grpcio (>=1.48.0,<2.0)
 Requires-Dist: protobuf (>=4.21.0,<5.0)
 Requires-Dist: types-protobuf (>=3.20.0,<5.0)
+Description-Content-Type: text/markdown
+
+# Prodvana Python Library
+This library is used to interface with Prodvana APIs.
+
```

