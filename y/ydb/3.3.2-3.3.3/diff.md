# Comparing `tmp/ydb-3.3.2.tar.gz` & `tmp/ydb-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydb-3.3.2.tar", last modified: Mon May 15 07:42:59 2023, max compression
+gzip compressed data, was "ydb-3.3.3.tar", last modified: Fri May 19 15:22:00 2023, max compression
```

## Comparing `ydb-3.3.2.tar` & `ydb-3.3.3.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.160507 ydb-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-15 07:42:47.000000 ydb-3.3.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-15 07:42:47.000000 ydb-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 07:42:47.000000 ydb-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-15 07:42:59.160507 ydb-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-15 07:42:47.000000 ydb-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 07:42:47.000000 ydb-3.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 07:42:47.000000 ydb-3.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:42:59.160507 ydb-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-15 07:42:52.000000 ydb-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.124506 ydb-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.124506 ydb-3.3.2/tests/aio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/aio/test_async_iter_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/aio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/aio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/aio/test_session_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/aio/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/aio/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/aio/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/session_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.124506 ydb-3.3.2/tests/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/ssl/test_ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.124506 ydb-3.3.2/tests/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/table/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/table/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/test_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.128506 ydb-3.3.2/tests/topics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/topics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/topics/test_control_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/topics/test_topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-15 07:42:47.000000 ydb-3.3.2/tests/topics/test_topic_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.132506 ydb-3.3.2/ydb/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.132506 ydb-3.3.2/ydb/_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.132506 ydb-3.3.2/ydb/_grpc/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.132506 ydb-3.3.2/ydb/_grpc/grpcwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/grpcwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/grpcwrapper/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/grpcwrapper/ydb_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    42486 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/grpcwrapper/ydb_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/grpcwrapper/ydb_topic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.136506 ydb-3.3.2/ydb/_grpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.144506 ydb-3.3.2/ydb/_grpc/v3/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.144506 ydb-3.3.2/ydb/_grpc/v3/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.148506 ydb-3.3.2/ydb/_grpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.152506 ydb-3.3.2/ydb/_grpc/v4/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.152506 ydb-3.3.2/ydb/_grpc/v4/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_session_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_sp_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.152506 ydb-3.3.2/ydb/_topic_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_common/common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_common/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.156507 ydb-3.3.2/ydb/_topic_reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_reader/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_reader/datatypes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_reader/topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_reader/topic_reader_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_reader/topic_reader_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_reader/topic_reader_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.156507 ydb-3.3.2/ydb/_topic_writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_writer/topic_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_writer/topic_writer_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_writer/topic_writer_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_writer/topic_writer_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_topic_writer/topic_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_tx_ctx_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/_utilities_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.156507 ydb-3.3.2/ydb/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/aio/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/auth_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.156507 ydb-3.3.2/ydb/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/dbapi/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/dbapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/default_pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.160507 ydb-3.3.2/ydb/iam/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/iam/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/import_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/scheme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.160507 ydb-3.3.2/ydb/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/sqlalchemy/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-15 07:42:47.000000 ydb-3.3.2/ydb/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 07:42:52.000000 ydb-3.3.2/ydb/ydb_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:42:59.160507 ydb-3.3.2/ydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-15 07:42:59.000000 ydb-3.3.2/ydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-15 07:42:59.000000 ydb-3.3.2/ydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:42:59.000000 ydb-3.3.2/ydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-15 07:42:59.000000 ydb-3.3.2/ydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 07:42:59.000000 ydb-3.3.2/ydb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.013723 ydb-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-19 15:21:46.000000 ydb-3.3.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-19 15:21:46.000000 ydb-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 15:21:46.000000 ydb-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-19 15:22:00.013723 ydb-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-19 15:21:46.000000 ydb-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 15:21:46.000000 ydb-3.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 15:21:46.000000 ydb-3.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:22:00.013723 ydb-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-19 15:21:51.000000 ydb-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.969716 ydb-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.973717 ydb-3.3.3/tests/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_async_iter_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_session_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/session_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.973717 ydb-3.3.3/tests/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/ssl/test_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.973717 ydb-3.3.3/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/table/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/table/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.973717 ydb-3.3.3/tests/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/topics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/topics/test_control_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/topics/test_topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/topics/test_topic_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.977717 ydb-3.3.3/ydb/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.977717 ydb-3.3.3/ydb/_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.977717 ydb-3.3.3/ydb/_grpc/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.981718 ydb-3.3.3/ydb/_grpc/grpcwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42486 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.985719 ydb-3.3.3/ydb/_grpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.993720 ydb-3.3.3/ydb/_grpc/v3/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.993720 ydb-3.3.3/ydb/_grpc/v3/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.997721 ydb-3.3.3/ydb/_grpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.005722 ydb-3.3.3/ydb/_grpc/v4/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.005722 ydb-3.3.3/ydb/_grpc/v4/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_session_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_sp_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.005722 ydb-3.3.3/ydb/_topic_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_common/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_common/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/_topic_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/datatypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/topic_reader_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/topic_reader_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/topic_reader_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/_topic_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_tx_ctx_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_utilities_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/auth_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/dbapi/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/dbapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/default_pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/iam/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/import_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/scheme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.013723 ydb-3.3.3/ydb/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/sqlalchemy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 15:21:51.000000 ydb-3.3.3/ydb/ydb_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.013723 ydb-3.3.3/ydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/top_level.txt
```

### Comparing `ydb-3.3.2/LICENSE` & `ydb-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/PKG-INFO` & `ydb-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.3.2
+Version: 3.3.3
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.3.2/README.md` & `ydb-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/setup.py` & `ydb-3.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for line in r.readlines():
         line = line.strip()
         if line != "":
             requirements.append(line)
 
 setuptools.setup(
     name="ydb",
-    version="3.3.2",  # AUTOVERSION
+    version="3.3.3",  # AUTOVERSION
     description="YDB Python SDK",
     author="Yandex LLC",
     author_email="ydb@yandex-team.ru",
     url="http://github.com/ydb-platform/ydb-python-sdk",
     license="Apache 2.0",
     package_dir={"": "."},
     long_description=long_description,
```

### Comparing `ydb-3.3.2/tests/aio/test_async_iter_stream.py` & `ydb-3.3.3/tests/aio/test_async_iter_stream.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/aio/test_connection.py` & `ydb-3.3.3/tests/aio/test_connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/aio/test_connection_pool.py` & `ydb-3.3.3/tests/aio/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/aio/test_session_pool.py` & `ydb-3.3.3/tests/aio/test_session_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/aio/test_tx.py` & `ydb-3.3.3/tests/aio/test_tx.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/aio/test_types.py` & `ydb-3.3.3/tests/aio/test_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/conftest.py` & `ydb-3.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/session_pool.py` & `ydb-3.3.3/tests/session_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/table/table_test.py` & `ydb-3.3.3/tests/table/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/table/test_tx.py` & `ydb-3.3.3/tests/table/test_tx.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/test_errors.py` & `ydb-3.3.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/topics/test_control_plane.py` & `ydb-3.3.3/tests/topics/test_control_plane.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/topics/test_topic_reader.py` & `ydb-3.3.3/tests/topics/test_topic_reader.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/tests/topics/test_topic_writer.py` & `ydb-3.3.3/tests/topics/test_topic_writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from __future__ import annotations
+
+import asyncio
 from typing import List
 
 import pytest
 
 import ydb.aio
 
 
@@ -92,20 +94,47 @@
         "codec",
         [
             ydb.TopicCodec.RAW,
             ydb.TopicCodec.GZIP,
             None,
         ],
     )
