# Comparing `tmp/polarismesh_specification-1.3.0a7.tar.gz` & `tmp/polarismesh_specification-1.3.1.tar.gz`

## Comparing `polarismesh_specification-1.3.0a7.tar` & `polarismesh_specification-1.3.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    15838 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0     4864 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/pyproject.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a7/PKG-INFO
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0     8830 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.1/PKG-INFO
```

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63onfig_file.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xa3\x06\n\x0f\x43onfigFileGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfileCount\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x08user_ids\x18\n \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x0b \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\r \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x0e \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12,\n\x08\x65\x64itable\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x05owner\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xfb\x05\n\nConfigFile\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\t \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0crelease_time\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nrelease_by\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\x0cis_encrypted\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"g\n\rConfigFileTag\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf8\x04\n\x11\x43onfigFileRelease\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf9\x05\n\x18\x43onfigFileReleaseHistory\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04type\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0c \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xbe\x03\n\x12\x43onfigFileTemplate\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xc2\x03\n\x14\x43lientConfigFileInfo\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12)\n\x03md5\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\x0cis_encrypted\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\x08\x64\x61ta_key\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\npublic_key\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xb2\x01\n\x1c\x43lientWatchConfigFileRequest\x12/\n\tclient_ip\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cservice_name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x0bwatch_files\x18\x03 \x03(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xa5\x01\n\x17\x43onfigFileExportRequest\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06groups\x18\x02 \x03(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05names\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValueB\x8e\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x0f\x43onfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63onfig_file.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xa3\x06\n\x0f\x43onfigFileGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfileCount\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x08user_ids\x18\n \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x0b \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\r \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x0e \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12,\n\x08\x65\x64itable\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x05owner\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xaf\x06\n\nConfigFile\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\t \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0crelease_time\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nrelease_by\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\x0cis_encrypted\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0c\x65ncrypt_algo\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"g\n\rConfigFileTag\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf8\x04\n\x11\x43onfigFileRelease\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf9\x05\n\x18\x43onfigFileReleaseHistory\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04type\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0c \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xbe\x03\n\x12\x43onfigFileTemplate\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xc2\x03\n\x14\x43lientConfigFileInfo\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12)\n\x03md5\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\x0cis_encrypted\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\x08\x64\x61ta_key\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\npublic_key\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xb2\x01\n\x1c\x43lientWatchConfigFileRequest\x12/\n\tclient_ip\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cservice_name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x0bwatch_files\x18\x03 \x03(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xa5\x01\n\x17\x43onfigFileExportRequest\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06groups\x18\x02 \x03(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05names\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValueB\x8e\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x0f\x43onfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n6com.tencent.polaris.specification.api.v1.config.manageB\017ConfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manage'
   _CONFIGFILEGROUP._serialized_start=58
   _CONFIGFILEGROUP._serialized_end=861
   _CONFIGFILE._serialized_start=864
-  _CONFIGFILE._serialized_end=1627
-  _CONFIGFILETAG._serialized_start=1629
-  _CONFIGFILETAG._serialized_end=1732
-  _CONFIGFILERELEASE._serialized_start=1735
-  _CONFIGFILERELEASE._serialized_end=2367
-  _CONFIGFILERELEASEHISTORY._serialized_start=2370
-  _CONFIGFILERELEASEHISTORY._serialized_end=3131
-  _CONFIGFILETEMPLATE._serialized_start=3134
-  _CONFIGFILETEMPLATE._serialized_end=3580
-  _CLIENTCONFIGFILEINFO._serialized_start=3583
-  _CLIENTCONFIGFILEINFO._serialized_end=4033
-  _CLIENTWATCHCONFIGFILEREQUEST._serialized_start=4036
-  _CLIENTWATCHCONFIGFILEREQUEST._serialized_end=4214
-  _CONFIGFILEEXPORTREQUEST._serialized_start=4217
-  _CONFIGFILEEXPORTREQUEST._serialized_end=4382
+  _CONFIGFILE._serialized_end=1679
+  _CONFIGFILETAG._serialized_start=1681
+  _CONFIGFILETAG._serialized_end=1784
+  _CONFIGFILERELEASE._serialized_start=1787
+  _CONFIGFILERELEASE._serialized_end=2419
+  _CONFIGFILERELEASEHISTORY._serialized_start=2422
+  _CONFIGFILERELEASEHISTORY._serialized_end=3183
+  _CONFIGFILETEMPLATE._serialized_start=3186
+  _CONFIGFILETEMPLATE._serialized_end=3632
+  _CLIENTCONFIGFILEINFO._serialized_start=3635
+  _CLIENTCONFIGFILEINFO._serialized_end=4085
+  _CLIENTWATCHCONFIGFILEREQUEST._serialized_start=4088
+  _CLIENTWATCHCONFIGFILEREQUEST._serialized_end=4266
+  _CONFIGFILEEXPORTREQUEST._serialized_start=4269
+  _CONFIGFILEEXPORTREQUEST._serialized_end=4434
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,20 @@
     WATCH_FILES_FIELD_NUMBER: _ClassVar[int]
     client_ip: _wrappers_pb2.StringValue
     service_name: _wrappers_pb2.StringValue
     watch_files: _containers.RepeatedCompositeFieldContainer[ClientConfigFileInfo]
     def __init__(self, client_ip: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., watch_files: _Optional[_Iterable[_Union[ClientConfigFileInfo, _Mapping]]] = ...) -> None: ...
 
 class ConfigFile(_message.Message):
-    __slots__ = ["comment", "content", "create_by", "create_time", "format", "group", "id", "is_encrypted", "modify_by", "modify_time", "name", "namespace", "release_by", "release_time", "status", "tags"]
+    __slots__ = ["comment", "content", "create_by", "create_time", "encrypt_algo", "format", "group", "id", "is_encrypted", "modify_by", "modify_time", "name", "namespace", "release_by", "release_time", "status", "tags"]
     COMMENT_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     CREATE_BY_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    ENCRYPT_ALGO_FIELD_NUMBER: _ClassVar[int]
     FORMAT_FIELD_NUMBER: _ClassVar[int]
     GROUP_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     IS_ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
     MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
     MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
@@ -56,27 +57,28 @@
     RELEASE_TIME_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
     comment: _wrappers_pb2.StringValue
     content: _wrappers_pb2.StringValue
     create_by: _wrappers_pb2.StringValue
     create_time: _wrappers_pb2.StringValue
+    encrypt_algo: _wrappers_pb2.StringValue
     format: _wrappers_pb2.StringValue
     group: _wrappers_pb2.StringValue
     id: _wrappers_pb2.UInt64Value
     is_encrypted: _wrappers_pb2.BoolValue
     modify_by: _wrappers_pb2.StringValue
     modify_time: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
     release_by: _wrappers_pb2.StringValue
     release_time: _wrappers_pb2.StringValue
     status: _wrappers_pb2.StringValue
     tags: _containers.RepeatedCompositeFieldContainer[ConfigFileTag]
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., format: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., tags: _Optional[_Iterable[_Union[ConfigFileTag, _Mapping]]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., is_encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., format: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., tags: _Optional[_Iterable[_Union[ConfigFileTag, _Mapping]]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., is_encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., encrypt_algo: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class ConfigFileExportRequest(_message.Message):
     __slots__ = ["groups", "names", "namespace"]
     GROUPS_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     NAMES_FIELD_NUMBER: _ClassVar[int]
     groups: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
```

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from ..config_manage import config_file_pb2 as config__file__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x63onfig_file_response.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x11\x63onfig_file.proto\"n\n\x14\x43onfigSimpleResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xe0\x02\n\x0e\x43onfigResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x0f\x63onfigFileGroup\x18\x03 \x01(\x0b\x32\x13.v1.ConfigFileGroup\x12\"\n\nconfigFile\x18\x04 \x01(\x0b\x32\x0e.v1.ConfigFile\x12\x30\n\x11\x63onfigFileRelease\x18\x05 \x01(\x0b\x32\x15.v1.ConfigFileRelease\x12>\n\x18\x63onfigFileReleaseHistory\x18\x06 \x01(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x32\n\x12\x63onfigFileTemplate\x18\x07 \x01(\x0b\x32\x16.v1.ConfigFileTemplate\"\xc6\x01\n\x18\x43onfigBatchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12%\n\tresponses\x18\x04 \x03(\x0b\x32\x12.v1.ConfigResponse\"\x9d\x03\n\x18\x43onfigBatchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x10\x63onfigFileGroups\x18\x04 \x03(\x0b\x32\x13.v1.ConfigFileGroup\x12#\n\x0b\x63onfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\x31\n\x12\x63onfigFileReleases\x18\x06 \x03(\x0b\x32\x15.v1.ConfigFileRelease\x12@\n\x1a\x63onfigFileReleaseHistories\x18\x07 \x03(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x33\n\x13\x63onfigFileTemplates\x18\x08 \x03(\x0b\x32\x16.v1.ConfigFileTemplate\"\x9c\x01\n\x14\x43onfigClientResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\nconfigFile\x18\x03 \x01(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xf0\x01\n\x14\x43onfigImportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x11\x63reateConfigFiles\x18\x03 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\'\n\x0fskipConfigFiles\x18\x04 \x03(\x0b\x32\x0e.v1.ConfigFile\x12,\n\x14overwriteConfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\"\x99\x01\n\x14\x43onfigExportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.BytesValueB\x96\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x17\x43onfigFileResponseProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x63onfig_file_response.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x11\x63onfig_file.proto\"n\n\x14\x43onfigSimpleResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xe0\x02\n\x0e\x43onfigResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x0f\x63onfigFileGroup\x18\x03 \x01(\x0b\x32\x13.v1.ConfigFileGroup\x12\"\n\nconfigFile\x18\x04 \x01(\x0b\x32\x0e.v1.ConfigFile\x12\x30\n\x11\x63onfigFileRelease\x18\x05 \x01(\x0b\x32\x15.v1.ConfigFileRelease\x12>\n\x18\x63onfigFileReleaseHistory\x18\x06 \x01(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x32\n\x12\x63onfigFileTemplate\x18\x07 \x01(\x0b\x32\x16.v1.ConfigFileTemplate\"\xc6\x01\n\x18\x43onfigBatchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12%\n\tresponses\x18\x04 \x03(\x0b\x32\x12.v1.ConfigResponse\"\x9d\x03\n\x18\x43onfigBatchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x10\x63onfigFileGroups\x18\x04 \x03(\x0b\x32\x13.v1.ConfigFileGroup\x12#\n\x0b\x63onfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\x31\n\x12\x63onfigFileReleases\x18\x06 \x03(\x0b\x32\x15.v1.ConfigFileRelease\x12@\n\x1a\x63onfigFileReleaseHistories\x18\x07 \x03(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x33\n\x13\x63onfigFileTemplates\x18\x08 \x03(\x0b\x32\x16.v1.ConfigFileTemplate\"\x9c\x01\n\x14\x43onfigClientResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\nconfigFile\x18\x03 \x01(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xf0\x01\n\x14\x43onfigImportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x11\x63reateConfigFiles\x18\x03 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\'\n\x0fskipConfigFiles\x18\x04 \x03(\x0b\x32\x0e.v1.ConfigFile\x12,\n\x14overwriteConfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\"\x99\x01\n\x14\x43onfigExportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.BytesValue\"\xaa\x01\n\x1e\x43onfigEncryptAlgorithmResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nalgorithms\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValueB\x96\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x17\x43onfigFileResponseProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_response_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n6com.tencent.polaris.specification.api.v1.config.manageB\027ConfigFileResponseProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manage'
@@ -33,8 +33,10 @@
   _CONFIGBATCHQUERYRESPONSE._serialized_end=1167
   _CONFIGCLIENTRESPONSE._serialized_start=1170
   _CONFIGCLIENTRESPONSE._serialized_end=1326
   _CONFIGIMPORTRESPONSE._serialized_start=1329
   _CONFIGIMPORTRESPONSE._serialized_end=1569
   _CONFIGEXPORTRESPONSE._serialized_start=1572
   _CONFIGEXPORTRESPONSE._serialized_end=1725
