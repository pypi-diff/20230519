# Comparing `tmp/ni_measurementlink_service-1.1.0.dev0.tar.gz` & `tmp/ni_measurementlink_service-1.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_service-1.1.0.dev0.tar", max compression
+gzip compressed data, was "ni_measurementlink_service-1.1.0.dev1.tar", max compression
```

## Comparing `ni_measurementlink_service-1.1.0.dev0.tar` & `ni_measurementlink_service-1.1.0.dev1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1071 2023-05-08 22:25:40.024292 ni_measurementlink_service-1.1.0.dev0/LICENSE
--rw-r--r--   0        0        0    15792 2023-05-08 22:25:40.024292 ni_measurementlink_service-1.1.0.dev0/README.md
--rw-r--r--   0        0        0      513 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/__init__.py
--rw-r--r--   0        0        0       62 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/__init__.py
--rw-r--r--   0        0        0    10404 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/discovery_client.py
--rw-r--r--   0        0        0    16735 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/grpc_servicer.py
--rw-r--r--   0        0        0       58 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/__init__.py
--rw-r--r--   0        0        0     2236 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/metadata.py
--rw-r--r--   0        0        0     9062 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
--rw-r--r--   0        0        0     6182 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/serializer.py
--rw-r--r--   0        0        0     3933 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/service_manager.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/__init__.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/__init__.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
--rw-r--r--   0        0        0     4264 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
--rw-r--r--   0        0        0     8921 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
--rw-r--r--   0        0        0    10817 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
--rw-r--r--   0        0        0     5345 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
--rw-r--r--   0        0        0    13593 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5546 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
--rw-r--r--   0        0        0     5777 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
--rw-r--r--   0        0        0    15001 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5549 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0     1532 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
--rw-r--r--   0        0        0     1314 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
--rw-r--r--   0        0        0     6202 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
--rw-r--r--   0        0        0    18188 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
--rw-r--r--   0        0        0    14078 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
--rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
--rw-r--r--   0        0        0     5955 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
--rw-r--r--   0        0        0    13237 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
--rw-r--r--   0        0        0    13882 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
--rw-r--r--   0        0        0      709 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/README.md
--rw-r--r--   0        0        0     6052 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
--rw-r--r--   0        0        0     6650 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
--rw-r--r--   0        0        0     7228 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
--rw-r--r--   0        0        0      712 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
--rw-r--r--   0        0        0     9622 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
--rw-r--r--   0        0        0     8468 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
--rw-r--r--   0        0        0     2426 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/session.proto
--rw-r--r--   0        0        0     4196 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.py
--rw-r--r--   0        0        0     8735 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
--rw-r--r--   0        0        0     8948 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/utilities/__init__.py
--rw-r--r--   0        0        0       37 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/__init__.py
--rw-r--r--   0        0        0     3021 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/info.py
--rw-r--r--   0        0        0    13261 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/service.py
--rw-r--r--   0        0        0        0 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/py.typed
--rw-r--r--   0        0        0    14466 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/session_management.py
--rw-r--r--   0        0        0     2650 2023-05-08 22:27:14.811198 ni_measurementlink_service-1.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0    18650 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev0/setup.py
--rw-r--r--   0        0        0    17006 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-18 21:55:42.165839 ni_measurementlink_service-1.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0    16415 2023-05-18 21:55:42.165839 ni_measurementlink_service-1.1.0.dev1/README.md
+-rw-r--r--   0        0        0      513 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/__init__.py
+-rw-r--r--   0        0        0    10404 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/discovery_client.py
+-rw-r--r--   0        0        0    16735 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/grpc_servicer.py
+-rw-r--r--   0        0        0       58 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/__init__.py
+-rw-r--r--   0        0        0     2236 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/metadata.py
+-rw-r--r--   0        0        0     9062 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
+-rw-r--r--   0        0        0     6182 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/serializer.py
+-rw-r--r--   0        0        0     3933 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/service_manager.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
+-rw-r--r--   0        0        0     4264 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
+-rw-r--r--   0        0        0     8921 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
+-rw-r--r--   0        0        0    10817 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
+-rw-r--r--   0        0        0     5345 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
+-rw-r--r--   0        0        0    13593 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5546 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
+-rw-r--r--   0        0        0     5777 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
+-rw-r--r--   0        0        0    15001 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5549 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1532 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
+-rw-r--r--   0        0        0     1314 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
+-rw-r--r--   0        0        0     6202 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
+-rw-r--r--   0        0        0    18188 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
+-rw-r--r--   0        0        0    14078 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
+-rw-r--r--   0        0        0     5955 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
+-rw-r--r--   0        0        0    13237 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13882 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0      709 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/README.md
+-rw-r--r--   0        0        0     6052 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
+-rw-r--r--   0        0        0     6650 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
+-rw-r--r--   0        0        0     7228 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
+-rw-r--r--   0        0        0      712 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
+-rw-r--r--   0        0        0     9622 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
+-rw-r--r--   0        0        0     8468 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
+-rw-r--r--   0        0        0     2426 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/session.proto
+-rw-r--r--   0        0        0     4196 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.py
+-rw-r--r--   0        0        0     8735 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
+-rw-r--r--   0        0        0     8948 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/utilities/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/__init__.py
+-rw-r--r--   0        0        0     3021 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/info.py
+-rw-r--r--   0        0        0    13261 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/service.py
+-rw-r--r--   0        0        0        0 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/py.typed
+-rw-r--r--   0        0        0    14466 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/session_management.py
+-rw-r--r--   0        0        0     2650 2023-05-18 21:57:24.107064 ni_measurementlink_service-1.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0    19283 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev1/setup.py
+-rw-r--r--   0        0        0    17629 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev1/PKG-INFO
```

### Comparing `ni_measurementlink_service-1.1.0.dev0/LICENSE` & `ni_measurementlink_service-1.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/README.md` & `ni_measurementlink_service-1.1.0.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,25 @@
   - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.
 - In the Windows registry, set `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FileSystem\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).
 
 ---
 
 ## Examples
 
-The [`examples`](https://github.com/ni/measurementlink-python/tree/main/examples/) directory contains example measurement services. See the [README.md](https://github.com/ni/measurementlink-python/tree/main/examples/README.md) file for more information.
+The `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If
+you are using a previous version of MeasurementLink, download the appropriate examples:
+
+- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
+- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
+
+For more information on setting up and running the example measurements, see the included `README.md` file.
+
+For best results, use the example measurements corresponding to the version of MeasurementLink
+that you are using. Newer examples may demonstrate features that are not available in older
+versions of MeasurementLink.
 
 ---
 
 ## Developing Measurements: Quick Start
 
 This section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.