-    async def test_write_encoded(self, driver: ydb.Driver, topic_path: str, codec):
+    async def test_write_encoded(self, driver: ydb.aio.Driver, topic_path: str, codec):
         async with driver.topic_client.writer(topic_path, codec=codec) as writer:
             await writer.write("a" * 1000)
             await writer.write("b" * 1000)
             await writer.write("c" * 1000)
 
+    async def test_create_writer_after_stop(self, driver: ydb.aio.Driver, topic_path: str):
+        await driver.stop()
+        with pytest.raises(ydb.Error):
+            async with driver.topic_client.writer(topic_path) as writer:
+                await writer.write_with_ack("123")
+
+    async def test_send_message_after_stop(self, driver: ydb.aio.Driver, topic_path: str):
+        writer = driver.topic_client.writer(topic_path)
+        await driver.stop()
+        with pytest.raises(ydb.Error):
+            await writer.write_with_ack("123")
+
+    async def test_preserve_exception_on_cm_close(self, driver: ydb.aio.Driver, topic_path: str):
+        class TestException(Exception):
+            pass
+
+        with pytest.raises(TestException):
+            async with driver.topic_client.writer(topic_path) as writer:
+                await writer.wait_init()
+                await driver.stop()  # will raise exception on topic writer __exit__
+
+                # ensure writer has exception internally
+                with pytest.raises((ydb.Error, asyncio.CancelledError)):
+                    await writer.write_with_ack("123")
+
+                raise TestException()
+
 
 class TestTopicWriterSync:
     def test_send_message(self, driver_sync: ydb.Driver, topic_path):
         writer = driver_sync.topic_client.writer(topic_path, producer_id="test")
         writer.write(ydb.TopicWriterMessage(data="123".encode()))
         writer.close()
 
