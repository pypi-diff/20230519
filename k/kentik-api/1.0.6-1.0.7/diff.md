# Comparing `tmp/kentik-api-1.0.6.tar.gz` & `tmp/kentik-api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kentik-api-1.0.6.tar", last modified: Fri Mar 10 23:02:02 2023, max compression
+gzip compressed data, was "kentik-api-1.0.7.tar", last modified: Fri May 19 03:42:54 2023, max compression
```

## Comparing `kentik-api-1.0.6.tar` & `kentik-api-1.0.7.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.372535 kentik-api-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-10 23:01:28.000000 kentik-api-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-03-10 23:02:02.372535 kentik-api-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-03-10 23:01:28.000000 kentik-api-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.356535 kentik-api-1.0.6/kentik_api/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.356535 kentik-api-1.0.6/kentik_api/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/analytics/data_frame_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/analytics/flatness.py
--rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/analytics/mapped_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.360535 kentik-api-1.0.6/kentik_api/api_calls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/active_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/api_call_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/custom_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/custom_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/device_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/my_kentik_portal.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/query_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/saved_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_calls/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.360535 kentik-api-1.0.6/kentik_api/api_connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_connection/api_call_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_connection/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_connection/api_connector_protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1323 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_connection/retryable_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.360535 kentik-api-1.0.6/kentik_api/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/alerting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/batch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/custom_applications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/custom_dimensions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/device_labels_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/devices_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/plans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/query_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/saved_filters_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/sites_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/tenants_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/api_resources/users_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.360535 kentik-api-1.0.6/kentik_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.364535 kentik-api-1.0.6/kentik_api/cloudexport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/cloudexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/cloudexport/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/cloudexport/api_connector_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/cloudexport/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/cloudexport/cloud_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.352535 kentik-api-1.0.6/kentik_api/generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.352535 kentik-api-1.0.6/kentik_api/generated/kentik/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.352535 kentik-api-1.0.6/kentik_api/generated/kentik/cloud_export/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.364535 kentik-api-1.0.6/kentik_api/generated/kentik/cloud_export/v202101beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-03-10 23:01:55.000000 kentik-api-1.0.6/kentik_api/generated/kentik/cloud_export/v202101beta1/cloud_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13005 2023-03-10 23:01:55.000000 kentik-api-1.0.6/kentik_api/generated/kentik/cloud_export/v202101beta1/cloud_export_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.352535 kentik-api-1.0.6/kentik_api/generated/kentik/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.364535 kentik-api-1.0.6/kentik_api/generated/kentik/core/v202303/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-10 23:01:55.000000 kentik-api-1.0.6/kentik_api/generated/kentik/core/v202303/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 23:01:55.000000 kentik-api-1.0.6/kentik_api/generated/kentik/core/v202303/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-10 23:01:55.000000 kentik-api-1.0.6/kentik_api/generated/kentik/core/v202303/user_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 23:01:55.000000 kentik-api-1.0.6/kentik_api/generated/kentik/core/v202303/user_info_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.356535 kentik-api-1.0.6/kentik_api/generated/kentik/synthetics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.364535 kentik-api-1.0.6/kentik_api/generated/kentik/synthetics/v202202/
--rw-r--r--   0 runner    (1001) docker     (123)   100425 2023-03-10 23:01:55.000000 kentik-api-1.0.6/kentik_api/generated/kentik/synthetics/v202202/synthetics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-03-10 23:01:55.000000 kentik-api-1.0.6/kentik_api/generated/kentik/synthetics/v202202/synthetics_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.364535 kentik-api-1.0.6/kentik_api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/internal/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/internal/datetime_zulu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/internal/grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/kentik_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.364535 kentik-api-1.0.6/kentik_api/public/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/custom_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/custom_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/device_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/manual_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/query_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/saved_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/public/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.368535 kentik-api-1.0.6/kentik_api/requests_payload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/batch_operations_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/custom_applications_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/custom_dimensions_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/devices_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/interfaces_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/labels_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/manual_mitigations_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/plans_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/populators_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/queries_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/saved_filters_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/sites_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/tags_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/tenants_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/users_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/requests_payload/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.368535 kentik-api-1.0.6/kentik_api/synthetics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/api_connector_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.372535 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/dns_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/network_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/network_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/page_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/synth_tests/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/synthetics/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.372535 kentik-api-1.0.6/kentik_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/utils/device_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/utils/time_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-10 23:01:28.000000 kentik-api-1.0.6/kentik_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 23:02:02.356535 kentik-api-1.0.6/kentik_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-03-10 23:02:02.000000 kentik-api-1.0.6/kentik_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-03-10 23:02:02.000000 kentik-api-1.0.6/kentik_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 23:02:02.000000 kentik-api-1.0.6/kentik_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-10 23:02:02.000000 kentik-api-1.0.6/kentik_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 23:02:02.000000 kentik-api-1.0.6/kentik_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-03-10 23:01:28.000000 kentik-api-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 23:02:02.372535 kentik-api-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-03-10 23:01:28.000000 kentik-api-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.625487 kentik-api-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 03:42:15.000000 kentik-api-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-19 03:42:54.625487 kentik-api-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-19 03:42:15.000000 kentik-api-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.609487 kentik-api-1.0.7/kentik_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.609487 kentik-api-1.0.7/kentik_api/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/analytics/data_frame_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/analytics/flatness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/analytics/mapped_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.613487 kentik-api-1.0.7/kentik_api/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/active_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/api_call_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/custom_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/custom_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/device_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/my_kentik_portal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/query_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/saved_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_calls/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.613487 kentik-api-1.0.7/kentik_api/api_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_connection/api_call_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_connection/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_connection/api_connector_protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1323 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_connection/retryable_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.613487 kentik-api-1.0.7/kentik_api/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/alerting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/batch_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/custom_applications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/custom_dimensions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/device_labels_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/devices_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/query_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/saved_filters_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/sites_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/tenants_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/api_resources/users_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.613487 kentik-api-1.0.7/kentik_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.613487 kentik-api-1.0.7/kentik_api/cloudexport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/cloudexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/cloudexport/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/cloudexport/api_connector_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/cloudexport/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/cloudexport/cloud_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.605487 kentik-api-1.0.7/kentik_api/generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.609487 kentik-api-1.0.7/kentik_api/generated/kentik/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.609487 kentik-api-1.0.7/kentik_api/generated/kentik/cloud_export/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.613487 kentik-api-1.0.7/kentik_api/generated/kentik/cloud_export/v202101beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-05-19 03:42:47.000000 kentik-api-1.0.7/kentik_api/generated/kentik/cloud_export/v202101beta1/cloud_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13005 2023-05-19 03:42:47.000000 kentik-api-1.0.7/kentik_api/generated/kentik/cloud_export/v202101beta1/cloud_export_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.609487 kentik-api-1.0.7/kentik_api/generated/kentik/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.617487 kentik-api-1.0.7/kentik_api/generated/kentik/core/v202303/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-19 03:42:47.000000 kentik-api-1.0.7/kentik_api/generated/kentik/core/v202303/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 03:42:47.000000 kentik-api-1.0.7/kentik_api/generated/kentik/core/v202303/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-19 03:42:47.000000 kentik-api-1.0.7/kentik_api/generated/kentik/core/v202303/user_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 03:42:47.000000 kentik-api-1.0.7/kentik_api/generated/kentik/core/v202303/user_info_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.609487 kentik-api-1.0.7/kentik_api/generated/kentik/synthetics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.617487 kentik-api-1.0.7/kentik_api/generated/kentik/synthetics/v202202/
+-rw-r--r--   0 runner    (1001) docker     (123)   101245 2023-05-19 03:42:47.000000 kentik-api-1.0.7/kentik_api/generated/kentik/synthetics/v202202/synthetics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-05-19 03:42:47.000000 kentik-api-1.0.7/kentik_api/generated/kentik/synthetics/v202202/synthetics_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.617487 kentik-api-1.0.7/kentik_api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/internal/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/internal/datetime_zulu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/internal/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/kentik_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.617487 kentik-api-1.0.7/kentik_api/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/custom_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/custom_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/device_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/manual_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/query_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/saved_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/public/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.621487 kentik-api-1.0.7/kentik_api/requests_payload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/batch_operations_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/custom_applications_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/custom_dimensions_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/devices_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/interfaces_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/labels_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/manual_mitigations_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/plans_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/populators_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/queries_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/saved_filters_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/sites_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/tags_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/tenants_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/users_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/requests_payload/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.621487 kentik-api-1.0.7/kentik_api/synthetics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/api_connector_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.621487 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/dns_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/network_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/network_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/page_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/synth_tests/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/synthetics/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.625487 kentik-api-1.0.7/kentik_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/utils/device_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/utils/time_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-19 03:42:15.000000 kentik-api-1.0.7/kentik_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:42:54.609487 kentik-api-1.0.7/kentik_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-19 03:42:54.000000 kentik-api-1.0.7/kentik_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-19 03:42:54.000000 kentik-api-1.0.7/kentik_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 03:42:54.000000 kentik-api-1.0.7/kentik_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-19 03:42:54.000000 kentik-api-1.0.7/kentik_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 03:42:54.000000 kentik-api-1.0.7/kentik_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-19 03:42:15.000000 kentik-api-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 03:42:54.625487 kentik-api-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-19 03:42:15.000000 kentik-api-1.0.7/setup.py
```

### Comparing `kentik-api-1.0.6/LICENSE` & `kentik-api-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/PKG-INFO` & `kentik-api-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kentik-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Kentik API SDK
 Author-email: Martin Machacek <martin.machacek@kentik.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -22,102 +22,106 @@
 This is a Python client library for [Kentik APIs](https://kb.kentik.com/v0/Ab09.htm).
 It is distributed as [_kentik-api_ PyPI package](https://pypi.org/project/kentik-api/).
 
 ## Installation with pip
 
 1. Install the library using pip:  
 ```pip3 install kentik-api```
-1. Check installation successful - no errors should be reported:  
+2. Check installation successful - no errors should be reported:
 ```python3 -c "import kentik_api"```
-1. Run an example (optional):
+3. Run an example (optional):
   ```bash
   export KTAPI_AUTH_EMAIL=<your kentik api credentials email>
   export KTAPI_AUTH_TOKEN=<your kentik api credentials token>
   python3 examples/sites_example.py
   ```
 
 ## Getting started
 
 The best way to get started coding with the SDK is to study provided [examples](examples).
 
 Interfaces for manipulating all Kentik API resources are available under the `KentikAPI` object.  
 Every Kentik API resource is represented by a public class, and all related data types are located in the same source
 file or directory as the implementation of the class:
-- [CustomApplication](kentik_apiublic/custom_application.py)
-- [CustomDimension](kentik_apiublic/custom_dimension.py)
-- [DeviceLabel](kentik_apiublic/device_label.py)
-- [Device](kentik_apiublic/device.py)
-- [ManualMitigation](kentik_apiublic/manual_mitigation.py)
-- [Plan](kentik_apiublic/plan.py)
-- [QueryObject](kentik_apiublic/query_object.py)
-- [QuerySQL](kentik_apiublic/query_sql.py)
-- [SavedFilter](kentik_apiublic/saved_filter.py)
-- [Site](kentik_apiublic/site.py)
-- [Synthetic Tests](kentik_api/synthetics/)
-- [Tag](kentik_apiublic/tag.py)
-- [Tenant](kentik_apiublic/tenant.py)
-- [User](kentik_apiublic/user.py)
+- [CustomApplication](kentik_api/public/custom_application.py)
+- [CustomDimension](kentik_api/public/custom_dimension.py)
+- [DeviceLabel](kentik_api/public/device_label.py)
+- [Device](kentik_api/public/device.py)
+- [ManualMitigation](kentik_api/public/manual_mitigation.py)
+- [Plan](kentik_api/public/plan.py)
+- [QueryObject](kentik_api/public/query_object.py)
+- [QuerySQL](kentik_api/public/query_sql.py)
+- [SavedFilter](kentik_api/public/saved_filter.py)
+- [Site](kentik_api/public/site.py)
+- [Synthetic Tests](kentik_api/synthetics)
+- [Tag](kentik_api/public/tag.py)
+- [Tenant](kentik_api/public/tenant.py)
+- [User](kentik_api/public/user.py)
 
 ## Additional utilities available in the `utils` sub-module
 
 ### Authentication support
 
-- `get_credentials`: function for retrieving authentication credentials from the environment or a profile stored on disk.
-  API authentication credentials can be provided via environment variables `KTAPI_AUTH_EMAIL` and `KTAPI_AUTH_TOKEN`
-  or via named profile (specified as argument to the `get_credentials` functions, defaulting to `default`) which is
-  a JSON file with following format:
+- `get_credentials`: function for retrieving authentication credentials from the environment or a profile stored on
+  the disk. API authentication credentials can be provided via environment variables `KTAPI_AUTH_EMAIL` and
+  `KTAPI_AUTH_TOKEN` or via named profile (specified as argument to the `get_credentials` functions, defaulting
+  to `default`) which is a JSON file with following format:
 ```json
 {
   "email": "<email address>",
   "api-key": "<the API key>"
 }
 ```
-Path to the profile file can be provided in `KTAPI_CFG_FILE`. Otherwise it is first searched in
+Path to the profile file can be provided in `KTAPI_CFG_FILE`. Otherwise, it is first searched in
 `${KTAPI_HOME}/<profile_name>` and then in `${HOME}/.kentik/<profile_name>`.
 
 ### Support for caching of device data
 
 The `DeviceCache` class allows caching of device related data obtained from the Kentik API. It internally builds
-index of devices by `name` and by `id`. Devices are represented by the [Device](kentik_apiublic/device.py) class which
+index of devices by `name` and by `id`. Devices are represented by the [Device](kentik_api/public/device.py) class which
 internally builds dictionary of device interfaces  (represented by the `DeviceInterface` class) by `name`.
 
 ## Analytic support
 
 The `analytics` package provides support for processing Kentik time series data using Pandas Dataframes.
 The [pandas](https://pandas.pydata.org) and [PyYAML](https://pyyaml.org/) modules are required by the `analytics`
 sub-module and are automatically installed with the `kentik-api[analytics]` option.
-See [analytics readme](kentik_apinalytics/README.md) for more details.
+See [analytics readme](kentik_api/analytics/README.md) for more details.
 
 ## Available Examples
 
-- [alerting_example.py](exampleslerting_example.py) - create Manual Mitigation
-- [applications_example.py](examplespplications_example.py) - create/update/delete Custom Application
-- [bulk_user_create.py](examplesulk_user_create.py) - create users from YAML file
-- [devices_example.py](examplesevices_example.py) - create/update/get/delete/list Devices
-- [dimensions_example.py](examplesimensions_example.py) - create/update/get/delete/list Custom Dimensions, create/update/delete Populator
-- [labels_example.py](examplesabels_example.py) - create/update/get/delete/list Device Labels
-- [my_kentik_portal_example.py](examplesy_kentik_portal_example.py) - get/list Tenants, create/delete Tenant User
-- [plans_example.py](exampleslans_example.py) - list plans
-- [queries_example.py](examplesueries_example.py) - query for SQL/URL/data/chart
-- [saved_filters_example.py](examplesaved_filters_example.py) - create/update/get/delete/list Saved Filters
-- [sites_example.py](examplesites_example.py) - create/update/get/delete/list Sites
-- [tags_example.py](examplesags_example.py) - create/update/get/delete/list Tags
-- [users_example.py](examplessers_example.py) - create/update/get/delete/list Users
-- [error_handling_example.py](examplesrror_handling_example.py) - handling errors raised by the library
-- [analytics_example_sql.py](examplesnalytics_example_sql.py) - use of `SQLQueryDefinition`, `flatness_analysis` method and the`DeviceCache`
-- [analytics_example_topx.py](examplesnalytics_example_sql.py) - use of `DataQueryDefinition`, `flatness_analysis` method and the`DeviceCache`
-  (see also [analytics readme](kentik_apinalytics/README.md))
-- [synthetics_example.py](examplesynthetics_example.py) - interact with synthetics API
-- [cloud_export_example.py](examplesloud_export_example.py) - interact with cloud export API
+- [alerting_example.py](examples/alerting_example.py) - create Manual Mitigation
+- [applications_example.py](examples/applications_example.py) - create/update/delete Custom Application
+- [bulk_user_create.py](examples/bulk_user_create.py) - create users from YAML file
+- [devices_example.py](examples/devices_example.py) - create/update/get/delete/list Devices
+- [dimensions_example.py](examples/dimensions_example.py) - create/update/get/delete/list Custom Dimensions,
+                                                            create/update/delete Populator
+- [labels_example.py](examples/labels_example.py) - create/update/get/delete/list Device Labels
+- [my_kentik_portal_example.py](examples/my_kentik_portal_example.py) - get/list Tenants, create/delete Tenant User
+- [plans_example.py](examples/plans_example.py) - list plans
+- [queries_example.py](examples/queries_example.py) - query for SQL/URL/data/chart
+- [saved_filters_example.py](examples/saved_filters_example.py) - create/update/get/delete/list Saved Filters
+- [sites_example.py](examples/sites_example.py) - create/update/get/delete/list Sites
+- [tags_example.py](examples/tags_example.py) - create/update/get/delete/list Tags
+- [users_example.py](examples/users_example.py) - create/update/get/delete/list Users
+- [error_handling_example.py](examples/error_handling_example.py) - handling errors raised by the library
+- [analytics_example_sql.py](examples/analytics_example_sql.py) - use of `SQLQueryDefinition`, `flatness_analysis`
+                                                                  methods and the`DeviceCache`
+- [analytics_example_topx.py](examples/analytics_example_sql.py) - use of `DataQueryDefinition`, `flatness_analysis`
+                                                                  methods and the`DeviceCache`
+  (see also [analytics readme](kentik_api/analytics/README.md))
+- [synthetics_example.py](examples/synthetics_example.py) - interact with synthetics API
+- [cloud_export_example.py](examples/cloud_export_example.py) - interact with cloud export API
 
 ## Development
 
 [Instructions for developers](docs/README.md)
 
 ## Open-source libraries
 
 This software uses the following open-source libraries:
 - [dacite](https://pypi.org/project/dacite/) by Konrad Hałas - MIT License
 - [requests](https://pypi.org/project/requests/) by Kenneth Reitz - Apache Software License (Apache 2.0)
-- [typing-extensions](https://pypi.org/project/typing-extensions/) by  Guido van Rossum, Jukka Lehtosalo, Lukasz Langa, Michael Lee - PSFL License
+- [typing-extensions](https://pypi.org/project/typing-extensions/) by  Guido van Rossum, Jukka Lehtosalo, Lukasz Langa,
+                                                                   Michael Lee - PSFL License
 - [pandas](https://pandas.pydata.org) supported by NumFOCUS - BSD 3-Clause License
 - [pyyaml](https://pyyaml.org/) by Ingy döt Net and Kirill Simonov - MIT license
```

### Comparing `kentik-api-1.0.6/README.md` & `kentik-api-1.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,102 +3,106 @@
 This is a Python client library for [Kentik APIs](https://kb.kentik.com/v0/Ab09.htm).
 It is distributed as [_kentik-api_ PyPI package](https://pypi.org/project/kentik-api/).
 
 ## Installation with pip
 
 1. Install the library using pip:  
 ```pip3 install kentik-api```
-1. Check installation successful - no errors should be reported:  
+2. Check installation successful - no errors should be reported:
 ```python3 -c "import kentik_api"```
-1. Run an example (optional):
+3. Run an example (optional):
   ```bash
   export KTAPI_AUTH_EMAIL=<your kentik api credentials email>
   export KTAPI_AUTH_TOKEN=<your kentik api credentials token>
   python3 examples/sites_example.py
   ```
 
 ## Getting started
 
 The best way to get started coding with the SDK is to study provided [examples](examples).
 
 Interfaces for manipulating all Kentik API resources are available under the `KentikAPI` object.  
 Every Kentik API resource is represented by a public class, and all related data types are located in the same source
 file or directory as the implementation of the class:
-- [CustomApplication](kentik_apiublic/custom_application.py)
-- [CustomDimension](kentik_apiublic/custom_dimension.py)
-- [DeviceLabel](kentik_apiublic/device_label.py)
-- [Device](kentik_apiublic/device.py)
-- [ManualMitigation](kentik_apiublic/manual_mitigation.py)
-- [Plan](kentik_apiublic/plan.py)
-- [QueryObject](kentik_apiublic/query_object.py)
-- [QuerySQL](kentik_apiublic/query_sql.py)
-- [SavedFilter](kentik_apiublic/saved_filter.py)
-- [Site](kentik_apiublic/site.py)
-- [Synthetic Tests](kentik_api/synthetics/)
-- [Tag](kentik_apiublic/tag.py)
-- [Tenant](kentik_apiublic/tenant.py)
-- [User](kentik_apiublic/user.py)
+- [CustomApplication](kentik_api/public/custom_application.py)
+- [CustomDimension](kentik_api/public/custom_dimension.py)
+- [DeviceLabel](kentik_api/public/device_label.py)
+- [Device](kentik_api/public/device.py)
+- [ManualMitigation](kentik_api/public/manual_mitigation.py)
+- [Plan](kentik_api/public/plan.py)
+- [QueryObject](kentik_api/public/query_object.py)
+- [QuerySQL](kentik_api/public/query_sql.py)
+- [SavedFilter](kentik_api/public/saved_filter.py)
+- [Site](kentik_api/public/site.py)
+- [Synthetic Tests](kentik_api/synthetics)
+- [Tag](kentik_api/public/tag.py)
+- [Tenant](kentik_api/public/tenant.py)
+- [User](kentik_api/public/user.py)
 
 ## Additional utilities available in the `utils` sub-module
 
 ### Authentication support
 
-- `get_credentials`: function for retrieving authentication credentials from the environment or a profile stored on disk.
-  API authentication credentials can be provided via environment variables `KTAPI_AUTH_EMAIL` and `KTAPI_AUTH_TOKEN`
-  or via named profile (specified as argument to the `get_credentials` functions, defaulting to `default`) which is
-  a JSON file with following format:
+- `get_credentials`: function for retrieving authentication credentials from the environment or a profile stored on
+  the disk. API authentication credentials can be provided via environment variables `KTAPI_AUTH_EMAIL` and
+  `KTAPI_AUTH_TOKEN` or via named profile (specified as argument to the `get_credentials` functions, defaulting
+  to `default`) which is a JSON file with following format:
 ```json
 {
   "email": "<email address>",
   "api-key": "<the API key>"
 }
 ```
-Path to the profile file can be provided in `KTAPI_CFG_FILE`. Otherwise it is first searched in
+Path to the profile file can be provided in `KTAPI_CFG_FILE`. Otherwise, it is first searched in
 `${KTAPI_HOME}/<profile_name>` and then in `${HOME}/.kentik/<profile_name>`.
 
 ### Support for caching of device data
 
 The `DeviceCache` class allows caching of device related data obtained from the Kentik API. It internally builds
-index of devices by `name` and by `id`. Devices are represented by the [Device](kentik_apiublic/device.py) class which
+index of devices by `name` and by `id`. Devices are represented by the [Device](kentik_api/public/device.py) class which
 internally builds dictionary of device interfaces  (represented by the `DeviceInterface` class) by `name`.
 
 ## Analytic support
 
 The `analytics` package provides support for processing Kentik time series data using Pandas Dataframes.
 The [pandas](https://pandas.pydata.org) and [PyYAML](https://pyyaml.org/) modules are required by the `analytics`
 sub-module and are automatically installed with the `kentik-api[analytics]` option.
-See [analytics readme](kentik_apinalytics/README.md) for more details.
+See [analytics readme](kentik_api/analytics/README.md) for more details.
 
 ## Available Examples
 
-- [alerting_example.py](exampleslerting_example.py) - create Manual Mitigation
-- [applications_example.py](examplespplications_example.py) - create/update/delete Custom Application
-- [bulk_user_create.py](examplesulk_user_create.py) - create users from YAML file
-- [devices_example.py](examplesevices_example.py) - create/update/get/delete/list Devices
-- [dimensions_example.py](examplesimensions_example.py) - create/update/get/delete/list Custom Dimensions, create/update/delete Populator
-- [labels_example.py](examplesabels_example.py) - create/update/get/delete/list Device Labels
-- [my_kentik_portal_example.py](examplesy_kentik_portal_example.py) - get/list Tenants, create/delete Tenant User
-- [plans_example.py](exampleslans_example.py) - list plans
-- [queries_example.py](examplesueries_example.py) - query for SQL/URL/data/chart
-- [saved_filters_example.py](examplesaved_filters_example.py) - create/update/get/delete/list Saved Filters
-- [sites_example.py](examplesites_example.py) - create/update/get/delete/list Sites
-- [tags_example.py](examplesags_example.py) - create/update/get/delete/list Tags
-- [users_example.py](examplessers_example.py) - create/update/get/delete/list Users
-- [error_handling_example.py](examplesrror_handling_example.py) - handling errors raised by the library
-- [analytics_example_sql.py](examplesnalytics_example_sql.py) - use of `SQLQueryDefinition`, `flatness_analysis` method and the`DeviceCache`
-- [analytics_example_topx.py](examplesnalytics_example_sql.py) - use of `DataQueryDefinition`, `flatness_analysis` method and the`DeviceCache`
-  (see also [analytics readme](kentik_apinalytics/README.md))
-- [synthetics_example.py](examplesynthetics_example.py) - interact with synthetics API
-- [cloud_export_example.py](examplesloud_export_example.py) - interact with cloud export API
+- [alerting_example.py](examples/alerting_example.py) - create Manual Mitigation
+- [applications_example.py](examples/applications_example.py) - create/update/delete Custom Application
+- [bulk_user_create.py](examples/bulk_user_create.py) - create users from YAML file
+- [devices_example.py](examples/devices_example.py) - create/update/get/delete/list Devices
+- [dimensions_example.py](examples/dimensions_example.py) - create/update/get/delete/list Custom Dimensions,
+                                                            create/update/delete Populator
+- [labels_example.py](examples/labels_example.py) - create/update/get/delete/list Device Labels
+- [my_kentik_portal_example.py](examples/my_kentik_portal_example.py) - get/list Tenants, create/delete Tenant User
+- [plans_example.py](examples/plans_example.py) - list plans
+- [queries_example.py](examples/queries_example.py) - query for SQL/URL/data/chart
+- [saved_filters_example.py](examples/saved_filters_example.py) - create/update/get/delete/list Saved Filters
+- [sites_example.py](examples/sites_example.py) - create/update/get/delete/list Sites
+- [tags_example.py](examples/tags_example.py) - create/update/get/delete/list Tags
+- [users_example.py](examples/users_example.py) - create/update/get/delete/list Users
+- [error_handling_example.py](examples/error_handling_example.py) - handling errors raised by the library
+- [analytics_example_sql.py](examples/analytics_example_sql.py) - use of `SQLQueryDefinition`, `flatness_analysis`
+                                                                  methods and the`DeviceCache`
+- [analytics_example_topx.py](examples/analytics_example_sql.py) - use of `DataQueryDefinition`, `flatness_analysis`
+                                                                  methods and the`DeviceCache`
+  (see also [analytics readme](kentik_api/analytics/README.md))
+- [synthetics_example.py](examples/synthetics_example.py) - interact with synthetics API
+- [cloud_export_example.py](examples/cloud_export_example.py) - interact with cloud export API
 
 ## Development
 
 [Instructions for developers](docs/README.md)
 
 ## Open-source libraries
 
 This software uses the following open-source libraries:
 - [dacite](https://pypi.org/project/dacite/) by Konrad Hałas - MIT License
 - [requests](https://pypi.org/project/requests/) by Kenneth Reitz - Apache Software License (Apache 2.0)
-- [typing-extensions](https://pypi.org/project/typing-extensions/) by  Guido van Rossum, Jukka Lehtosalo, Lukasz Langa, Michael Lee - PSFL License
+- [typing-extensions](https://pypi.org/project/typing-extensions/) by  Guido van Rossum, Jukka Lehtosalo, Lukasz Langa,
+                                                                   Michael Lee - PSFL License
 - [pandas](https://pandas.pydata.org) supported by NumFOCUS - BSD 3-Clause License
 - [pyyaml](https://pyyaml.org/) by Ingy döt Net and Kirill Simonov - MIT license
```

### Comparing `kentik-api-1.0.6/kentik_api/analytics/data_frame_cache.py` & `kentik-api-1.0.7/kentik_api/analytics/data_frame_cache.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/analytics/flatness.py` & `kentik-api-1.0.7/kentik_api/analytics/flatness.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/analytics/mapped_query.py` & `kentik-api-1.0.7/kentik_api/analytics/mapped_query.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/alerts.py` & `kentik-api-1.0.7/kentik_api/api_calls/alerts.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/api_call.py` & `kentik-api-1.0.7/kentik_api/api_calls/api_call.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/api_call_decorators.py` & `kentik-api-1.0.7/kentik_api/api_calls/api_call_decorators.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/batch.py` & `kentik-api-1.0.7/kentik_api/api_calls/batch.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/custom_applications.py` & `kentik-api-1.0.7/kentik_api/api_calls/custom_applications.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/custom_dimensions.py` & `kentik-api-1.0.7/kentik_api/api_calls/custom_dimensions.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/device_labels.py` & `kentik-api-1.0.7/kentik_api/api_calls/device_labels.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/devices.py` & `kentik-api-1.0.7/kentik_api/api_calls/devices.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/my_kentik_portal.py` & `kentik-api-1.0.7/kentik_api/api_calls/my_kentik_portal.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/query_methods.py` & `kentik-api-1.0.7/kentik_api/api_calls/query_methods.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/saved_filters.py` & `kentik-api-1.0.7/kentik_api/api_calls/saved_filters.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/sites.py` & `kentik-api-1.0.7/kentik_api/api_calls/sites.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/tags.py` & `kentik-api-1.0.7/kentik_api/api_calls/tags.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_calls/users.py` & `kentik-api-1.0.7/kentik_api/api_calls/users.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_connection/api_connector.py` & `kentik-api-1.0.7/kentik_api/api_connection/api_connector.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_connection/retryable_session.py` & `kentik-api-1.0.7/kentik_api/api_connection/retryable_session.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/alerting_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/alerting_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/base_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/base_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/batch_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/batch_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/custom_applications_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/custom_applications_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/custom_dimensions_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/custom_dimensions_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/device_labels_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/device_labels_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/devices_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/devices_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/query_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/query_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/saved_filters_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/saved_filters_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/sites_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/sites_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/tags_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/tags_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/tenants_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/tenants_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/api_resources/users_api.py` & `kentik-api-1.0.7/kentik_api/api_resources/users_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/auth/auth.py` & `kentik-api-1.0.7/kentik_api/auth/auth.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/cloudexport/api_connector.py` & `kentik-api-1.0.7/kentik_api/cloudexport/api_connector.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/cloudexport/api_connector_protocol.py` & `kentik-api-1.0.7/kentik_api/cloudexport/api_connector_protocol.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/cloudexport/client.py` & `kentik-api-1.0.7/kentik_api/cloudexport/client.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/cloudexport/cloud_export.py` & `kentik-api-1.0.7/kentik_api/cloudexport/cloud_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import List, Optional
 
 import kentik_api.generated.kentik.cloud_export.v202101beta1.cloud_export_pb2 as pb
 from kentik_api.internal.grpc import DoNotSerializeMarker, SerializableEnum, _ConfigElement
 from kentik_api.public.types import ID
 
 
@@ -99,15 +99,15 @@
     bgp: Optional[BgpProperties] = None  # note: not a cloud provider type
     enabled: bool = True
     id: ID = ID()
 
     # read-only
     _api_root: str = ""
     _flow_dest: str = ""
-    _current_status: Status = Status()
+    _current_status: Status = field(default_factory=Status)
 
     @property
     def current_status(self) -> Status:
         return self._current_status
 
 
 @dataclass
```

### Comparing `kentik-api-1.0.6/kentik_api/generated/kentik/cloud_export/v202101beta1/cloud_export_pb2.py` & `kentik-api-1.0.7/kentik_api/generated/kentik/cloud_export/v202101beta1/cloud_export_pb2.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/generated/kentik/cloud_export/v202101beta1/cloud_export_pb2_grpc.py` & `kentik-api-1.0.7/kentik_api/generated/kentik/cloud_export/v202101beta1/cloud_export_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/generated/kentik/core/v202303/annotations_pb2.py` & `kentik-api-1.0.7/kentik_api/generated/kentik/core/v202303/annotations_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%kentik/core/v202303/annotations.proto\x12\x13kentik.core.v202303\x1a google/protobuf/descriptor.proto*\x95\x01\n\x11ServiceVisibility\x12\x1e\n\x1aSERVICE_VISIBILITY_PRIVATE\x10\x00\x12 \n\x1cSERVICE_VISIBILITY_PROTECTED\x10\x01\x12\x1f\n\x1bSERVICE_VISIBILITY_INTERNAL\x10\x02\x12\x1d\n\x19SERVICE_VISIBILITY_PUBLIC\x10\x03:7\n\rservice_scope\x12\x1f.google.protobuf.ServiceOptions\x18\xfd* \x01(\t:9\n\x0fprivate_service\x12\x1f.google.protobuf.ServiceOptions\x18\xff* \x01(\x08:\\\n\nvisibility\x12\x1f.google.protobuf.ServiceOptions\x18\x82+ \x01(\x0e\x32&.kentik.core.v202303.ServiceVisibility:5\n\x0cmethod_scope\x12\x1e.google.protobuf.MethodOptions\x18\xfe* \x01(\t:7\n\x0eprivate_method\x12\x1e.google.protobuf.MethodOptions\x18\x80+ \x01(\x08:8\n\x0fmethod_category\x12\x1e.google.protobuf.MethodOptions\x18\x81+ \x01(\tBLZJgithub.com/kentik/api-schema-public/gen/go/kentik/core/v202303;kentik_coreb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%kentik/core/v202303/annotations.proto\x12\x13kentik.core.v202303\x1a google/protobuf/descriptor.proto*\x95\x01\n\x11ServiceVisibility\x12\x1e\n\x1aSERVICE_VISIBILITY_PRIVATE\x10\x00\x12 \n\x1cSERVICE_VISIBILITY_PROTECTED\x10\x01\x12\x1f\n\x1bSERVICE_VISIBILITY_INTERNAL\x10\x02\x12\x1d\n\x19SERVICE_VISIBILITY_PUBLIC\x10\x03:7\n\rservice_scope\x12\x1f.google.protobuf.ServiceOptions\x18\xfd* \x01(\t:9\n\x0fprivate_service\x12\x1f.google.protobuf.ServiceOptions\x18\xff* \x01(\x08:\\\n\nvisibility\x12\x1f.google.protobuf.ServiceOptions\x18\x82+ \x01(\x0e\x32&.kentik.core.v202303.ServiceVisibility:5\n\x0cmethod_scope\x12\x1e.google.protobuf.MethodOptions\x18\xfe* \x01(\t:7\n\x0eprivate_method\x12\x1e.google.protobuf.MethodOptions\x18\x80+ \x01(\x08:8\n\x0fmethod_category\x12\x1e.google.protobuf.MethodOptions\x18\x81+ \x01(\t::\n\x11method_permission\x12\x1e.google.protobuf.MethodOptions\x18\x82+ \x01(\tBLZJgithub.com/kentik/api-schema-public/gen/go/kentik/core/v202303;kentik_coreb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kentik.core.v202303.annotations_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(service_scope)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(private_service)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(visibility)
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(method_scope)
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(private_method)
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(method_category)
+  google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(method_permission)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZJgithub.com/kentik/api-schema-public/gen/go/kentik/core/v202303;kentik_core'
   _SERVICEVISIBILITY._serialized_start=97
   _SERVICEVISIBILITY._serialized_end=246
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kentik-api-1.0.6/kentik_api/generated/kentik/core/v202303/user_info_pb2.py` & `kentik-api-1.0.7/kentik_api/generated/kentik/core/v202303/user_info_pb2.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/generated/kentik/synthetics/v202202/synthetics_pb2.py` & `kentik-api-1.0.7/kentik_api/generated/kentik/synthetics/v202202/synthetics_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 from kentik.core.v202303 import annotations_pb2 as kentik_dot_core_dot_v202303_dot_annotations__pb2
 from kentik.core.v202303 import user_info_pb2 as kentik_dot_core_dot_v202303_dot_user__info__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*kentik/synthetics/v202202/synthetics.proto\x12\x19kentik.synthetics.v202202\x1a\x1cgoogle/api/annotations.proto\x1a\x17google/api/client.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a%kentik/core/v202303/annotations.proto\x1a#kentik/core/v202303/user_info.proto\"\xad\r\n\x05\x41gent\x12\x32\n\x02id\x18\x01 \x01(\tB&\xe0\x41\x03\x92\x41 2\x1eUnique identifier of the agent\x12?\n\tsite_name\x18\x02 \x01(\tB,\x92\x41)2\'Name of the site where agent is located\x12O\n\x06status\x18\x03 \x01(\x0e\x32&.kentik.synthetics.v202202.AgentStatusB\x17\x92\x41\x14\x32\x12Operational status\x12?\n\x05\x61lias\x18\x04 \x01(\tB0\x92\x41-2+User selected descriptive name of the agent\x12\x36\n\x04type\x18\x05 \x01(\tB(\xe0\x41\x03\x92\x41\"2 Type of agent (global | private)\x12=\n\x02os\x18\x06 \x01(\tB1\xe0\x41\x03\x92\x41+2)OS version of server/VM hosting the agent\x12\x44\n\x02ip\x18\x07 \x01(\tB8\x18\x01\xe0\x41\x03\x92\x41\x30\x32.Public IP address of the agent (auto-detected)\x12G\n\x03lat\x18\x08 \x01(\x01\x42:\x92\x41\x37\x32\x35Latitude of agent\'s location (signed decimal degrees)\x12I\n\x04long\x18\t \x01(\x01\x42;\x92\x41\x38\x32\x36Longitude of agent\'s location (signed decimal degrees)\x12\\\n\x0blast_authed\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB+\xe0\x41\x03\x92\x41%2#Timestamp of the last authorization\x12\x62\n\x06\x66\x61mily\x18\x0b \x01(\x0e\x32#.kentik.synthetics.v202202.IPFamilyB-\x92\x41*2(IP address family supported by the agent\x12=\n\x03\x61sn\x18\x0c \x01(\rB0\x92\x41-2+ASN of the AS owning agent\'s public address\x12P\n\x07site_id\x18\r \x01(\tB?\x92\x41<2:ID of the site hosting the agent (if configured in Kentik)\x12\x36\n\x07version\x18\x0e \x01(\tB%\xe0\x41\x03\x92\x41\x1f\x32\x1dSoftware version of the agent\x12\x32\n\x04\x63ity\x18\x10 \x01(\tB$\x92\x41!2\x1f\x43ity where the agent is located\x12<\n\x06region\x18\x11 \x01(\tB,\x92\x41)2\'Geographical region of agent\'s location\x12\x31\n\x07\x63ountry\x18\x12 \x01(\tB \x92\x41\x1d\x32\x1b\x43ountry of agent\'s location\x12\x41\n\x08test_ids\x18\x13 \x03(\tB/\xe0\x41\x03\x92\x41)2\'IDs of user\'s test running on the agent\x12\x39\n\x08local_ip\x18\x14 \x01(\tB\'\x18\x01\x92\x41\"2 Internal IP address of the agent\x12\x42\n\x0c\x63loud_region\x18\x16 \x01(\tB,\x92\x41)2\'Cloud region (if any) hosting the agent\x12\x46\n\x0e\x63loud_provider\x18\x17 \x01(\tB.\x92\x41+2)Cloud provider (if any) hosting the agent\x12\x41\n\nagent_impl\x18\x18 \x01(\x0e\x32(.kentik.synthetics.v202202.ImplementTypeB\x03\xe0\x41\x03\x12\x46\n\x06labels\x18\x19 \x03(\tB6\x92\x41\x33\x32\x31List of names of labels associated with the agent\x12\x86\x01\n\x08metadata\x18\x1a \x01(\x0b\x32(.kentik.synthetics.v202202.AgentMetadataBJ\x92\x41G2EAdditional information about agent\'s configuration and run-time state\"\x87\x04\n\rAgentMetadata\x12u\n\x16private_ipv4_addresses\x18\x01 \x03(\x0b\x32\x30.kentik.synthetics.v202202.AgentMetadata.IpValueB#\x92\x41 2\x1eList of private IPv4 addresses\x12v\n\x15public_ipv4_addresses\x18\x02 \x03(\x0b\x32\x30.kentik.synthetics.v202202.AgentMetadata.IpValueB%\xe0\x41\x03\x92\x41\x1f\x32\x1dList of public IPv4 addresses\x12u\n\x16private_ipv6_addresses\x18\x03 \x03(\x0b\x32\x30.kentik.synthetics.v202202.AgentMetadata.IpValueB#\x92\x41 2\x1eList of private IPv6 addresses\x12v\n\x15public_ipv6_addresses\x18\x04 \x03(\x0b\x32\x30.kentik.synthetics.v202202.AgentMetadata.IpValueB%\xe0\x41\x03\x92\x41\x1f\x32\x1dList of public IPv6 addresses\x1a\x18\n\x07IpValue\x12\r\n\x05value\x18\x01 \x01(\t\"\xdf\x05\n\x04Test\x12)\n\x02id\x18\x01 \x01(\tB\x1d\xe0\x41\x03\x92\x41\x17\x32\x15Unique ID of the test\x12\x31\n\x04name\x18\x02 \x01(\tB#\x92\x41 2\x1eUser selected name of the test\x12#\n\x04type\x18\x03 \x01(\tB\x15\x92\x41\x12\x32\x10Type of the test\x12Z\n\x06status\x18\x05 \x01(\x0e\x32%.kentik.synthetics.v202202.TestStatusB#\x92\x41 2\x1eOperational status of the test\x12R\n\x08settings\x18\x06 \x01(\x0b\x32\'.kentik.synthetics.v202202.TestSettingsB\x17\x92\x41\x14\x32\x12Test configuration\x12K\n\x05\x63\x64\x61te\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampB \xe0\x41\x03\x92\x41\x1a\x32\x18\x43reation timestamp (UTC)\x12T\n\x05\x65\x64\x61te\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB)\xe0\x41\x03\x92\x41#2!Last modification timestamp (UTC)\x12S\n\ncreated_by\x18\t \x01(\x0b\x32\x1d.kentik.core.v202303.UserInfoB \xe0\x41\x03\x92\x41\x1a\x32\x18Identity of test creator\x12o\n\x0flast_updated_by\x18\n \x01(\x0b\x32\x1d.kentik.core.v202303.UserInfoB7\xe0\x41\x03\x92\x41\x31\x32/Identity of use that has modified the test last\x12;\n\x06labels\x18\x0b \x03(\tB+\x92\x41(2&Set of labels associated with the test\"\xa6\x0b\n\x0cTestSettings\x12;\n\x08hostname\x18\x01 \x01(\x0b\x32\'.kentik.synthetics.v202202.HostnameTestH\x00\x12/\n\x02ip\x18\x02 \x01(\x0b\x32!.kentik.synthetics.v202202.IpTestH\x00\x12\x35\n\x05\x61gent\x18\x03 \x01(\x0b\x32$.kentik.synthetics.v202202.AgentTestH\x00\x12\x33\n\x04\x66low\x18\x04 \x01(\x0b\x32#.kentik.synthetics.v202202.FlowTestH\x00\x12\x31\n\x03\x64ns\x18\x05 \x01(\x0b\x32\".kentik.synthetics.v202202.DnsTestH\x00\x12\x31\n\x03url\x18\x06 \x01(\x0b\x32\".kentik.synthetics.v202202.UrlTestH\x00\x12\x39\n\x0cnetwork_grid\x18\x07 \x01(\x0b\x32!.kentik.synthetics.v202202.IpTestH\x00\x12<\n\tpage_load\x18\x08 \x01(\x0b\x32\'.kentik.synthetics.v202202.PageLoadTestH\x00\x12\x36\n\x08\x64ns_grid\x18\t \x01(\x0b\x32\".kentik.synthetics.v202202.DnsTestH\x00\x12\x42\n\x0cnetwork_mesh\x18\x12 \x01(\x0b\x32*.kentik.synthetics.v202202.NetworkMeshTestH\x00\x12Q\n\tagent_ids\x18\n \x03(\tB>\x92\x41;29IDs of agents assigned to run tasks on behalf of the test\x12:\n\x05tasks\x18\x0b \x03(\tB+\x92\x41(2&List of task names to run for the test\x12\x99\x01\n\x0fhealth_settings\x18\x0c \x01(\x0b\x32).kentik.synthetics.v202202.HealthSettingsBU\x92\x41R2PHealth evaluation thresholds, acceptable responses and alarm activation settings\x12\x63\n\x04ping\x18\r \x01(\x0b\x32+.kentik.synthetics.v202202.TestPingSettingsB(\x92\x41%2#Ping tasks configuration parameters\x12j\n\x05trace\x18\x0e \x01(\x0b\x32,.kentik.synthetics.v202202.TestTraceSettingsB-\x92\x41*2(Traceroute task configuration parameters\x12\x38\n\x06period\x18\x0f \x01(\rB(\x92\x41%2#Test evaluation period (in seconds)\x12y\n\x06\x66\x61mily\x18\x10 \x01(\x0e\x32#.kentik.synthetics.v202202.IPFamilyBD\x92\x41\x41\x32?IP address family to select from available DNS name resolutions\x12i\n\x15notification_channels\x18\x11 \x03(\tBJ\x92\x41G2EList of IDs of notification channels for alarms triggered by the test\x12\x37\n\x05notes\x18\x13 \x01(\tB(\x92\x41%2#Add a note or comment for this testB\x0c\n\ndefinition\"\x9f\x03\n\x10TestPingSettings\x12\x44\n\x05\x63ount\x18\x01 \x01(\rB5\x92\x41\x32\x32\x30Number of probe packets to send in one iteration\x12=\n\x08protocol\x18\x02 \x01(\tB+\x92\x41(2&Transport protocol to use (icmp | tcp)\x12@\n\x04port\x18\x03 \x01(\rB2\x92\x41/2-Target port for TCP probes (ignored for ICMP)\x12G\n\x07timeout\x18\x04 \x01(\rB6\x92\x41\x33\x32\x31Timeout in milliseconds for execution of the task\x12\x35\n\x05\x64\x65lay\x18\x05 \x01(\x02\x42&\x92\x41#2!Inter-probe delay in milliseconds\x12\x44\n\x04\x64scp\x18\x06 \x01(\rB6\x92\x41\x33\x32\x31\x44SCP code to be set in IP header of probe packets\"\xf5\x03\n\x11TestTraceSettings\x12\x44\n\x05\x63ount\x18\x01 \x01(\rB5\x92\x41\x32\x32\x30Number of probe packets to send in one iteration\x12\x43\n\x08protocol\x18\x02 \x01(\tB1\x92\x41.2,Transport protocol to use (icmp | tcp | udp)\x12G\n\x04port\x18\x03 \x01(\rB9\x92\x41\x36\x32\x34Target port for TCP or UDP probes (ignored for ICMP)\x12G\n\x07timeout\x18\x04 \x01(\rB6\x92\x41\x33\x32\x31Timeout in milliseconds for execution of the task\x12\x46\n\x05limit\x18\x05 \x01(\rB7\x92\x41\x34\x32\x32Maximum number of hops to probe (i.e. maximum TTL)\x12\x35\n\x05\x64\x65lay\x18\x06 \x01(\x02\x42&\x92\x41#2!Inter-probe delay in milliseconds\x12\x44\n\x04\x64scp\x18\x07 \x01(\rB6\x92\x41\x33\x32\x31\x44SCP code to be set in IP header of probe packets\"\x9b\x03\n\x12\x41\x63tivationSettings\x12u\n\x0cgrace_period\x18\x01 \x01(\tB_\x92\x41\\2ZPeriod of healthy status in minutes within the time window not cancelling alarm activation\x12\x44\n\ttime_unit\x18\x02 \x01(\tB1\x92\x41.2,Time unit for specifying time window (m | h)\x12Q\n\x0btime_window\x18\x03 \x01(\tB<\x92\x41\x39\x32\x37Time window for evaluating of test for alarm activation\x12u\n\x05times\x18\x04 \x01(\tBf\x92\x41\x63\x32\x61Number of occurrences of unhealthy test status within the time window triggering alarm activation\"\xd1\x13\n\x0eHealthSettings\x12u\n\x10latency_critical\x18\x01 \x01(\x02\x42[\x92\x41X2VThreshold for ping or DNS response latency (in microseconds) to trigger critical alarm\x12s\n\x0flatency_warning\x18\x02 \x01(\x02\x42Z\x92\x41W2UThreshold for ping or DNS response latency (in microseconds) to trigger warning alarm\x12\x62\n\x14packet_loss_critical\x18\x03 \x01(\x02\x42\x44\x92\x41\x41\x32?Threshold for ping packet loss (in %) to trigger critical alarm\x12`\n\x13packet_loss_warning\x18\x04 \x01(\x02\x42\x43\x92\x41@2>Threshold for ping packet loss (in %) to trigger warning alarm\x12\x63\n\x0fjitter_critical\x18\x05 \x01(\x02\x42J\x92\x41G2EThreshold for ping jitter (in microseconds) to trigger critical alarm\x12\x62\n\x0ejitter_warning\x18\x06 \x01(\x02\x42J\x92\x41G2EThreshold for ping jitter (in microseconds) to trigger critical alarm\x12s\n\x15http_latency_critical\x18\x07 \x01(\x02\x42T\x92\x41Q2OThreshold for HTTP response latency (in microseconds) to trigger critical alarm\x12q\n\x14http_latency_warning\x18\x08 \x01(\x02\x42S\x92\x41P2NThreshold for HTTP response latency (in microseconds) to trigger warning alarm\x12Q\n\x10http_valid_codes\x18\t \x03(\rB7\x92\x41\x34\x32\x32List of HTTP status codes indicating healthy state\x12O\n\x0f\x64ns_valid_codes\x18\n \x03(\rB6\x92\x41\x33\x32\x31List of DNS status codes indicating healthy state\x12\x92\x01\n\x17latency_critical_stddev\x18\x0b \x01(\x02\x42q\x92\x41n2lThreshold for standard deviation (in microseconds) of ping or DNS response latency to trigger critical alarm\x12\x90\x01\n\x16latency_warning_stddev\x18\x0c \x01(\x02\x42p\x92\x41m2kThreshold for standard deviation (in microseconds) of ping or DNS response latency to trigger warning alarm\x12\x80\x01\n\x16jitter_critical_stddev\x18\r \x01(\x02\x42`\x92\x41]2[Threshold for standard deviation of ping jitter (in microseconds) to trigger critical alarm\x12~\n\x15jitter_warning_stddev\x18\x0e \x01(\x02\x42_\x92\x41\\2ZThreshold for standard deviation of ping jitter (in microseconds) to trigger warning alarm\x12\x90\x01\n\x1chttp_latency_critical_stddev\x18\x0f \x01(\x02\x42j\x92\x41g2eThreshold for standard deviation of HTTP response latency (in microseconds) to trigger critical alarm\x12\x8e\x01\n\x1bhttp_latency_warning_stddev\x18\x10 \x01(\x02\x42i\x92\x41\x66\x32\x64Threshold for standard deviation of HTTP response latency (in microseconds) to trigger warning alarm\x12\x92\x01\n\x1bunhealthy_subtest_threshold\x18\x11 \x01(\rBm\x92\x41j2hNumber of tasks (across all agents) that must report unhealthy status in order for alarm to be triggered\x12\x61\n\nactivation\x18\x12 \x01(\x0b\x32-.kentik.synthetics.v202202.ActivationSettingsB\x1e\x92\x41\x1b\x32\x19\x41larm activation settings\x12x\n\x13\x63\x65rt_expiry_warning\x18\x13 \x01(\rB[\x92\x41X2VThreshold for remaining validity of TLS certificate (in days) to trigger warning alarm\x12z\n\x14\x63\x65rt_expiry_critical\x18\x14 \x01(\rB\\\x92\x41Y2WThreshold for remaining validity of TLS certificate (in days) to trigger critical alarm\x12{\n\rdns_valid_ips\x18\x15 \x01(\tBd\x92\x41\x61\x32_Comma separated list of IP addresses expected to be received in response to DNS A or AAAA query\"P\n\x0cHostnameTest\x12@\n\x06target\x18\x01 \x01(\tB0\x92\x41-2+Fully qualified DNS name of the target host\"?\n\x06IpTest\x12\x35\n\x07targets\x18\x01 \x03(\tB$\x92\x41!2\x1fList of IP addresses of targets\"\xab\x01\n\tAgentTest\x12+\n\x06target\x18\x01 \x01(\tB\x1b\x92\x41\x18\x32\x16ID of the target agent\x12q\n\x0cuse_local_ip\x18\x02 \x01(\x08\x42[\x92\x41X2VBoolean value indicating whether to use local (private) IP address of the target agent\"\xa9\x06\n\x08\x46lowTest\x12\x7f\n\x06target\x18\x01 \x01(\tBo\x92\x41l2jTarget ASN, CDN, Country, Region of City for autonomous test (type of value depends on flow test sub-type)\x12\x81\x01\n\x1etarget_refresh_interval_millis\x18\x02 \x01(\rBY\x92\x41V2TPeriod (in milliseconds) for refreshing list of targets based on available flow data\x12P\n\rmax_providers\x18\x03 \x01(\rB9\x92\x41\x36\x32\x34Maximum number of IP providers to track autonomously\x12\x62\n\x0emax_ip_targets\x18\x04 \x01(\rBJ\x92\x41G2EMaximum number of target IP addresses to select based flow data query\x12Q\n\x04type\x18\x05 \x01(\tBC\x92\x41@2>Autonomous test sub-type (asn | cdn | country | region | city)\x12\x99\x01\n\x0einet_direction\x18\x06 \x01(\tB\x80\x01\x92\x41}2{Selection of address from flow data (src = source address in inbound flows | dst = destination addresses in outbound flows)\x12s\n\tdirection\x18\x07 \x01(\tB`\x92\x41]2[Direction of flows to match target attribute for extraction of target addresses (src | dst)\"\xc3\x02\n\x07\x44nsTest\x12\x36\n\x06target\x18\x01 \x01(\tB&\x92\x41#2!Fully qualified DNS name to query\x12=\n\x07timeout\x18\x02 \x01(\rB,\x18\x01\x92\x41\'2%--- Deprecated: value is ignored. ---\x12[\n\x0brecord_type\x18\x03 \x01(\x0e\x32$.kentik.synthetics.v202202.DNSRecordB \x92\x41\x1d\x32\x1bType of DNS record to query\x12\x39\n\x07servers\x18\x04 \x03(\tB(\x92\x41%2#List of IP addresses of DNS servers\x12)\n\x04port\x18\x05 \x01(\rB\x1b\x92\x41\x18\x32\x16Target DNS server port\"\x81\x04\n\x07UrlTest\x12\x31\n\x06target\x18\x01 \x01(\tB!\x92\x41\x1e\x32\x1cHTTP or HTTPS URL to request\x12@\n\x07timeout\x18\x02 \x01(\rB/\x92\x41,2*HTTP transaction timeout (in milliseconds)\x12I\n\x06method\x18\x03 \x01(\tB9\x92\x41\x36\x32\x34HTTP method to use (GET | HEAD | PATCH | POST | PUT)\x12v\n\x07headers\x18\x04 \x03(\x0b\x32/.kentik.synthetics.v202202.UrlTest.HeadersEntryB4\x92\x41\x31\x32/Map of HTTP header values keyed by header names\x12$\n\x04\x62ody\x18\x05 \x01(\tB\x16\x92\x41\x13\x32\x11HTTP request body\x12h\n\x11ignore_tls_errors\x18\x06 \x01(\x08\x42M\x92\x41J2HBoolean indicating whether to ignore TLS certificate verification errors\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xda\x04\n\x0cPageLoadTest\x12\x31\n\x06target\x18\x01 \x01(\tB!\x92\x41\x1e\x32\x1cHTTP or HTTPS URL to request\x12@\n\x07timeout\x18\x02 \x01(\rB/\x92\x41,2*HTTP transaction timeout (in milliseconds)\x12{\n\x07headers\x18\x03 \x03(\x0b\x32\x34.kentik.synthetics.v202202.PageLoadTest.HeadersEntryB4\x92\x41\x31\x32/Map of HTTP header values keyed by header names\x12h\n\x11ignore_tls_errors\x18\x04 \x01(\x08\x42M\x92\x41J2HBoolean indicating whether to ignore TLS certificate verification errors\x12\x88\x01\n\rcss_selectors\x18\x05 \x03(\x0b\x32\x39.kentik.synthetics.v202202.PageLoadTest.CssSelectorsEntryB6\x92\x41\x33\x32\x31Map of CSS selector values keyed by selector name\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x33\n\x11\x43ssSelectorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x85\x01\n\x0fNetworkMeshTest\x12r\n\x0cuse_local_ip\x18\x01 \x01(\x08\x42\\\x92\x41Y2WBoolean value indicating whether to use local (private) IP address of the target agents\"\x9b\x02\n\nMetricData\x12-\n\x07\x63urrent\x18\x01 \x01(\rB\x1c\x92\x41\x19\x32\x17\x43urrent value of metric\x12\x33\n\x0brolling_avg\x18\x02 \x01(\rB\x1e\x92\x41\x1b\x32\x19Rolling average of metric\x12L\n\x0erolling_stddev\x18\x03 \x01(\rB4\x92\x41\x31\x32/Rolling average of standard deviation of metric\x12[\n\x06health\x18\x04 \x01(\tBK\x92\x41H2FHealth evaluation status for the metric (healthy | warning | critical)\"\x9e\x01\n\x0ePacketLossData\x12/\n\x07\x63urrent\x18\x01 \x01(\x01\x42\x1e\x92\x41\x1b\x32\x19\x43urrent packet loss value\x12[\n\x06health\x18\x02 \x01(\tBK\x92\x41H2FHealth evaluation status for the metric (healthy | warning | critical)\"\xaa\x03\n\x0bPingResults\x12=\n\x06target\x18\x01 \x01(\tB-\x92\x41*2(Hostname or address of the probed target\x12\x62\n\x0bpacket_loss\x18\x02 \x01(\x0b\x32).kentik.synthetics.v202202.PacketLossDataB\"\x92\x41\x1f\x32\x1dPacket loss metric and health\x12]\n\x07latency\x18\x03 \x01(\x0b\x32%.kentik.synthetics.v202202.MetricDataB%\x92\x41\"2 Packet latency metric and health\x12g\n\x06jitter\x18\x04 \x01(\x0b\x32%.kentik.synthetics.v202202.MetricDataB0\x92\x41-2+Latency jitter (variance) metric and health\x12\x30\n\x06\x64st_ip\x18\x05 \x01(\tB \x92\x41\x1d\x32\x1bIP address of probed target\"\xe5\x01\n\x10HTTPResponseData\x12,\n\x06status\x18\x01 \x01(\rB\x1c\x92\x41\x19\x32\x17HTTP status in response\x12\x38\n\x04size\x18\x02 \x01(\rB*\x92\x41\'2%Total size of  received response body\x12i\n\x04\x64\x61ta\x18\x03 \x01(\tB[\x92\x41X2VDetailed information about transaction timing, connection characteristics and response\"\xc2\x02\n\x0bHTTPResults\x12&\n\x06target\x18\x01 \x01(\tB\x16\x92\x41\x13\x32\x11Target probed URL\x12\x64\n\x07latency\x18\x02 \x01(\x0b\x32%.kentik.synthetics.v202202.MetricDataB,\x92\x41)2\'HTTP response latency metric and health\x12l\n\x08response\x18\x04 \x01(\x0b\x32+.kentik.synthetics.v202202.HTTPResponseDataB-\x92\x41*2(Information about received HTTP response\x12\x37\n\x06\x64st_ip\x18\x05 \x01(\tB\'\x92\x41$2\"IP address of probed target server\"y\n\x0f\x44NSResponseData\x12(\n\x06status\x18\x01 \x01(\rB\x18\x92\x41\x15\x32\x13Received DNS status\x12<\n\x04\x64\x61ta\x18\x02 \x01(\tB.\x92\x41+2)Text rendering of received DNS resolution\"\xba\x02\n\nDNSResults\x12\'\n\x06target\x18\x01 \x01(\tB\x17\x92\x41\x14\x32\x12Queried DNS record\x12\x32\n\x06server\x18\x02 \x01(\tB\"\x92\x41\x1f\x32\x1d\x44NS server used for the query\x12\x63\n\x07latency\x18\x03 \x01(\x0b\x32%.kentik.synthetics.v202202.MetricDataB+\x92\x41(2&DNS response latency metric and health\x12j\n\x08response\x18\x05 \x01(\x0b\x32*.kentik.synthetics.v202202.DNSResponseDataB,\x92\x41)2\'Information about received DNS response\"\xea\x02\n\x0bTaskResults\x12_\n\x04ping\x18\x01 \x01(\x0b\x32&.kentik.synthetics.v202202.PingResultsB\'\x92\x41$2\"Entry containing ping task resultsH\x00\x12_\n\x04http\x18\x02 \x01(\x0b\x32&.kentik.synthetics.v202202.HTTPResultsB\'\x92\x41$2\"Entry containing HTTP task resultsH\x00\x12\\\n\x03\x64ns\x18\x03 \x01(\x0b\x32%.kentik.synthetics.v202202.DNSResultsB&\x92\x41#2!Entry containing DNS task resultsH\x00\x12.\n\x06health\x18\x04 \x01(\tB\x1e\x92\x41\x1b\x32\x19Health status of the taskB\x0b\n\ttask_type\"\x86\x02\n\x0c\x41gentResults\x12\x38\n\x08\x61gent_id\x18\x01 \x01(\tB&\x92\x41#2!ID of the agent providing results\x12Z\n\x06health\x18\x02 \x01(\tBJ\x92\x41G2EOverall health status of all task for the test executed by this agent\x12`\n\x05tasks\x18\x03 \x03(\x0b\x32&.kentik.synthetics.v202202.TaskResultsB)\x92\x41&2$List of results for individual tasks\"\xcb\x02\n\x0bTestResults\x12\x43\n\x07test_id\x18\x01 \x01(\tB2\x92\x41/2-ID of the test for which results are provided\x12\x46\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x1c\x92\x41\x19\x32\x17Results timestamp (UTC)\x12.\n\x06health\x18\x03 \x01(\tB\x1e\x92\x41\x1b\x32\x19Health status of the test\x12\x7f\n\x06\x61gents\x18\x04 \x03(\x0b\x32\'.kentik.synthetics.v202202.AgentResultsBF\x92\x41\x43\x32\x41List of results from agents executing tasks on behalf of the test\"n\n\x05Stats\x12#\n\x07\x61verage\x18\x01 \x01(\x05\x42\x12\x92\x41\x0f\x32\rAverage value\x12\x1f\n\x03min\x18\x02 \x01(\x05\x42\x12\x92\x41\x0f\x32\rMinimum value\x12\x1f\n\x03max\x18\x03 \x01(\x05\x42\x12\x92\x41\x0f\x32\rMaximum value\"\x95\x02\n\x08Location\x12\x39\n\x08latitude\x18\x08 \x01(\x01\x42\'\x92\x41$2\"Latitude in signed decimal degrees\x12;\n\tlongitude\x18\t \x01(\x01\x42(\x92\x41%2#Longitude in signed decimal degrees\x12-\n\x07\x63ountry\x18\x01 \x01(\tB\x1c\x92\x41\x19\x32\x17\x43ountry of the location\x12\x39\n\x06region\x18\x02 \x01(\tB)\x92\x41&2$Geographic region within the country\x12\'\n\x04\x63ity\x18\x03 \x01(\tB\x19\x92\x41\x16\x32\x14\x43ity of the location\"\xd0\x04\n\x07NetNode\x12\x44\n\x02ip\x18\x02 \x01(\tB8\x92\x41\x35\x32\x33IP address of the node in standard textual notation\x12:\n\x03\x61sn\x18\x03 \x01(\rB-\x92\x41*2(AS number owning the address of the node\x12\x43\n\x07\x61s_name\x18\x04 \x01(\tB2\x92\x41/2-Name of the AS owning the address of the node\x12^\n\x08location\x18\x05 \x01(\x0b\x32#.kentik.synthetics.v202202.LocationB\'\x92\x41$2\"Location of IP address of the node\x12P\n\x08\x64ns_name\x18\x06 \x01(\tB>\x92\x41;29DNS name of the node (obtained by reverse DNS resolution)\x12\\\n\tdevice_id\x18\x07 \x01(\tBI\x92\x41\x46\x32\x44ID of the device corresponding with the node in Kentik configuration\x12n\n\x07site_id\x18\x08 \x01(\tB]\x92\x41Z2XID of the site containing the device corresponding with the node in Kentik configuration\"\xe2\x01\n\x08TraceHop\x12m\n\x07latency\x18\x03 \x01(\x05\x42\\\x92\x41Y2WRound-trip packet latency to the node (in microseconds) - 0 if no response was received\x12g\n\x07node_id\x18\x05 \x01(\tBV\x92\x41S2QID of the node for this hop in the Nodes map  - empty if no response was received\"\xe2\x01\n\tPathTrace\x12\x32\n\x07\x61s_path\x18\x01 \x03(\x05\x42!\x92\x41\x1e\x32\x1c\x41S path of the network trace\x12N\n\x0bis_complete\x18\x02 \x01(\x08\x42\x39\x92\x41\x36\x32\x34Indication whether response from target was received\x12Q\n\x04hops\x18\x06 \x03(\x0b\x32#.kentik.synthetics.v202202.TraceHopB\x1e\x92\x41\x1b\x32\x19List of hops in the trace\"\xec\x03\n\x04Path\x12?\n\x08\x61gent_id\x18\x01 \x01(\tB-\x92\x41*2(ID of the agent generating the path data\x12<\n\ttarget_ip\x18\x03 \x01(\tB)\x92\x41&2$IP address of the target of the path\x12`\n\thop_count\x18\x04 \x01(\x0b\x32 .kentik.synthetics.v202202.StatsB+\x92\x41(2&Hop count statistics across all traces\x12L\n\x12max_as_path_length\x18\x07 \x01(\x05\x42\x30\x92\x41-2+Maximum length of AS path across all traces\x12U\n\x06traces\x18\x08 \x03(\x0b\x32$.kentik.synthetics.v202202.PathTraceB\x1f\x92\x41\x1c\x32\x1a\x44\x61ta for individual traces\x12^\n\x04time\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB4\x92\x41\x31\x32/Timestamp (UTC) of initiation of the path trace\"\xda\x04\n\x19GetResultsForTestsRequest\x12\x43\n\x03ids\x18\x01 \x03(\tB6\x92\x41\x30\x32.List of test IDs for which to retrieve results\xe0\x41\x02\x12m\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB=\x92\x41\x37\x32\x35Timestamp of the oldest results to include in results\xe0\x41\x02\x12k\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB=\x92\x41\x37\x32\x35Timestamp of the newest results to include in results\xe0\x41\x02\x12\x46\n\tagent_ids\x18\x04 \x03(\tB3\x92\x41\x30\x32.List of agent IDs from which to return results\x12T\n\x07targets\x18\x05 \x03(\tBC\x92\x41@2>List of targets (test dependent) for which to retrieve results\x12~\n\taggregate\x18\x06 \x01(\x08\x42k\x92\x41h2fIf true, retrieve result aggregated across the requested time period, else return complete time series\"U\n\x1aGetResultsForTestsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.kentik.synthetics.v202202.TestResults\"\xdb\x03\n\x16GetTraceForTestRequest\x12I\n\x02id\x18\x01 \x01(\tB=\x92\x41:28ID of test for which to retrieve network path trace data\x12m\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB=\x92\x41\x37\x32\x35Timestamp of the oldest results to include in results\xe0\x41\x02\x12k\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB=\x92\x41\x37\x32\x35Timestamp of the newest results to include in results\xe0\x41\x02\x12\x46\n\tagent_ids\x18\x04 \x03(\tB3\x92\x41\x30\x32.List of agent IDs from which to return results\x12R\n\ntarget_ips\x18\x05 \x03(\tB>\x92\x41;29List of target IP addresses for which to retrieve results\"\xcc\x02\n\x17GetTraceForTestResponse\x12\x84\x01\n\x05nodes\x18\x01 \x03(\x0b\x32=.kentik.synthetics.v202202.GetTraceForTestResponse.NodesEntryB6\x92\x41\x33\x32\x31Map of network node information keyed by node IDs\x12X\n\x05paths\x18\x02 \x03(\x0b\x32\x1f.kentik.synthetics.v202202.PathB(\x92\x41%2#List of retrieved network path data\x1aP\n\nNodesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".kentik.synthetics.v202202.NetNode:\x02\x38\x01\"\x13\n\x11ListAgentsRequest\"\xbe\x01\n\x12ListAgentsResponse\x12O\n\x06\x61gents\x18\x01 \x03(\x0b\x32 .kentik.synthetics.v202202.AgentB\x1d\x92\x41\x1a\x32\x18List of available agents\x12W\n\rinvalid_count\x18\x02 \x01(\rB@\x92\x41=2;Number of invalid entries encountered while collecting data\"@\n\x0fGetAgentRequest\x12-\n\x02id\x18\x01 \x01(\tB!\x92\x41\x1b\x32\x19ID of the requested agent\xe0\x41\x02\"m\n\x10GetAgentResponse\x12Y\n\x05\x61gent\x18\x01 \x01(\x0b\x32 .kentik.synthetics.v202202.AgentB(\x92\x41%2#Agent configuration and status data\"d\n\x12UpdateAgentRequest\x12N\n\x05\x61gent\x18\x01 \x01(\x0b\x32 .kentik.synthetics.v202202.AgentB\x1d\x92\x41\x1a\x32\x18\x41gent configuration data\"p\n\x13UpdateAgentResponse\x12Y\n\x05\x61gent\x18\x01 \x01(\x0b\x32 .kentik.synthetics.v202202.AgentB(\x92\x41%2#Agent configuration and status data\"G\n\x12\x44\x65leteAgentRequest\x12\x31\n\x02id\x18\x01 \x01(\tB%\x92\x41\x1f\x32\x1dID of the agent to be deleted\xe0\x41\x02\"\x15\n\x13\x44\x65leteAgentResponse\"\x12\n\x10ListTestsRequest\"\xcc\x01\n\x11ListTestsResponse\x12^\n\x05tests\x18\x01 \x03(\x0b\x32\x1f.kentik.synthetics.v202202.TestB.\x92\x41+2)List of configured active or paused tests\x12W\n\rinvalid_count\x18\x02 \x01(\rB@\x92\x41=2;Number of invalid entries encountered while collecting data\"c\n\x11\x43reateTestRequest\x12N\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\x1f\x92\x41\x19\x32\x17Test configuration data\xe0\x41\x02\"l\n\x12\x43reateTestResponse\x12V\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\'\x92\x41$2\"Test configuration and status data\":\n\x0eGetTestRequest\x12(\n\x02id\x18\x01 \x01(\tB\x1c\x92\x41\x16\x32\x14ID of requested test\xe0\x41\x02\"i\n\x0fGetTestResponse\x12V\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\'\x92\x41$2\"Test configuration and status data\"`\n\x11UpdateTestRequest\x12K\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\x1c\x92\x41\x19\x32\x17Test configuration data\"l\n\x12UpdateTestResponse\x12V\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\'\x92\x41$2\"Test configuration and status data\"E\n\x11\x44\x65leteTestRequest\x12\x30\n\x02id\x18\x01 \x01(\tB$\x92\x41\x1e\x32\x1cID of the test to be deleted\xe0\x41\x02\"\x14\n\x12\x44\x65leteTestResponse\"\xac\x01\n\x14SetTestStatusRequest\x12\x41\n\x02id\x18\x01 \x01(\tB5\x92\x41/2-ID of the test which status is to be modified\xe0\x41\x02\x12Q\n\x06status\x18\x02 \x01(\x0e\x32%.kentik.synthetics.v202202.TestStatusB\x1a\x92\x41\x14\x32\x12Target test status\xe0\x41\x02\"\x17\n\x15SetTestStatusResponse*}\n\rImplementType\x12\x1e\n\x1aIMPLEMENT_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13IMPLEMENT_TYPE_RUST\x10\x01\x12\x17\n\x13IMPLEMENT_TYPE_NODE\x10\x02\x12\x1a\n\x16IMPLEMENT_TYPE_NETWORK\x10\x03*]\n\x08IPFamily\x12\x19\n\x15IP_FAMILY_UNSPECIFIED\x10\x00\x12\x10\n\x0cIP_FAMILY_V4\x10\x01\x12\x10\n\x0cIP_FAMILY_V6\x10\x02\x12\x12\n\x0eIP_FAMILY_DUAL\x10\x03*r\n\nTestStatus\x12\x1b\n\x17TEST_STATUS_UNSPECIFIED\x10\x00\x12\x16\n\x12TEST_STATUS_ACTIVE\x10\x01\x12\x16\n\x12TEST_STATUS_PAUSED\x10\x02\x12\x17\n\x13TEST_STATUS_DELETED\x10\x03*q\n\x0b\x41gentStatus\x12\x1c\n\x18\x41GENT_STATUS_UNSPECIFIED\x10\x00\x12\x13\n\x0f\x41GENT_STATUS_OK\x10\x01\x12\x15\n\x11\x41GENT_STATUS_WAIT\x10\x02\x12\x18\n\x14\x41GENT_STATUS_DELETED\x10\x03*\xc8\x01\n\tDNSRecord\x12\x1a\n\x16\x44NS_RECORD_UNSPECIFIED\x10\x00\x12\x10\n\x0c\x44NS_RECORD_A\x10\x01\x12\x13\n\x0f\x44NS_RECORD_AAAA\x10\x02\x12\x14\n\x10\x44NS_RECORD_CNAME\x10\x03\x12\x14\n\x10\x44NS_RECORD_DNAME\x10\x04\x12\x11\n\rDNS_RECORD_NS\x10\x05\x12\x11\n\rDNS_RECORD_MX\x10\x06\x12\x12\n\x0e\x44NS_RECORD_PTR\x10\x07\x12\x12\n\x0e\x44NS_RECORD_SOA\x10\x08\x32\xca\x05\n\x15SyntheticsDataService\x12\xb3\x02\n\x12GetResultsForTests\x12\x34.kentik.synthetics.v202202.GetResultsForTestsRequest\x1a\x35.kentik.synthetics.v202202.GetResultsForTestsResponse\"\xaf\x01\xf2\xd7\x02\x0fsynthetics:read\x82\xd3\xe4\x93\x02 \"\x1b/synthetics/v202202/results:\x01*\x92\x41s\x12\x15Get results for tests\x1a\x46Returns probe results for a set of tests for specified period of time.*\x12GetResultsForTests\x12\xd0\x02\n\x0fGetTraceForTest\x12\x31.kentik.synthetics.v202202.GetTraceForTestRequest\x1a\x32.kentik.synthetics.v202202.GetTraceForTestResponse\"\xd5\x01\xf2\xd7\x02\x0fsynthetics:read\x82\xd3\xe4\x93\x02\x1e\"\x19/synthetics/v202202/trace:\x01*\x92\x41\x9a\x01\x12!Get network trace data for a test\x1a\x64Get network trace data for a specific synthetic test. The test must have traceroute task configured.*\x0fGetTraceForTest\x1a(\xca\x41\x13grpc.api.kentik.com\x90\xd8\x02\x03\xea\xd7\x02\nsynthetics2\xc0\x16\n\x16SyntheticsAdminService\x12\x8d\x02\n\nListAgents\x12,.kentik.synthetics.v202202.ListAgentsRequest\x1a-.kentik.synthetics.v202202.ListAgentsResponse\"\xa1\x01\xf2\xd7\x02\x15\x61\x64min.synthetics:read\x82\xd3\xe4\x93\x02\x1c\x12\x1a/synthetics/v202202/agents\x92\x41\x63\x12\x15List available agents\x1a>Returns list of all synthetic agents available in the account.*\nListAgents\x12\x8d\x02\n\x08GetAgent\x12*.kentik.synthetics.v202202.GetAgentRequest\x1a+.kentik.synthetics.v202202.GetAgentResponse\"\xa7\x01\xf2\xd7\x02\x15\x61\x64min.synthetics:read\x82\xd3\xe4\x93\x02!\x12\x1f/synthetics/v202202/agents/{id}\x92\x41\x64\x12\x1eGet information about an agent\x1a\x38Returns information about the requested synthetic agent.*\x08GetAgent\x12\x97\x02\n\x0bUpdateAgent\x12-.kentik.synthetics.v202202.UpdateAgentRequest\x1a..kentik.synthetics.v202202.UpdateAgentResponse\"\xa8\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x82\xd3\xe4\x93\x02*\x1a%/synthetics/v202202/agents/{agent.id}:\x01*\x92\x41[\x12 Update configuration of an agent\x1a*Update configuration of a synthetic agent.*\x0bUpdateAgent\x12\xad\x02\n\x0b\x44\x65leteAgent\x12-.kentik.synthetics.v202202.DeleteAgentRequest\x1a..kentik.synthetics.v202202.DeleteAgentResponse\"\xbe\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x82\xd3\xe4\x93\x02!*\x1f/synthetics/v202202/agents/{id}\x92\x41z\x12\x0f\x44\x65lete an agent\x1aZDeletes the requested agent. The deleted agent is removed from configuration of all tests.*\x0b\x44\x65leteAgent\x12\x86\x02\n\tListTests\x12+.kentik.synthetics.v202202.ListTestsRequest\x1a,.kentik.synthetics.v202202.ListTestsResponse\"\x9d\x01\xf2\xd7\x02\x15\x61\x64min.synthetics:read\x82\xd3\xe4\x93\x02\x1b\x12\x19/synthetics/v202202/tests\x92\x41`\x12\x0eList all tests\x1a\x43Returns a list of all configured active and paused synthetic tests.*\tListTests\x12\x8f\x02\n\nCreateTest\x12,.kentik.synthetics.v202202.CreateTestRequest\x1a-.kentik.synthetics.v202202.CreateTestResponse\"\xa3\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x82\xd3\xe4\x93\x02\x1e\"\x19/synthetics/v202202/tests:\x01*\x92\x41\x62\x12\rCreate a test\x1a\x45\x43reate synthetic test based on configuration provided in the request.*\nCreateTest\x12\x90\x02\n\x07GetTest\x12).kentik.synthetics.v202202.GetTestRequest\x1a*.kentik.synthetics.v202202.GetTestResponse\"\xad\x01\xf2\xd7\x02\x15\x61\x64min.synthetics:read\x82\xd3\xe4\x93\x02 \x12\x1e/synthetics/v202202/tests/{id}\x92\x41k\x12\x1cGet information about a test\x1a\x42Returns configuration and status for the requested synthetic test.*\x07GetTest\x12\x8f\x02\n\nUpdateTest\x12,.kentik.synthetics.v202202.UpdateTestRequest\x1a-.kentik.synthetics.v202202.UpdateTestResponse\"\xa3\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x82\xd3\xe4\x93\x02(\x1a#/synthetics/v202202/tests/{test.id}:\x01*\x92\x41X\x12\x1eUpdate configuration of a test\x1a*Updates configuration of a synthetic test.*\nUpdateTest\x12\xb1\x02\n\nDeleteTest\x12,.kentik.synthetics.v202202.DeleteTestRequest\x1a-.kentik.synthetics.v202202.DeleteTestResponse\"\xc5\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x82\xd3\xe4\x93\x02 *\x1e/synthetics/v202202/tests/{id}\x92\x41\x81\x01\x12\x18\x44\x65lete a synthetic test.\x1aYDeletes the synthetics test. All accumulated results for the test cease to be accessible.*\nDeleteTest\x12\x97\x02\n\rSetTestStatus\x12/.kentik.synthetics.v202202.SetTestStatusRequest\x1a\x30.kentik.synthetics.v202202.SetTestStatusResponse\"\xa2\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x82\xd3\xe4\x93\x02*\x1a%/synthetics/v202202/tests/{id}/status:\x01*\x92\x41U\x12!Update status of a synthetic test\x1a!Update status of a synthetic test*\rSetTestStatus\x1a.\xca\x41\x13grpc.api.kentik.com\x90\xd8\x02\x03\xea\xd7\x02\x10\x61\x64min.syntheticsB\xc3?ZOgithub.com/kentik/api-schema-public/gen/go/kentik/synthetics/v202202;synthetics\x92\x41\xee>\x12\x84=\n\x19Synthetics Monitoring API\x12\x96<# Overview\nThe Synthetics Monitoring API provides programmatic access to Kentik\'s [synthetic monitoring system](https://kb.kentik.com/v4/Ma00.htm). The API consists of two endpoints:\n| Endpoint | Purpose |\n|-----------|---------|\n| SyntheticsAdminService | CRUD operations for synthetic tests and agents |\n| SyntheticsDataService  | Retrieval of synthetic test results and network traces |\n\nBoth REST endpoint and gRPC RPCs are provided.\n### Known Limitations\nThe API currently does not support the following [Synthetic Test Types](https://kb.kentik.com/v4/Ma00.htm#Ma00-Synthetic_Test_Types):\n* BGP Monitor tests, which are supported in a [separate API](https://github.com/kentik/api-schema-public/blob/master/proto/kentik/bgp_monitoring/v202205beta1/bgp_monitoring.proto)\n* Transaction tests.\n\n### Additional Public Resources\nKentik community [Python](https://github.com/kentik/community_sdk_python) and [Go](https://github.com/kentik/community_sdk_golang) SDKs provide language-specific support for using this and other Kentik APIs. These SDKs can be also used as example code for development. \n A [Terraform provider](https://registry.terraform.io/providers/kentik/kentik-synthetics) is available for configuring tests and agents for Kentik synthetic monitoring.\n# Anatomy of a Synthetic Test\nEach `Test` consists of one or more tasks. Tasks are executed by monitoring `Agents` that send synthetic traffic (probes) over the network. The API currently supports following tasks:\n| Task name  | Purpose |\n|------------|---------|\n| ping       | Test basic address, and optionally TCP port reachability |\n| traceroute (a.k.a. trace)| Discover unidirectional network path |\n| http | Perform a simple HTTP/HTTPS request |\n| page-load | Use headless Chromium to execute an HTTP/HTTPS request |\n| dns | Execute a DNS query|\n\nThe set of tasks executed on behalf of a given test depends on the `type` of that test. The following test types are currently supported by the API:\n| API type | Portal (UI) equivalent | Tasks |\n|---------------|--------------|-------|\n| ip | IP Address | ping, traceroute |\n| hostname | Hostname | ping, traceroute |\n| network_grid | Network Grid | ping, traceroute |\n| agent | Agent-to-Agent | ping, traceroute |\n| network_mesh | Network Mesh | ping, traceroute |\n| flow | Autonomous Tests (5 variants) | ping, traceroute |\n| url | HTTP(S) or API | http, ping (optional), traceroute (optional) |\n| page_load | Page Load | page-load, ping (optional), traceroute (optional) |\n| dns | DNS Server Monitor | dns |\n| dns_grid | DNS Server Grid | dns |\n\n***Note:*** `ping` and `traceroute` tasks are always run together (never one without the other).\n\n# Test Attributes and Settings\nThe attributes of the test object enable configuration of test settings, access to test metadata, and access to runtime state information.\n### State and Metadata Attributes\n The following table lists the metadata and state attributes:\n| Attribute | Access | Purpose |\n|-----------|--------|---------|\n| id | RO | System-generated unique identifier of the test |\n| name | RW | User specified name for the test (need not be unique) |\n| type | RO (after creation) | Type of the test (set on creation; read-only thereafter) |\n| status | RW | Life-cycle status of the test |\n| cdate | RO | Creation timestamp |\n| edate | RO | Last-modification timestamp |\n| created_by | RO | Identity of the user that created the test |\n| last_updated_by | RO | Identity of the latest user to modify the test |\n| labels | RW | List of names of labels applied to the test |\n\nTest configuration is performed via the test\'s `settings` attribute. Some settings are common to all tests while others are specific to tests of a given type.\n### Common Test Settings\nThe following settings are used for tests of all types:\n| Attribute | Purpose | Required |\n|-----------|---------|----------|\n| agentIds  | IDs of agents to execute tasks for the test | YES |\n| period | Test execution interval in seconds | NO (default 60s) |\n| family | IP address family. Used only for tests whose type is url or dns. Selects which type of DNS resource is queried for resolving hostname to target address | NO (default IP_FAMILY_DUAL) |\n| notificationChannels | List of notification channels for the test | NO (default empty list) |\n| healthSettings | A HealthSettings object that configures health settings for this test, which includes metric thresholds that define health status (warning and critical) and trigger associated alarms. | YES |\n| ping | A TestPingSettings object that configures the ping task of the test | NO (default depends on test type) |\n| trace | A TestTraceSettings object that configures the trace task of the test | NO (default depends on test type) |\n| tasks | List of names of the tasks that will be executed for this test | YES |\n\n### Type-specific Settings\nEach test type has its own configuration object that represents the settings for that type. These type-specific objects are referenced by the attributes in `Test.settings`:\n| Test type    | Settings attribute | Configuration object |\n|--------------|-------------------------|---------------------------|\n| ip           | ip                      | IpTest                    |\n| hostname     | hostname                | HostnameTest              |\n| network_grid | networkGrid             | IpTest                    |\n| agent        | agent                   | AgentTest                 |\n| network_mesh | networkMesh             | NetworkMeshTest           |\n| flow         | flow                    | FlowTest                  |\n| url          | url                     | UrlTest                   |\n| page_load    | pageLoad                | PageLoadTest              |\n| dns          | dns                     | DnsTest                   |\n| dns_grid     | dnsGrid                 | DnsTest                   |\n\n# Test Results\nResults of synthetic tests are returned as a sequence of `TestResults` objects. Each such object represents measurements and health evaluation for a single test at specific point in time. Measurements and health evaluation are grouped by agent and by task.\nGranularity of timestamps in test results depends on the frequency (period) of the test and on the requested time range. The minimum granularity is 1 minute (even when period < 1 minute). The longer the time range, the lower the granularity.\n# Network Traces\nSynthetic tests that include the `traceroute` task collect the unidirectional network path from the agent to the target for each agent/target pair. The trace data are returned in the `GetTraceForTestResponse` object. The `paths` attribute of this object contains the collected network path for each agent/target pair and the round-trip time (RTT) to each hop.\nHops in actual network traces are identified by a `nodeId`. The mapping of node IDs to address, name, location, and other attributes of the hop is provided in a map that is stored in the `nodes` attribute of the `GetTraceForTestResponse` object.\n# Agents\nThe Kentik synthetic monitoring system recognizes 2 types of agents:\n* **Global** (public): Managed by Kentik and available to every Kentik user. All information about global agents in this API is read-only.\n* **Private**: Deployed by each customer and available only to that customer.\nTo be visible in this API, a private agent must first associate itself with a customer account by contacting the Kentik system (via private API). Once the agent is associated it can be authorized via the API by changing its `status` to `AGENT_STATUS_OK`. For more information about private agent deployment, see [**Synthetic Agent Deployments**](https://kb.kentik.com/v4/Ma01.htm#Ma01-Synthetic_Agent_Deployments).\n\"E\n\x16Kentik API Engineering\x12+https://github.com/kentik/api-schema-public2\x07v202202*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZD\n\x1e\n\x05\x65mail\x12\x15\x08\x02\x1a\x0fX-CH-Auth-Email \x02\n\"\n\x05token\x12\x19\x08\x02\x1a\x13X-CH-Auth-API-Token \x02\x62\x16\n\t\n\x05\x65mail\x12\x00\n\t\n\x05token\x12\x00r`\n\"Kentik synthetic monitoring system\x12:https://kb.kentik.com/v4/Ma00.htm#Ma00-Synthetics_Overviewb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*kentik/synthetics/v202202/synthetics.proto\x12\x19kentik.synthetics.v202202\x1a\x1cgoogle/api/annotations.proto\x1a\x17google/api/client.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a%kentik/core/v202303/annotations.proto\x1a#kentik/core/v202303/user_info.proto\"\xad\r\n\x05\x41gent\x12\x32\n\x02id\x18\x01 \x01(\tB&\xe0\x41\x03\x92\x41 2\x1eUnique identifier of the agent\x12?\n\tsite_name\x18\x02 \x01(\tB,\x92\x41)2\'Name of the site where agent is located\x12O\n\x06status\x18\x03 \x01(\x0e\x32&.kentik.synthetics.v202202.AgentStatusB\x17\x92\x41\x14\x32\x12Operational status\x12?\n\x05\x61lias\x18\x04 \x01(\tB0\x92\x41-2+User selected descriptive name of the agent\x12\x36\n\x04type\x18\x05 \x01(\tB(\xe0\x41\x03\x92\x41\"2 Type of agent (global | private)\x12=\n\x02os\x18\x06 \x01(\tB1\xe0\x41\x03\x92\x41+2)OS version of server/VM hosting the agent\x12\x44\n\x02ip\x18\x07 \x01(\tB8\x18\x01\xe0\x41\x03\x92\x41\x30\x32.Public IP address of the agent (auto-detected)\x12G\n\x03lat\x18\x08 \x01(\x01\x42:\x92\x41\x37\x32\x35Latitude of agent\'s location (signed decimal degrees)\x12I\n\x04long\x18\t \x01(\x01\x42;\x92\x41\x38\x32\x36Longitude of agent\'s location (signed decimal degrees)\x12\\\n\x0blast_authed\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB+\xe0\x41\x03\x92\x41%2#Timestamp of the last authorization\x12\x62\n\x06\x66\x61mily\x18\x0b \x01(\x0e\x32#.kentik.synthetics.v202202.IPFamilyB-\x92\x41*2(IP address family supported by the agent\x12=\n\x03\x61sn\x18\x0c \x01(\rB0\x92\x41-2+ASN of the AS owning agent\'s public address\x12P\n\x07site_id\x18\r \x01(\tB?\x92\x41<2:ID of the site hosting the agent (if configured in Kentik)\x12\x36\n\x07version\x18\x0e \x01(\tB%\xe0\x41\x03\x92\x41\x1f\x32\x1dSoftware version of the agent\x12\x32\n\x04\x63ity\x18\x10 \x01(\tB$\x92\x41!2\x1f\x43ity where the agent is located\x12<\n\x06region\x18\x11 \x01(\tB,\x92\x41)2\'Geographical region of agent\'s location\x12\x31\n\x07\x63ountry\x18\x12 \x01(\tB \x92\x41\x1d\x32\x1b\x43ountry of agent\'s location\x12\x41\n\x08test_ids\x18\x13 \x03(\tB/\xe0\x41\x03\x92\x41)2\'IDs of user\'s test running on the agent\x12\x39\n\x08local_ip\x18\x14 \x01(\tB\'\x18\x01\x92\x41\"2 Internal IP address of the agent\x12\x42\n\x0c\x63loud_region\x18\x16 \x01(\tB,\x92\x41)2\'Cloud region (if any) hosting the agent\x12\x46\n\x0e\x63loud_provider\x18\x17 \x01(\tB.\x92\x41+2)Cloud provider (if any) hosting the agent\x12\x41\n\nagent_impl\x18\x18 \x01(\x0e\x32(.kentik.synthetics.v202202.ImplementTypeB\x03\xe0\x41\x03\x12\x46\n\x06labels\x18\x19 \x03(\tB6\x92\x41\x33\x32\x31List of names of labels associated with the agent\x12\x86\x01\n\x08metadata\x18\x1a \x01(\x0b\x32(.kentik.synthetics.v202202.AgentMetadataBJ\x92\x41G2EAdditional information about agent\'s configuration and run-time state\"\x87\x04\n\rAgentMetadata\x12u\n\x16private_ipv4_addresses\x18\x01 \x03(\x0b\x32\x30.kentik.synthetics.v202202.AgentMetadata.IpValueB#\x92\x41 2\x1eList of private IPv4 addresses\x12v\n\x15public_ipv4_addresses\x18\x02 \x03(\x0b\x32\x30.kentik.synthetics.v202202.AgentMetadata.IpValueB%\xe0\x41\x03\x92\x41\x1f\x32\x1dList of public IPv4 addresses\x12u\n\x16private_ipv6_addresses\x18\x03 \x03(\x0b\x32\x30.kentik.synthetics.v202202.AgentMetadata.IpValueB#\x92\x41 2\x1eList of private IPv6 addresses\x12v\n\x15public_ipv6_addresses\x18\x04 \x03(\x0b\x32\x30.kentik.synthetics.v202202.AgentMetadata.IpValueB%\xe0\x41\x03\x92\x41\x1f\x32\x1dList of public IPv6 addresses\x1a\x18\n\x07IpValue\x12\r\n\x05value\x18\x01 \x01(\t\"\xdf\x05\n\x04Test\x12)\n\x02id\x18\x01 \x01(\tB\x1d\xe0\x41\x03\x92\x41\x17\x32\x15Unique ID of the test\x12\x31\n\x04name\x18\x02 \x01(\tB#\x92\x41 2\x1eUser selected name of the test\x12#\n\x04type\x18\x03 \x01(\tB\x15\x92\x41\x12\x32\x10Type of the test\x12Z\n\x06status\x18\x05 \x01(\x0e\x32%.kentik.synthetics.v202202.TestStatusB#\x92\x41 2\x1eOperational status of the test\x12R\n\x08settings\x18\x06 \x01(\x0b\x32\'.kentik.synthetics.v202202.TestSettingsB\x17\x92\x41\x14\x32\x12Test configuration\x12K\n\x05\x63\x64\x61te\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampB \xe0\x41\x03\x92\x41\x1a\x32\x18\x43reation timestamp (UTC)\x12T\n\x05\x65\x64\x61te\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB)\xe0\x41\x03\x92\x41#2!Last modification timestamp (UTC)\x12S\n\ncreated_by\x18\t \x01(\x0b\x32\x1d.kentik.core.v202303.UserInfoB \xe0\x41\x03\x92\x41\x1a\x32\x18Identity of test creator\x12o\n\x0flast_updated_by\x18\n \x01(\x0b\x32\x1d.kentik.core.v202303.UserInfoB7\xe0\x41\x03\x92\x41\x31\x32/Identity of use that has modified the test last\x12;\n\x06labels\x18\x0b \x03(\tB+\x92\x41(2&Set of labels associated with the test\"\xa6\x0b\n\x0cTestSettings\x12;\n\x08hostname\x18\x01 \x01(\x0b\x32\'.kentik.synthetics.v202202.HostnameTestH\x00\x12/\n\x02ip\x18\x02 \x01(\x0b\x32!.kentik.synthetics.v202202.IpTestH\x00\x12\x35\n\x05\x61gent\x18\x03 \x01(\x0b\x32$.kentik.synthetics.v202202.AgentTestH\x00\x12\x33\n\x04\x66low\x18\x04 \x01(\x0b\x32#.kentik.synthetics.v202202.FlowTestH\x00\x12\x31\n\x03\x64ns\x18\x05 \x01(\x0b\x32\".kentik.synthetics.v202202.DnsTestH\x00\x12\x31\n\x03url\x18\x06 \x01(\x0b\x32\".kentik.synthetics.v202202.UrlTestH\x00\x12\x39\n\x0cnetwork_grid\x18\x07 \x01(\x0b\x32!.kentik.synthetics.v202202.IpTestH\x00\x12<\n\tpage_load\x18\x08 \x01(\x0b\x32\'.kentik.synthetics.v202202.PageLoadTestH\x00\x12\x36\n\x08\x64ns_grid\x18\t \x01(\x0b\x32\".kentik.synthetics.v202202.DnsTestH\x00\x12\x42\n\x0cnetwork_mesh\x18\x12 \x01(\x0b\x32*.kentik.synthetics.v202202.NetworkMeshTestH\x00\x12Q\n\tagent_ids\x18\n \x03(\tB>\x92\x41;29IDs of agents assigned to run tasks on behalf of the test\x12:\n\x05tasks\x18\x0b \x03(\tB+\x92\x41(2&List of task names to run for the test\x12\x99\x01\n\x0fhealth_settings\x18\x0c \x01(\x0b\x32).kentik.synthetics.v202202.HealthSettingsBU\x92\x41R2PHealth evaluation thresholds, acceptable responses and alarm activation settings\x12\x63\n\x04ping\x18\r \x01(\x0b\x32+.kentik.synthetics.v202202.TestPingSettingsB(\x92\x41%2#Ping tasks configuration parameters\x12j\n\x05trace\x18\x0e \x01(\x0b\x32,.kentik.synthetics.v202202.TestTraceSettingsB-\x92\x41*2(Traceroute task configuration parameters\x12\x38\n\x06period\x18\x0f \x01(\rB(\x92\x41%2#Test evaluation period (in seconds)\x12y\n\x06\x66\x61mily\x18\x10 \x01(\x0e\x32#.kentik.synthetics.v202202.IPFamilyBD\x92\x41\x41\x32?IP address family to select from available DNS name resolutions\x12i\n\x15notification_channels\x18\x11 \x03(\tBJ\x92\x41G2EList of IDs of notification channels for alarms triggered by the test\x12\x37\n\x05notes\x18\x13 \x01(\tB(\x92\x41%2#Add a note or comment for this testB\x0c\n\ndefinition\"\x9f\x03\n\x10TestPingSettings\x12\x44\n\x05\x63ount\x18\x01 \x01(\rB5\x92\x41\x32\x32\x30Number of probe packets to send in one iteration\x12=\n\x08protocol\x18\x02 \x01(\tB+\x92\x41(2&Transport protocol to use (icmp | tcp)\x12@\n\x04port\x18\x03 \x01(\rB2\x92\x41/2-Target port for TCP probes (ignored for ICMP)\x12G\n\x07timeout\x18\x04 \x01(\rB6\x92\x41\x33\x32\x31Timeout in milliseconds for execution of the task\x12\x35\n\x05\x64\x65lay\x18\x05 \x01(\x02\x42&\x92\x41#2!Inter-probe delay in milliseconds\x12\x44\n\x04\x64scp\x18\x06 \x01(\rB6\x92\x41\x33\x32\x31\x44SCP code to be set in IP header of probe packets\"\xf5\x03\n\x11TestTraceSettings\x12\x44\n\x05\x63ount\x18\x01 \x01(\rB5\x92\x41\x32\x32\x30Number of probe packets to send in one iteration\x12\x43\n\x08protocol\x18\x02 \x01(\tB1\x92\x41.2,Transport protocol to use (icmp | tcp | udp)\x12G\n\x04port\x18\x03 \x01(\rB9\x92\x41\x36\x32\x34Target port for TCP or UDP probes (ignored for ICMP)\x12G\n\x07timeout\x18\x04 \x01(\rB6\x92\x41\x33\x32\x31Timeout in milliseconds for execution of the task\x12\x46\n\x05limit\x18\x05 \x01(\rB7\x92\x41\x34\x32\x32Maximum number of hops to probe (i.e. maximum TTL)\x12\x35\n\x05\x64\x65lay\x18\x06 \x01(\x02\x42&\x92\x41#2!Inter-probe delay in milliseconds\x12\x44\n\x04\x64scp\x18\x07 \x01(\rB6\x92\x41\x33\x32\x31\x44SCP code to be set in IP header of probe packets\"\x9b\x03\n\x12\x41\x63tivationSettings\x12u\n\x0cgrace_period\x18\x01 \x01(\tB_\x92\x41\\2ZPeriod of healthy status in minutes within the time window not cancelling alarm activation\x12\x44\n\ttime_unit\x18\x02 \x01(\tB1\x92\x41.2,Time unit for specifying time window (m | h)\x12Q\n\x0btime_window\x18\x03 \x01(\tB<\x92\x41\x39\x32\x37Time window for evaluating of test for alarm activation\x12u\n\x05times\x18\x04 \x01(\tBf\x92\x41\x63\x32\x61Number of occurrences of unhealthy test status within the time window triggering alarm activation\"\xd1\x13\n\x0eHealthSettings\x12u\n\x10latency_critical\x18\x01 \x01(\x02\x42[\x92\x41X2VThreshold for ping or DNS response latency (in microseconds) to trigger critical alarm\x12s\n\x0flatency_warning\x18\x02 \x01(\x02\x42Z\x92\x41W2UThreshold for ping or DNS response latency (in microseconds) to trigger warning alarm\x12\x62\n\x14packet_loss_critical\x18\x03 \x01(\x02\x42\x44\x92\x41\x41\x32?Threshold for ping packet loss (in %) to trigger critical alarm\x12`\n\x13packet_loss_warning\x18\x04 \x01(\x02\x42\x43\x92\x41@2>Threshold for ping packet loss (in %) to trigger warning alarm\x12\x63\n\x0fjitter_critical\x18\x05 \x01(\x02\x42J\x92\x41G2EThreshold for ping jitter (in microseconds) to trigger critical alarm\x12\x62\n\x0ejitter_warning\x18\x06 \x01(\x02\x42J\x92\x41G2EThreshold for ping jitter (in microseconds) to trigger critical alarm\x12s\n\x15http_latency_critical\x18\x07 \x01(\x02\x42T\x92\x41Q2OThreshold for HTTP response latency (in microseconds) to trigger critical alarm\x12q\n\x14http_latency_warning\x18\x08 \x01(\x02\x42S\x92\x41P2NThreshold for HTTP response latency (in microseconds) to trigger warning alarm\x12Q\n\x10http_valid_codes\x18\t \x03(\rB7\x92\x41\x34\x32\x32List of HTTP status codes indicating healthy state\x12O\n\x0f\x64ns_valid_codes\x18\n \x03(\rB6\x92\x41\x33\x32\x31List of DNS status codes indicating healthy state\x12\x92\x01\n\x17latency_critical_stddev\x18\x0b \x01(\x02\x42q\x92\x41n2lThreshold for standard deviation (in microseconds) of ping or DNS response latency to trigger critical alarm\x12\x90\x01\n\x16latency_warning_stddev\x18\x0c \x01(\x02\x42p\x92\x41m2kThreshold for standard deviation (in microseconds) of ping or DNS response latency to trigger warning alarm\x12\x80\x01\n\x16jitter_critical_stddev\x18\r \x01(\x02\x42`\x92\x41]2[Threshold for standard deviation of ping jitter (in microseconds) to trigger critical alarm\x12~\n\x15jitter_warning_stddev\x18\x0e \x01(\x02\x42_\x92\x41\\2ZThreshold for standard deviation of ping jitter (in microseconds) to trigger warning alarm\x12\x90\x01\n\x1chttp_latency_critical_stddev\x18\x0f \x01(\x02\x42j\x92\x41g2eThreshold for standard deviation of HTTP response latency (in microseconds) to trigger critical alarm\x12\x8e\x01\n\x1bhttp_latency_warning_stddev\x18\x10 \x01(\x02\x42i\x92\x41\x66\x32\x64Threshold for standard deviation of HTTP response latency (in microseconds) to trigger warning alarm\x12\x92\x01\n\x1bunhealthy_subtest_threshold\x18\x11 \x01(\rBm\x92\x41j2hNumber of tasks (across all agents) that must report unhealthy status in order for alarm to be triggered\x12\x61\n\nactivation\x18\x12 \x01(\x0b\x32-.kentik.synthetics.v202202.ActivationSettingsB\x1e\x92\x41\x1b\x32\x19\x41larm activation settings\x12x\n\x13\x63\x65rt_expiry_warning\x18\x13 \x01(\rB[\x92\x41X2VThreshold for remaining validity of TLS certificate (in days) to trigger warning alarm\x12z\n\x14\x63\x65rt_expiry_critical\x18\x14 \x01(\rB\\\x92\x41Y2WThreshold for remaining validity of TLS certificate (in days) to trigger critical alarm\x12{\n\rdns_valid_ips\x18\x15 \x01(\tBd\x92\x41\x61\x32_Comma separated list of IP addresses expected to be received in response to DNS A or AAAA query\"P\n\x0cHostnameTest\x12@\n\x06target\x18\x01 \x01(\tB0\x92\x41-2+Fully qualified DNS name of the target host\"?\n\x06IpTest\x12\x35\n\x07targets\x18\x01 \x03(\tB$\x92\x41!2\x1fList of IP addresses of targets\"\xab\x01\n\tAgentTest\x12+\n\x06target\x18\x01 \x01(\tB\x1b\x92\x41\x18\x32\x16ID of the target agent\x12q\n\x0cuse_local_ip\x18\x02 \x01(\x08\x42[\x92\x41X2VBoolean value indicating whether to use local (private) IP address of the target agent\"\xa9\x06\n\x08\x46lowTest\x12\x7f\n\x06target\x18\x01 \x01(\tBo\x92\x41l2jTarget ASN, CDN, Country, Region of City for autonomous test (type of value depends on flow test sub-type)\x12\x81\x01\n\x1etarget_refresh_interval_millis\x18\x02 \x01(\rBY\x92\x41V2TPeriod (in milliseconds) for refreshing list of targets based on available flow data\x12P\n\rmax_providers\x18\x03 \x01(\rB9\x92\x41\x36\x32\x34Maximum number of IP providers to track autonomously\x12\x62\n\x0emax_ip_targets\x18\x04 \x01(\rBJ\x92\x41G2EMaximum number of target IP addresses to select based flow data query\x12Q\n\x04type\x18\x05 \x01(\tBC\x92\x41@2>Autonomous test sub-type (asn | cdn | country | region | city)\x12\x99\x01\n\x0einet_direction\x18\x06 \x01(\tB\x80\x01\x92\x41}2{Selection of address from flow data (src = source address in inbound flows | dst = destination addresses in outbound flows)\x12s\n\tdirection\x18\x07 \x01(\tB`\x92\x41]2[Direction of flows to match target attribute for extraction of target addresses (src | dst)\"\xc3\x02\n\x07\x44nsTest\x12\x36\n\x06target\x18\x01 \x01(\tB&\x92\x41#2!Fully qualified DNS name to query\x12=\n\x07timeout\x18\x02 \x01(\rB,\x18\x01\x92\x41\'2%--- Deprecated: value is ignored. ---\x12[\n\x0brecord_type\x18\x03 \x01(\x0e\x32$.kentik.synthetics.v202202.DNSRecordB \x92\x41\x1d\x32\x1bType of DNS record to query\x12\x39\n\x07servers\x18\x04 \x03(\tB(\x92\x41%2#List of IP addresses of DNS servers\x12)\n\x04port\x18\x05 \x01(\rB\x1b\x92\x41\x18\x32\x16Target DNS server port\"\x81\x04\n\x07UrlTest\x12\x31\n\x06target\x18\x01 \x01(\tB!\x92\x41\x1e\x32\x1cHTTP or HTTPS URL to request\x12@\n\x07timeout\x18\x02 \x01(\rB/\x92\x41,2*HTTP transaction timeout (in milliseconds)\x12I\n\x06method\x18\x03 \x01(\tB9\x92\x41\x36\x32\x34HTTP method to use (GET | HEAD | PATCH | POST | PUT)\x12v\n\x07headers\x18\x04 \x03(\x0b\x32/.kentik.synthetics.v202202.UrlTest.HeadersEntryB4\x92\x41\x31\x32/Map of HTTP header values keyed by header names\x12$\n\x04\x62ody\x18\x05 \x01(\tB\x16\x92\x41\x13\x32\x11HTTP request body\x12h\n\x11ignore_tls_errors\x18\x06 \x01(\x08\x42M\x92\x41J2HBoolean indicating whether to ignore TLS certificate verification errors\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xda\x04\n\x0cPageLoadTest\x12\x31\n\x06target\x18\x01 \x01(\tB!\x92\x41\x1e\x32\x1cHTTP or HTTPS URL to request\x12@\n\x07timeout\x18\x02 \x01(\rB/\x92\x41,2*HTTP transaction timeout (in milliseconds)\x12{\n\x07headers\x18\x03 \x03(\x0b\x32\x34.kentik.synthetics.v202202.PageLoadTest.HeadersEntryB4\x92\x41\x31\x32/Map of HTTP header values keyed by header names\x12h\n\x11ignore_tls_errors\x18\x04 \x01(\x08\x42M\x92\x41J2HBoolean indicating whether to ignore TLS certificate verification errors\x12\x88\x01\n\rcss_selectors\x18\x05 \x03(\x0b\x32\x39.kentik.synthetics.v202202.PageLoadTest.CssSelectorsEntryB6\x92\x41\x33\x32\x31Map of CSS selector values keyed by selector name\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x33\n\x11\x43ssSelectorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x85\x01\n\x0fNetworkMeshTest\x12r\n\x0cuse_local_ip\x18\x01 \x01(\x08\x42\\\x92\x41Y2WBoolean value indicating whether to use local (private) IP address of the target agents\"\x9b\x02\n\nMetricData\x12-\n\x07\x63urrent\x18\x01 \x01(\rB\x1c\x92\x41\x19\x32\x17\x43urrent value of metric\x12\x33\n\x0brolling_avg\x18\x02 \x01(\rB\x1e\x92\x41\x1b\x32\x19Rolling average of metric\x12L\n\x0erolling_stddev\x18\x03 \x01(\rB4\x92\x41\x31\x32/Rolling average of standard deviation of metric\x12[\n\x06health\x18\x04 \x01(\tBK\x92\x41H2FHealth evaluation status for the metric (healthy | warning | critical)\"\x9e\x01\n\x0ePacketLossData\x12/\n\x07\x63urrent\x18\x01 \x01(\x01\x42\x1e\x92\x41\x1b\x32\x19\x43urrent packet loss value\x12[\n\x06health\x18\x02 \x01(\tBK\x92\x41H2FHealth evaluation status for the metric (healthy | warning | critical)\"\xaa\x03\n\x0bPingResults\x12=\n\x06target\x18\x01 \x01(\tB-\x92\x41*2(Hostname or address of the probed target\x12\x62\n\x0bpacket_loss\x18\x02 \x01(\x0b\x32).kentik.synthetics.v202202.PacketLossDataB\"\x92\x41\x1f\x32\x1dPacket loss metric and health\x12]\n\x07latency\x18\x03 \x01(\x0b\x32%.kentik.synthetics.v202202.MetricDataB%\x92\x41\"2 Packet latency metric and health\x12g\n\x06jitter\x18\x04 \x01(\x0b\x32%.kentik.synthetics.v202202.MetricDataB0\x92\x41-2+Latency jitter (variance) metric and health\x12\x30\n\x06\x64st_ip\x18\x05 \x01(\tB \x92\x41\x1d\x32\x1bIP address of probed target\"\xe5\x01\n\x10HTTPResponseData\x12,\n\x06status\x18\x01 \x01(\rB\x1c\x92\x41\x19\x32\x17HTTP status in response\x12\x38\n\x04size\x18\x02 \x01(\rB*\x92\x41\'2%Total size of  received response body\x12i\n\x04\x64\x61ta\x18\x03 \x01(\tB[\x92\x41X2VDetailed information about transaction timing, connection characteristics and response\"\xc2\x02\n\x0bHTTPResults\x12&\n\x06target\x18\x01 \x01(\tB\x16\x92\x41\x13\x32\x11Target probed URL\x12\x64\n\x07latency\x18\x02 \x01(\x0b\x32%.kentik.synthetics.v202202.MetricDataB,\x92\x41)2\'HTTP response latency metric and health\x12l\n\x08response\x18\x04 \x01(\x0b\x32+.kentik.synthetics.v202202.HTTPResponseDataB-\x92\x41*2(Information about received HTTP response\x12\x37\n\x06\x64st_ip\x18\x05 \x01(\tB\'\x92\x41$2\"IP address of probed target server\"y\n\x0f\x44NSResponseData\x12(\n\x06status\x18\x01 \x01(\rB\x18\x92\x41\x15\x32\x13Received DNS status\x12<\n\x04\x64\x61ta\x18\x02 \x01(\tB.\x92\x41+2)Text rendering of received DNS resolution\"\xba\x02\n\nDNSResults\x12\'\n\x06target\x18\x01 \x01(\tB\x17\x92\x41\x14\x32\x12Queried DNS record\x12\x32\n\x06server\x18\x02 \x01(\tB\"\x92\x41\x1f\x32\x1d\x44NS server used for the query\x12\x63\n\x07latency\x18\x03 \x01(\x0b\x32%.kentik.synthetics.v202202.MetricDataB+\x92\x41(2&DNS response latency metric and health\x12j\n\x08response\x18\x05 \x01(\x0b\x32*.kentik.synthetics.v202202.DNSResponseDataB,\x92\x41)2\'Information about received DNS response\"\xea\x02\n\x0bTaskResults\x12_\n\x04ping\x18\x01 \x01(\x0b\x32&.kentik.synthetics.v202202.PingResultsB\'\x92\x41$2\"Entry containing ping task resultsH\x00\x12_\n\x04http\x18\x02 \x01(\x0b\x32&.kentik.synthetics.v202202.HTTPResultsB\'\x92\x41$2\"Entry containing HTTP task resultsH\x00\x12\\\n\x03\x64ns\x18\x03 \x01(\x0b\x32%.kentik.synthetics.v202202.DNSResultsB&\x92\x41#2!Entry containing DNS task resultsH\x00\x12.\n\x06health\x18\x04 \x01(\tB\x1e\x92\x41\x1b\x32\x19Health status of the taskB\x0b\n\ttask_type\"\x86\x02\n\x0c\x41gentResults\x12\x38\n\x08\x61gent_id\x18\x01 \x01(\tB&\x92\x41#2!ID of the agent providing results\x12Z\n\x06health\x18\x02 \x01(\tBJ\x92\x41G2EOverall health status of all task for the test executed by this agent\x12`\n\x05tasks\x18\x03 \x03(\x0b\x32&.kentik.synthetics.v202202.TaskResultsB)\x92\x41&2$List of results for individual tasks\"\xcb\x02\n\x0bTestResults\x12\x43\n\x07test_id\x18\x01 \x01(\tB2\x92\x41/2-ID of the test for which results are provided\x12\x46\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x1c\x92\x41\x19\x32\x17Results timestamp (UTC)\x12.\n\x06health\x18\x03 \x01(\tB\x1e\x92\x41\x1b\x32\x19Health status of the test\x12\x7f\n\x06\x61gents\x18\x04 \x03(\x0b\x32\'.kentik.synthetics.v202202.AgentResultsBF\x92\x41\x43\x32\x41List of results from agents executing tasks on behalf of the test\"n\n\x05Stats\x12#\n\x07\x61verage\x18\x01 \x01(\x05\x42\x12\x92\x41\x0f\x32\rAverage value\x12\x1f\n\x03min\x18\x02 \x01(\x05\x42\x12\x92\x41\x0f\x32\rMinimum value\x12\x1f\n\x03max\x18\x03 \x01(\x05\x42\x12\x92\x41\x0f\x32\rMaximum value\"\x95\x02\n\x08Location\x12\x39\n\x08latitude\x18\x08 \x01(\x01\x42\'\x92\x41$2\"Latitude in signed decimal degrees\x12;\n\tlongitude\x18\t \x01(\x01\x42(\x92\x41%2#Longitude in signed decimal degrees\x12-\n\x07\x63ountry\x18\x01 \x01(\tB\x1c\x92\x41\x19\x32\x17\x43ountry of the location\x12\x39\n\x06region\x18\x02 \x01(\tB)\x92\x41&2$Geographic region within the country\x12\'\n\x04\x63ity\x18\x03 \x01(\tB\x19\x92\x41\x16\x32\x14\x43ity of the location\"\xd0\x04\n\x07NetNode\x12\x44\n\x02ip\x18\x02 \x01(\tB8\x92\x41\x35\x32\x33IP address of the node in standard textual notation\x12:\n\x03\x61sn\x18\x03 \x01(\rB-\x92\x41*2(AS number owning the address of the node\x12\x43\n\x07\x61s_name\x18\x04 \x01(\tB2\x92\x41/2-Name of the AS owning the address of the node\x12^\n\x08location\x18\x05 \x01(\x0b\x32#.kentik.synthetics.v202202.LocationB\'\x92\x41$2\"Location of IP address of the node\x12P\n\x08\x64ns_name\x18\x06 \x01(\tB>\x92\x41;29DNS name of the node (obtained by reverse DNS resolution)\x12\\\n\tdevice_id\x18\x07 \x01(\tBI\x92\x41\x46\x32\x44ID of the device corresponding with the node in Kentik configuration\x12n\n\x07site_id\x18\x08 \x01(\tB]\x92\x41Z2XID of the site containing the device corresponding with the node in Kentik configuration\"\xe2\x01\n\x08TraceHop\x12m\n\x07latency\x18\x03 \x01(\x05\x42\\\x92\x41Y2WRound-trip packet latency to the node (in microseconds) - 0 if no response was received\x12g\n\x07node_id\x18\x05 \x01(\tBV\x92\x41S2QID of the node for this hop in the Nodes map  - empty if no response was received\"\xe2\x01\n\tPathTrace\x12\x32\n\x07\x61s_path\x18\x01 \x03(\x05\x42!\x92\x41\x1e\x32\x1c\x41S path of the network trace\x12N\n\x0bis_complete\x18\x02 \x01(\x08\x42\x39\x92\x41\x36\x32\x34Indication whether response from target was received\x12Q\n\x04hops\x18\x06 \x03(\x0b\x32#.kentik.synthetics.v202202.TraceHopB\x1e\x92\x41\x1b\x32\x19List of hops in the trace\"\xec\x03\n\x04Path\x12?\n\x08\x61gent_id\x18\x01 \x01(\tB-\x92\x41*2(ID of the agent generating the path data\x12<\n\ttarget_ip\x18\x03 \x01(\tB)\x92\x41&2$IP address of the target of the path\x12`\n\thop_count\x18\x04 \x01(\x0b\x32 .kentik.synthetics.v202202.StatsB+\x92\x41(2&Hop count statistics across all traces\x12L\n\x12max_as_path_length\x18\x07 \x01(\x05\x42\x30\x92\x41-2+Maximum length of AS path across all traces\x12U\n\x06traces\x18\x08 \x03(\x0b\x32$.kentik.synthetics.v202202.PathTraceB\x1f\x92\x41\x1c\x32\x1a\x44\x61ta for individual traces\x12^\n\x04time\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB4\x92\x41\x31\x32/Timestamp (UTC) of initiation of the path trace\"\xda\x04\n\x19GetResultsForTestsRequest\x12\x43\n\x03ids\x18\x01 \x03(\tB6\x92\x41\x30\x32.List of test IDs for which to retrieve results\xe0\x41\x02\x12m\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB=\x92\x41\x37\x32\x35Timestamp of the oldest results to include in results\xe0\x41\x02\x12k\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB=\x92\x41\x37\x32\x35Timestamp of the newest results to include in results\xe0\x41\x02\x12\x46\n\tagent_ids\x18\x04 \x03(\tB3\x92\x41\x30\x32.List of agent IDs from which to return results\x12T\n\x07targets\x18\x05 \x03(\tBC\x92\x41@2>List of targets (test dependent) for which to retrieve results\x12~\n\taggregate\x18\x06 \x01(\x08\x42k\x92\x41h2fIf true, retrieve result aggregated across the requested time period, else return complete time series\"U\n\x1aGetResultsForTestsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.kentik.synthetics.v202202.TestResults\"\xdb\x03\n\x16GetTraceForTestRequest\x12I\n\x02id\x18\x01 \x01(\tB=\x92\x41:28ID of test for which to retrieve network path trace data\x12m\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB=\x92\x41\x37\x32\x35Timestamp of the oldest results to include in results\xe0\x41\x02\x12k\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB=\x92\x41\x37\x32\x35Timestamp of the newest results to include in results\xe0\x41\x02\x12\x46\n\tagent_ids\x18\x04 \x03(\tB3\x92\x41\x30\x32.List of agent IDs from which to return results\x12R\n\ntarget_ips\x18\x05 \x03(\tB>\x92\x41;29List of target IP addresses for which to retrieve results\"\xcc\x02\n\x17GetTraceForTestResponse\x12\x84\x01\n\x05nodes\x18\x01 \x03(\x0b\x32=.kentik.synthetics.v202202.GetTraceForTestResponse.NodesEntryB6\x92\x41\x33\x32\x31Map of network node information keyed by node IDs\x12X\n\x05paths\x18\x02 \x03(\x0b\x32\x1f.kentik.synthetics.v202202.PathB(\x92\x41%2#List of retrieved network path data\x1aP\n\nNodesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".kentik.synthetics.v202202.NetNode:\x02\x38\x01\"\x13\n\x11ListAgentsRequest\"\xbe\x01\n\x12ListAgentsResponse\x12O\n\x06\x61gents\x18\x01 \x03(\x0b\x32 .kentik.synthetics.v202202.AgentB\x1d\x92\x41\x1a\x32\x18List of available agents\x12W\n\rinvalid_count\x18\x02 \x01(\rB@\x92\x41=2;Number of invalid entries encountered while collecting data\"@\n\x0fGetAgentRequest\x12-\n\x02id\x18\x01 \x01(\tB!\x92\x41\x1b\x32\x19ID of the requested agent\xe0\x41\x02\"m\n\x10GetAgentResponse\x12Y\n\x05\x61gent\x18\x01 \x01(\x0b\x32 .kentik.synthetics.v202202.AgentB(\x92\x41%2#Agent configuration and status data\"d\n\x12UpdateAgentRequest\x12N\n\x05\x61gent\x18\x01 \x01(\x0b\x32 .kentik.synthetics.v202202.AgentB\x1d\x92\x41\x1a\x32\x18\x41gent configuration data\"p\n\x13UpdateAgentResponse\x12Y\n\x05\x61gent\x18\x01 \x01(\x0b\x32 .kentik.synthetics.v202202.AgentB(\x92\x41%2#Agent configuration and status data\"G\n\x12\x44\x65leteAgentRequest\x12\x31\n\x02id\x18\x01 \x01(\tB%\x92\x41\x1f\x32\x1dID of the agent to be deleted\xe0\x41\x02\"\x15\n\x13\x44\x65leteAgentResponse\"\x12\n\x10ListTestsRequest\"\xcc\x01\n\x11ListTestsResponse\x12^\n\x05tests\x18\x01 \x03(\x0b\x32\x1f.kentik.synthetics.v202202.TestB.\x92\x41+2)List of configured active or paused tests\x12W\n\rinvalid_count\x18\x02 \x01(\rB@\x92\x41=2;Number of invalid entries encountered while collecting data\"c\n\x11\x43reateTestRequest\x12N\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\x1f\x92\x41\x19\x32\x17Test configuration data\xe0\x41\x02\"l\n\x12\x43reateTestResponse\x12V\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\'\x92\x41$2\"Test configuration and status data\":\n\x0eGetTestRequest\x12(\n\x02id\x18\x01 \x01(\tB\x1c\x92\x41\x16\x32\x14ID of requested test\xe0\x41\x02\"i\n\x0fGetTestResponse\x12V\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\'\x92\x41$2\"Test configuration and status data\"`\n\x11UpdateTestRequest\x12K\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\x1c\x92\x41\x19\x32\x17Test configuration data\"l\n\x12UpdateTestResponse\x12V\n\x04test\x18\x01 \x01(\x0b\x32\x1f.kentik.synthetics.v202202.TestB\'\x92\x41$2\"Test configuration and status data\"E\n\x11\x44\x65leteTestRequest\x12\x30\n\x02id\x18\x01 \x01(\tB$\x92\x41\x1e\x32\x1cID of the test to be deleted\xe0\x41\x02\"\x14\n\x12\x44\x65leteTestResponse\"\xac\x01\n\x14SetTestStatusRequest\x12\x41\n\x02id\x18\x01 \x01(\tB5\x92\x41/2-ID of the test which status is to be modified\xe0\x41\x02\x12Q\n\x06status\x18\x02 \x01(\x0e\x32%.kentik.synthetics.v202202.TestStatusB\x1a\x92\x41\x14\x32\x12Target test status\xe0\x41\x02\"\x17\n\x15SetTestStatusResponse*}\n\rImplementType\x12\x1e\n\x1aIMPLEMENT_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13IMPLEMENT_TYPE_RUST\x10\x01\x12\x17\n\x13IMPLEMENT_TYPE_NODE\x10\x02\x12\x1a\n\x16IMPLEMENT_TYPE_NETWORK\x10\x03*]\n\x08IPFamily\x12\x19\n\x15IP_FAMILY_UNSPECIFIED\x10\x00\x12\x10\n\x0cIP_FAMILY_V4\x10\x01\x12\x10\n\x0cIP_FAMILY_V6\x10\x02\x12\x12\n\x0eIP_FAMILY_DUAL\x10\x03*\x8b\x01\n\nTestStatus\x12\x1b\n\x17TEST_STATUS_UNSPECIFIED\x10\x00\x12\x16\n\x12TEST_STATUS_ACTIVE\x10\x01\x12\x16\n\x12TEST_STATUS_PAUSED\x10\x02\x12\x17\n\x13TEST_STATUS_DELETED\x10\x03\x12\x17\n\x13TEST_STATUS_PREVIEW\x10\x04*q\n\x0b\x41gentStatus\x12\x1c\n\x18\x41GENT_STATUS_UNSPECIFIED\x10\x00\x12\x13\n\x0f\x41GENT_STATUS_OK\x10\x01\x12\x15\n\x11\x41GENT_STATUS_WAIT\x10\x02\x12\x18\n\x14\x41GENT_STATUS_DELETED\x10\x03*\xc8\x01\n\tDNSRecord\x12\x1a\n\x16\x44NS_RECORD_UNSPECIFIED\x10\x00\x12\x10\n\x0c\x44NS_RECORD_A\x10\x01\x12\x13\n\x0f\x44NS_RECORD_AAAA\x10\x02\x12\x14\n\x10\x44NS_RECORD_CNAME\x10\x03\x12\x14\n\x10\x44NS_RECORD_DNAME\x10\x04\x12\x11\n\rDNS_RECORD_NS\x10\x05\x12\x11\n\rDNS_RECORD_MX\x10\x06\x12\x12\n\x0e\x44NS_RECORD_PTR\x10\x07\x12\x12\n\x0e\x44NS_RECORD_SOA\x10\x08\x32\xca\x05\n\x15SyntheticsDataService\x12\xb3\x02\n\x12GetResultsForTests\x12\x34.kentik.synthetics.v202202.GetResultsForTestsRequest\x1a\x35.kentik.synthetics.v202202.GetResultsForTestsResponse\"\xaf\x01\xf2\xd7\x02\x0fsynthetics:read\x82\xd3\xe4\x93\x02 \"\x1b/synthetics/v202202/results:\x01*\x92\x41s\x12\x15Get results for tests\x1a\x46Returns probe results for a set of tests for specified period of time.*\x12GetResultsForTests\x12\xd0\x02\n\x0fGetTraceForTest\x12\x31.kentik.synthetics.v202202.GetTraceForTestRequest\x1a\x32.kentik.synthetics.v202202.GetTraceForTestResponse\"\xd5\x01\xf2\xd7\x02\x0fsynthetics:read\x82\xd3\xe4\x93\x02\x1e\"\x19/synthetics/v202202/trace:\x01*\x92\x41\x9a\x01\x12!Get network trace data for a test\x1a\x64Get network trace data for a specific synthetic test. The test must have traceroute task configured.*\x0fGetTraceForTest\x1a(\xca\x41\x13grpc.api.kentik.com\x90\xd8\x02\x03\xea\xd7\x02\nsynthetics2\xca\x18\n\x16SyntheticsAdminService\x12\xa7\x02\n\nListAgents\x12,.kentik.synthetics.v202202.ListAgentsRequest\x1a-.kentik.synthetics.v202202.ListAgentsResponse\"\xbb\x01\xf2\xd7\x02\x15\x61\x64min.synthetics:read\x92\xd8\x02\x16synthetics.agent::read\x82\xd3\xe4\x93\x02\x1c\x12\x1a/synthetics/v202202/agents\x92\x41\x63\x12\x15List available agents\x1a>Returns list of all synthetic agents available in the account.*\nListAgents\x12\xa7\x02\n\x08GetAgent\x12*.kentik.synthetics.v202202.GetAgentRequest\x1a+.kentik.synthetics.v202202.GetAgentResponse\"\xc1\x01\xf2\xd7\x02\x15\x61\x64min.synthetics:read\x92\xd8\x02\x16synthetics.agent::read\x82\xd3\xe4\x93\x02!\x12\x1f/synthetics/v202202/agents/{id}\x92\x41\x64\x12\x1eGet information about an agent\x1a\x38Returns information about the requested synthetic agent.*\x08GetAgent\x12\xb3\x02\n\x0bUpdateAgent\x12-.kentik.synthetics.v202202.UpdateAgentRequest\x1a..kentik.synthetics.v202202.UpdateAgentResponse\"\xc4\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x92\xd8\x02\x18synthetics.agent::update\x82\xd3\xe4\x93\x02*\x1a%/synthetics/v202202/agents/{agent.id}:\x01*\x92\x41[\x12 Update configuration of an agent\x1a*Update configuration of a synthetic agent.*\x0bUpdateAgent\x12\xc9\x02\n\x0b\x44\x65leteAgent\x12-.kentik.synthetics.v202202.DeleteAgentRequest\x1a..kentik.synthetics.v202202.DeleteAgentResponse\"\xda\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x92\xd8\x02\x18synthetics.agent::delete\x82\xd3\xe4\x93\x02!*\x1f/synthetics/v202202/agents/{id}\x92\x41z\x12\x0f\x44\x65lete an agent\x1aZDeletes the requested agent. The deleted agent is removed from configuration of all tests.*\x0b\x44\x65leteAgent\x12\x9f\x02\n\tListTests\x12+.kentik.synthetics.v202202.ListTestsRequest\x1a,.kentik.synthetics.v202202.ListTestsResponse\"\xb6\x01\xf2\xd7\x02\x15\x61\x64min.synthetics:read\x92\xd8\x02\x15synthetics.test::read\x82\xd3\xe4\x93\x02\x1b\x12\x19/synthetics/v202202/tests\x92\x41`\x12\x0eList all tests\x1a\x43Returns a list of all configured active and paused synthetic tests.*\tListTests\x12\xaa\x02\n\nCreateTest\x12,.kentik.synthetics.v202202.CreateTestRequest\x1a-.kentik.synthetics.v202202.CreateTestResponse\"\xbe\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x92\xd8\x02\x17synthetics.test::create\x82\xd3\xe4\x93\x02\x1e\"\x19/synthetics/v202202/tests:\x01*\x92\x41\x62\x12\rCreate a test\x1a\x45\x43reate synthetic test based on configuration provided in the request.*\nCreateTest\x12\xa9\x02\n\x07GetTest\x12).kentik.synthetics.v202202.GetTestRequest\x1a*.kentik.synthetics.v202202.GetTestResponse\"\xc6\x01\xf2\xd7\x02\x15\x61\x64min.synthetics:read\x92\xd8\x02\x15synthetics.test::read\x82\xd3\xe4\x93\x02 \x12\x1e/synthetics/v202202/tests/{id}\x92\x41k\x12\x1cGet information about a test\x1a\x42Returns configuration and status for the requested synthetic test.*\x07GetTest\x12\xaa\x02\n\nUpdateTest\x12,.kentik.synthetics.v202202.UpdateTestRequest\x1a-.kentik.synthetics.v202202.UpdateTestResponse\"\xbe\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x92\xd8\x02\x17synthetics.test::update\x82\xd3\xe4\x93\x02(\x1a#/synthetics/v202202/tests/{test.id}:\x01*\x92\x41X\x12\x1eUpdate configuration of a test\x1a*Updates configuration of a synthetic test.*\nUpdateTest\x12\xcc\x02\n\nDeleteTest\x12,.kentik.synthetics.v202202.DeleteTestRequest\x1a-.kentik.synthetics.v202202.DeleteTestResponse\"\xe0\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x92\xd8\x02\x17synthetics.test::delete\x82\xd3\xe4\x93\x02 *\x1e/synthetics/v202202/tests/{id}\x92\x41\x81\x01\x12\x18\x44\x65lete a synthetic test.\x1aYDeletes the synthetics test. All accumulated results for the test cease to be accessible.*\nDeleteTest\x12\xb2\x02\n\rSetTestStatus\x12/.kentik.synthetics.v202202.SetTestStatusRequest\x1a\x30.kentik.synthetics.v202202.SetTestStatusResponse\"\xbd\x01\xf2\xd7\x02\x16\x61\x64min.synthetics:write\x92\xd8\x02\x17synthetics.test::update\x82\xd3\xe4\x93\x02*\x1a%/synthetics/v202202/tests/{id}/status:\x01*\x92\x41U\x12!Update status of a synthetic test\x1a!Update status of a synthetic test*\rSetTestStatus\x1a.\xca\x41\x13grpc.api.kentik.com\x90\xd8\x02\x03\xea\xd7\x02\x10\x61\x64min.syntheticsB\xc3?ZOgithub.com/kentik/api-schema-public/gen/go/kentik/synthetics/v202202;synthetics\x92\x41\xee>\x12\x84=\n\x19Synthetics Monitoring API\x12\x96<# Overview\nThe Synthetics Monitoring API provides programmatic access to Kentik\'s [synthetic monitoring system](https://kb.kentik.com/v4/Ma00.htm). The API consists of two endpoints:\n| Endpoint | Purpose |\n|-----------|---------|\n| SyntheticsAdminService | CRUD operations for synthetic tests and agents |\n| SyntheticsDataService  | Retrieval of synthetic test results and network traces |\n\nBoth REST endpoint and gRPC RPCs are provided.\n### Known Limitations\nThe API currently does not support the following [Synthetic Test Types](https://kb.kentik.com/v4/Ma00.htm#Ma00-Synthetic_Test_Types):\n* BGP Monitor tests, which are supported in a [separate API](https://github.com/kentik/api-schema-public/blob/master/proto/kentik/bgp_monitoring/v202205beta1/bgp_monitoring.proto)\n* Transaction tests.\n\n### Additional Public Resources\nKentik community [Python](https://github.com/kentik/community_sdk_python) and [Go](https://github.com/kentik/community_sdk_golang) SDKs provide language-specific support for using this and other Kentik APIs. These SDKs can be also used as example code for development. \n A [Terraform provider](https://registry.terraform.io/providers/kentik/kentik-synthetics) is available for configuring tests and agents for Kentik synthetic monitoring.\n# Anatomy of a Synthetic Test\nEach `Test` consists of one or more tasks. Tasks are executed by monitoring `Agents` that send synthetic traffic (probes) over the network. The API currently supports following tasks:\n| Task name  | Purpose |\n|------------|---------|\n| ping       | Test basic address, and optionally TCP port reachability |\n| traceroute (a.k.a. trace)| Discover unidirectional network path |\n| http | Perform a simple HTTP/HTTPS request |\n| page-load | Use headless Chromium to execute an HTTP/HTTPS request |\n| dns | Execute a DNS query|\n\nThe set of tasks executed on behalf of a given test depends on the `type` of that test. The following test types are currently supported by the API:\n| API type | Portal (UI) equivalent | Tasks |\n|---------------|--------------|-------|\n| ip | IP Address | ping, traceroute |\n| hostname | Hostname | ping, traceroute |\n| network_grid | Network Grid | ping, traceroute |\n| agent | Agent-to-Agent | ping, traceroute |\n| network_mesh | Network Mesh | ping, traceroute |\n| flow | Autonomous Tests (5 variants) | ping, traceroute |\n| url | HTTP(S) or API | http, ping (optional), traceroute (optional) |\n| page_load | Page Load | page-load, ping (optional), traceroute (optional) |\n| dns | DNS Server Monitor | dns |\n| dns_grid | DNS Server Grid | dns |\n\n***Note:*** `ping` and `traceroute` tasks are always run together (never one without the other).\n\n# Test Attributes and Settings\nThe attributes of the test object enable configuration of test settings, access to test metadata, and access to runtime state information.\n### State and Metadata Attributes\n The following table lists the metadata and state attributes:\n| Attribute | Access | Purpose |\n|-----------|--------|---------|\n| id | RO | System-generated unique identifier of the test |\n| name | RW | User specified name for the test (need not be unique) |\n| type | RO (after creation) | Type of the test (set on creation; read-only thereafter) |\n| status | RW | Life-cycle status of the test |\n| cdate | RO | Creation timestamp |\n| edate | RO | Last-modification timestamp |\n| created_by | RO | Identity of the user that created the test |\n| last_updated_by | RO | Identity of the latest user to modify the test |\n| labels | RW | List of names of labels applied to the test |\n\nTest configuration is performed via the test\'s `settings` attribute. Some settings are common to all tests while others are specific to tests of a given type.\n### Common Test Settings\nThe following settings are used for tests of all types:\n| Attribute | Purpose | Required |\n|-----------|---------|----------|\n| agentIds  | IDs of agents to execute tasks for the test | YES |\n| period | Test execution interval in seconds | NO (default 60s) |\n| family | IP address family. Used only for tests whose type is url or dns. Selects which type of DNS resource is queried for resolving hostname to target address | NO (default IP_FAMILY_DUAL) |\n| notificationChannels | List of notification channels for the test | NO (default empty list) |\n| healthSettings | A HealthSettings object that configures health settings for this test, which includes metric thresholds that define health status (warning and critical) and trigger associated alarms. | YES |\n| ping | A TestPingSettings object that configures the ping task of the test | NO (default depends on test type) |\n| trace | A TestTraceSettings object that configures the trace task of the test | NO (default depends on test type) |\n| tasks | List of names of the tasks that will be executed for this test | YES |\n\n### Type-specific Settings\nEach test type has its own configuration object that represents the settings for that type. These type-specific objects are referenced by the attributes in `Test.settings`:\n| Test type    | Settings attribute | Configuration object |\n|--------------|-------------------------|---------------------------|\n| ip           | ip                      | IpTest                    |\n| hostname     | hostname                | HostnameTest              |\n| network_grid | networkGrid             | IpTest                    |\n| agent        | agent                   | AgentTest                 |\n| network_mesh | networkMesh             | NetworkMeshTest           |\n| flow         | flow                    | FlowTest                  |\n| url          | url                     | UrlTest                   |\n| page_load    | pageLoad                | PageLoadTest              |\n| dns          | dns                     | DnsTest                   |\n| dns_grid     | dnsGrid                 | DnsTest                   |\n\n# Test Results\nResults of synthetic tests are returned as a sequence of `TestResults` objects. Each such object represents measurements and health evaluation for a single test at specific point in time. Measurements and health evaluation are grouped by agent and by task.\nGranularity of timestamps in test results depends on the frequency (period) of the test and on the requested time range. The minimum granularity is 1 minute (even when period < 1 minute). The longer the time range, the lower the granularity.\n# Network Traces\nSynthetic tests that include the `traceroute` task collect the unidirectional network path from the agent to the target for each agent/target pair. The trace data are returned in the `GetTraceForTestResponse` object. The `paths` attribute of this object contains the collected network path for each agent/target pair and the round-trip time (RTT) to each hop.\nHops in actual network traces are identified by a `nodeId`. The mapping of node IDs to address, name, location, and other attributes of the hop is provided in a map that is stored in the `nodes` attribute of the `GetTraceForTestResponse` object.\n# Agents\nThe Kentik synthetic monitoring system recognizes 2 types of agents:\n* **Global** (public): Managed by Kentik and available to every Kentik user. All information about global agents in this API is read-only.\n* **Private**: Deployed by each customer and available only to that customer.\nTo be visible in this API, a private agent must first associate itself with a customer account by contacting the Kentik system (via private API). Once the agent is associated it can be authorized via the API by changing its `status` to `AGENT_STATUS_OK`. For more information about private agent deployment, see [**Synthetic Agent Deployments**](https://kb.kentik.com/v4/Ma01.htm#Ma01-Synthetic_Agent_Deployments).\n\"E\n\x16Kentik API Engineering\x12+https://github.com/kentik/api-schema-public2\x07v202202*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZD\n\x1e\n\x05\x65mail\x12\x15\x08\x02\x1a\x0fX-CH-Auth-Email \x02\n\"\n\x05token\x12\x19\x08\x02\x1a\x13X-CH-Auth-API-Token \x02\x62\x16\n\t\n\x05\x65mail\x12\x00\n\t\n\x05token\x12\x00r`\n\"Kentik synthetic monitoring system\x12:https://kb.kentik.com/v4/Ma00.htm#Ma00-Synthetics_Overviewb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kentik.synthetics.v202202.synthetics_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZOgithub.com/kentik/api-schema-public/gen/go/kentik/synthetics/v202202;synthetics\222A\356>\022\204=\n\031Synthetics Monitoring API\022\226<# Overview\nThe Synthetics Monitoring API provides programmatic access to Kentik\'s [synthetic monitoring system](https://kb.kentik.com/v4/Ma00.htm). The API consists of two endpoints:\n| Endpoint | Purpose |\n|-----------|---------|\n| SyntheticsAdminService | CRUD operations for synthetic tests and agents |\n| SyntheticsDataService  | Retrieval of synthetic test results and network traces |\n\nBoth REST endpoint and gRPC RPCs are provided.\n### Known Limitations\nThe API currently does not support the following [Synthetic Test Types](https://kb.kentik.com/v4/Ma00.htm#Ma00-Synthetic_Test_Types):\n* BGP Monitor tests, which are supported in a [separate API](https://github.com/kentik/api-schema-public/blob/master/proto/kentik/bgp_monitoring/v202205beta1/bgp_monitoring.proto)\n* Transaction tests.\n\n### Additional Public Resources\nKentik community [Python](https://github.com/kentik/community_sdk_python) and [Go](https://github.com/kentik/community_sdk_golang) SDKs provide language-specific support for using this and other Kentik APIs. These SDKs can be also used as example code for development. \n A [Terraform provider](https://registry.terraform.io/providers/kentik/kentik-synthetics) is available for configuring tests and agents for Kentik synthetic monitoring.\n# Anatomy of a Synthetic Test\nEach `Test` consists of one or more tasks. Tasks are executed by monitoring `Agents` that send synthetic traffic (probes) over the network. The API currently supports following tasks:\n| Task name  | Purpose |\n|------------|---------|\n| ping       | Test basic address, and optionally TCP port reachability |\n| traceroute (a.k.a. trace)| Discover unidirectional network path |\n| http | Perform a simple HTTP/HTTPS request |\n| page-load | Use headless Chromium to execute an HTTP/HTTPS request |\n| dns | Execute a DNS query|\n\nThe set of tasks executed on behalf of a given test depends on the `type` of that test. The following test types are currently supported by the API:\n| API type | Portal (UI) equivalent | Tasks |\n|---------------|--------------|-------|\n| ip | IP Address | ping, traceroute |\n| hostname | Hostname | ping, traceroute |\n| network_grid | Network Grid | ping, traceroute |\n| agent | Agent-to-Agent | ping, traceroute |\n| network_mesh | Network Mesh | ping, traceroute |\n| flow | Autonomous Tests (5 variants) | ping, traceroute |\n| url | HTTP(S) or API | http, ping (optional), traceroute (optional) |\n| page_load | Page Load | page-load, ping (optional), traceroute (optional) |\n| dns | DNS Server Monitor | dns |\n| dns_grid | DNS Server Grid | dns |\n\n***Note:*** `ping` and `traceroute` tasks are always run together (never one without the other).\n\n# Test Attributes and Settings\nThe attributes of the test object enable configuration of test settings, access to test metadata, and access to runtime state information.\n### State and Metadata Attributes\n The following table lists the metadata and state attributes:\n| Attribute | Access | Purpose |\n|-----------|--------|---------|\n| id | RO | System-generated unique identifier of the test |\n| name | RW | User specified name for the test (need not be unique) |\n| type | RO (after creation) | Type of the test (set on creation; read-only thereafter) |\n| status | RW | Life-cycle status of the test |\n| cdate | RO | Creation timestamp |\n| edate | RO | Last-modification timestamp |\n| created_by | RO | Identity of the user that created the test |\n| last_updated_by | RO | Identity of the latest user to modify the test |\n| labels | RW | List of names of labels applied to the test |\n\nTest configuration is performed via the test\'s `settings` attribute. Some settings are common to all tests while others are specific to tests of a given type.\n### Common Test Settings\nThe following settings are used for tests of all types:\n| Attribute | Purpose | Required |\n|-----------|---------|----------|\n| agentIds  | IDs of agents to execute tasks for the test | YES |\n| period | Test execution interval in seconds | NO (default 60s) |\n| family | IP address family. Used only for tests whose type is url or dns. Selects which type of DNS resource is queried for resolving hostname to target address | NO (default IP_FAMILY_DUAL) |\n| notificationChannels | List of notification channels for the test | NO (default empty list) |\n| healthSettings | A HealthSettings object that configures health settings for this test, which includes metric thresholds that define health status (warning and critical) and trigger associated alarms. | YES |\n| ping | A TestPingSettings object that configures the ping task of the test | NO (default depends on test type) |\n| trace | A TestTraceSettings object that configures the trace task of the test | NO (default depends on test type) |\n| tasks | List of names of the tasks that will be executed for this test | YES |\n\n### Type-specific Settings\nEach test type has its own configuration object that represents the settings for that type. These type-specific objects are referenced by the attributes in `Test.settings`:\n| Test type    | Settings attribute | Configuration object |\n|--------------|-------------------------|---------------------------|\n| ip           | ip                      | IpTest                    |\n| hostname     | hostname                | HostnameTest              |\n| network_grid | networkGrid             | IpTest                    |\n| agent        | agent                   | AgentTest                 |\n| network_mesh | networkMesh             | NetworkMeshTest           |\n| flow         | flow                    | FlowTest                  |\n| url          | url                     | UrlTest                   |\n| page_load    | pageLoad                | PageLoadTest              |\n| dns          | dns                     | DnsTest                   |\n| dns_grid     | dnsGrid                 | DnsTest                   |\n\n# Test Results\nResults of synthetic tests are returned as a sequence of `TestResults` objects. Each such object represents measurements and health evaluation for a single test at specific point in time. Measurements and health evaluation are grouped by agent and by task.\nGranularity of timestamps in test results depends on the frequency (period) of the test and on the requested time range. The minimum granularity is 1 minute (even when period < 1 minute). The longer the time range, the lower the granularity.\n# Network Traces\nSynthetic tests that include the `traceroute` task collect the unidirectional network path from the agent to the target for each agent/target pair. The trace data are returned in the `GetTraceForTestResponse` object. The `paths` attribute of this object contains the collected network path for each agent/target pair and the round-trip time (RTT) to each hop.\nHops in actual network traces are identified by a `nodeId`. The mapping of node IDs to address, name, location, and other attributes of the hop is provided in a map that is stored in the `nodes` attribute of the `GetTraceForTestResponse` object.\n# Agents\nThe Kentik synthetic monitoring system recognizes 2 types of agents:\n* **Global** (public): Managed by Kentik and available to every Kentik user. All information about global agents in this API is read-only.\n* **Private**: Deployed by each customer and available only to that customer.\nTo be visible in this API, a private agent must first associate itself with a customer account by contacting the Kentik system (via private API). Once the agent is associated it can be authorized via the API by changing its `status` to `AGENT_STATUS_OK`. For more information about private agent deployment, see [**Synthetic Agent Deployments**](https://kb.kentik.com/v4/Ma01.htm#Ma01-Synthetic_Agent_Deployments).\n\"E\n\026Kentik API Engineering\022+https://github.com/kentik/api-schema-public2\007v202202*\001\0022\020application/json:\020application/jsonZD\n\036\n\005email\022\025\010\002\032\017X-CH-Auth-Email \002\n\"\n\005token\022\031\010\002\032\023X-CH-Auth-API-Token \002b\026\n\t\n\005email\022\000\n\t\n\005token\022\000r`\n\"Kentik synthetic monitoring system\022:https://kb.kentik.com/v4/Ma00.htm#Ma00-Synthetics_Overview'
@@ -451,43 +451,43 @@
   _SYNTHETICSDATASERVICE.methods_by_name['GetResultsForTests']._options = None
   _SYNTHETICSDATASERVICE.methods_by_name['GetResultsForTests']._serialized_options = b'\362\327\002\017synthetics:read\202\323\344\223\002 \"\033/synthetics/v202202/results:\001*\222As\022\025Get results for tests\032FReturns probe results for a set of tests for specified period of time.*\022GetResultsForTests'
   _SYNTHETICSDATASERVICE.methods_by_name['GetTraceForTest']._options = None
   _SYNTHETICSDATASERVICE.methods_by_name['GetTraceForTest']._serialized_options = b'\362\327\002\017synthetics:read\202\323\344\223\002\036\"\031/synthetics/v202202/trace:\001*\222A\232\001\022!Get network trace data for a test\032dGet network trace data for a specific synthetic test. The test must have traceroute task configured.*\017GetTraceForTest'
   _SYNTHETICSADMINSERVICE._options = None
   _SYNTHETICSADMINSERVICE._serialized_options = b'\312A\023grpc.api.kentik.com\220\330\002\003\352\327\002\020admin.synthetics'
   _SYNTHETICSADMINSERVICE.methods_by_name['ListAgents']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['ListAgents']._serialized_options = b'\362\327\002\025admin.synthetics:read\202\323\344\223\002\034\022\032/synthetics/v202202/agents\222Ac\022\025List available agents\032>Returns list of all synthetic agents available in the account.*\nListAgents'
+  _SYNTHETICSADMINSERVICE.methods_by_name['ListAgents']._serialized_options = b'\362\327\002\025admin.synthetics:read\222\330\002\026synthetics.agent::read\202\323\344\223\002\034\022\032/synthetics/v202202/agents\222Ac\022\025List available agents\032>Returns list of all synthetic agents available in the account.*\nListAgents'
   _SYNTHETICSADMINSERVICE.methods_by_name['GetAgent']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['GetAgent']._serialized_options = b'\362\327\002\025admin.synthetics:read\202\323\344\223\002!\022\037/synthetics/v202202/agents/{id}\222Ad\022\036Get information about an agent\0328Returns information about the requested synthetic agent.*\010GetAgent'
+  _SYNTHETICSADMINSERVICE.methods_by_name['GetAgent']._serialized_options = b'\362\327\002\025admin.synthetics:read\222\330\002\026synthetics.agent::read\202\323\344\223\002!\022\037/synthetics/v202202/agents/{id}\222Ad\022\036Get information about an agent\0328Returns information about the requested synthetic agent.*\010GetAgent'
   _SYNTHETICSADMINSERVICE.methods_by_name['UpdateAgent']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['UpdateAgent']._serialized_options = b'\362\327\002\026admin.synthetics:write\202\323\344\223\002*\032%/synthetics/v202202/agents/{agent.id}:\001*\222A[\022 Update configuration of an agent\032*Update configuration of a synthetic agent.*\013UpdateAgent'
+  _SYNTHETICSADMINSERVICE.methods_by_name['UpdateAgent']._serialized_options = b'\362\327\002\026admin.synthetics:write\222\330\002\030synthetics.agent::update\202\323\344\223\002*\032%/synthetics/v202202/agents/{agent.id}:\001*\222A[\022 Update configuration of an agent\032*Update configuration of a synthetic agent.*\013UpdateAgent'
   _SYNTHETICSADMINSERVICE.methods_by_name['DeleteAgent']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['DeleteAgent']._serialized_options = b'\362\327\002\026admin.synthetics:write\202\323\344\223\002!*\037/synthetics/v202202/agents/{id}\222Az\022\017Delete an agent\032ZDeletes the requested agent. The deleted agent is removed from configuration of all tests.*\013DeleteAgent'
+  _SYNTHETICSADMINSERVICE.methods_by_name['DeleteAgent']._serialized_options = b'\362\327\002\026admin.synthetics:write\222\330\002\030synthetics.agent::delete\202\323\344\223\002!*\037/synthetics/v202202/agents/{id}\222Az\022\017Delete an agent\032ZDeletes the requested agent. The deleted agent is removed from configuration of all tests.*\013DeleteAgent'
   _SYNTHETICSADMINSERVICE.methods_by_name['ListTests']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['ListTests']._serialized_options = b'\362\327\002\025admin.synthetics:read\202\323\344\223\002\033\022\031/synthetics/v202202/tests\222A`\022\016List all tests\032CReturns a list of all configured active and paused synthetic tests.*\tListTests'
+  _SYNTHETICSADMINSERVICE.methods_by_name['ListTests']._serialized_options = b'\362\327\002\025admin.synthetics:read\222\330\002\025synthetics.test::read\202\323\344\223\002\033\022\031/synthetics/v202202/tests\222A`\022\016List all tests\032CReturns a list of all configured active and paused synthetic tests.*\tListTests'
   _SYNTHETICSADMINSERVICE.methods_by_name['CreateTest']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['CreateTest']._serialized_options = b'\362\327\002\026admin.synthetics:write\202\323\344\223\002\036\"\031/synthetics/v202202/tests:\001*\222Ab\022\rCreate a test\032ECreate synthetic test based on configuration provided in the request.*\nCreateTest'
+  _SYNTHETICSADMINSERVICE.methods_by_name['CreateTest']._serialized_options = b'\362\327\002\026admin.synthetics:write\222\330\002\027synthetics.test::create\202\323\344\223\002\036\"\031/synthetics/v202202/tests:\001*\222Ab\022\rCreate a test\032ECreate synthetic test based on configuration provided in the request.*\nCreateTest'
   _SYNTHETICSADMINSERVICE.methods_by_name['GetTest']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['GetTest']._serialized_options = b'\362\327\002\025admin.synthetics:read\202\323\344\223\002 \022\036/synthetics/v202202/tests/{id}\222Ak\022\034Get information about a test\032BReturns configuration and status for the requested synthetic test.*\007GetTest'
+  _SYNTHETICSADMINSERVICE.methods_by_name['GetTest']._serialized_options = b'\362\327\002\025admin.synthetics:read\222\330\002\025synthetics.test::read\202\323\344\223\002 \022\036/synthetics/v202202/tests/{id}\222Ak\022\034Get information about a test\032BReturns configuration and status for the requested synthetic test.*\007GetTest'
   _SYNTHETICSADMINSERVICE.methods_by_name['UpdateTest']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['UpdateTest']._serialized_options = b'\362\327\002\026admin.synthetics:write\202\323\344\223\002(\032#/synthetics/v202202/tests/{test.id}:\001*\222AX\022\036Update configuration of a test\032*Updates configuration of a synthetic test.*\nUpdateTest'
+  _SYNTHETICSADMINSERVICE.methods_by_name['UpdateTest']._serialized_options = b'\362\327\002\026admin.synthetics:write\222\330\002\027synthetics.test::update\202\323\344\223\002(\032#/synthetics/v202202/tests/{test.id}:\001*\222AX\022\036Update configuration of a test\032*Updates configuration of a synthetic test.*\nUpdateTest'
   _SYNTHETICSADMINSERVICE.methods_by_name['DeleteTest']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['DeleteTest']._serialized_options = b'\362\327\002\026admin.synthetics:write\202\323\344\223\002 *\036/synthetics/v202202/tests/{id}\222A\201\001\022\030Delete a synthetic test.\032YDeletes the synthetics test. All accumulated results for the test cease to be accessible.*\nDeleteTest'
+  _SYNTHETICSADMINSERVICE.methods_by_name['DeleteTest']._serialized_options = b'\362\327\002\026admin.synthetics:write\222\330\002\027synthetics.test::delete\202\323\344\223\002 *\036/synthetics/v202202/tests/{id}\222A\201\001\022\030Delete a synthetic test.\032YDeletes the synthetics test. All accumulated results for the test cease to be accessible.*\nDeleteTest'
   _SYNTHETICSADMINSERVICE.methods_by_name['SetTestStatus']._options = None
-  _SYNTHETICSADMINSERVICE.methods_by_name['SetTestStatus']._serialized_options = b'\362\327\002\026admin.synthetics:write\202\323\344\223\002*\032%/synthetics/v202202/tests/{id}/status:\001*\222AU\022!Update status of a synthetic test\032!Update status of a synthetic test*\rSetTestStatus'
+  _SYNTHETICSADMINSERVICE.methods_by_name['SetTestStatus']._serialized_options = b'\362\327\002\026admin.synthetics:write\222\330\002\027synthetics.test::update\202\323\344\223\002*\032%/synthetics/v202202/tests/{id}/status:\001*\222AU\022!Update status of a synthetic test\032!Update status of a synthetic test*\rSetTestStatus'
   _IMPLEMENTTYPE._serialized_start=19398
   _IMPLEMENTTYPE._serialized_end=19523
   _IPFAMILY._serialized_start=19525
   _IPFAMILY._serialized_end=19618
-  _TESTSTATUS._serialized_start=19620
-  _TESTSTATUS._serialized_end=19734
-  _AGENTSTATUS._serialized_start=19736
-  _AGENTSTATUS._serialized_end=19849
-  _DNSRECORD._serialized_start=19852
-  _DNSRECORD._serialized_end=20052
+  _TESTSTATUS._serialized_start=19621
+  _TESTSTATUS._serialized_end=19760
+  _AGENTSTATUS._serialized_start=19762
+  _AGENTSTATUS._serialized_end=19875
+  _DNSRECORD._serialized_start=19878
+  _DNSRECORD._serialized_end=20078
   _AGENT._serialized_start=319
   _AGENT._serialized_end=2028
   _AGENTMETADATA._serialized_start=2031
   _AGENTMETADATA._serialized_end=2550
   _AGENTMETADATA_IPVALUE._serialized_start=2526
   _AGENTMETADATA_IPVALUE._serialized_end=2550
   _TEST._serialized_start=2553
@@ -602,12 +602,12 @@
   _DELETETESTREQUEST._serialized_end=19174
   _DELETETESTRESPONSE._serialized_start=19176
   _DELETETESTRESPONSE._serialized_end=19196
   _SETTESTSTATUSREQUEST._serialized_start=19199
   _SETTESTSTATUSREQUEST._serialized_end=19371
   _SETTESTSTATUSRESPONSE._serialized_start=19373
   _SETTESTSTATUSRESPONSE._serialized_end=19396
-  _SYNTHETICSDATASERVICE._serialized_start=20055
-  _SYNTHETICSDATASERVICE._serialized_end=20769
-  _SYNTHETICSADMINSERVICE._serialized_start=20772
-  _SYNTHETICSADMINSERVICE._serialized_end=23652
+  _SYNTHETICSDATASERVICE._serialized_start=20081
+  _SYNTHETICSDATASERVICE._serialized_end=20795
+  _SYNTHETICSADMINSERVICE._serialized_start=20798
+  _SYNTHETICSADMINSERVICE._serialized_end=23944
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kentik-api-1.0.6/kentik_api/generated/kentik/synthetics/v202202/synthetics_pb2_grpc.py` & `kentik-api-1.0.7/kentik_api/generated/kentik/synthetics/v202202/synthetics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/internal/grpc.py` & `kentik-api-1.0.7/kentik_api/internal/grpc.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/kentik_api.py` & `kentik-api-1.0.7/kentik_api/kentik_api.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/__init__.py` & `kentik-api-1.0.7/kentik_api/public/__init__.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/batch_operation.py` & `kentik-api-1.0.7/kentik_api/public/batch_operation.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/custom_application.py` & `kentik-api-1.0.7/kentik_api/public/custom_application.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/custom_dimension.py` & `kentik-api-1.0.7/kentik_api/public/custom_dimension.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/device.py` & `kentik-api-1.0.7/kentik_api/public/device.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/device_label.py` & `kentik-api-1.0.7/kentik_api/public/device_label.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/errors.py` & `kentik-api-1.0.7/kentik_api/public/errors.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/manual_mitigation.py` & `kentik-api-1.0.7/kentik_api/public/manual_mitigation.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/plan.py` & `kentik-api-1.0.7/kentik_api/public/plan.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/query_object.py` & `kentik-api-1.0.7/kentik_api/public/query_object.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/saved_filter.py` & `kentik-api-1.0.7/kentik_api/public/saved_filter.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/site.py` & `kentik-api-1.0.7/kentik_api/public/site.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/tag.py` & `kentik-api-1.0.7/kentik_api/public/tag.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/tenant.py` & `kentik-api-1.0.7/kentik_api/public/tenant.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/types.py` & `kentik-api-1.0.7/kentik_api/public/types.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/public/user.py` & `kentik-api-1.0.7/kentik_api/public/user.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/batch_operations_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/batch_operations_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/conversions.py` & `kentik-api-1.0.7/kentik_api/requests_payload/conversions.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/custom_applications_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/custom_applications_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/custom_dimensions_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/custom_dimensions_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/devices_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/devices_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/interfaces_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/interfaces_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/labels_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/labels_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/manual_mitigations_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/manual_mitigations_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/plans_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/plans_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/populators_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/populators_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/queries_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/queries_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/saved_filters_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/saved_filters_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/sites_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/sites_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/tags_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/tags_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/tenants_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/tenants_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/users_payload.py` & `kentik-api-1.0.7/kentik_api/requests_payload/users_payload.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/requests_payload/validation.py` & `kentik-api-1.0.7/kentik_api/requests_payload/validation.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/agent.py` & `kentik-api-1.0.7/kentik_api/synthetics/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,24 +44,24 @@
     _last_authed: DateTime = DateTime.fromtimestamp(0, tz=timezone.utc)
 
     # read-write
     id: ID = ID()  # id is written in agent update request
     site_name: str = ""
     status: AgentStatus = AgentStatus.UNSPECIFIED
     alias: str = ""
-    ip: IP = IP()
+    ip: IP = field(default_factory=IP)
     lat: float = 0.0
     long: float = 0.0
     family: IPFamily = IPFamily.UNSPECIFIED
     asn: int = 0
     site_id: ID = ID()
     city: str = ""
     region: str = ""
     country: str = ""
-    local_ip: IP = IP()
+    local_ip: IP = field(default_factory=IP)
     cloud_region: str = ""
     cloud_provider: str = ""
     labels: List[str] = field(default_factory=list)
 
     @property
     def os(self) -> str:
         return self._os
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/api_connector.py` & `kentik-api-1.0.7/kentik_api/synthetics/api_connector.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/api_connector_protocol.py` & `kentik-api-1.0.7/kentik_api/synthetics/api_connector_protocol.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_client.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_client.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/agent.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     target: ID = ID()
     use_local_ip: bool = False
 
 
 @dataclass
 class AgentTestSettings(PingTraceTestSettings):
     tasks: List[TaskType] = field(default_factory=list_factory([TaskType.PING, TaskType.TRACE_ROUTE]))
-    agent: AgentTestSpecific = AgentTestSpecific()
+    agent: AgentTestSpecific = field(default_factory=AgentTestSpecific)
 
 
 AgentTestT = TypeVar("AgentTestT", bound="AgentTest")
 
 
 @dataclass
 class AgentTest(PingTraceTest):
     type: TestType = field(init=False, default=TestType.AGENT)
-    settings: AgentTestSettings = field(default=AgentTestSettings(agent_ids=[]))
+    settings: AgentTestSettings = field(default_factory=AgentTestSettings)
 
     @classmethod
     def create(cls: Type[AgentTestT], name: str, target: str, agent_ids: List[str]) -> AgentTestT:
         return cls(
             name=name,
             settings=AgentTestSettings(
                 agent_ids=agent_ids,
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/base.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/base.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/dns.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/dns.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     servers: List[str] = field(default_factory=list)
     port: int = 0
 
 
 @dataclass
 class DNSTestSettings(SynTestSettings):
     tasks: List[TaskType] = field(default_factory=list_factory([TaskType.DNS]))
-    dns: DNSTestSpecific = DNSTestSpecific()
+    dns: DNSTestSpecific = field(default_factory=DNSTestSpecific)
 
     @classmethod
     def task_name(cls) -> Optional[str]:
         return "dns"
 
 
 DNSTestT = TypeVar("DNSTestT", bound="DNSTest")
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/dns_grid.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/dns_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 DSNGridTestSpecific = DNSTestSpecific
 
 
 @dataclass
 class DNSGridTestSettings(SynTestSettings):
     tasks: List[TaskType] = field(default_factory=list_factory([TaskType.DNS]))
-    dns_grid: DSNGridTestSpecific = DSNGridTestSpecific()
+    dns_grid: DSNGridTestSpecific = field(default_factory=DSNGridTestSpecific)
 
 
 DNSGridTestT = TypeVar("DNSGridTestT", bound="DNSGridTest")
 
 
 @dataclass
 class DNSGridTest(SynTest):
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/flow.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 FlowTestT = TypeVar("FlowTestT", bound="FlowTest")
 
 
 @dataclass
 class FlowTest(PingTraceTest):
     type: TestType = field(init=False, default=TestType.FLOW)
-    settings: FlowTestSettings = field(default=FlowTestSettings(agent_ids=[]))
+    settings: FlowTestSettings = field(default_factory=FlowTestSettings)
 
     # noinspection PyShadowingBuiltins
     @classmethod
     def create(
         cls: Type[FlowTestT],
         name: str,
         target: str,
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/hostname.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/hostname.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     target: str = ""
 
 
 @dataclass
 class HostnameTestSettings(PingTraceTestSettings):
     tasks: List[TaskType] = field(default_factory=list_factory([TaskType.PING, TaskType.TRACE_ROUTE]))
-    hostname: HostnameTestSpecific = HostnameTestSpecific()
+    hostname: HostnameTestSpecific = field(default_factory=HostnameTestSpecific)
 
 
 HostnameTestT = TypeVar("HostnameTestT", bound="HostnameTest")
 
 
 @dataclass
 class HostnameTest(PingTraceTest):
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/ip.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/ip.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     targets: List[IP] = field(default_factory=list)
 
 
 @dataclass
 class IPTestSettings(PingTraceTestSettings):
     tasks: List[TaskType] = field(default_factory=list_factory([TaskType.PING, TaskType.TRACE_ROUTE]))
-    ip: IPTestSpecific = IPTestSpecific()
+    ip: IPTestSpecific = field(default_factory=IPTestSpecific)
 
 
 IPTestT = TypeVar("IPTestT", bound="IPTest")
 
 
 @dataclass
 class IPTest(PingTraceTest):
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/network_grid.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/network_grid.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 NetworkGridTestSpecific = IPTestSpecific
 
 
 @dataclass
 class GridTestSettings(PingTraceTestSettings):
     tasks: List[TaskType] = field(default_factory=list_factory([TaskType.PING, TaskType.TRACE_ROUTE]))
-    network_grid: NetworkGridTestSpecific = NetworkGridTestSpecific()
+    network_grid: NetworkGridTestSpecific = field(default_factory=NetworkGridTestSpecific)
 
 
 NetworkGridTestT = TypeVar("NetworkGridTestT", bound="NetworkGridTest")
 
 
 @dataclass
 class NetworkGridTest(PingTraceTest):
     type: TestType = field(init=False, default=TestType.NETWORK_GRID)
-    settings: GridTestSettings = field(default=GridTestSettings(agent_ids=[]))
+    settings: GridTestSettings = field(default_factory=GridTestSettings)
 
     @classmethod
     def create(cls: Type[NetworkGridTestT], name: str, targets: List[str], agent_ids: List[str]) -> NetworkGridTestT:
         return cls(
             name=name,
             settings=GridTestSettings(
                 agent_ids=agent_ids,
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/network_mesh.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/network_mesh.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     use_local_ip: bool = False
 
 
 @dataclass
 class NetworkMeshTestSettings(PingTraceTestSettings):
     tasks: List[TaskType] = field(default_factory=list_factory([TaskType.PING, TaskType.TRACE_ROUTE]))
-    network_mesh: NetworkMeshTestSpecific = NetworkMeshTestSpecific()
+    network_mesh: NetworkMeshTestSpecific = field(default_factory=NetworkMeshTestSpecific)
 
 
 NetworkMeshTestT = TypeVar("NetworkMeshTestT", bound="NetworkMeshTest")
 
 
 @dataclass
 class NetworkMeshTest(PingTraceTest):
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/page_load.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/page_load.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/results.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/results.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 
 PingTaskResultsT = TypeVar("PingTaskResultsT", bound="PingTaskResults")
 
 
 @dataclass
 class PingTaskResults(_ConfigElement):
     target: str = ""  # hostname or IP
-    packet_loss: PacketLossData = PacketLossData()
-    latency: MetricData = MetricData()
-    jitter: MetricData = MetricData()
-    dst_ip: IP = IP()
+    packet_loss: PacketLossData = field(default_factory=PacketLossData)
+    latency: MetricData = field(default_factory=MetricData)
+    jitter: MetricData = field(default_factory=MetricData)
+    dst_ip: IP = field(default_factory=IP)
 
 
 HttpResponseDataT = TypeVar("HttpResponseDataT", bound="HttpResponseData")
 
 
 @dataclass
 class HttpResponseData(_ConfigElement):
@@ -52,17 +52,17 @@
 
 HttpTaskResultsT = TypeVar("HttpTaskResultsT", bound="HttpTaskResults")
 
 
 @dataclass
 class HttpTaskResults(_ConfigElement):
     target: str = ""  # url
-    latency: MetricData = MetricData()
-    response: HttpResponseData = HttpResponseData()
-    dst_ip: IP = IP()
+    latency: MetricData = field(default_factory=MetricData)
+    response: HttpResponseData = field(default_factory=HttpResponseData)
+    dst_ip: IP = field(default_factory=IP)
 
 
 DnsResponseDataT = TypeVar("DnsResponseDataT", bound="DnsResponseData")
 
 
 @dataclass
 class DnsResponseData(_ConfigElement):
@@ -73,16 +73,16 @@
 DnsTaskResultsT = TypeVar("DnsTaskResultsT", bound="DnsTaskResults")
 
 
 @dataclass
 class DnsTaskResults(_ConfigElement):
     target: str = ""  # url
     server: str = ""
-    latency: MetricData = MetricData()
-    response: DnsResponseData = DnsResponseData()
+    latency: MetricData = field(default_factory=MetricData)
+    response: DnsResponseData = field(default_factory=DnsResponseData)
 
 
 TaskResultsT = TypeVar("TaskResultsT", bound="TaskResults")
 
 
 @dataclass
 class TaskResults:
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/traces.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/traces.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 
 NetNodeT = TypeVar("NetNodeT", bound="NetNode")
 
 
 @dataclass
 class NetNode(_ConfigElement):
-    ip: IP = IP()
+    ip: IP = field(default_factory=IP)
     asn: int = 0
     as_name: str = ""
-    location: Location = Location()
+    location: Location = field(default_factory=Location)
     dns_name: str = ""
     device_id: ID = ID()
     site_id: ID = ID()
 
 
 StatsT = TypeVar("StatsT", bound="Stats")
 
@@ -62,16 +62,16 @@
 
 PathT = TypeVar("PathT", bound="Path")
 
 
 @dataclass
 class Path(_ConfigElement):
     agent_id: ID = ID()
-    target_ip: IP = IP()
-    hop_count: Stats = Stats()
+    target_ip: IP = field(default_factory=IP)
+    hop_count: Stats = field(default_factory=Stats)
     max_as_path_length: int = 0
     traces: List[PathTrace] = field(default_factory=list)
     time: DateTime = DateTime.fromtimestamp(0, tz=timezone.utc)
 
 
 TraceResponseT = TypeVar("TraceResponseT", bound="TraceResponse")
```

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/synth_tests/url.py` & `kentik-api-1.0.7/kentik_api/synthetics/synth_tests/url.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/synthetics/types.py` & `kentik-api-1.0.7/kentik_api/synthetics/types.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/utils/auth.py` & `kentik-api-1.0.7/kentik_api/utils/auth.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/utils/device_cache.py` & `kentik-api-1.0.7/kentik_api/utils/device_cache.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api/utils/time_sequence.py` & `kentik-api-1.0.7/kentik_api/utils/time_sequence.py`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/kentik_api.egg-info/PKG-INFO` & `kentik-api-1.0.7/kentik_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kentik-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Kentik API SDK
 Author-email: Martin Machacek <martin.machacek@kentik.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -22,102 +22,106 @@
 This is a Python client library for [Kentik APIs](https://kb.kentik.com/v0/Ab09.htm).
 It is distributed as [_kentik-api_ PyPI package](https://pypi.org/project/kentik-api/).
 
 ## Installation with pip
 
 1. Install the library using pip:  
 ```pip3 install kentik-api```
-1. Check installation successful - no errors should be reported:  
+2. Check installation successful - no errors should be reported:
 ```python3 -c "import kentik_api"```
-1. Run an example (optional):
+3. Run an example (optional):
   ```bash
   export KTAPI_AUTH_EMAIL=<your kentik api credentials email>
   export KTAPI_AUTH_TOKEN=<your kentik api credentials token>
   python3 examples/sites_example.py
   ```
 
 ## Getting started
 
 The best way to get started coding with the SDK is to study provided [examples](examples).
 
 Interfaces for manipulating all Kentik API resources are available under the `KentikAPI` object.  
 Every Kentik API resource is represented by a public class, and all related data types are located in the same source
 file or directory as the implementation of the class:
-- [CustomApplication](kentik_apiublic/custom_application.py)
-- [CustomDimension](kentik_apiublic/custom_dimension.py)
-- [DeviceLabel](kentik_apiublic/device_label.py)
-- [Device](kentik_apiublic/device.py)
-- [ManualMitigation](kentik_apiublic/manual_mitigation.py)
-- [Plan](kentik_apiublic/plan.py)
-- [QueryObject](kentik_apiublic/query_object.py)
-- [QuerySQL](kentik_apiublic/query_sql.py)
-- [SavedFilter](kentik_apiublic/saved_filter.py)
-- [Site](kentik_apiublic/site.py)
-- [Synthetic Tests](kentik_api/synthetics/)
-- [Tag](kentik_apiublic/tag.py)
-- [Tenant](kentik_apiublic/tenant.py)
-- [User](kentik_apiublic/user.py)
+- [CustomApplication](kentik_api/public/custom_application.py)
+- [CustomDimension](kentik_api/public/custom_dimension.py)
+- [DeviceLabel](kentik_api/public/device_label.py)
+- [Device](kentik_api/public/device.py)
+- [ManualMitigation](kentik_api/public/manual_mitigation.py)
+- [Plan](kentik_api/public/plan.py)
+- [QueryObject](kentik_api/public/query_object.py)
+- [QuerySQL](kentik_api/public/query_sql.py)
+- [SavedFilter](kentik_api/public/saved_filter.py)
+- [Site](kentik_api/public/site.py)
+- [Synthetic Tests](kentik_api/synthetics)
+- [Tag](kentik_api/public/tag.py)
+- [Tenant](kentik_api/public/tenant.py)
+- [User](kentik_api/public/user.py)
 
 ## Additional utilities available in the `utils` sub-module
 
 ### Authentication support
 
-- `get_credentials`: function for retrieving authentication credentials from the environment or a profile stored on disk.
-  API authentication credentials can be provided via environment variables `KTAPI_AUTH_EMAIL` and `KTAPI_AUTH_TOKEN`
-  or via named profile (specified as argument to the `get_credentials` functions, defaulting to `default`) which is
-  a JSON file with following format:
+- `get_credentials`: function for retrieving authentication credentials from the environment or a profile stored on
+  the disk. API authentication credentials can be provided via environment variables `KTAPI_AUTH_EMAIL` and
+  `KTAPI_AUTH_TOKEN` or via named profile (specified as argument to the `get_credentials` functions, defaulting
+  to `default`) which is a JSON file with following format:
 ```json
 {
   "email": "<email address>",
   "api-key": "<the API key>"
 }
 ```
-Path to the profile file can be provided in `KTAPI_CFG_FILE`. Otherwise it is first searched in
+Path to the profile file can be provided in `KTAPI_CFG_FILE`. Otherwise, it is first searched in
 `${KTAPI_HOME}/<profile_name>` and then in `${HOME}/.kentik/<profile_name>`.
 
 ### Support for caching of device data
 
 The `DeviceCache` class allows caching of device related data obtained from the Kentik API. It internally builds
-index of devices by `name` and by `id`. Devices are represented by the [Device](kentik_apiublic/device.py) class which
+index of devices by `name` and by `id`. Devices are represented by the [Device](kentik_api/public/device.py) class which
 internally builds dictionary of device interfaces  (represented by the `DeviceInterface` class) by `name`.
 
 ## Analytic support
 
 The `analytics` package provides support for processing Kentik time series data using Pandas Dataframes.
 The [pandas](https://pandas.pydata.org) and [PyYAML](https://pyyaml.org/) modules are required by the `analytics`
 sub-module and are automatically installed with the `kentik-api[analytics]` option.
-See [analytics readme](kentik_apinalytics/README.md) for more details.
+See [analytics readme](kentik_api/analytics/README.md) for more details.
 
 ## Available Examples
 
-- [alerting_example.py](exampleslerting_example.py) - create Manual Mitigation
-- [applications_example.py](examplespplications_example.py) - create/update/delete Custom Application
-- [bulk_user_create.py](examplesulk_user_create.py) - create users from YAML file
-- [devices_example.py](examplesevices_example.py) - create/update/get/delete/list Devices
-- [dimensions_example.py](examplesimensions_example.py) - create/update/get/delete/list Custom Dimensions, create/update/delete Populator
-- [labels_example.py](examplesabels_example.py) - create/update/get/delete/list Device Labels
-- [my_kentik_portal_example.py](examplesy_kentik_portal_example.py) - get/list Tenants, create/delete Tenant User
-- [plans_example.py](exampleslans_example.py) - list plans
-- [queries_example.py](examplesueries_example.py) - query for SQL/URL/data/chart
-- [saved_filters_example.py](examplesaved_filters_example.py) - create/update/get/delete/list Saved Filters
-- [sites_example.py](examplesites_example.py) - create/update/get/delete/list Sites
-- [tags_example.py](examplesags_example.py) - create/update/get/delete/list Tags
-- [users_example.py](examplessers_example.py) - create/update/get/delete/list Users
-- [error_handling_example.py](examplesrror_handling_example.py) - handling errors raised by the library
-- [analytics_example_sql.py](examplesnalytics_example_sql.py) - use of `SQLQueryDefinition`, `flatness_analysis` method and the`DeviceCache`
-- [analytics_example_topx.py](examplesnalytics_example_sql.py) - use of `DataQueryDefinition`, `flatness_analysis` method and the`DeviceCache`
-  (see also [analytics readme](kentik_apinalytics/README.md))
-- [synthetics_example.py](examplesynthetics_example.py) - interact with synthetics API
-- [cloud_export_example.py](examplesloud_export_example.py) - interact with cloud export API
+- [alerting_example.py](examples/alerting_example.py) - create Manual Mitigation
+- [applications_example.py](examples/applications_example.py) - create/update/delete Custom Application
+- [bulk_user_create.py](examples/bulk_user_create.py) - create users from YAML file
+- [devices_example.py](examples/devices_example.py) - create/update/get/delete/list Devices
+- [dimensions_example.py](examples/dimensions_example.py) - create/update/get/delete/list Custom Dimensions,
+                                                            create/update/delete Populator
+- [labels_example.py](examples/labels_example.py) - create/update/get/delete/list Device Labels
+- [my_kentik_portal_example.py](examples/my_kentik_portal_example.py) - get/list Tenants, create/delete Tenant User
+- [plans_example.py](examples/plans_example.py) - list plans
+- [queries_example.py](examples/queries_example.py) - query for SQL/URL/data/chart
+- [saved_filters_example.py](examples/saved_filters_example.py) - create/update/get/delete/list Saved Filters
+- [sites_example.py](examples/sites_example.py) - create/update/get/delete/list Sites
+- [tags_example.py](examples/tags_example.py) - create/update/get/delete/list Tags
+- [users_example.py](examples/users_example.py) - create/update/get/delete/list Users
+- [error_handling_example.py](examples/error_handling_example.py) - handling errors raised by the library
+- [analytics_example_sql.py](examples/analytics_example_sql.py) - use of `SQLQueryDefinition`, `flatness_analysis`
+                                                                  methods and the`DeviceCache`
+- [analytics_example_topx.py](examples/analytics_example_sql.py) - use of `DataQueryDefinition`, `flatness_analysis`
+                                                                  methods and the`DeviceCache`
+  (see also [analytics readme](kentik_api/analytics/README.md))
+- [synthetics_example.py](examples/synthetics_example.py) - interact with synthetics API
+- [cloud_export_example.py](examples/cloud_export_example.py) - interact with cloud export API
 
 ## Development
 
 [Instructions for developers](docs/README.md)
 
 ## Open-source libraries
 
 This software uses the following open-source libraries:
 - [dacite](https://pypi.org/project/dacite/) by Konrad Hałas - MIT License
 - [requests](https://pypi.org/project/requests/) by Kenneth Reitz - Apache Software License (Apache 2.0)
-- [typing-extensions](https://pypi.org/project/typing-extensions/) by  Guido van Rossum, Jukka Lehtosalo, Lukasz Langa, Michael Lee - PSFL License
+- [typing-extensions](https://pypi.org/project/typing-extensions/) by  Guido van Rossum, Jukka Lehtosalo, Lukasz Langa,
+                                                                   Michael Lee - PSFL License
 - [pandas](https://pandas.pydata.org) supported by NumFOCUS - BSD 3-Clause License
 - [pyyaml](https://pyyaml.org/) by Ingy döt Net and Kirill Simonov - MIT license
```

### Comparing `kentik-api-1.0.6/kentik_api.egg-info/SOURCES.txt` & `kentik-api-1.0.7/kentik_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/pyproject.toml` & `kentik-api-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kentik-api-1.0.6/setup.py` & `kentik-api-1.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # mypy: ignore-errors
+import logging
 import os
 import shutil
 import subprocess
-from distutils import log
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from setuptools import Command, setup
 
 # The directory containing this file
 HERE = Path(__file__).parent
 
+log = logging.getLogger()
 
-def run_cmd(cmd, reporter) -> None:
+
+def run_cmd(cmd) -> None:
     """Run arbitrary command as subprocess"""
-    reporter("Run command: {}".format(str(cmd)), level=log.DEBUG)
+    log.debug("Running command: %s", str(cmd))
     try:
         subprocess.check_call(cmd)
     except subprocess.CalledProcessError as ex:
-        reporter(str(ex), level=log.ERROR)
+        log.error("%s", ex)
         exit(1)
 
 
 class Pylint(Command):
     """Custom command to run Pylint"""
 
     description = "run Pylint on kentik_api, tests and examples directories; read configuration from pyproject.toml"
@@ -36,15 +38,15 @@
 
     def run(self):
         """Run command."""
         cmd = ["pylint"]
         paths = ["kentik_api"]
         for path in paths:
             cmd.append(path)
-        run_cmd(cmd, self.announce)
+        run_cmd(cmd)
 
 
 # noinspection PyAttributeOutsideInit
 class Mypy(Command):
     """Custom command to run Mypy"""
 
     description = "run Mypy on kentik_api, tests and examples directories; read configuration from pyproject.toml"
@@ -60,15 +62,15 @@
             assert os.path.exists(package), "Path {} does not exist.".format(package)
 
     def run(self):
         """Run command"""
         cmd = ["mypy"]
         for package in self.packages:
             cmd.append(package)
-        run_cmd(cmd, self.announce)
+        run_cmd(cmd)
 
 
 class Pytest(Command):
     """Custom command to run pytest"""
 
     description = "run pytest on all relevant code; read configuration from pyproject.toml"
     user_options = []
@@ -78,15 +80,15 @@
 
     def finalize_options(self):
         pass
 
     def run(self):
         """Run command"""
         cmd = ["pytest"]
-        run_cmd(cmd, self.announce)
+        run_cmd(cmd)
 
 
 # noinspection PyAttributeOutsideInit
 class Format(Command):
     """Custom command to run black + isort"""
 
     description = "run black and isort on all relevant code; read configuration from pyproject.toml"
@@ -112,24 +114,24 @@
     def _black(self) -> None:
         print("Tool: black")
         cmd = ["black"]
         if self.check:
             cmd.append("--check")
         for d in self.dirs:
             cmd.append(d)
-        run_cmd(cmd, self.announce)
+        run_cmd(cmd)
 
     def _isort(self) -> None:
         print("Tool: isort")
         cmd = ["isort"]
         if self.check:
             cmd.append("--check")
         for d in self.dirs:
             cmd.append(d)
-        run_cmd(cmd, self.announce)
+        run_cmd(cmd)
 
 
 # noinspection PyAttributeOutsideInit
 class GenerateGRPCStubs(Command):
     """Generate Python gRPC stubs from proto files in the source repo."""
 
     description = "Generate Python stubs from proto files in the source repo"
@@ -162,15 +164,15 @@
         print("for following Kentik APIs:")
         for a in apis:
             print(f"\t{a['name']}/{a['version']}")
 
         deps = [
             "protovendor/github.com/googleapis/googleapis",
             "protovendor/github.com/grpc-ecosystem/grpc-gateway",
-            "protovendor/github.com/protocolbuffers/src",
+            "protovendor/github.com/protocolbuffers/protobuf/src",
         ]
         # cleanup destination directory
         shutil.rmtree(dst_path, ignore_errors=True)  # ignore "No such file or directory"
         # create destination directory, if it does not exist
         dst = Path(dst_path)
         dst.mkdir(parents=True)
         # checkout source repo and copy stubs
@@ -193,15 +195,15 @@
             for d in deps:
                 cmd.append(
                     f"-I{tmp}/{d}/",
                 )
             for a in apis:
                 for f in Path(f"{tmp}/proto/kentik/").joinpath(a["name"]).joinpath(a["version"]).glob("*.proto"):
                     cmd.append(f.as_posix())
-            run_cmd(cmd, self.announce)
+            run_cmd(cmd)
 
 
 setup(
     cmdclass={
         "mypy": Mypy,
         "pylint": Pylint,
         "pytest": Pytest,
```