```

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/__init__.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/__init__.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/discovery_client.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/discovery_client.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/grpc_servicer.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/grpc_servicer.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/metadata.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/metadata.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/serialization_strategy.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/serialization_strategy.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/serializer.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/serializer.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/service_manager.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/service_manager.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/README.md` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/session.proto` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/session.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/info.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/info.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/service.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/service.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/session_management.py` & `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/session_management.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev0/pyproject.toml` & `ni_measurementlink_service-1.1.0.dev1/pyproject.toml`

 * *Files identical despite different names*

```diff
@@ -7,15 +7,15 @@
 | \.venv
 | venv
 )
 '''
 
 [tool.poetry]
 name = "ni_measurementlink_service"
-version = "1.1.0-dev0"
+version = "1.1.0-dev1"
 description = "MeasurementLink Support for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md" # apply the repo readme to the package as well
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `ni_measurementlink_service-1.1.0.dev0/setup.py` & `ni_measurementlink_service-1.1.0.dev1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 ['grpcio>=1.49.1,<2.0.0', 'protobuf>=4.21,<5.0']
 
 extras_require = \
 {':sys_platform == "win32"': ['pywin32>=303']}
 
 setup_kwargs = {
     'name': 'ni-measurementlink-service',
-    'version': '1.1.0.dev0',
+    'version': '1.1.0.dev1',
     'description': 'MeasurementLink Support for Python',
-    'long_description': '# MeasurementLink™ Support for Python\n\n- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)\n  - [Introduction](#introduction)\n  - [Dependencies](#dependencies)\n  - [Documentation](#documentation)\n  - [Examples](#examples)\n  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)\n    - [Installation](#installation)\n    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)\n  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)\n  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)\n    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)\n    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)\n  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)\n    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)\n    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)\n    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)\n\n---\n\n## Introduction\n\nMeasurementLink Support for Python (`ni-measurementlink-service`) is a Python framework that enables measurement developers to quickly create Python measurements and run them as a service (gRPC).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)\n- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)\n- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)\n\n---\n\n## Documentation\n\n- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)\n- [API Reference](https://ni.github.io/measurementlink-python/)\n\n---\n\n## System Configuration\n\n### Enable Win32 Long Paths\n\nBy default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. \n\nThere are three ways to do this:\n- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.\n- Set the `Enable Win32 long paths` group policy:\n  - Run `gpedit.msc`.\n  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.\n  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.\n- In the Windows registry, set `HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\FileSystem\\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).\n\n---\n\n## Examples\n\nThe [`examples`](https://github.com/ni/measurementlink-python/tree/main/examples/) directory contains example measurement services. See the [README.md](https://github.com/ni/measurementlink-python/tree/main/examples/README.md) file for more information.\n\n---\n\n## Developing Measurements: Quick Start\n\nThis section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.\n\n### Installation\n\nMake sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-service\n```\n\nCheck if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:\n\n```cmd\npip show ni-measurementlink-service\n```\n\n### Developing a minimal Python measurement\n\n1. Install the `ni-measurementlink-generator` package.\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-generator\n```\n\n2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.\n\n    1. Running `ni-measurementlink-generator` without optional arguments:\n\n    `ni-measurementlink-generator SampleMeasurement`\n\n    \'SampleMeasurement\' is the display name of your measurement service. Without the optional arguments,\n    the other arguments are generated for you based on the display name.\n\n    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,\n    `service-class`, and `description-url`:\n\n    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`\n\n    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`\n\n    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`\n\n    If no output directory is specified, the files will\n    be placed in a new folder under the current directory\n    named after the display name without spaces.\n\n3. To customize the created measurement, provide metadata of the measurement\'s configuration (input parameters) and outputs (output parameters) in `measurement.py`.\n    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        #Display Names can not contains backslash or front slash.\n        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")\n        def measure(input_1, input_2):\n            \'\'\' A simple Measurement method\'\'\'\n            return ["foo", "bar"]\n        ```\n\n    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")\n        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)\n        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)\n        def measure(input_1, input_2):\n            return ["foo", "bar"]\n        ```\n\n4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)\n\n---\n\n## Steps to run/debug the measurement service\n\n1. Start the discovery service if not already started.\n\n2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    .venv\\scripts\\activate\n    ```\n\n    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.\n    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:\n\n        ```cmd\n        Set-ExecutionPolicy RemoteSigned \n        ```\n\n3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.\n\n4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.\n\n5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    deactivate\n    ```\n\n---\n\n## Static Registration of Python Measurements\n\nThe MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.\n\nTo statically register a measurement service with the MeasurementLink discovery service, do the following:\n\n1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.\n\n2. Edit the measurement service\'s `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.\n\n3. Copy the measurement service\'s directory (including the `.venv` subdirectory if present, `.serviceconfig` file, and startup batch file) to a subdirectory of `C:\\ProgramData\\National Instruments\\MeasurementLink\\Services`. \n\nOnce your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.\n\n### Create a batch file that runs a Python measurement\n\nThe batch file used for static registration is responsible for starting the Python Scripts.\n\nTypical Batch File:\n\n``` cmd\n"<path_to_python_exe>" "<path_to_measurement_file>"\n```\n\nExamples to start the fictitious file named `foo_measurement.py`:\n\n1. Using the Python system distribution\n\n    ```cmd\n    python foo_measurement.py\n    ```\n\n2. Using the virtual environment\n\n    ```cmd\n    REM Windows\n    .\\.venv\\Scripts\\python.exe foo_measurement.py\n\n    REM Linux \n    .venv/bin/python foo_measurement.py\n    ```\n\n### Create Executable for Python Scripts\n\nTo create an executable from a measurement, measurement authors can use the [pyinstaller](https://www.pyinstaller.org/) tooling. During the executable creation, the user can also embed the User Interface file using the `--add-data "<path_of_the_UI_File>;."`.\n\nTypical Pyinstaller command to build executable.\n\n```cmd\npyinstaller --onefile --console --add-data "<path_of_the_UI_File>;." --paths .venv\\Lib\\site-packages\\ <path_of_the_measurement_script>\n```\n\n## Troubleshooting\n\n### "File not found" or "No such file or directory" errors when copying or running a measurement service\n\nIf copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.\n\n## Appendix: Managing Measurement as Python Package (Project)\n\nMeasurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:\n\n1. Measurement Python module (`.py` file)\n    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.\n    - This file is run to start the measurement as a service.\n\n2. UI File\n    - UI file for the measurement. Types of supported UI files are:\n        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.\n        - LabVIEW UI (`.vi`)\n    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).\n\nPython communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.\n\n### Create and Manage Python Measurement Package using Poetry\n\n1. Install `poetry` (one-time setup)\n\n    1. Make sure the system has the recommended Python version installed.\n\n    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.\n\n2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.\n\n    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.\n\n        ``` cmd\n        cd <path_of_directory_of_your_choice>\n        ```\n\n    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.\n\n        ``` cmd\n        poetry new <name_of_the_project>\n        ```\n\n    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.\n\n        ``` cmd\n        cd <name_of_the_project>\n        poetry add ni-measurementlink-service\n        ```\n\n    4. The virtual environment will be auto-created by poetry.\n\n    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).\n\n            ``` cmd\n            poetry add <dependency_package_name>\n            ```\n\nFor detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).\n\n### Create and Manage Python Measurement Package using `venv`\n\n1. Make sure the system has the recommended Python version installed.\n\n2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.\n\n    ``` cmd\n    cd <path_of_directory_of_your_choice>\n    ```\n\n3. Create a virtual environment.\n\n    ``` cmd\n    REM This creates a virtual environment named .venv\n    python -m venv .venv\n    ```\n\n4. Activate the virtual environment. After successful activation\n\n    ``` cmd\n    .venv\\scripts\\activate\n    REM Optionally upgrade the pip within the venv by executing the command\n    python -m pip install -U pip\n    ```\n\n5. Install the `ni-measurementlink-service` package into the virtual environment.\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n    - Any additional dependencies required by measurement can be added pip install.\n\n        ``` cmd\n        pip install <dependency_package_name>\n        ```\n\nFor detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).\n\n### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package\n\nMeasurement developers can also install `ni-measurementlink-service` as a system package if necessary.\n\n1. Install the `ni-measurementlink-service` package from the command prompt\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n\n---\n',
+    'long_description': '# MeasurementLink™ Support for Python\n\n- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)\n  - [Introduction](#introduction)\n  - [Dependencies](#dependencies)\n  - [Documentation](#documentation)\n  - [Examples](#examples)\n  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)\n    - [Installation](#installation)\n    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)\n  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)\n  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)\n    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)\n    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)\n  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)\n    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)\n    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)\n    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)\n\n---\n\n## Introduction\n\nMeasurementLink Support for Python (`ni-measurementlink-service`) is a Python framework that enables measurement developers to quickly create Python measurements and run them as a service (gRPC).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)\n- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)\n- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)\n\n---\n\n## Documentation\n\n- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)\n- [API Reference](https://ni.github.io/measurementlink-python/)\n\n---\n\n## System Configuration\n\n### Enable Win32 Long Paths\n\nBy default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. \n\nThere are three ways to do this:\n- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.\n- Set the `Enable Win32 long paths` group policy:\n  - Run `gpedit.msc`.\n  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.\n  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.\n- In the Windows registry, set `HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\FileSystem\\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).\n\n---\n\n## Examples\n\nThe `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If\nyou are using a previous version of MeasurementLink, download the appropriate examples:\n\n- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n\nFor more information on setting up and running the example measurements, see the included `README.md` file.\n\nFor best results, use the example measurements corresponding to the version of MeasurementLink\nthat you are using. Newer examples may demonstrate features that are not available in older\nversions of MeasurementLink.\n\n---\n\n## Developing Measurements: Quick Start\n\nThis section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.\n\n### Installation\n\nMake sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-service\n```\n\nCheck if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:\n\n```cmd\npip show ni-measurementlink-service\n```\n\n### Developing a minimal Python measurement\n\n1. Install the `ni-measurementlink-generator` package.\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-generator\n```\n\n2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.\n\n    1. Running `ni-measurementlink-generator` without optional arguments:\n\n    `ni-measurementlink-generator SampleMeasurement`\n\n    \'SampleMeasurement\' is the display name of your measurement service. Without the optional arguments,\n    the other arguments are generated for you based on the display name.\n\n    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,\n    `service-class`, and `description-url`:\n\n    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`\n\n    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`\n\n    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`\n\n    If no output directory is specified, the files will\n    be placed in a new folder under the current directory\n    named after the display name without spaces.\n\n3. To customize the created measurement, provide metadata of the measurement\'s configuration (input parameters) and outputs (output parameters) in `measurement.py`.\n    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        #Display Names can not contains backslash or front slash.\n        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")\n        def measure(input_1, input_2):\n            \'\'\' A simple Measurement method\'\'\'\n            return ["foo", "bar"]\n        ```\n\n    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")\n        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)\n        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)\n        def measure(input_1, input_2):\n            return ["foo", "bar"]\n        ```\n\n4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)\n\n---\n\n## Steps to run/debug the measurement service\n\n1. Start the discovery service if not already started.\n\n2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    .venv\\scripts\\activate\n    ```\n\n    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.\n    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:\n\n        ```cmd\n        Set-ExecutionPolicy RemoteSigned \n        ```\n\n3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.\n\n4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.\n\n5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    deactivate\n    ```\n\n---\n\n## Static Registration of Python Measurements\n\nThe MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.\n\nTo statically register a measurement service with the MeasurementLink discovery service, do the following:\n\n1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.\n\n2. Edit the measurement service\'s `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.\n\n3. Copy the measurement service\'s directory (including the `.venv` subdirectory if present, `.serviceconfig` file, and startup batch file) to a subdirectory of `C:\\ProgramData\\National Instruments\\MeasurementLink\\Services`. \n\nOnce your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.\n\n### Create a batch file that runs a Python measurement\n\nThe batch file used for static registration is responsible for starting the Python Scripts.\n\nTypical Batch File:\n\n``` cmd\n"<path_to_python_exe>" "<path_to_measurement_file>"\n```\n\nExamples to start the fictitious file named `foo_measurement.py`:\n\n1. Using the Python system distribution\n\n    ```cmd\n    python foo_measurement.py\n    ```\n\n2. Using the virtual environment\n\n    ```cmd\n    REM Windows\n    .\\.venv\\Scripts\\python.exe foo_measurement.py\n\n    REM Linux \n    .venv/bin/python foo_measurement.py\n    ```\n\n### Create Executable for Python Scripts\n\nTo create an executable from a measurement, measurement authors can use the [pyinstaller](https://www.pyinstaller.org/) tooling. During the executable creation, the user can also embed the User Interface file using the `--add-data "<path_of_the_UI_File>;."`.\n\nTypical Pyinstaller command to build executable.\n\n```cmd\npyinstaller --onefile --console --add-data "<path_of_the_UI_File>;." --paths .venv\\Lib\\site-packages\\ <path_of_the_measurement_script>\n```\n\n## Troubleshooting\n\n### "File not found" or "No such file or directory" errors when copying or running a measurement service\n\nIf copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.\n\n## Appendix: Managing Measurement as Python Package (Project)\n\nMeasurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:\n\n1. Measurement Python module (`.py` file)\n    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.\n    - This file is run to start the measurement as a service.\n\n2. UI File\n    - UI file for the measurement. Types of supported UI files are:\n        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.\n        - LabVIEW UI (`.vi`)\n    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).\n\nPython communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.\n\n### Create and Manage Python Measurement Package using Poetry\n\n1. Install `poetry` (one-time setup)\n\n    1. Make sure the system has the recommended Python version installed.\n\n    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.\n\n2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.\n\n    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.\n\n        ``` cmd\n        cd <path_of_directory_of_your_choice>\n        ```\n\n    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.\n\n        ``` cmd\n        poetry new <name_of_the_project>\n        ```\n\n    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.\n\n        ``` cmd\n        cd <name_of_the_project>\n        poetry add ni-measurementlink-service\n        ```\n\n    4. The virtual environment will be auto-created by poetry.\n\n    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).\n\n            ``` cmd\n            poetry add <dependency_package_name>\n            ```\n\nFor detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).\n\n### Create and Manage Python Measurement Package using `venv`\n\n1. Make sure the system has the recommended Python version installed.\n\n2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.\n\n    ``` cmd\n    cd <path_of_directory_of_your_choice>\n    ```\n\n3. Create a virtual environment.\n\n    ``` cmd\n    REM This creates a virtual environment named .venv\n    python -m venv .venv\n    ```\n\n4. Activate the virtual environment. After successful activation\n\n    ``` cmd\n    .venv\\scripts\\activate\n    REM Optionally upgrade the pip within the venv by executing the command\n    python -m pip install -U pip\n    ```\n\n5. Install the `ni-measurementlink-service` package into the virtual environment.\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n    - Any additional dependencies required by measurement can be added pip install.\n\n        ``` cmd\n        pip install <dependency_package_name>\n        ```\n\nFor detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).\n\n### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package\n\nMeasurement developers can also install `ni-measurementlink-service` as a system package if necessary.\n\n1. Install the `ni-measurementlink-service` package from the command prompt\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n\n---\n',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/measurementlink-python/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ni_measurementlink_service-1.1.0.dev0/PKG-INFO` & `ni_measurementlink_service-1.1.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ni-measurementlink-service
-Version: 1.1.0.dev0
+Version: 1.1.0.dev1
 Summary: MeasurementLink Support for Python
 Home-page: https://github.com/ni/measurementlink-python/
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -84,15 +84,25 @@
   - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.
 - In the Windows registry, set `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FileSystem\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).
 
 ---
 
 ## Examples
 
-The [`examples`](https://github.com/ni/measurementlink-python/tree/main/examples/) directory contains example measurement services. See the [README.md](https://github.com/ni/measurementlink-python/tree/main/examples/README.md) file for more information.
+The `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If
+you are using a previous version of MeasurementLink, download the appropriate examples:
+
+- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
+- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
+
+For more information on setting up and running the example measurements, see the included `README.md` file.
+
+For best results, use the example measurements corresponding to the version of MeasurementLink
+that you are using. Newer examples may demonstrate features that are not available in older
+versions of MeasurementLink.
 
 ---
 
 ## Developing Measurements: Quick Start
 
 This section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.
```