@@ -208,7 +237,34 @@
             writers.append(writer)
 
         for i, writer in enumerate(writers):
             writer.write(str(i))
 
         for writer in writers:
             writer.close()
+
+    def test_create_writer_after_stop(self, driver_sync: ydb.Driver, topic_path: str):
+        driver_sync.stop()
+        with pytest.raises(ydb.Error):
+            with driver_sync.topic_client.writer(topic_path) as writer:
+                writer.write_with_ack("123")
+
+    def test_send_message_after_stop(self, driver_sync: ydb.Driver, topic_path: str):
+        writer = driver_sync.topic_client.writer(topic_path)
+        driver_sync.stop()
+        with pytest.raises(ydb.Error):
+            writer.write_with_ack("123")
+
+    def test_preserve_exception_on_cm_close(self, driver_sync: ydb.Driver, topic_path: str):
+        class TestException(Exception):
+            pass
+
+        with pytest.raises(TestException):
+            with driver_sync.topic_client.writer(topic_path) as writer:
+                writer.wait_init()
+                driver_sync.stop()  # will raise exception on topic writer __exit__
+
+                # ensure writer has exception internally
+                with pytest.raises(ydb.Error):
+                    writer.write_with_ack("123")
+
+                raise TestException()
```

### Comparing `ydb-3.3.2/ydb/__init__.py` & `ydb-3.3.3/ydb/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_apis.py` & `ydb-3.3.3/ydb/_apis.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_errors.py` & `ydb-3.3.3/ydb/_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/common/__init__.py` & `ydb-3.3.3/ydb/_grpc/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/grpcwrapper/common_utils.py` & `ydb-3.3.3/ydb/_grpc/grpcwrapper/common_utils.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/grpcwrapper/ydb_scheme.py` & `ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/grpcwrapper/ydb_topic.py` & `ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py` & `ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/grpcwrapper/ydb_topic_test.py` & `ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/annotations/validation_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_auth_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_cms_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_common_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_coordination_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_discovery_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_export_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_formats_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_import_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_operation_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_scheme_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_scripting_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_table_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_topic_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/protos/ydb_value_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_auth_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_cms_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_coordination_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_discovery_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_export_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_import_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_operation_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_scheme_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_scripting_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_table_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_topic_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/annotations/validation_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_auth_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_cms_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_common_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_coordination_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_discovery_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_export_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_formats_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_import_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_operation_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_scheme_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_scripting_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_table_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_topic_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/protos/ydb_value_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_auth_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_cms_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_coordination_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_discovery_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_export_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_import_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_operation_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_scheme_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_scripting_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_table_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_topic_v1_pb2.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.3/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_session_impl.py` & `ydb-3.3.3/ydb/_session_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_sp_impl.py` & `ydb-3.3.3/ydb/_sp_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_common/common.py` & `ydb-3.3.3/ydb/_topic_common/common.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_common/common_test.py` & `ydb-3.3.3/ydb/_topic_common/common_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_common/test_helpers.py` & `ydb-3.3.3/ydb/_topic_common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_reader/datatypes.py` & `ydb-3.3.3/ydb/_topic_reader/datatypes.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_reader/datatypes_test.py` & `ydb-3.3.3/ydb/_topic_reader/datatypes_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_reader/topic_reader.py` & `ydb-3.3.3/ydb/_topic_reader/topic_reader.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_reader/topic_reader_asyncio.py` & `ydb-3.3.3/ydb/_topic_reader/topic_reader_asyncio.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_reader/topic_reader_asyncio_test.py` & `ydb-3.3.3/ydb/_topic_reader/topic_reader_asyncio_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_reader/topic_reader_sync.py` & `ydb-3.3.3/ydb/_topic_reader/topic_reader_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_writer/topic_writer.py` & `ydb-3.3.3/ydb/_topic_writer/topic_writer.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_writer/topic_writer_asyncio.py` & `ydb-3.3.3/ydb/_topic_writer/topic_writer_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,19 @@
         self._reconnector = WriterAsyncIOReconnector(driver=driver, settings=WriterSettings(settings))
         self._parent = _client
 
     async def __aenter__(self) -> "WriterAsyncIO":
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.close()
+        try:
+            await self.close()
+        except BaseException:
+            if exc_val is None:
+                raise
 
     def __del__(self):
         if self._closed or self._loop.is_closed():
             return
 
         self._loop.call_soon(self.close, False)
 