+  _CONFIGENCRYPTALGORITHMRESPONSE._serialized_start=1728
+  _CONFIGENCRYPTALGORITHMRESPONSE._serialized_end=1898
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,24 @@
     CONFIGFILE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     configFile: _config_file_pb2.ClientConfigFileInfo
     info: _wrappers_pb2.StringValue
     def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., configFile: _Optional[_Union[_config_file_pb2.ClientConfigFileInfo, _Mapping]] = ...) -> None: ...
 
+class ConfigEncryptAlgorithmResponse(_message.Message):
+    __slots__ = ["algorithms", "code", "info"]
+    ALGORITHMS_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    INFO_FIELD_NUMBER: _ClassVar[int]
+    algorithms: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
+    code: _wrappers_pb2.UInt32Value
+    info: _wrappers_pb2.StringValue
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., algorithms: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ...) -> None: ...
+
 class ConfigExportResponse(_message.Message):
     __slots__ = ["code", "data", "info"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     DATA_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     data: _wrappers_pb2.BytesValue
```

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ncode.proto\x12\x02v1*\x82%\n\x04\x43ode\x12\x0b\n\x07Unknown\x10\x00\x12\x14\n\x0e\x45xecuteSuccess\x10\xc0\x9a\x0c\x12\x12\n\x0c\x44\x61taNoChange\x10\xc1\x9a\x0c\x12\x12\n\x0cNoNeedUpdate\x10\xc2\x9a\x0c\x12\x10\n\nBadRequest\x10\x80\xb5\x18\x12\x14\n\x0eParseException\x10\x81\xb5\x18\x12\x12\n\x0c\x45mptyRequest\x10\x82\xb5\x18\x12\x18\n\x12\x42\x61tchSizeOverLimit\x10\x83\xb5\x18\x12\x1d\n\x17InvalidDiscoverResource\x10\x84\xb5\x18\x12\x16\n\x10InvalidRequestID\x10\xe4\xb5\x18\x12\x15\n\x0fInvalidUserName\x10\xe5\xb5\x18\x12\x16\n\x10InvalidUserToken\x10\xe6\xb5\x18\x12\x16\n\x10InvalidParameter\x10\xe7\xb5\x18\x12\x19\n\x13\x45mptyQueryParameter\x10\xe8\xb5\x18\x12\x1e\n\x18InvalidQueryInsParameter\x10\xe9\xb5\x18\x12\x1a\n\x14InvalidNamespaceName\x10\xee\xb5\x18\x12\x1c\n\x16InvalidNamespaceOwners\x10\xef\xb5\x18\x12\x1b\n\x15InvalidNamespaceToken\x10\xf0\xb5\x18\x12\x18\n\x12InvalidServiceName\x10\xf8\xb5\x18\x12\x1a\n\x14InvalidServiceOwners\x10\xf9\xb5\x18\x12\x19\n\x13InvalidServiceToken\x10\xfa\xb5\x18\x12\x1c\n\x16InvalidServiceMetadata\x10\xfb\xb5\x18\x12\x19\n\x13InvalidServicePorts\x10\xfc\xb5\x18\x12\x1c\n\x16InvalidServiceBusiness\x10\xfd\xb5\x18\x12\x1e\n\x18InvalidServiceDepartment\x10\xfe\xb5\x18\x12\x18\n\x12InvalidServiceCMDB\x10\xff\xb5\x18\x12\x1b\n\x15InvalidServiceComment\x10\x80\xb6\x18\x12 \n\x1aInvalidServiceAliasComment\x10\x81\xb6\x18\x12\x17\n\x11InvalidInstanceID\x10\x82\xb6\x18\x12\x19\n\x13InvalidInstanceHost\x10\x83\xb6\x18\x12\x19\n\x13InvalidInstancePort\x10\x84\xb6\x18\x12\x19\n\x13InvalidServiceAlias\x10\x85\xb6\x18\x12\x1f\n\x19InvalidNamespaceWithAlias\x10\x86\xb6\x18\x12\x1f\n\x19InvalidServiceAliasOwners\x10\x87\xb6\x18\x12\x1d\n\x17InvalidInstanceProtocol\x10\x88\xb6\x18\x12\x1c\n\x16InvalidInstanceVersion\x10\x89\xb6\x18\x12\x1d\n\x17InvalidInstanceLogicSet\x10\x8a\xb6\x18\x12\x1c\n\x16InvalidInstanceIsolate\x10\x8b\xb6\x18\x12\x18\n\x12HealthCheckNotOpen\x10\x8c\xb6\x18\x12\x1c\n\x16HeartbeatOnDisabledIns\x10\x8d\xb6\x18\x12\x1a\n\x14HeartbeatExceedLimit\x10\x8e\xb6\x18\x12\x1b\n\x15HeartbeatTypeNotFound\x10\x8f\xb6\x18\x12\x15\n\x0fInvalidMetadata\x10\x96\xb6\x18\x12\x18\n\x12InvalidRateLimitID\x10\x97\xb6\x18\x12\x1c\n\x16InvalidRateLimitLabels\x10\x98\xb6\x18\x12\x1d\n\x17InvalidRateLimitAmounts\x10\x99\xb6\x18\x12\x1a\n\x14InvalidRateLimitName\x10\x9a\xb6\x18\x12\x1d\n\x17InvalidCircuitBreakerID\x10\xa0\xb6\x18\x12\"\n\x1cInvalidCircuitBreakerVersion\x10\xa1\xb6\x18\x12\x1f\n\x19InvalidCircuitBreakerName\x10\xa2\xb6\x18\x12$\n\x1eInvalidCircuitBreakerNamespace\x10\xa3\xb6\x18\x12!\n\x1bInvalidCircuitBreakerOwners\x10\xa4\xb6\x18\x12 \n\x1aInvalidCircuitBreakerToken\x10\xa5\xb6\x18\x12#\n\x1dInvalidCircuitBreakerBusiness\x10\xa6\xb6\x18\x12%\n\x1fInvalidCircuitBreakerDepartment\x10\xa7\xb6\x18\x12\"\n\x1cInvalidCircuitBreakerComment\x10\xa8\xb6\x18\x12\x1f\n\x19\x43ircuitBreakerRuleExisted\x10\xa9\xb6\x18\x12\x16\n\x10InvalidRoutingID\x10\xbc\xba\x18\x12\x1a\n\x14InvalidRoutingPolicy\x10\xbd\xba\x18\x12\x18\n\x12InvalidRoutingName\x10\xbe\xba\x18\x12\x1c\n\x16InvalidRoutingPriority\x10\xbf\xba\x18\x12\x1a\n\x14InvalidFaultDetectID\x10\x84\xbc\x18\x12\x1c\n\x16InvalidFaultDetectName\x10\x85\xbc\x18\x12!\n\x1bInvalidFaultDetectNamespace\x10\x86\xbc\x18\x12\x1c\n\x16\x46\x61ultDetectRuleExisted\x10\x87\xbc\x18\x12\x19\n\x13ServicesExistedMesh\x10\xaa\xb6\x18\x12\x1a\n\x14ResourcesExistedMesh\x10\xab\xb6\x18\x12\x1a\n\x14InvalidMeshParameter\x10\xac\xb6\x18\x12\x17\n\x11InvalidPlatformID\x10\xb4\xb6\x18\x12\x19\n\x13InvalidPlatformName\x10\xb5\xb6\x18\x12\x1b\n\x15InvalidPlatformDomain\x10\xb6\xb6\x18\x12\x18\n\x12InvalidPlatformQPS\x10\xb7\xb6\x18\x12\x1a\n\x14InvalidPlatformToken\x10\xb8\xb6\x18\x12\x1a\n\x14InvalidPlatformOwner\x10\xb9\xb6\x18\x12\x1f\n\x19InvalidPlatformDepartment\x10\xba\xb6\x18\x12\x1c\n\x16InvalidPlatformComment\x10\xbb\xb6\x18\x12\x16\n\x10NotFoundPlatform\x10\xbc\xb6\x18\x12\x1c\n\x16InvalidFluxRateLimitId\x10\xbe\xb6\x18\x12\x1d\n\x17InvalidFluxRateLimitQps\x10\xbf\xb6\x18\x12 \n\x1aInvalidFluxRateLimitSetKey\x10\xc0\xb6\x18\x12\x15\n\x0f\x45xistedResource\x10\xc9\xb6\x18\x12\x16\n\x10NotFoundResource\x10\xca\xb6\x18\x12\x1e\n\x18NamespaceExistedServices\x10\xcb\xb6\x18\x12\x1d\n\x17ServiceExistedInstances\x10\xcc\xb6\x18\x12\x1c\n\x16ServiceExistedRoutings\x10\xcd\xb6\x18\x12\x1e\n\x18ServiceExistedRateLimits\x10\xce\xb6\x18\x12\x19\n\x13\x45xistReleasedConfig\x10\xcf\xb6\x18\x12\x19\n\x13SameInstanceRequest\x10\xd0\xb6\x18\x12#\n\x1dServiceExistedCircuitBreakers\x10\xd1\xb6\x18\x12\x19\n\x13ServiceExistedAlias\x10\xd2\xb6\x18\x12#\n\x1dNamespaceExistedMeshResources\x10\xd3\xb6\x18\x12%\n\x1fNamespaceExistedCircuitBreakers\x10\xd4\xb6\x18\x12\x1f\n\x19ServiceSubscribedByMeshes\x10\xd5\xb6\x18\x12\"\n\x1cServiceExistedFluxRateLimits\x10\xd6\xb6\x18\x12\"\n\x1cNamespaceExistedConfigGroups\x10\xdb\xb6\x18\x12\x15\n\x0fNotFoundService\x10\xad\xb7\x18\x12\x15\n\x0fNotFoundRouting\x10\xae\xb7\x18\x12\x16\n\x10NotFoundInstance\x10\xaf\xb7\x18\x12\x1a\n\x14NotFoundServiceAlias\x10\xb0\xb7\x18\x12\x17\n\x11NotFoundNamespace\x10\xb1\xb7\x18\x12\x1b\n\x15NotFoundSourceService\x10\xb2\xb7\x18\x12\x17\n\x11NotFoundRateLimit\x10\xb3\xb7\x18\x12\x1c\n\x16NotFoundCircuitBreaker\x10\xb4\xb7\x18\x12\x1a\n\x14NotFoundMasterConfig\x10\xb5\xb7\x18\x12\x17\n\x11NotFoundTagConfig\x10\xb6\xb7\x18\x12 \n\x1aNotFoundTagConfigOrService\x10\xb7\xb7\x18\x12\x16\n\x10\x43lientAPINotOpen\x10\x91\xb8\x18\x12\x1d\n\x17NotAllowBusinessService\x10\x92\xb8\x18\x12\x19\n\x13NotAllowAliasUpdate\x10\xf5\xb8\x18\x12!\n\x1bNotAllowAliasCreateInstance\x10\xf6\xb8\x18\x12 \n\x1aNotAllowAliasCreateRouting\x10\xf7\xb8\x18\x12!\n\x1bNotAllowCreateAliasForAlias\x10\xf8\xb8\x18\x12\"\n\x1cNotAllowAliasCreateRateLimit\x10\xf9\xb8\x18\x12\x1b\n\x15NotAllowAliasBindRule\x10\xfa\xb8\x18\x12(\n\"NotAllowDifferentNamespaceBindRule\x10\xfb\xb8\x18\x12\x12\n\x0cUnauthorized\x10\xe8\xbc\x18\x12\x16\n\x10NotAllowedAccess\x10\xe9\xbc\x18\x12\x15\n\x0f\x43MDBNotFindHost\x10\xa1\xd4\x18\x12\x12\n\x0c\x44\x61taConflict\x10\xa8\xfb\x18\x12\x1d\n\x17InstanceTooManyRequests\x10\xc9\x97\x1a\x12\x11\n\x0bIPRateLimit\x10\xca\x97\x1a\x12\x12\n\x0c\x41PIRateLimit\x10\xbb\xcc\x18\x12\x16\n\x10\x45xecuteException\x10\xa0\xc2\x1e\x12\x19\n\x13StoreLayerException\x10\xa1\xc2\x1e\x12\x19\n\x13\x43MDBPluginException\x10\xa2\xc2\x1e\x12\x1b\n\x15ParseRoutingException\x10\xa4\xc2\x1e\x12\x1d\n\x17ParseRateLimitException\x10\xa5\xc2\x1e\x12\"\n\x1cParseCircuitBreakerException\x10\xa6\xc2\x1e\x12\x18\n\x12HeartbeatException\x10\xa7\xc2\x1e\x12\x1a\n\x14InstanceRegisTimeout\x10\xa8\xc2\x1e\x12 \n\x1aInvalidConfigFileGroupName\x10\xa1\xbb\x18\x12\x1b\n\x15InvalidConfigFileName\x10\xa2\xbb\x18\x12$\n\x1eInvalidConfigFileContentLength\x10\xa3\xbb\x18\x12\x1d\n\x17InvalidConfigFileFormat\x10\xa4\xbb\x18\x12\x1b\n\x15InvalidConfigFileTags\x10\xa5\xbb\x18\x12\"\n\x1cInvalidWatchConfigFileFormat\x10\xa6\xbb\x18\x12 \n\x1aNotFoundResourceConfigFile\x10\xa7\xbb\x18\x12#\n\x1dInvalidConfigFileTemplateName\x10\xa8\xbb\x18\x12 \n\x1a\x45ncryptConfigFileException\x10\xa9\xbb\x18\x12\x17\n\x11InvalidUserOwners\x10\x9a\xb8\x18\x12\x13\n\rInvalidUserID\x10\x9b\xb8\x18\x12\x19\n\x13InvalidUserPassword\x10\x9c\xb8\x18\x12\x17\n\x11InvalidUserMobile\x10\x9d\xb8\x18\x12\x16\n\x10InvalidUserEmail\x10\x9e\xb8\x18\x12\x1c\n\x16InvalidUserGroupOwners\x10\xa4\xb8\x18\x12\x18\n\x12InvalidUserGroupID\x10\xa5\xb8\x18\x12\x1f\n\x19InvalidAuthStrategyOwners\x10\xae\xb8\x18\x12\x1d\n\x17InvalidAuthStrategyName\x10\xaf\xb8\x18\x12\x1b\n\x15InvalidAuthStrategyID\x10\xb0\xb8\x18\x12\x1a\n\x14InvalidPrincipalType\x10\xb8\xb8\x18\x12\x11\n\x0bUserExisted\x10\xd7\xb6\x18\x12\x16\n\x10UserGroupExisted\x10\xd8\xb6\x18\x12\x1d\n\x17\x41uthStrategyRuleExisted\x10\xd9\xb6\x18\x12\x17\n\x11SubAccountExisted\x10\xda\xb6\x18\x12\x12\n\x0cNotFoundUser\x10\xb8\xb7\x18\x12\x17\n\x11NotFoundOwnerUser\x10\xb9\xb7\x18\x12\x17\n\x11NotFoundUserGroup\x10\xba\xb7\x18\x12\x1e\n\x18NotFoundAuthStrategyRule\x10\xbb\xb7\x18\x12,\n&NotAllowModifyDefaultStrategyPrincipal\x10\xfc\xb8\x18\x12(\n\"NotAllowModifyOwnerDefaultStrategy\x10\xfd\xb8\x18\x12\x13\n\rEmptyAutToken\x10\xea\xbc\x18\x12\x13\n\rTokenDisabled\x10\xeb\xbc\x18\x12\x15\n\x0fTokenNotExisted\x10\xec\xbc\x18\x12\x18\n\x12\x41uthTokenForbidden\x10\xb9\xcc\x18\x12\x1c\n\x16OperationRoleForbidden\x10\xba\xcc\x18\x42x\n.com.tencent.polaris.specification.api.v1.modelB\tCodeProtoZ;github.com/polarismesh/specification/source/go/api/v1/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ncode.proto\x12\x02v1*\xa4%\n\x04\x43ode\x12\x0b\n\x07Unknown\x10\x00\x12\x14\n\x0e\x45xecuteSuccess\x10\xc0\x9a\x0c\x12\x12\n\x0c\x44\x61taNoChange\x10\xc1\x9a\x0c\x12\x12\n\x0cNoNeedUpdate\x10\xc2\x9a\x0c\x12\x10\n\nBadRequest\x10\x80\xb5\x18\x12\x14\n\x0eParseException\x10\x81\xb5\x18\x12\x12\n\x0c\x45mptyRequest\x10\x82\xb5\x18\x12\x18\n\x12\x42\x61tchSizeOverLimit\x10\x83\xb5\x18\x12\x1d\n\x17InvalidDiscoverResource\x10\x84\xb5\x18\x12\x16\n\x10InvalidRequestID\x10\xe4\xb5\x18\x12\x15\n\x0fInvalidUserName\x10\xe5\xb5\x18\x12\x16\n\x10InvalidUserToken\x10\xe6\xb5\x18\x12\x16\n\x10InvalidParameter\x10\xe7\xb5\x18\x12\x19\n\x13\x45mptyQueryParameter\x10\xe8\xb5\x18\x12\x1e\n\x18InvalidQueryInsParameter\x10\xe9\xb5\x18\x12\x1a\n\x14InvalidNamespaceName\x10\xee\xb5\x18\x12\x1c\n\x16InvalidNamespaceOwners\x10\xef\xb5\x18\x12\x1b\n\x15InvalidNamespaceToken\x10\xf0\xb5\x18\x12\x18\n\x12InvalidServiceName\x10\xf8\xb5\x18\x12\x1a\n\x14InvalidServiceOwners\x10\xf9\xb5\x18\x12\x19\n\x13InvalidServiceToken\x10\xfa\xb5\x18\x12\x1c\n\x16InvalidServiceMetadata\x10\xfb\xb5\x18\x12\x19\n\x13InvalidServicePorts\x10\xfc\xb5\x18\x12\x1c\n\x16InvalidServiceBusiness\x10\xfd\xb5\x18\x12\x1e\n\x18InvalidServiceDepartment\x10\xfe\xb5\x18\x12\x18\n\x12InvalidServiceCMDB\x10\xff\xb5\x18\x12\x1b\n\x15InvalidServiceComment\x10\x80\xb6\x18\x12 \n\x1aInvalidServiceAliasComment\x10\x81\xb6\x18\x12\x17\n\x11InvalidInstanceID\x10\x82\xb6\x18\x12\x19\n\x13InvalidInstanceHost\x10\x83\xb6\x18\x12\x19\n\x13InvalidInstancePort\x10\x84\xb6\x18\x12\x19\n\x13InvalidServiceAlias\x10\x85\xb6\x18\x12\x1f\n\x19InvalidNamespaceWithAlias\x10\x86\xb6\x18\x12\x1f\n\x19InvalidServiceAliasOwners\x10\x87\xb6\x18\x12\x1d\n\x17InvalidInstanceProtocol\x10\x88\xb6\x18\x12\x1c\n\x16InvalidInstanceVersion\x10\x89\xb6\x18\x12\x1d\n\x17InvalidInstanceLogicSet\x10\x8a\xb6\x18\x12\x1c\n\x16InvalidInstanceIsolate\x10\x8b\xb6\x18\x12\x18\n\x12HealthCheckNotOpen\x10\x8c\xb6\x18\x12\x1c\n\x16HeartbeatOnDisabledIns\x10\x8d\xb6\x18\x12\x1a\n\x14HeartbeatExceedLimit\x10\x8e\xb6\x18\x12\x1b\n\x15HeartbeatTypeNotFound\x10\x8f\xb6\x18\x12\x15\n\x0fInvalidMetadata\x10\x96\xb6\x18\x12\x18\n\x12InvalidRateLimitID\x10\x97\xb6\x18\x12\x1c\n\x16InvalidRateLimitLabels\x10\x98\xb6\x18\x12\x1d\n\x17InvalidRateLimitAmounts\x10\x99\xb6\x18\x12\x1a\n\x14InvalidRateLimitName\x10\x9a\xb6\x18\x12\x1d\n\x17InvalidCircuitBreakerID\x10\xa0\xb6\x18\x12\"\n\x1cInvalidCircuitBreakerVersion\x10\xa1\xb6\x18\x12\x1f\n\x19InvalidCircuitBreakerName\x10\xa2\xb6\x18\x12$\n\x1eInvalidCircuitBreakerNamespace\x10\xa3\xb6\x18\x12!\n\x1bInvalidCircuitBreakerOwners\x10\xa4\xb6\x18\x12 \n\x1aInvalidCircuitBreakerToken\x10\xa5\xb6\x18\x12#\n\x1dInvalidCircuitBreakerBusiness\x10\xa6\xb6\x18\x12%\n\x1fInvalidCircuitBreakerDepartment\x10\xa7\xb6\x18\x12\"\n\x1cInvalidCircuitBreakerComment\x10\xa8\xb6\x18\x12\x1f\n\x19\x43ircuitBreakerRuleExisted\x10\xa9\xb6\x18\x12\x16\n\x10InvalidRoutingID\x10\xbc\xba\x18\x12\x1a\n\x14InvalidRoutingPolicy\x10\xbd\xba\x18\x12\x18\n\x12InvalidRoutingName\x10\xbe\xba\x18\x12\x1c\n\x16InvalidRoutingPriority\x10\xbf\xba\x18\x12\x1a\n\x14InvalidFaultDetectID\x10\x84\xbc\x18\x12\x1c\n\x16InvalidFaultDetectName\x10\x85\xbc\x18\x12!\n\x1bInvalidFaultDetectNamespace\x10\x86\xbc\x18\x12\x1c\n\x16\x46\x61ultDetectRuleExisted\x10\x87\xbc\x18\x12\x19\n\x13ServicesExistedMesh\x10\xaa\xb6\x18\x12\x1a\n\x14ResourcesExistedMesh\x10\xab\xb6\x18\x12\x1a\n\x14InvalidMeshParameter\x10\xac\xb6\x18\x12\x17\n\x11InvalidPlatformID\x10\xb4\xb6\x18\x12\x19\n\x13InvalidPlatformName\x10\xb5\xb6\x18\x12\x1b\n\x15InvalidPlatformDomain\x10\xb6\xb6\x18\x12\x18\n\x12InvalidPlatformQPS\x10\xb7\xb6\x18\x12\x1a\n\x14InvalidPlatformToken\x10\xb8\xb6\x18\x12\x1a\n\x14InvalidPlatformOwner\x10\xb9\xb6\x18\x12\x1f\n\x19InvalidPlatformDepartment\x10\xba\xb6\x18\x12\x1c\n\x16InvalidPlatformComment\x10\xbb\xb6\x18\x12\x16\n\x10NotFoundPlatform\x10\xbc\xb6\x18\x12\x1c\n\x16InvalidFluxRateLimitId\x10\xbe\xb6\x18\x12\x1d\n\x17InvalidFluxRateLimitQps\x10\xbf\xb6\x18\x12 \n\x1aInvalidFluxRateLimitSetKey\x10\xc0\xb6\x18\x12\x15\n\x0f\x45xistedResource\x10\xc9\xb6\x18\x12\x16\n\x10NotFoundResource\x10\xca\xb6\x18\x12\x1e\n\x18NamespaceExistedServices\x10\xcb\xb6\x18\x12\x1d\n\x17ServiceExistedInstances\x10\xcc\xb6\x18\x12\x1c\n\x16ServiceExistedRoutings\x10\xcd\xb6\x18\x12\x1e\n\x18ServiceExistedRateLimits\x10\xce\xb6\x18\x12\x19\n\x13\x45xistReleasedConfig\x10\xcf\xb6\x18\x12\x19\n\x13SameInstanceRequest\x10\xd0\xb6\x18\x12#\n\x1dServiceExistedCircuitBreakers\x10\xd1\xb6\x18\x12\x19\n\x13ServiceExistedAlias\x10\xd2\xb6\x18\x12#\n\x1dNamespaceExistedMeshResources\x10\xd3\xb6\x18\x12%\n\x1fNamespaceExistedCircuitBreakers\x10\xd4\xb6\x18\x12\x1f\n\x19ServiceSubscribedByMeshes\x10\xd5\xb6\x18\x12\"\n\x1cServiceExistedFluxRateLimits\x10\xd6\xb6\x18\x12\"\n\x1cNamespaceExistedConfigGroups\x10\xdb\xb6\x18\x12\x15\n\x0fNotFoundService\x10\xad\xb7\x18\x12\x15\n\x0fNotFoundRouting\x10\xae\xb7\x18\x12\x16\n\x10NotFoundInstance\x10\xaf\xb7\x18\x12\x1a\n\x14NotFoundServiceAlias\x10\xb0\xb7\x18\x12\x17\n\x11NotFoundNamespace\x10\xb1\xb7\x18\x12\x1b\n\x15NotFoundSourceService\x10\xb2\xb7\x18\x12\x17\n\x11NotFoundRateLimit\x10\xb3\xb7\x18\x12\x1c\n\x16NotFoundCircuitBreaker\x10\xb4\xb7\x18\x12\x1a\n\x14NotFoundMasterConfig\x10\xb5\xb7\x18\x12\x17\n\x11NotFoundTagConfig\x10\xb6\xb7\x18\x12 \n\x1aNotFoundTagConfigOrService\x10\xb7\xb7\x18\x12\x16\n\x10\x43lientAPINotOpen\x10\x91\xb8\x18\x12\x1d\n\x17NotAllowBusinessService\x10\x92\xb8\x18\x12\x19\n\x13NotAllowAliasUpdate\x10\xf5\xb8\x18\x12!\n\x1bNotAllowAliasCreateInstance\x10\xf6\xb8\x18\x12 \n\x1aNotAllowAliasCreateRouting\x10\xf7\xb8\x18\x12!\n\x1bNotAllowCreateAliasForAlias\x10\xf8\xb8\x18\x12\"\n\x1cNotAllowAliasCreateRateLimit\x10\xf9\xb8\x18\x12\x1b\n\x15NotAllowAliasBindRule\x10\xfa\xb8\x18\x12(\n\"NotAllowDifferentNamespaceBindRule\x10\xfb\xb8\x18\x12\x12\n\x0cUnauthorized\x10\xe8\xbc\x18\x12\x16\n\x10NotAllowedAccess\x10\xe9\xbc\x18\x12\x15\n\x0f\x43MDBNotFindHost\x10\xa1\xd4\x18\x12\x12\n\x0c\x44\x61taConflict\x10\xa8\xfb\x18\x12\x1d\n\x17InstanceTooManyRequests\x10\xc9\x97\x1a\x12\x11\n\x0bIPRateLimit\x10\xca\x97\x1a\x12\x12\n\x0c\x41PIRateLimit\x10\xbb\xcc\x18\x12\x16\n\x10\x45xecuteException\x10\xa0\xc2\x1e\x12\x19\n\x13StoreLayerException\x10\xa1\xc2\x1e\x12\x19\n\x13\x43MDBPluginException\x10\xa2\xc2\x1e\x12\x1b\n\x15ParseRoutingException\x10\xa4\xc2\x1e\x12\x1d\n\x17ParseRateLimitException\x10\xa5\xc2\x1e\x12\"\n\x1cParseCircuitBreakerException\x10\xa6\xc2\x1e\x12\x18\n\x12HeartbeatException\x10\xa7\xc2\x1e\x12\x1a\n\x14InstanceRegisTimeout\x10\xa8\xc2\x1e\x12 \n\x1aInvalidConfigFileGroupName\x10\xa1\xbb\x18\x12\x1b\n\x15InvalidConfigFileName\x10\xa2\xbb\x18\x12$\n\x1eInvalidConfigFileContentLength\x10\xa3\xbb\x18\x12\x1d\n\x17InvalidConfigFileFormat\x10\xa4\xbb\x18\x12\x1b\n\x15InvalidConfigFileTags\x10\xa5\xbb\x18\x12\"\n\x1cInvalidWatchConfigFileFormat\x10\xa6\xbb\x18\x12 \n\x1aNotFoundResourceConfigFile\x10\xa7\xbb\x18\x12#\n\x1dInvalidConfigFileTemplateName\x10\xa8\xbb\x18\x12 \n\x1a\x45ncryptConfigFileException\x10\xa9\xbb\x18\x12 \n\x1a\x44\x65\x63ryptConfigFileException\x10\xaa\xbb\x18\x12\x17\n\x11InvalidUserOwners\x10\x9a\xb8\x18\x12\x13\n\rInvalidUserID\x10\x9b\xb8\x18\x12\x19\n\x13InvalidUserPassword\x10\x9c\xb8\x18\x12\x17\n\x11InvalidUserMobile\x10\x9d\xb8\x18\x12\x16\n\x10InvalidUserEmail\x10\x9e\xb8\x18\x12\x1c\n\x16InvalidUserGroupOwners\x10\xa4\xb8\x18\x12\x18\n\x12InvalidUserGroupID\x10\xa5\xb8\x18\x12\x1f\n\x19InvalidAuthStrategyOwners\x10\xae\xb8\x18\x12\x1d\n\x17InvalidAuthStrategyName\x10\xaf\xb8\x18\x12\x1b\n\x15InvalidAuthStrategyID\x10\xb0\xb8\x18\x12\x1a\n\x14InvalidPrincipalType\x10\xb8\xb8\x18\x12\x11\n\x0bUserExisted\x10\xd7\xb6\x18\x12\x16\n\x10UserGroupExisted\x10\xd8\xb6\x18\x12\x1d\n\x17\x41uthStrategyRuleExisted\x10\xd9\xb6\x18\x12\x17\n\x11SubAccountExisted\x10\xda\xb6\x18\x12\x12\n\x0cNotFoundUser\x10\xb8\xb7\x18\x12\x17\n\x11NotFoundOwnerUser\x10\xb9\xb7\x18\x12\x17\n\x11NotFoundUserGroup\x10\xba\xb7\x18\x12\x1e\n\x18NotFoundAuthStrategyRule\x10\xbb\xb7\x18\x12,\n&NotAllowModifyDefaultStrategyPrincipal\x10\xfc\xb8\x18\x12(\n\"NotAllowModifyOwnerDefaultStrategy\x10\xfd\xb8\x18\x12\x13\n\rEmptyAutToken\x10\xea\xbc\x18\x12\x13\n\rTokenDisabled\x10\xeb\xbc\x18\x12\x15\n\x0fTokenNotExisted\x10\xec\xbc\x18\x12\x18\n\x12\x41uthTokenForbidden\x10\xb9\xcc\x18\x12\x1c\n\x16OperationRoleForbidden\x10\xba\xcc\x18\x42x\n.com.tencent.polaris.specification.api.v1.modelB\tCodeProtoZ;github.com/polarismesh/specification/source/go/api/v1/modelb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'code_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n.com.tencent.polaris.specification.api.v1.modelB\tCodeProtoZ;github.com/polarismesh/specification/source/go/api/v1/model'
   _CODE._serialized_start=19
-  _CODE._serialized_end=4757
+  _CODE._serialized_end=4791
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/code_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/code_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 CMDBNotFindHost: Code
 CMDBPluginException: Code
 CircuitBreakerRuleExisted: Code
 ClientAPINotOpen: Code
 DESCRIPTOR: _descriptor.FileDescriptor
 DataConflict: Code
 DataNoChange: Code
+DecryptConfigFileException: Code
 EmptyAutToken: Code
 EmptyQueryParameter: Code
 EmptyRequest: Code
 EncryptConfigFileException: Code
 ExecuteException: Code
 ExecuteSuccess: Code
 ExistReleasedConfig: Code
```

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.3.1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/LICENSE.txt` & `polarismesh_specification-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/README.md` & `polarismesh_specification-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/pyproject.toml` & `polarismesh_specification-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a7/PKG-INFO` & `polarismesh_specification-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarismesh-specification
-Version: 1.3.0a7
+Version: 1.3.1
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