@@ -326,15 +330,15 @@
 
             res.append(internal_message)
 
         return res
 
     def _check_stop(self):
         if self._stop_reason.done():
-            raise self._stop_reason.result()
+            raise self._stop_reason.exception()
 
     async def _connection_loop(self):
         retry_settings = RetrySettings()  # todo
 
         while True:
             attempt = 0  # todo calc and reset
             tasks = []
@@ -539,15 +543,15 @@
     def _stop(self, reason: BaseException):
         if reason is None:
             raise Exception("writer stop reason can not be None")
 
         if self._stop_reason.done():
             return
 
-        self._stop_reason.set_result(reason)
+        self._stop_reason.set_exception(reason)
 
         for f in self._messages_future:
             f.set_exception(reason)
 
         self._state_changed.set()
         logger.info("Stop topic writer: %s" % reason)
```

### Comparing `ydb-3.3.2/ydb/_topic_writer/topic_writer_asyncio_test.py` & `ydb-3.3.3/ydb/_topic_writer/topic_writer_asyncio_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_topic_writer/topic_writer_sync.py` & `ydb-3.3.3/ydb/_topic_writer/topic_writer_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,19 @@
         self._async_writer = self._caller.safe_call_with_result(create_async_writer(), None)
         self._parent = _parent
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close()
+        try:
+            self.close()
+        except BaseException:
+            if exc_val is None:
+                raise
 
     def __del__(self):
         self.close(flush=False)
 
     def close(self, *, flush: bool = True, timeout: TimeoutType = None):
         if self._closed:
             return
```

### Comparing `ydb-3.3.2/ydb/_topic_writer/topic_writer_test.py` & `ydb-3.3.3/ydb/_topic_writer/topic_writer_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_tx_ctx_impl.py` & `ydb-3.3.3/ydb/_tx_ctx_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/_utilities.py` & `ydb-3.3.3/ydb/_utilities.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/aio/connection.py` & `ydb-3.3.3/ydb/aio/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/aio/credentials.py` & `ydb-3.3.3/ydb/aio/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/aio/driver.py` & `ydb-3.3.3/ydb/aio/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/aio/iam.py` & `ydb-3.3.3/ydb/aio/iam.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/aio/pool.py` & `ydb-3.3.3/ydb/aio/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,16 @@
         rpc_name,
         wrap_result=None,
         settings=None,
         wrap_args=(),
         preferred_endpoint=None,
         fast_fail=False,
     ):
+        if self._stopped:
+            raise issues.Error("Driver was stopped")
         wait_timeout = settings.timeout if settings else 10
         try:
             connection = await self._store.get(preferred_endpoint, fast_fail=fast_fail, wait_timeout=wait_timeout)
         except Exception:
             self._discovery.notify_disconnected()
             raise
```

### Comparing `ydb-3.3.2/ydb/aio/resolver.py` & `ydb-3.3.3/ydb/aio/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/aio/scheme.py` & `ydb-3.3.3/ydb/aio/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/aio/table.py` & `ydb-3.3.3/ydb/aio/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/connection.py` & `ydb-3.3.3/ydb/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/convert.py` & `ydb-3.3.3/ydb/convert.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/credentials.py` & `ydb-3.3.3/ydb/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/dbapi/__init__.py` & `ydb-3.3.3/ydb/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/dbapi/connection.py` & `ydb-3.3.3/ydb/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/dbapi/cursor.py` & `ydb-3.3.3/ydb/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/dbapi/errors.py` & `ydb-3.3.3/ydb/dbapi/errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/default_pem.py` & `ydb-3.3.3/ydb/default_pem.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/driver.py` & `ydb-3.3.3/ydb/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/export.py` & `ydb-3.3.3/ydb/export.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/global_settings.py` & `ydb-3.3.3/ydb/global_settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/iam/auth.py` & `ydb-3.3.3/ydb/iam/auth.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/import_client.py` & `ydb-3.3.3/ydb/import_client.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/interceptor.py` & `ydb-3.3.3/ydb/interceptor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/issues.py` & `ydb-3.3.3/ydb/issues.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/operation.py` & `ydb-3.3.3/ydb/operation.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/pool.py` & `ydb-3.3.3/ydb/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,14 +425,17 @@
         :param wrap_result: A callable that intercepts call and wraps received response
         :param settings: An instance of BaseRequestSettings that can be used
         for RPC metadata construction
         :param wrap_args: And arguments to be passed into wrap_result callable
 
         :return: A result of computation
         """
+        if self._stopped:
+            raise issues.Error("Driver was stopped")
+
         tracing.trace(self.tracer, {"request": request, "stub": stub, "rpc_name": rpc_name})
         try:
             connection = self._store.get(preferred_endpoint)
         except Exception:
             self._discovery_thread.notify_disconnected()
             raise
```

### Comparing `ydb-3.3.2/ydb/resolver.py` & `ydb-3.3.3/ydb/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/scheme.py` & `ydb-3.3.3/ydb/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/scheme_test.py` & `ydb-3.3.3/ydb/scheme_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/scripting.py` & `ydb-3.3.3/ydb/scripting.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/settings.py` & `ydb-3.3.3/ydb/settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/sqlalchemy/__init__.py` & `ydb-3.3.3/ydb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/sqlalchemy/types.py` & `ydb-3.3.3/ydb/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/table.py` & `ydb-3.3.3/ydb/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/table_test.py` & `ydb-3.3.3/ydb/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/topic.py` & `ydb-3.3.3/ydb/topic.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/tracing.py` & `ydb-3.3.3/ydb/tracing.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb/types.py` & `ydb-3.3.3/ydb/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.2/ydb.egg-info/PKG-INFO` & `ydb-3.3.3/ydb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.3.2
+Version: 3.3.3
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.3.2/ydb.egg-info/SOURCES.txt` & `ydb-3.3.3/ydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

