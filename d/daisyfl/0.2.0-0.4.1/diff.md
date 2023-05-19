# Comparing `tmp/daisyfl-0.2.0.tar.gz` & `tmp/daisyfl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisyfl-0.2.0.tar", max compression
+gzip compressed data, was "daisyfl-0.4.1.tar", max compression
```

## Comparing `daisyfl-0.2.0.tar` & `daisyfl-0.4.1.tar`

### file list

```diff
@@ -1,81 +1,83 @@
--rw-r--r--   0        0        0    11358 2023-01-10 07:20:47.485254 daisyfl-0.2.0/LICENSE
--rw-r--r--   0        0        0      691 2023-01-10 07:20:47.485254 daisyfl-0.2.0/README.md
--rw-r--r--   0        0        0     3764 2023-03-10 02:59:17.556454 daisyfl-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1093 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/__init__.py
--rw-r--r--   0        0        0     1171 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/client/__init__.py
--rw-r--r--   0        0        0     9956 2023-03-09 10:49:18.962868 daisyfl-0.2.0/src/py/daisyfl/client/app.py
--rw-r--r--   0        0        0     3733 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/client/client.py
--rw-r--r--   0        0        0      761 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/client/client_api_handler.py
--rw-r--r--   0        0        0     3780 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/client/client_operator_manager.py
--rw-r--r--   0        0        0     3367 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      714 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     5781 2023-03-09 10:24:41.854860 daisyfl-0.2.0/src/py/daisyfl/client/grpc_client/connection.py
--rw-r--r--   0        0        0     6801 2023-02-09 07:15:43.884694 daisyfl-0.2.0/src/py/daisyfl/client/grpc_client/message_handler.py
--rw-r--r--   0        0        0     5084 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/client/numpy_client.py
--rw-r--r--   0        0        0     1734 2023-03-10 02:45:01.768952 daisyfl-0.2.0/src/py/daisyfl/client/zone_client.py
--rw-r--r--   0        0        0     4109 2023-03-09 10:09:49.041258 daisyfl-0.2.0/src/py/daisyfl/common/__init__.py
--rw-r--r--   0        0        0     1830 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/common/dp.py
--rw-r--r--   0        0        0     3483 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/common/logger.py
--rw-r--r--   0        0        0     3938 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/common/parameter.py
--rw-r--r--   0        0        0    15254 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/common/serde.py
--rw-r--r--   0        0        0     3637 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/common/typing.py
--rw-r--r--   0        0        0        0 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/operator/base/__init__.py
--rw-r--r--   0        0        0     1162 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/operator/base/client_logic.py
--rw-r--r--   0        0        0     7092 2023-03-10 02:39:09.689922 daisyfl-0.2.0/src/py/daisyfl/operator/base/server_logic.py
--rw-r--r--   0        0        0        0 2023-02-08 08:28:14.950340 daisyfl-0.2.0/src/py/daisyfl/operator/base_async/__init__.py
--rw-r--r--   0        0        0     1162 2023-02-09 07:20:06.916018 daisyfl-0.2.0/src/py/daisyfl/operator/base_async/client_logic.py
--rw-r--r--   0        0        0     6790 2023-03-09 06:45:51.640932 daisyfl-0.2.0/src/py/daisyfl/operator/base_async/server_logic.py
--rw-r--r--   0        0        0     1987 2023-01-10 07:20:47.633253 daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/client_logic.py
--rw-r--r--   0        0        0      381 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/msg.py
--rw-r--r--   0        0        0     6334 2023-03-09 06:30:24.189588 daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/server_logic.py
--rw-r--r--   0        0        0      961 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
--rw-r--r--   0        0        0     6427 2023-03-09 06:33:46.253879 daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
--rw-r--r--   0        0        0    12049 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/sec_agg/client_logic.py
--rw-r--r--   0        0        0     1755 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/sec_agg/common.py
--rw-r--r--   0        0        0    10070 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/sec_agg/primitives.py
--rw-r--r--   0        0        0    22684 2023-03-09 06:38:35.573765 daisyfl-0.2.0/src/py/daisyfl/operator/sec_agg/server_logic.py
--rw-r--r--   0        0        0     1456 2023-02-09 06:56:21.776202 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/__init__.py
--rw-r--r--   0        0        0     3012 2023-02-09 06:53:49.280829 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/aggregate.py
--rw-r--r--   0        0        0     4536 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     5072 2023-03-09 09:24:37.500618 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5987 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6846 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7096 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedadam.py
--rw-r--r--   0        0        0    12362 2023-03-09 06:48:27.052528 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedasync.py
--rw-r--r--   0        0        0    11702 2023-03-09 05:59:59.943053 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedavg.py
--rw-r--r--   0        0        0    10227 2023-03-09 09:30:04.656031 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8987 2023-03-09 09:27:10.272348 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedavgm.py
--rw-r--r--   0        0        0     5366 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedopt.py
--rw-r--r--   0        0        0     7116 2023-03-09 09:25:46.012498 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedyogi.py
--rw-r--r--   0        0        0    10970 2023-03-09 09:26:45.468392 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/qfedavg.py
--rw-r--r--   0        0        0     7575 2023-03-09 05:49:48.419387 daisyfl-0.2.0/src/py/daisyfl/operator/strategy/strategy.py
--rw-r--r--   0        0        0      746 2023-02-16 12:06:55.588223 daisyfl-0.2.0/src/py/daisyfl/operator/utils/__init__.py
--rw-r--r--   0        0        0     4942 2023-03-10 02:34:30.518682 daisyfl-0.2.0/src/py/daisyfl/operator/utils/op_tools.py
--rw-r--r--   0        0        0      676 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/proto/__init__.py
--rw-r--r--   0        0        0    62902 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/proto/transport_pb2.py
--rw-r--r--   0        0        0    23142 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2601 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      781 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0     1064 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/server/__init__.py
--rw-r--r--   0        0        0     4483 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/server/app.py
--rw-r--r--   0        0        0     6630 2023-03-10 01:41:44.010037 daisyfl-0.2.0/src/py/daisyfl/server/client_manager.py
--rw-r--r--   0        0        0     2213 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/server/client_proxy.py
--rw-r--r--   0        0        0      714 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/__init__.py
--rw-r--r--   0        0        0     6038 2023-03-08 06:29:11.534006 daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6418 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4632 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11274 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     3626 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/server/history.py
--rw-r--r--   0        0        0    10982 2023-03-09 03:05:50.096057 daisyfl-0.2.0/src/py/daisyfl/server/server.py
--rw-r--r--   0        0        0     1411 2023-02-22 05:46:45.300324 daisyfl-0.2.0/src/py/daisyfl/server/server_api_handler.py
--rw-r--r--   0        0        0     5095 2023-02-22 07:11:48.908762 daisyfl-0.2.0/src/py/daisyfl/server/server_operator_manager.py
--rw-r--r--   0        0        0    13145 2023-02-17 11:57:05.712372 daisyfl-0.2.0/src/py/daisyfl/server/task_manager.py
--rw-r--r--   0        0        0     1273 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/simulation/__init__.py
--rw-r--r--   0        0        0     7335 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/simulation/app.py
--rw-r--r--   0        0        0      727 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     4661 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0      859 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-01-10 07:20:47.637253 daisyfl-0.2.0/src/py/daisyfl/utils/dynamic_loader.py
--rw-r--r--   0        0        0     2277 2023-03-10 03:00:21.033478 daisyfl-0.2.0/setup.py
--rw-r--r--   0        0        0     2819 2023-03-10 03:00:21.033685 daisyfl-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-10 07:20:47.485254 daisyfl-0.4.1/LICENSE
+-rw-r--r--   0        0        0      691 2023-01-10 07:20:47.485254 daisyfl-0.4.1/README.md
+-rw-r--r--   0        0        0     3661 2023-05-19 02:09:36.975406 daisyfl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1093 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/__init__.py
+-rw-r--r--   0        0        0     1171 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/client/__init__.py
+-rw-r--r--   0        0        0     9944 2023-05-13 09:42:27.721736 daisyfl-0.4.1/src/py/daisyfl/client/app.py
+-rw-r--r--   0        0        0     3733 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/client/client.py
+-rw-r--r--   0        0        0     1363 2023-05-11 01:39:32.910194 daisyfl-0.4.1/src/py/daisyfl/client/client_api_handler.py
+-rw-r--r--   0        0        0     3780 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/client/client_operator_manager.py
+-rw-r--r--   0        0        0     3367 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      714 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0    10038 2023-05-16 08:32:20.489432 daisyfl-0.4.1/src/py/daisyfl/client/grpc_client/connection.py
+-rw-r--r--   0        0        0     6704 2023-04-22 08:34:34.572565 daisyfl-0.4.1/src/py/daisyfl/client/grpc_client/message_handler.py
+-rw-r--r--   0        0        0     5084 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/client/numpy_client.py
+-rw-r--r--   0        0        0     4913 2023-05-16 09:25:04.651405 daisyfl-0.4.1/src/py/daisyfl/client/trainer.py
+-rw-r--r--   0        0        0     1663 2023-04-24 08:39:30.199565 daisyfl-0.4.1/src/py/daisyfl/client/zone_client.py
+-rw-r--r--   0        0        0     5109 2023-05-15 01:42:48.994568 daisyfl-0.4.1/src/py/daisyfl/common/__init__.py
+-rw-r--r--   0        0        0     1830 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/common/dp.py
+-rw-r--r--   0        0        0     3482 2023-05-03 08:10:21.588582 daisyfl-0.4.1/src/py/daisyfl/common/logger.py
+-rw-r--r--   0        0        0     1430 2023-05-16 09:07:57.079143 daisyfl-0.4.1/src/py/daisyfl/common/metadata.py
+-rw-r--r--   0        0        0     3938 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/common/parameter.py
+-rw-r--r--   0        0        0    16903 2023-05-14 06:48:53.590144 daisyfl-0.4.1/src/py/daisyfl/common/serde.py
+-rw-r--r--   0        0        0     4044 2023-05-16 07:23:10.624100 daisyfl-0.4.1/src/py/daisyfl/common/typing.py
+-rw-r--r--   0        0        0        0 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/operator/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/operator/base/__init__.py
+-rw-r--r--   0        0        0     1162 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/operator/base/client_logic.py
+-rw-r--r--   0        0        0     5314 2023-05-16 08:40:46.238319 daisyfl-0.4.1/src/py/daisyfl/operator/base/server_logic.py
+-rw-r--r--   0        0        0        0 2023-02-08 08:28:14.950340 daisyfl-0.4.1/src/py/daisyfl/operator/base_async/__init__.py
+-rw-r--r--   0        0        0     1162 2023-02-09 07:20:06.916018 daisyfl-0.4.1/src/py/daisyfl/operator/base_async/client_logic.py
+-rw-r--r--   0        0        0     5381 2023-05-16 11:59:38.489016 daisyfl-0.4.1/src/py/daisyfl/operator/base_async/server_logic.py
+-rw-r--r--   0        0        0     1987 2023-01-10 07:20:47.633253 daisyfl-0.4.1/src/py/daisyfl/operator/msg_demo/client_logic.py
+-rw-r--r--   0        0        0      381 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/operator/msg_demo/msg.py
+-rw-r--r--   0        0        0     5320 2023-05-16 11:35:42.881982 daisyfl-0.4.1/src/py/daisyfl/operator/msg_demo/server_logic.py
+-rw-r--r--   0        0        0      961 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
+-rw-r--r--   0        0        0     5409 2023-05-16 11:40:56.320957 daisyfl-0.4.1/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
+-rw-r--r--   0        0        0    12049 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/operator/sec_agg/client_logic.py
+-rw-r--r--   0        0        0     1755 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/operator/sec_agg/common.py
+-rw-r--r--   0        0        0    10070 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/operator/sec_agg/primitives.py
+-rw-r--r--   0        0        0    20378 2023-05-16 11:45:43.312726 daisyfl-0.4.1/src/py/daisyfl/operator/sec_agg/server_logic.py
+-rw-r--r--   0        0        0     1456 2023-02-09 06:56:21.776202 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/__init__.py
+-rw-r--r--   0        0        0     3012 2023-02-09 06:53:49.280829 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/aggregate.py
+-rw-r--r--   0        0        0     4538 2023-05-16 12:09:01.916334 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     5095 2023-05-16 12:13:03.915973 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     6134 2023-05-16 12:14:40.331823 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6993 2023-05-16 12:15:36.883734 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7245 2023-05-16 12:16:34.455643 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedadam.py
+-rw-r--r--   0        0        0    13114 2023-05-16 12:17:30.311554 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedasync.py
+-rw-r--r--   0        0        0    12454 2023-05-16 07:22:14.364120 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedavg.py
+-rw-r--r--   0        0        0    10983 2023-05-16 12:18:28.123569 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     9115 2023-05-16 12:19:23.807713 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedavgm.py
+-rw-r--r--   0        0        0     5513 2023-05-16 12:20:07.411811 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedopt.py
+-rw-r--r--   0        0        0     7263 2023-05-16 12:20:50.715896 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedyogi.py
+-rw-r--r--   0        0        0    11020 2023-05-16 12:22:36.468058 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7867 2023-05-15 01:53:20.710219 daisyfl-0.4.1/src/py/daisyfl/operator/strategy/strategy.py
+-rw-r--r--   0        0        0      728 2023-05-16 06:37:26.602959 daisyfl-0.4.1/src/py/daisyfl/operator/utils/__init__.py
+-rw-r--r--   0        0        0     5003 2023-05-16 07:20:49.404138 daisyfl-0.4.1/src/py/daisyfl/operator/utils/op_tools.py
+-rw-r--r--   0        0        0      676 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/proto/__init__.py
+-rw-r--r--   0        0        0    70900 2023-05-14 06:35:47.413527 daisyfl-0.4.1/src/py/daisyfl/proto/transport_pb2.py
+-rw-r--r--   0        0        0    25816 2023-05-14 06:35:47.413527 daisyfl-0.4.1/src/py/daisyfl/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2631 2023-05-14 06:35:47.413527 daisyfl-0.4.1/src/py/daisyfl/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      781 2023-05-14 06:35:47.413527 daisyfl-0.4.1/src/py/daisyfl/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1064 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/server/__init__.py
+-rw-r--r--   0        0        0     5085 2023-05-16 03:16:56.626232 daisyfl-0.4.1/src/py/daisyfl/server/app.py
+-rw-r--r--   0        0        0     6901 2023-05-16 07:14:08.099939 daisyfl-0.4.1/src/py/daisyfl/server/client_manager.py
+-rw-r--r--   0        0        0     2371 2023-05-16 06:58:02.621351 daisyfl-0.4.1/src/py/daisyfl/server/client_proxy.py
+-rw-r--r--   0        0        0      714 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0    12860 2023-05-16 09:25:33.571412 daisyfl-0.4.1/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6707 2023-05-16 08:08:05.114034 daisyfl-0.4.1/src/py/daisyfl/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4459 2023-05-16 08:12:28.157478 daisyfl-0.4.1/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11290 2023-05-09 06:31:30.706022 daisyfl-0.4.1/src/py/daisyfl/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     3626 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/server/history.py
+-rw-r--r--   0        0        0    11104 2023-05-16 11:51:48.437191 daisyfl-0.4.1/src/py/daisyfl/server/server.py
+-rw-r--r--   0        0        0     1011 2023-04-24 07:53:15.707000 daisyfl-0.4.1/src/py/daisyfl/server/server_api_handler.py
+-rw-r--r--   0        0        0     4560 2023-05-16 03:14:42.710438 daisyfl-0.4.1/src/py/daisyfl/server/server_operator_manager.py
+-rw-r--r--   0        0        0    11969 2023-04-24 08:56:27.545364 daisyfl-0.4.1/src/py/daisyfl/server/task_manager.py
+-rw-r--r--   0        0        0     1273 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/simulation/__init__.py
+-rw-r--r--   0        0        0     7335 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     4661 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0      859 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-01-10 07:20:47.637253 daisyfl-0.4.1/src/py/daisyfl/utils/dynamic_loader.py
+-rw-r--r--   0        0        0     2277 2023-05-19 02:13:08.289900 daisyfl-0.4.1/setup.py
+-rw-r--r--   0        0        0     2819 2023-05-19 02:13:08.290114 daisyfl-0.4.1/PKG-INFO
```

### Comparing `daisyfl-0.2.0/LICENSE` & `daisyfl-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/README.md` & `daisyfl-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/pyproject.toml` & `daisyfl-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "daisyfl"
-version = "0.2.0"
+version = "0.4.1"
 description = "Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing"
 license = "Apache-2.0"
 authors = ["tcfwbper <b05208031@ntu.edu.tw>"]
 readme = "README.md"
 homepage = "https://github.com/Intelligent-Systems-Lab/daisy"
 repository = "https://github.com/Intelligent-Systems-Lab/daisy"
 documentation = "https://github.com/Intelligent-Systems-Lab/daisy/tree/main/doc/daisy"
@@ -91,43 +91,38 @@
 [tool.isort]
 line_length = 88
 indent = "    "
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
-known_first_party = ["daisyfl", "flwr_experimental", "flwr_tool"]
+known_first_party = ["daisyfl", "daisy_tools"]
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310"]
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = "bad-continuation,duplicate-code,too-few-public-methods,useless-import-alias"
 
 [tool.pytest.ini_options]
 minversion = "6.2"
 addopts = "-qq"
 testpaths = [
     "src/py/daisyfl",
-    "src/py/flwr_tool",
+    "src/py/daisy_tools",
 ]
 
 [tool.mypy]
 plugins = [
     "numpy.typing.mypy_plugin",
 ]
 ignore_missing_imports = true
 strict = true
 
-[[tool.mypy.overrides]]
-module = [
-    "flwr_example.*",
-    "flwr_experimental.*",
-]
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = [
     "importlib.metadata.*",
     "importlib_metadata.*",
 ]
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/app.py` & `daisyfl-0.4.1/src/py/daisyfl/client/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client app."""
 
 
-import time
-from logging import INFO, ERROR
-from typing import Callable, Dict, Optional, Union, Tuple
+from queue import Queue
+from logging import INFO, ERROR, WARNING
+from typing import Callable, Dict, Optional, Union, Tuple, List
 import threading
 
 from daisyfl.common import (
     GRPC_MAX_MESSAGE_LENGTH,
     CURRENT_ROUND,
     FIT_SAMPLES,
     EVALUATE_SAMPLES,
     LOSS,
     METRICS,
     CLIENT_OPERATOR,
     ZONE_CLIENT_OPERATOR,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
-    ZONE_CREDENTIAL,
+    IS_ZONE,
+    CREDENTIAL,
+    metadata_to_dict,
+    dict_to_metadata,
+    CID,
 )
 from daisyfl.common.logger import log
 from daisyfl.common.typing import (
     Code,
     EvaluateIns,
     EvaluateRes,
     FitIns,
@@ -46,18 +50,18 @@
     GetPropertiesRes,
     NDArrays,
     Status,
     Report,
 )
 
 from .client import Client
-from .client_api_handler import listening, get_alive
-from .grpc_client.connection import grpc_connection, get_connect_to, get_reconnect, get_sleep_duration, set_connect_to, set_reconnect, set_sleep_duration
-from .grpc_client.connection import grpc_connection
-from .grpc_client.message_handler import handle, set_client_operator_manager
+from .client_api_handler import ClientListener
+from .trainer import Trainer
+from .grpc_client.connection import gRPCConnection
+from .grpc_client.message_handler import set_client_operator_manager
 from daisyfl.client.client_operator_manager import ClientOperatorManager
 from .numpy_client import NumPyClient
 from .numpy_client import has_evaluate as numpyclient_has_evaluate
 from .numpy_client import has_fit as numpyclient_has_fit
 from .numpy_client import has_get_parameters as numpyclient_has_get_parameters
 from .numpy_client import has_get_properties as numpyclient_has_get_properties
 
@@ -98,73 +102,75 @@
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[bytes] = None,
     api_ip: str = None,
     api_port: int = None,
     metadata: Tuple = None,
     _zone: bool = False,
 ) -> None:
-
-    set_connect_to(parent_address)
-
     # client_operator_manager
     client_operator_manager = ClientOperatorManager(client=client)
     operator_key = ZONE_CLIENT_OPERATOR if _zone else CLIENT_OPERATOR
-    if _zone:
-        metadata = _handle_zone_credential(metadata)
     client_operator_manager.set_operator_key(key=operator_key)
     set_client_operator_manager(client_operator_manager)
 
-    if isinstance(api_ip, str) and isinstance(api_port, int):
-        listener = threading.Thread(target=listening, args=(api_ip, api_port))
-        listener.setDaemon(True)
-        listener.start()
-        time.sleep(1)
-        if not listener.is_alive():
-            log(
-                ERROR,
-                "client_api_handler failed",
-            )
-            exit(1)
-
-    while True:
-        with grpc_connection(
-            get_connect_to(),
-            max_message_length=grpc_max_message_length,
-            root_certificates=root_certificates,
-            metadata=metadata,
-        ) as conn:
-            receive, send = conn
-
-            while True:
-                try:
-                    server_message = receive()
-                    client_message = handle(server_message)
-                    send(client_message)
-                except:
-                    set_reconnect(True)
-                    set_sleep_duration(5)
-                    log(
-                        ERROR,
-                        "ConnectionError. Will reconnect after 5 seconds.",
-                    )
-                if (get_reconnect()) or (not get_alive()):
-                    set_reconnect(False)
-                    break
-        if not get_alive():
-            log(
-                INFO,
-                "Client shutdown",
-            )
-            break
-        log(
-            INFO,
-            "Disconnect, then re-establish connection after %s second(s)",
-            get_sleep_duration(),
-        )
-        time.sleep(get_sleep_duration())
+    # check metadata
+    if metadata is None:
+        metadata = ()
+    ## zone: process metadata
+    if _zone:
+        metadata_dict = metadata_to_dict(metadata=metadata, _check_required=False)
+        metadata_dict[IS_ZONE] = "is_zone"
+        if metadata_dict.__contains__(CREDENTIAL):
+            log(WARNING, "CREDENTIAL is defined in the metadata of a zone. It will be ignored.")
+            del metadata_dict[CREDENTIAL]
+        if not metadata_dict.__contains__(CID):
+            metadata_dict[CID] = api_ip + str(api_port)
+        metadata = dict_to_metadata(metadata_dict)
+    ## client: check metadata
+    else:
+        metadata_dict = metadata_to_dict(metadata=metadata)
+        metadata = dict_to_metadata(metadata_dict)
+
+    # declare instances: Trainer, gRPCConnection, ClientListener
+    trainer = Trainer()
+    connector = gRPCConnection(
+        parent_address=parent_address,
+        max_message_length=grpc_max_message_length,
+        root_certificates=root_certificates,
+        metadata=metadata,
+        trainer=trainer,
+    )
+    listener = ClientListener(
+        ip=api_ip,
+        port=api_port,
+        connector=connector,
+        trainer=trainer,
+    )
+    trainer.set_connector(connector=connector)
+
+    # start threads: ClientListener, gRPCConnection, Trainer
+    
+    ## ClientListener
+    listener_thread = threading.Thread(target=listener.run, args=())
+    listener_thread.setDaemon(True)
+    listener_thread.start()
+    ## gRPCConnection
+    connector_thread = threading.Thread(target=connector.run, args=())
+    connector_thread.setDaemon(True)
+    connector_thread.start()
+    ### check
+    threading.Event().wait(timeout=1)
+    if not listener_thread.is_alive():
+        log(ERROR, "ClientListener failed")
+        exit(1)
+    if not connector_thread.is_alive():
+        log(ERROR, "gRPCConnection failed")
+        exit(1)
+    ## Trainer
+    trainer.run()
 
 
 def start_numpy_client(
     *,
     parent_address: str,
     client: NumPyClient,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
@@ -181,31 +187,25 @@
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
         api_ip=api_ip,
         api_port=api_port,
         metadata=metadata,
         _zone=_zone,
     )
-    # DEBUG: check if we need this condition
-    if hasattr(client, "shutdown"):
+    if _zone:
         client.shutdown()
 
 
+# wrap numpy_client to client
 def to_client(client_like: ClientLike) -> Client:
     """Take any Client-like object and return it as a Client."""
     if isinstance(client_like, NumPyClient):
         return _wrap_numpy_client(client=client_like)
     return client_like
 
-def _handle_zone_credential(metadata):
-    if metadata is None:
-        metadata = ()
-    lm = list(metadata)
-    lm.append((ZONE_CREDENTIAL, ''))
-    return tuple(lm)
 
 def _constructor(self: Client, numpy_client: NumPyClient) -> None:
     self.numpy_client = numpy_client  # type: ignore
 
 
 def _get_properties(self: Client, ins: GetPropertiesIns) -> GetPropertiesRes:
     """Return the current client properties."""
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/client.py` & `daisyfl-0.4.1/src/py/daisyfl/client/client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/client_operator_manager.py` & `daisyfl-0.4.1/src/py/daisyfl/client/client_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/dpfedavg_numpy_client.py` & `daisyfl-0.4.1/src/py/daisyfl/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/grpc_client/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/grpc_client/message_handler.py` & `daisyfl-0.4.1/src/py/daisyfl/client/grpc_client/message_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from daisyfl.client.client import (
     Client,
     has_evaluate,
     has_fit,
     has_get_parameters,
     has_get_properties,
 )
-from daisyfl.client.grpc_client.connection import reconnect_request, set_reconnect
 from daisyfl.client.client_operator_manager import ClientOperatorManager
 from daisyfl.common import serde, typing
 from daisyfl.common.typing import Parameters
 from daisyfl.proto.transport_pb2 import ClientMessage, Reason, ServerMessage
 
 # pylint: disable=missing-function-docstring
 
@@ -85,15 +84,15 @@
         reason = Reason.RECONNECT
         sleep_duration = reconnect_msg.seconds
     # Build DisconnectRes message
     disconnect_res = ClientMessage.DisconnectRes(reason=reason)
 
     client_operator_manager = get_client_operator_manager()
     client_operator_manager.disconnect()
-    reconnect_request(sleep=sleep_duration)
+    # TODO: reconnect request
     return ClientMessage(disconnect_res=disconnect_res)
 
 
 def _get_properties(
     get_properties_msg: ServerMessage.GetPropertiesIns
 ) -> ClientMessage:
     client = get_client_operator_manager().get_client()
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/numpy_client.py` & `daisyfl-0.4.1/src/py/daisyfl/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/client/zone_client.py` & `daisyfl-0.4.1/src/py/daisyfl/client/zone_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,25 +7,27 @@
     METRICS,
     LOSS,
     EVALUATE_SAMPLES,
     TID,
 )
 import argparse
 from daisyfl.client.numpy_client import NumPyClient
-from daisyfl.client.grpc_client.connection import reconnect_request
+import threading
 
 # Define Flower Zone client
 class ZoneClient(NumPyClient):
-    def __init__(self, task_manager, parent_address, set_zc,):
+    def __init__(self, parent_address, api_ip, api_port, task_manager, cnd_stop):
         self.task_manager = task_manager
-        set_zc(task_manager=task_manager, zone_client=self)
+        self._cnd_stop: threading.Condition = cnd_stop
         # Start Flower client
         fl.client.start_numpy_client(
             parent_address=parent_address,
             client=self,
+            api_ip=api_ip,
+            api_port=api_port,
             _zone=True,
         )
 
     def get_parameters(self, tid: str):
         # return ndarrays
         parameters = self.task_manager.get_parameters(tid=tid)
         return parameters_to_ndarrays(parameters) if parameters is not None else None
@@ -38,11 +40,9 @@
 
     def evaluate(self, parameters, config):
         _, report =  self.task_manager.receive_task(parameters=ndarrays_to_parameters(parameters) , task_config=config)
         # return "loss, num_examples, metrics"
         return report.config[LOSS], report.config[EVALUATE_SAMPLES], report.config
 
     def shutdown(self):
-        self.task_manager.shutdown()
-    
-    def reconnect(self, address: str = None, sleep: int = None) -> None:
-        reconnect_request(address, sleep)
+        with self._cnd_stop:
+            self._cnd_stop.notify()
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/common/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/common/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,20 +17,33 @@
 
 from .parameter import bytes_to_ndarray as bytes_to_ndarray
 from .parameter import ndarray_to_bytes as ndarray_to_bytes
 from .parameter import ndarrays_to_parameters as ndarrays_to_parameters
 from .parameter import parameters_to_ndarrays as parameters_to_ndarrays
 from .parameter import encode_ndarrays as encode_ndarrays
 from .parameter import decode_ndarrays as decode_ndarrays
+from .metadata import metadata_to_dict as metadata_to_dict
+from .metadata import dict_to_metadata as dict_to_metadata
+from .metadata import ANCHOR as ANCHOR
+from .metadata import HANDOVER as HANDOVER
+from .metadata import IS_ZONE as IS_ZONE
+from .metadata import CID as CID
+from .metadata import CREDENTIAL as CREDENTIAL
+from .metadata import DATASET as DATASET
+from .metadata import DEVICE as DEVICE
+from .metadata import ROOT_CERTIFICATES as ROOT_CERTIFICATES
 from .typing import Code as Code
 from .typing import DisconnectRes as DisconnectRes
 from .typing import EvaluateIns as EvaluateIns
 from .typing import EvaluateRes as EvaluateRes
 from .typing import FitIns as FitIns
 from .typing import FitRes as FitRes
+from .typing import ClientStatus as ClientStatus
+from .typing import ServerReceivedSignal as ServerReceivedSignal
+from .typing import ClientReceivedSignal as ClientReceivedSignal
 from .typing import GetParametersIns as GetParametersIns
 from .typing import GetParametersRes as GetParametersRes
 from .typing import GetPropertiesIns as GetPropertiesIns
 from .typing import GetPropertiesRes as GetPropertiesRes
 from .typing import Metrics as Metrics
 from .typing import MetricsAggregationFn as MetricsAggregationFn
 from .typing import NDArray as NDArray
@@ -40,21 +53,24 @@
 from .typing import ReconnectIns as ReconnectIns
 from .typing import Scalar as Scalar
 from .typing import Element as Element
 from .typing import Status as Status
 from .typing import Task as Task
 from .typing import Report as Report
 from .typing import Type as Type
+from .typing import CheckResults as CheckResults
+from .typing import CurrentReturns as CurrentReturns
 
 
 GRPC_MAX_MESSAGE_LENGTH: int = 536_870_912  # == 512 * 1024 * 1024
 NUM_ROUNDS = "NUM_ROUNDS"
 CURRENT_ROUND = "CURRENT_ROUND"
 EVALUATE = "EVALUATE"
 TIMEOUT = "TIMEOUT"
+FORWARDING_TIMEOUT = "FORWARDING_TIMEOUT"
 FIT_SAMPLES = "FIT_SAMPLES"
 EVALUATE_SAMPLES = "EVALUATE_SAMPLES"
 LOSS = "LOSS"
 METRICS = "METRICS"
 TID = "TID"
 SUBTASK = "SUBTASK"
 EVALUATE_INTERVAL = "EVALUATE_INTERVAL"
@@ -65,46 +81,53 @@
 CLIENT_OPERATOR = "CLIENT_OPERATOR"
 ZONE_SERVER_OPERATOR = "ZONE_SERVER_OPERATOR"
 ZONE_CLIENT_OPERATOR = "ZONE_CLIENT_OPERATOR"
 STRATEGIES = "STRATEGIES"
 MASTER_STRATEGY = "MASTER_STRATEGY"
 ZONE_STRATEGY = "ZONE_STRATEGY"
 PERIOD = "PERIOD"
-CREDENTIAL = "credential"
-NO_CREDENTIAL = "no_credential"
-STRICT_SELECTION = "strict_selection"
-ZONE_CREDENTIAL = "zone_credential"
+CLIENT_HANDLING = "CLIENT_HANDLING"
+CLIENT_IDLING = "CLIENT_IDLING"
+
 
 __all__ = [
     "NUM_ROUNDS",
     "CURRENT_ROUND",
     "EVALUATE",
     "TIMEOUT",
+    "FORWARDING_TIMEOUT",
     "SUBTASK",
     "FIT_SAMPLES",
     "EVALUATE_SAMPLES",
     "LOSS",
     "METRICS",
     "EVALUATE_INTERVAL",
     "MODEL_PATH",
     "Type",
+    "CheckResults",
+    "CurrentReturns",
     "encode_ndarrays",
     "decode_ndarrays",
     "bytes_to_ndarray",
+    "metadata_to_dict",
+    "dict_to_metadata",
     "Code",
     "Element",
     "DisconnectRes",
     "EvaluateIns",
     "EvaluateRes",
     "FitIns",
     "FitRes",
     "GetParametersIns",
     "GetParametersRes",
     "GetPropertiesIns",
     "GetPropertiesRes",
+    "ClientStatus",
+    "ServerReceivedSignal",
+    "ClientReceivedSignal",
     "GRPC_MAX_MESSAGE_LENGTH",
     "Metrics",
     "MetricsAggregationFn",
     "ndarray_to_bytes",
     "NDArray",
     "NDArrays",
     "ndarrays_to_parameters",
@@ -124,11 +147,17 @@
     "ZONE_SERVER_OPERATOR",
     "ZONE_CLIENT_OPERATOR",
     "STRATEGIES",
     "MASTER_STRATEGY",
     "ZONE_STRATEGY",
     "PERIOD",
     "CREDENTIAL",
-    "NO_CREDENTIAL",
-    "STRICT_SELECTION",
-    "ZONE_CREDENTIAL",
+    "IS_ZONE",
+    "CLIENT_HANDLING",
+    "CLIENT_IDLING",
+    "ANCHOR",
+    "ROOT_CERTIFICATES",
+    "HANDOVER",
+    "CID",
+    "DATASET",
+    "DEVICE",
 ]
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/common/dp.py` & `daisyfl-0.4.1/src/py/daisyfl/common/dp.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/common/logger.py` & `daisyfl-0.4.1/src/py/daisyfl/common/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Flower Logger."""
 import logging
 from logging import LogRecord
 from logging.handlers import HTTPHandler
 from typing import Any, Dict, Optional, Tuple
 
 # Create logger
-LOGGER_NAME = "flower"
+LOGGER_NAME = "daisy"
 FLOWER_LOGGER = logging.getLogger(LOGGER_NAME)
 FLOWER_LOGGER.setLevel(logging.DEBUG)
 
 DEFAULT_FORMATTER = logging.Formatter(
     "%(levelname)s %(name)s %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
 )
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/common/parameter.py` & `daisyfl-0.4.1/src/py/daisyfl/common/parameter.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/common/serde.py` & `daisyfl-0.4.1/src/py/daisyfl/common/serde.py`

 * *Files 8% similar despite different names*

```diff
@@ -218,28 +218,32 @@
         code = Code.GET_PROPERTIES_NOT_IMPLEMENTED
     if status.code == typing.Code.GET_PARAMETERS_NOT_IMPLEMENTED:
         code = Code.GET_PARAMETERS_NOT_IMPLEMENTED
     if status.code == typing.Code.FIT_NOT_IMPLEMENTED:
         code = Code.FIT_NOT_IMPLEMENTED
     if status.code == typing.Code.EVALUATE_NOT_IMPLEMENTED:
         code = Code.EVALUATE_NOT_IMPLEMENTED
+    if status.code == typing.Code.MESSAGE_LOST:
+        code = Code.MESSAGE_LOST
     return Status(code=code, message=status.message)
 
 
 def status_from_proto(msg: Status) -> typing.Status:
     """Deserialize Code from ProtoBuf message."""
     code = typing.Code.OK
     if msg.code == Code.GET_PROPERTIES_NOT_IMPLEMENTED:
         code = typing.Code.GET_PROPERTIES_NOT_IMPLEMENTED
     if msg.code == Code.GET_PARAMETERS_NOT_IMPLEMENTED:
         code = typing.Code.GET_PARAMETERS_NOT_IMPLEMENTED
     if msg.code == Code.FIT_NOT_IMPLEMENTED:
         code = typing.Code.FIT_NOT_IMPLEMENTED
     if msg.code == Code.EVALUATE_NOT_IMPLEMENTED:
         code = typing.Code.EVALUATE_NOT_IMPLEMENTED
+    if msg.code == Code.MESSAGE_LOST:
+        code = typing.Code.MESSAGE_LOST
     return typing.Status(code=code, message=msg.message)
 
 
 # === Evaluate messages ===
 
 
 def evaluate_ins_to_proto(ins: typing.EvaluateIns) -> ServerMessage.EvaluateIns:
@@ -274,14 +278,54 @@
     config = None if msg.config is None else inner_map_from_proto(msg.config)
     return typing.EvaluateRes(
         status=status,
         config=config,
     )
 
 
+#  === ClientStatus ===
+
+
+def client_status_to_proto(res: typing.ClientStatus) -> ClientMessage.ClientStatus:
+    """Serialize ClientStatus to ProtoBuf message."""
+    return ClientMessage.ClientStatus(status=res.status)
+
+
+def client_status_from_proto(msg: ClientMessage.ClientStatus) -> typing.ClientStatus:
+    """Deserialize ProtoBuf message to ClientStatus."""
+    return typing.ClientStatus(status=msg.status)
+
+
+# === SRS, CRS ===
+
+
+def server_received_signal_to_proto(ins: typing.ServerReceivedSignal) -> ServerMessage.ServerReceivedSignal:
+    """Serialize SRS to ProtoBuf message."""
+    status_proto = status_to_proto(ins.status)
+    return ServerMessage.ServerReceivedSignal(status=status_proto)
+
+
+def server_received_signal_from_proto(msg: ServerMessage.ServerReceivedSignal) -> typing.ServerReceivedSignal:
+    """Deserialize ProtoBug message to SRS"""
+    status = status_from_proto(msg.status)
+    return typing.ServerReceivedSignal(status=status)
+
+
+def client_received_signal_to_proto(res: typing.ClientReceivedSignal) -> ClientMessage.ClientReceivedSignal:
+    """Serialize CRS to ProtoBuf message."""
+    status_proto = status_to_proto(res.status)
+    return ClientMessage.ClientReceivedSignal(status=status_proto)
+
+
+def client_received_signal_from_proto(msg: ClientMessage.ClientReceivedSignal) -> typing.ClientReceivedSignal:
+    """Deserialize ProtoBug message to CRS"""
+    status = status_from_proto(msg.status)
+    return typing.ClientReceivedSignal(status=status)
+
+
 # === Properties messages ===
 
 
 def properties_to_proto(properties: typing.Properties) -> Any:
     """Serialize... ."""
     proto = {}
     for key in properties:
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/common/typing.py` & `daisyfl-0.4.1/src/py/daisyfl/common/typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Flower type definitions."""
 
 
 from dataclasses import dataclass
 from dataclasses_json import dataclass_json
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, TypedDict
-
+from threading import Condition
 import numpy.typing as npt
 
 NDArray = npt.NDArray[Any]
 NDArrays = List[NDArray]
 
 # The following union type contains Python types corresponding to ProtoBuf types that
 # ProtoBuf considers to be "Scalar Value Types", even though some of them arguably do
@@ -44,14 +44,15 @@
     """Client status codes."""
 
     OK = 0
     GET_PROPERTIES_NOT_IMPLEMENTED = 1
     GET_PARAMETERS_NOT_IMPLEMENTED = 2
     FIT_NOT_IMPLEMENTED = 3
     EVALUATE_NOT_IMPLEMENTED = 4
+    MESSAGE_LOST = 5
 
 
 @dataclass
 class Status:
     """Client status."""
 
     code: Code
@@ -162,8 +163,38 @@
     # LOSS: float
     # METRICS: Metrics
 
 class Type(Enum):
     """Type of the task manager."""
     
     MASTER = 1
-    ZONE = 2
+    ZONE = 2
+
+
+class CheckResults(Enum):
+    OK = 0
+    FAIL = 1
+    CONTINUE = 2
+
+
+@dataclass
+class CurrentReturns:
+    selected: int
+    results_num: int
+    failures_num: int
+    cnd: Condition
+
+
+@dataclass
+class ClientStatus:
+    status: str
+
+
+@dataclass
+class ServerReceivedSignal:
+    status: Status
+
+
+@dataclass
+class ClientReceivedSignal:
+    status: Status
+
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/base/client_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/base/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/base/server_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/simulation/app.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,184 +8,184 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
-from typing import Dict, List, Optional, Tuple, TypedDict, Callable
-from queue import Queue
-from threading import Timer, Condition, Event
-from daisyfl.operator.strategy import Strategy
-from daisyfl.common import (
-    Parameters,
-    Report,
-    Task,
-    CURRENT_ROUND,
-    TIMEOUT,
-    PERIOD,
-    NO_CREDENTIAL,
-    CREDENTIAL,
-    STRICT_SELECTION,
-)
-from daisyfl.common.logger import log
+"""Flower simulation app."""
 
-from daisyfl.operator.utils import (
-    get_configure_fit,
-    aggregate_fit,
-    generate_fit_report,
-    get_configure_evaluate,
-    aggregate_evaluate,
-    generate_evaluate_report,
-    get_results_from_queue,
-)
-
-
-class ServerLogic():
-    def __init__(self,
-        server,
-        strategy: Strategy,
-        ticket_dispenser: Callable,
-    ) -> None:
-        self.server = server
-        self.strategy: Strategy = strategy
-        self.ticket_dispenser_fn = ticket_dispenser
-        self.tickets = []
-
-    def disconnect_all_clients(self, timeout: Optional[float]) -> None:
-        """Send shutdown signal to all clients."""
-        self.server.disconnect_all_clients(timeout=timeout)
-
-    def fit_round(
-        self,
-        parameters: Parameters,
-        task: Task,
-        returns_q: Queue,
-    ) -> Optional[
-        Tuple[Optional[Parameters], Optional[Report]]
-    ]:
-        """Perform a single round fit."""
-        # Get clients and their respective instructions from strategy
-        ## credential
-        credential = task.config[CREDENTIAL] if CREDENTIAL in task.config else NO_CREDENTIAL
-        strict = task.config[STRICT_SELECTION] if STRICT_SELECTION in task.config else True
-        ## get_clients
-        client_instructions = get_configure_fit(
-            strategy=self.strategy,
-            server_round=task.config[CURRENT_ROUND],
-            parameters=parameters,
-            server=self.server,
-            config=task.config,
-            credential=credential,
-            strict=strict,
-        )
-        # Collect `fit` results from all clients participating in this round
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
-        self.server.fit_clients(
-            client_instructions=client_instructions,
-            max_workers=self.server.get_max_workers(),
-            timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
-        )
-        # periodically check
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, 2, selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
-        # Aggregate training results
-        parameters_aggregated, samples, metrics_aggregated  = aggregate_fit(
-            strategy=self.strategy,
-            server_round=task.config[CURRENT_ROUND],
-            results=results,
-            failures=[],
-        )
-        # Get report
-        report = generate_fit_report(
-            server_round=task.config[CURRENT_ROUND],
-            samples=samples,
-            metrics_aggregated=metrics_aggregated,
-        )
 
-        return parameters_aggregated, report
+import sys
+from logging import ERROR, INFO
+from typing import Any, Callable, Dict, List, Optional
 
-    def evaluate_round(
-        self,
-        parameters: Parameters,
-        task: Task,
-        returns_q: Queue,
-    ) -> Optional[Report]:
-        """Validate current global model on a number of clients."""
-        # Get clients and their respective instructions from strategy
-        ## credential
-        credential = task.config[CREDENTIAL] if CREDENTIAL in task.config else NO_CREDENTIAL
-        strict = task.config[STRICT_SELECTION] if STRICT_SELECTION in task.config else True
-        ## get_clients
-        client_instructions = get_configure_evaluate(
-            strategy=self.strategy,
-            server_round=task.config[CURRENT_ROUND],
-            parameters=parameters,
-            server=self.server,
-            config=task.config,
-            credential=credential,
-            strict=strict,
-        )
-        # Collect `evaluate` results from all clients participating in this round
-        ticket = self.ticket_dispenser_fn()
-        self.server.evaluate_clients(
-            client_instructions=client_instructions,
-            max_workers=self.server.get_max_workers(),
-            timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
-        )
-        # periodically check
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, 2, selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
-        # Aggregate the evaluation results
-        loss_aggregated, samples, metrics_aggregated = aggregate_evaluate(
-            strategy=self.strategy,
-            server_round=task.config[CURRENT_ROUND],
-            results=results,
-            failures=[],
-        )
-        # Get report
-        report = generate_evaluate_report(
-            server_round=task.config[CURRENT_ROUND],
-            samples=samples,
-            loss_aggregated=loss_aggregated,
-            metrics_aggregated=metrics_aggregated,
-        )
+import ray
 
-        return report
+from daisyfl.client.client import Client
+from daisyfl.common.logger import log
+from daisyfl.server import Server
+from daisyfl.server.app import _init_defaults
+from daisyfl.server.client_manager import ClientManager
+from daisyfl.server.history import History
+from daisyfl.simulation.ray_transport.ray_client_proxy import RayClientProxy
+
+INVALID_ARGUMENTS_START_SIMULATION = """
+INVALID ARGUMENTS ERROR
+
+Invalid Arguments in method:
+
+`start_simulation(
+    *,
+    client_fn: Callable[[str], Client],
+    num_clients: Optional[int] = None,
+    clients_ids: Optional[List[str]] = None,
+    client_resources: Optional[Dict[str, int]] = None,
+    server: Optional[Server] = None,
+    config: ServerConfig = None,
+    strategy: Optional[Strategy] = None,
+    client_manager: Optional[ClientManager] = None,
+    ray_init_args: Optional[Dict[str, Any]] = None,
+) -> None:`
+
+REASON:
+    Method requires:
+        - Either `num_clients`[int] or `clients_ids`[List[str]]
+        to be set exclusively.
+        OR
+        - `len(clients_ids)` == `num_clients`
+
+"""
+
+
+def start_simulation(  # pylint: disable=too-many-arguments
+    *,
+    client_fn: Callable[[str], Client],
+    num_clients: Optional[int] = None,
+    clients_ids: Optional[List[str]] = None,
+    client_resources: Optional[Dict[str, int]] = None,
+    server: Optional[Server] = None,
+    config = None,
+    strategy = None,
+    client_manager: Optional[ClientManager] = None,
+    ray_init_args: Optional[Dict[str, Any]] = None,
+    keep_initialised: Optional[bool] = False,
+) -> History:
+    """Start a Ray-based Flower simulation server.
+
+    Parameters
+    ----------
+    client_fn : Callable[[str], Client]
+        A function creating client instances. The function must take a single
+        str argument called `cid`. It should return a single client instance.
+        Note that the created client instances are ephemeral and will often be
+        destroyed after a single method invocation. Since client instances are
+        not long-lived, they should not attempt to carry state over method
+        invocations. Any state required by the instance (model, dataset,
+        hyperparameters, ...) should be (re-)created in either the call to
+        `client_fn` or the call to any of the client methods (e.g., load
+        evaluation data in the `evaluate` method itself).
+    num_clients : Optional[int]
+        The total number of clients in this simulation. This must be set if
+        `clients_ids` is not set and vice-versa.
+    clients_ids : Optional[List[str]]
+        List `client_id`s for each client. This is only required if
+        `num_clients` is not set. Setting both `num_clients` and `clients_ids`
+        with `len(clients_ids)` not equal to `num_clients` generates an error.
+    client_resources : Optional[Dict[str, int]] (default: None)
+        CPU and GPU resources for a single client. Supported keys are
+        `num_cpus` and `num_gpus`. Example: `{"num_cpus": 4, "num_gpus": 1}`.
+        To understand the GPU utilization caused by `num_gpus`, consult the Ray
+        documentation on GPU support.
+    server: Optional[flwr.server.Server] (default: None). An implementation
+        of the abstract base class `flwr.server.Server`. If no instance is
+        provided, then `start_server` will create one.
+    config: ServerConfig (default: None).
+        Currently supported values are `num_rounds` (int, default: 1) and
+        `round_timeout` in seconds (float, default: None).
+    strategy : Optional[flwr.server.Strategy] (default: None)
+        An implementation of the abstract base class `flwr.server.Strategy`. If
+        no strategy is provided, then `start_server` will use
+        `flwr.server.strategy.FedAvg`.
+    client_manager: Optional[flwr.server.ClientManager] (default: None)
+        An implementation of the abstract base class `flwr.server.ClientManager`.
+        If no implementation is provided, then `start_simulation` will use
+        `flwr.server.client_manager.SimpleClientManager`.
+    ray_init_args : Optional[Dict[str, Any]] (default: None)
+        Optional dictionary containing arguments for the call to `ray.init`.
+        If ray_init_args is None (the default), Ray will be initialized with
+        the following default args:
+
+            {
+                "ignore_reinit_error": True,
+                "include_dashboard": False,
+            }
+
+        An empty dictionary can be used (ray_init_args={}) to prevent any
+        arguments from being passed to ray.init.
+    keep_initialised: Optional[bool] (default: False)
+        Set to True to prevent `ray.shutdown()` in case `ray.is_initialized()=True`.
+
+    Returns
+    -------
+        hist: flwr.server.history.History. Object containing metrics from training.
+    """
+    # pylint: disable-msg=too-many-locals
+
+    # Initialize server and server config
+    initialized_server, initialized_config = _init_defaults(
+        server=server,
+        config=config,
+        strategy=strategy,
+        client_manager=client_manager,
+    )
+    log(
+        INFO,
+        "Starting Flower simulation, config: %s",
+        initialized_config,
+    )
+
+    # clients_ids takes precedence
+    cids: List[str]
+    if clients_ids is not None:
+        if (num_clients is not None) and (len(clients_ids) != num_clients):
+            log(ERROR, INVALID_ARGUMENTS_START_SIMULATION)
+            sys.exit()
+        else:
+            cids = clients_ids
+    else:
+        if num_clients is None:
+            log(ERROR, INVALID_ARGUMENTS_START_SIMULATION)
+            sys.exit()
+        else:
+            cids = [str(x) for x in range(num_clients)]
+
+    # Default arguments for Ray initialization
+    if not ray_init_args:
+        ray_init_args = {
+            "ignore_reinit_error": True,
+            "include_dashboard": False,
+        }
+
+    # Shut down Ray if it has already been initialized (unless asked not to)
+    if ray.is_initialized() and not keep_initialised:
+        ray.shutdown()
+
+    # Initialize Ray
+    ray.init(**ray_init_args)
+    log(
+        INFO,
+        "Flower VCE: Ray initialized with resources: %s",
+        ray.cluster_resources(),
+    )
+
+    # Register one RayClientProxy object for each client with the ClientManager
+    resources = client_resources if client_resources is not None else {}
+    for cid in cids:
+        client_proxy = RayClientProxy(
+            client_fn=client_fn,
+            cid=cid,
+            resources=resources,
+        )
+        initialized_server.client_manager().register(client=client_proxy)
 
-    def notify(self, cnd: Condition):
-        with cnd:
-            cnd.notify()
-
-    def check_enough_returns(self, event: Event, fraction: float, min_num: int, selected: int, results_num: int, failures_num: int) -> bool:
-        if ((fraction * selected <= results_num) and (min_num <= results_num)):
-            event.set()
-            return True
-        if ((fraction * selected) <= (selected - failures_num)) and (min_num <= (selected - failures_num)):
-            return True
-        return False
+    return None
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/base_async/client_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/base_async/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/base_async/server_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/base_async/server_logic.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,102 +8,89 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
+from logging import INFO, WARNING, ERROR
 from typing import Dict, List, Optional, Tuple, TypedDict, Callable
 from queue import Queue
-from threading import Timer, Condition, Event
+from threading import Event
 from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
     Parameters,
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
     PERIOD,
-    NO_CREDENTIAL,
     CREDENTIAL,
-    STRICT_SELECTION,
 )
 from daisyfl.common.logger import log
 
 from daisyfl.operator.utils import (
     get_configure_fit,
     aggregate_fit,
     generate_fit_report,
     get_configure_evaluate,
     aggregate_evaluate,
     generate_evaluate_report,
-    get_results_from_queue,
+    wait_for_results,
 )
 
 
 class ServerLogic():
     def __init__(self,
         server,
         strategy: Strategy,
-        ticket_dispenser: Callable,
     ) -> None:
         self.server = server
         self.strategy: Strategy = strategy
-        self.ticket_dispenser_fn = ticket_dispenser
-        self.tickets = []
-
-    def disconnect_all_clients(self, timeout: Optional[float]) -> None:
-        """Send shutdown signal to all clients."""
-        self.server.disconnect_all_clients(timeout=timeout)
+        self.subtasks = {}
 
     def fit_round(
         self,
         parameters: Parameters,
         task: Task,
-        returns_q: Queue,
     ) -> Optional[
         Tuple[Optional[Parameters], Optional[Report]]
     ]:
         """Perform a single round fit."""
         # Get clients and their respective instructions from strategy
         ## credential
-        credential = task.config[CREDENTIAL] if CREDENTIAL in task.config else NO_CREDENTIAL
-        strict = task.config[STRICT_SELECTION] if STRICT_SELECTION in task.config else True
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
         ## get_clients
         client_instructions = get_configure_fit(
             strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             parameters=parameters,
             server=self.server,
             config=task.config,
             credential=credential,
-            strict=strict,
         )
         # Collect `fit` results from all clients participating in this round
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
-        self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-        # wait
-        cnd = Condition()
-        timer = Timer(task.config[PERIOD], self.notify, [cnd])
-        timer.start()
-        with cnd:
-            cnd.wait()
-        results = get_results_from_queue(returns_q=returns_q)
+        self.subtasks[subtask_id] = subtask_id
+        Event.wait(timeout=task.config[PERIOD])
+        # check
+        results = []
+        for stid in list(self.subtasks.values()):
+            results = results + self.server.get_results(stid)
         if len(results) == 0:
             return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
         # Aggregate training results
-        parameters_aggregated, samples, metrics_aggregated  = aggregate_fit(
+        parameters_aggregated, samples, metrics_aggregated = aggregate_fit(
             strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             results=results,
             failures=[],
         )
         # Get report
         report = generate_fit_report(
@@ -114,53 +101,43 @@
 
         return parameters_aggregated, report
 
     def evaluate_round(
         self,
         parameters: Parameters,
         task: Task,
-        returns_q: Queue,
     ) -> Optional[Report]:
         """Validate current global model on a number of clients."""
         # Get clients and their respective instructions from strategy
         ## credential
-        credential = task.config[CREDENTIAL] if CREDENTIAL in task.config else NO_CREDENTIAL
-        strict = task.config[STRICT_SELECTION] if STRICT_SELECTION in task.config else True
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
         ## get_clients
         client_instructions = get_configure_evaluate(
             strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             parameters=parameters,
             server=self.server,
             config=task.config,
             credential=credential,
-            strict=strict,
         )
         # Collect `evaluate` results from all clients participating in this round
-        ticket = self.ticket_dispenser_fn()
-        self.server.evaluate_clients(
+        subtask_id = self.server.evaluate_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-        # wait
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, 2, selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_evaluate_report(task.config[CURRENT_ROUND], 0, 9999.0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
         # Aggregate the evaluation results
         loss_aggregated, samples, metrics_aggregated = aggregate_evaluate(
             strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             results=results,
             failures=[],
         )
@@ -169,19 +146,7 @@
             server_round=task.config[CURRENT_ROUND],
             samples=samples,
             loss_aggregated=loss_aggregated,
             metrics_aggregated=metrics_aggregated,
         )
 
         return report
-
-    def notify(self, cnd: Condition):
-        with cnd:
-            cnd.notify()
-
-    def check_enough_returns(self, event: Event, fraction: float, min_num: int, selected: int, results_num: int, failures_num: int) -> bool:
-        if ((fraction * selected <= results_num) and (min_num <= results_num)):
-            event.set()
-            return True
-        if ((fraction * selected) <= (selected - failures_num)) and (min_num <= (selected - failures_num)):
-            return True
-        return False
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/client_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/msg_demo/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/server_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/msg_demo/server_logic.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,29 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
+from logging import INFO, WARNING, ERROR
 from queue import Queue
-from threading import Timer, Condition, Event
 from typing import Dict, List, Optional, Tuple, TypedDict, Callable
 from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
     Parameters,
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
     PERIOD,
-    NO_CREDENTIAL,
     CREDENTIAL,
-    STRICT_SELECTION,
 )
 from .msg import (
     WHO_CREATE_THIS_DEMO,
     TIME,
     STUDENT,
     Time,
     Student,
@@ -40,107 +37,84 @@
 from daisyfl.operator.utils import (
     get_configure_fit,
     aggregate_fit,
     generate_fit_report,
     get_configure_evaluate,
     aggregate_evaluate,
     generate_evaluate_report,
-    get_results_from_queue,
+    wait_for_results,
 )
 from daisyfl.server import Server
 
 from daisyfl.operator.base.server_logic import ServerLogic as BaseServerLogic
 
 
 class ServerLogic(BaseServerLogic):
     def __init__(self,
         server: Server,
         strategy: Strategy,
-        ticket_dispenser: Callable,
     ) -> None:
         self.server: Server = server
         self.strategy: Strategy = strategy
-        self.ticket_dispenser_fn = ticket_dispenser
-        self.tickets = []
 
     def fit_round(
         self,
         parameters: Parameters,
         task: Task,
-        returns_q: Queue,
     ) -> Optional[
         Tuple[Optional[Parameters], Optional[Report]]
     ]:
         """Perform a single round fit."""
         # SAY_HI
         ## Get clients and their respective instructions from strategy
         ### credential
-        credential = task.config[CREDENTIAL] if CREDENTIAL in task.config else NO_CREDENTIAL
-        strict = task.config[STRICT_SELECTION] if STRICT_SELECTION in task.config else True
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
         ### get_clients
         client_instructions = get_configure_fit(
             strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             parameters=parameters,
             server=self.server,
             config=task.config,
             credential=credential,
-            strict=strict,
         )
         config = task.config
         config = _setup_info(config, "Tsung-Han Chang", "Alice", 18, False)
         config = _transition(config)
         client_instructions = _set_config(config, client_instructions)
         ## Collect `fit` results from all clients participating in this round
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
-        self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, 2, selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        get_results_from_queue(returns_q=returns_q)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
         # TRAIN
         config = _transition(config)
         client_instructions = _set_config(config, client_instructions)
         ## Collect `fit` results from all clients participating in this round
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
-        self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, 2, selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
         ## Aggregate training results
         parameters_aggregated, samples, metrics_aggregated  = aggregate_fit(
             strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             results=results,
             failures=[],
         )
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/zone_client_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/msg_demo/zone_client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/msg_demo/zone_server_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/base/server_logic.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,177 +8,141 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
+from logging import INFO, WARNING, ERROR
 from typing import Dict, List, Optional, Tuple, TypedDict, Callable
-from threading import Timer, Condition, Event
 from queue import Queue
 from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
     Parameters,
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
     PERIOD,
-    NO_CREDENTIAL,
     CREDENTIAL,
-    STRICT_SELECTION,
-)
-from .msg import (
-    TIME,
-    Time,
 )
 from daisyfl.common.logger import log
 
 from daisyfl.operator.utils import (
     get_configure_fit,
     aggregate_fit,
     generate_fit_report,
     get_configure_evaluate,
     aggregate_evaluate,
     generate_evaluate_report,
-    get_results_from_queue,
+    wait_for_results,
 )
-from daisyfl.server import Server
-from daisyfl.operator.base.server_logic import ServerLogic as BaseServerLogic
 
 
-class ZoneServerLogic(BaseServerLogic):
+class ServerLogic():
     def __init__(self,
-        server: Server,
+        server,
         strategy: Strategy,
-        ticket_dispenser: Callable,
     ) -> None:
-        self.server: Server = server
+        self.server = server
         self.strategy: Strategy = strategy
-        self.ticket_dispenser_fn = ticket_dispenser
-        self.tickets = []
 
     def fit_round(
         self,
         parameters: Parameters,
         task: Task,
-        returns_q: Queue,
     ) -> Optional[
         Tuple[Optional[Parameters], Optional[Report]]
     ]:
         """Perform a single round fit."""
-        stage = Time(task.config[TIME])
-        if stage == Time.SAY_HI:
-            return _say_hi(self, parameters, task, returns_q)
-        elif stage == Time.TRAIN:
-            return _fit(self, parameters, task, returns_q)
+        # Get clients and their respective instructions from strategy
+        ## credential
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
         else:
-            raise ValueError("Invalid stage received")
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
+        ## get_clients
+        client_instructions = get_configure_fit(
+            strategy=self.strategy,
+            server_round=task.config[CURRENT_ROUND],
+            parameters=parameters,
+            server=self.server,
+            config=task.config,
+            credential=credential,
+        )
+        # Collect `fit` results from all clients participating in this round
+        subtask_id = self.server.fit_clients(
+            client_instructions=client_instructions,
+            max_workers=self.server.get_max_workers(),
+            timeout=task.config[TIMEOUT],
+        )
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
+        # Aggregate training results
+        parameters_aggregated, samples, metrics_aggregated  = aggregate_fit(
+            strategy=self.strategy,
+            server_round=task.config[CURRENT_ROUND],
+            results=results,
+            failures=[],
+        )
+        # Get report
+        report = generate_fit_report(
+            server_round=task.config[CURRENT_ROUND],
+            samples=samples,
+            metrics_aggregated=metrics_aggregated,
+        )
 
+        return parameters_aggregated, report
 
-def _say_hi(
-    server_logic: ZoneServerLogic,
-    parameters: Parameters,
-    task: Task,
-    returns_q: Queue,
-) -> Optional[
-    Tuple[Optional[Parameters], Optional[Report]]
-]:
-    ## Get clients and their respective instructions from strategy
-    ### credential
-    credential = task.config[CREDENTIAL] if CREDENTIAL in task.config else NO_CREDENTIAL
-    strict = task.config[STRICT_SELECTION] if STRICT_SELECTION in task.config else True
-    ### get_clients
-    client_instructions = get_configure_fit(
-        strategy=server_logic.strategy,
-        server_round=task.config[CURRENT_ROUND],
-        parameters=parameters,
-        server=server_logic.server,
-        config=task.config,
-        credential=credential,
-        strict=strict,
-    )
-    ## Collect `fit` results from all clients participating in this round
-    ticket = server_logic.ticket_dispenser_fn()
-    server_logic.tickets.append(ticket)
-    server_logic.server.fit_clients(
-        client_instructions=client_instructions,
-        max_workers=server_logic.server.get_max_workers(),
-        timeout=task.config[TIMEOUT],
-        returns_q=returns_q,
-        ticket=ticket,
-    )
-    event = Event()
-    while(not event.is_set()):
-        cnd = Condition()
-        timer = Timer(task.config[PERIOD], server_logic.notify, [cnd])
-        timer.start()
-        with cnd:
-            cnd.wait()
-        selected, results_num, failures_num = server_logic.server.query_status(ticket)
-        if not server_logic.check_enough_returns(event, 0.8, 2, selected, results_num, failures_num):
-            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-    server_logic.server.stop_return(ticket)
-    get_results_from_queue(returns_q=returns_q)
-    # Get report
-    report = generate_fit_report(
-        server_round=task.config[CURRENT_ROUND],
-        samples=0,
-        metrics_aggregated={},
-    )
-        
-    return parameters, report
-
-def _fit(server_logic: ZoneServerLogic, parameters: Parameters, task: Task, returns_q: Queue,):
-    """Perform a single round fit."""
-    # Get clients and their respective instructions from strategy
-    ### credential
-    credential = task.config[CREDENTIAL] if CREDENTIAL in task.config else NO_CREDENTIAL
-    strict = task.config[STRICT_SELECTION] if STRICT_SELECTION in task.config else True
-    ### get_clients
-    client_instructions = get_configure_fit(
-        strategy=server_logic.strategy,
-        server_round=task.config[CURRENT_ROUND],
-        parameters=parameters,
-        server=server_logic.server,
-        config=task.config,
-        credential=credential,
-        strict=strict,
-    )
-    # Collect `fit` results from all clients participating in this round
-    ticket = server_logic.ticket_dispenser_fn()
-    server_logic.tickets.append(ticket)
-    server_logic.server.fit_clients(
-        client_instructions=client_instructions,
-        max_workers=server_logic.server.get_max_workers(),
-        timeout=task.config[TIMEOUT],
-        returns_q=returns_q,
-        ticket=ticket,
-    )
-    event = Event()
-    while(not event.is_set()):
-        cnd = Condition()
-        timer = Timer(task.config[PERIOD], server_logic.notify, [cnd])
-        timer.start()
-        with cnd:
-            cnd.wait()
-        selected, results_num, failures_num = server_logic.server.query_status(ticket)
-        if not server_logic.check_enough_returns(event, 0.8, 2, selected, results_num, failures_num):
-            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-    server_logic.server.stop_return(ticket)
-    results = get_results_from_queue(returns_q=returns_q)
-    # Aggregate training results
-    parameters_aggregated, samples, metrics_aggregated  = aggregate_fit(
-        strategy=server_logic.strategy,
-        server_round=task.config[CURRENT_ROUND],
-        results=results,
-        failures=[],
-    )
-    # Get report
-    report = generate_fit_report(
-        server_round=task.config[CURRENT_ROUND],
-        samples=samples,
-        metrics_aggregated=metrics_aggregated,
-    )
+    def evaluate_round(
+        self,
+        parameters: Parameters,
+        task: Task,
+    ) -> Optional[Report]:
+        """Validate current global model on a number of clients."""
+        # Get clients and their respective instructions from strategy
+        ## credential
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
+        ## get_clients
+        client_instructions = get_configure_evaluate(
+            strategy=self.strategy,
+            server_round=task.config[CURRENT_ROUND],
+            parameters=parameters,
+            server=self.server,
+            config=task.config,
+            credential=credential,
+        )
+        # Collect `evaluate` results from all clients participating in this round
+        subtask_id = self.server.evaluate_clients(
+            client_instructions=client_instructions,
+            max_workers=self.server.get_max_workers(),
+            timeout=task.config[TIMEOUT],
+        )
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_evaluate_report(task.config[CURRENT_ROUND], 0, 9999.0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
+        # Aggregate the evaluation results
+        loss_aggregated, samples, metrics_aggregated = aggregate_evaluate(
+            strategy=self.strategy,
+            server_round=task.config[CURRENT_ROUND],
+            results=results,
+            failures=[],
+        )
+        # Get report
+        report = generate_evaluate_report(
+            server_round=task.config[CURRENT_ROUND],
+            samples=samples,
+            loss_aggregated=loss_aggregated,
+            metrics_aggregated=metrics_aggregated,
+        )
 
-    return parameters_aggregated, report
+        return report
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/sec_agg/client_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/sec_agg/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/sec_agg/common.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/sec_agg/common.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/sec_agg/primitives.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/sec_agg/primitives.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/sec_agg/server_logic.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/sec_agg/server_logic.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
+from logging import INFO, WARNING, ERROR
 from typing import Dict, List, Optional, Tuple, TypedDict, Callable
 from queue import Queue
 from daisyfl.common.typing import NDArrays
 from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
     FitIns,
     FitRes,
@@ -25,17 +25,15 @@
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
     FIT_SAMPLES,
     METRICS,
     PERIOD,
-    NO_CREDENTIAL,
     CREDENTIAL,
-    STRICT_SELECTION,
     parameters_to_ndarrays,
     ndarrays_to_parameters,
 )
 from .common import (
     Proto,
     PROTO_KEY,
     SEC_AGG_PARAM_DICT,
@@ -54,216 +52,158 @@
 from threading import Event, Condition, Timer
 from daisyfl.server.server import FitResultsAndFailures
 from daisyfl.server.client_proxy import ClientProxy
 from daisyfl.operator.utils import (
     get_configure_fit,
     aggregate_fit,
     generate_fit_report,
-    get_results_from_queue,
+    wait_for_results,
 )
 from daisyfl.common.logger import log
 
 
 class ServerLogic(BaseServerLogic):
     """Wrapper which adds SecAgg methods."""
 
     def __init__(
         self,
         server: Server,
         strategy: Strategy,
-        ticket_dispenser: Callable
     ) -> None:
         self.server: Server = server
         self.strategy: Strategy = strategy
-        self.ticket_dispenser_fn = ticket_dispenser
-        self.tickets = []
 
     def fit_round(
         self,
         parameters: Parameters,
         task: Task,
-        returns_q: Queue,
     ) -> Optional[
         Tuple[Optional[Parameters], Optional[Report]]
     ]:
         """Perform a single round fit."""
         # Get clients and their respective instructions from strategy
         ## credential
-        credential = task.config[CREDENTIAL] if CREDENTIAL in task.config else NO_CREDENTIAL
-        strict = task.config[STRICT_SELECTION] if STRICT_SELECTION in task.config else True
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
         ## get_clients
         client_instructions = get_configure_fit(
             strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             parameters=parameters,
             server=self.server,
             config=task.config,
             credential=credential,
-            strict=strict,
         )
 
         # === Stage 0: Setup ===
         log(INFO, "SecAgg Stage 0: Setting up Params")
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
         sec_agg_param_dict = get_sec_agg_param_dict(task,len(client_instructions))
         setup_dict: Dict[int, Tuple[ClientProxy, FitIns]] = \
             initialize_ins_dict(client_instructions)
         setup_dict = set_ins_stage(setup_dict, Proto.SETUP.value)
         setup_dict = set_sec_agg_param_dict(setup_dict, sec_agg_param_dict)
         # pass dummy parameters via gRPC
         setup_dict = set_ins_parameters(setup_dict, Parameters(tensors=[], tensor_type=""))
         client_instructions = client_ins_from_ins_dict(setup_dict)
 
-        self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-        
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, sec_agg_param_dict['min_num'], selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
-        
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
+
         # === Stage 1: Ask Public Keys ===
         log(INFO, "SecAgg Stage 1: Asking Keys")
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
         ask_keys_dict: Dict[int, Tuple[ClientProxy, FitIns]] = \
             next_ins_dict(setup_dict, results)
         ask_keys_dict = set_ins_stage(ask_keys_dict, Proto.ASK_KEYS.value)
         client_instructions = client_ins_from_ins_dict(ask_keys_dict)
 
-        self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-        
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, sec_agg_param_dict['min_num'], selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
 
         # === Stage 2: Share Keys ===
         log(INFO, "SecAgg Stage 2: Sharing Keys")
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
         share_keys_dict: Dict[int, Tuple[ClientProxy, FitIns]] = \
             next_ins_dict(ask_keys_dict, results)
         share_keys_dict = set_ins_stage(share_keys_dict, Proto.SHARE_KEYS.value)
         share_keys_dict = set_pks_dict(share_keys_dict, results)
         client_instructions = client_ins_from_ins_dict(share_keys_dict)
 
-        self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-        
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, sec_agg_param_dict['min_num'], selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
 
         # === Stage 3: Ask Vectors ===
         log(INFO, "SecAgg Stage 3: Asking Vectors")
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
         ask_vectors_dict = next_ins_dict(share_keys_dict, results)
         ask_vectors_dict = set_ins_stage(ask_vectors_dict, Proto.ASK_VECTORS.value)
         ask_vectors_dict = set_packet_list(ask_vectors_dict, results)
         # parameters for training
         ask_vectors_dict = set_ins_parameters(ask_vectors_dict, parameters)
         client_instructions = client_ins_from_ins_dict(ask_vectors_dict)
 
-        self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, sec_agg_param_dict['min_num'], selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
 
         # === Stage 4: Unmask Vectors ===
         log(INFO, "SecAgg Stage 4: Unmasking Vectors")
-        ticket = self.ticket_dispenser_fn()
-        self.tickets.append(ticket)
         unmask_vectors_dict = next_ins_dict(ask_vectors_dict, results)
         unmask_vectors_dict = set_ins_stage(unmask_vectors_dict, Proto.UNMASK_VECTORS.value)
         masked_vectors, num_examples, metrics = aggregate_fit(results)
         unmask_vectors_dict = set_surviving_info(unmask_vectors_dict, ask_vectors_dict)
         # pass dummy parameters via gRPC
         unmask_vectors_dict = set_ins_parameters(unmask_vectors_dict, Parameters(tensors=[], tensor_type=""))
         client_instructions = client_ins_from_ins_dict(unmask_vectors_dict)
         
-        self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
-            returns_q=returns_q,
-            ticket=ticket,
         )
-
-        event = Event()
-        while(not event.is_set()):
-            cnd = Condition()
-            timer = Timer(task.config[PERIOD], self.notify, [cnd])
-            timer.start()
-            with cnd:
-                cnd.wait()
-            selected, results_num, failures_num = self.server.query_status(ticket)
-            if not self.check_enough_returns(event, 0.8, sec_agg_param_dict['min_num'], selected, results_num, failures_num):
-                return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
-        self.server.stop_return(ticket)
-        results = get_results_from_queue(returns_q=returns_q)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
 
         parameters_aggregated = unmask_vector(unmask_vectors_dict, ask_vectors_dict, masked_vectors, results, sec_agg_param_dict)
 
         report = generate_fit_report(
             server_round=task.config[CURRENT_ROUND],
             samples=num_examples,
             metrics_aggregated=metrics,
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/aggregate.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 from daisyfl.common import FitIns, FitRes, Parameters, Scalar
 from daisyfl.server.client_manager import ClientManager
 from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.server.strategy.dpfedavg_fixed import DPFedAvgFixed
+from daisyfl.operator.strategy.dpfedavg_fixed import DPFedAvgFixed
 from daisyfl.operator.strategy.strategy import Strategy
 
 
 class DPFedAvgAdaptive(DPFedAvgFixed):
     """Wrapper for configuring a Strategy for DP with Adaptive Clipping."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """DP-FedAvg [McMahan et al., 2018] strategy.
 
 Paper: https://arxiv.org/pdf/1710.06963.pdf
 """
 
 from typing import Dict, List, Optional, Tuple, Union
 
-from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar, CURRENT_ROUND, NO_CREDENTIAL
+from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar, CURRENT_ROUND, CurrentReturns, CheckResults
 from daisyfl.common.dp import add_gaussian_noise
 from daisyfl.common.parameter import ndarrays_to_parameters, parameters_to_ndarrays
 from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 from daisyfl.operator.strategy.strategy import Strategy
 
 
@@ -69,44 +69,42 @@
         return self.strategy.initialize_parameters(server)
 
     def configure_fit(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
 
         additional_config = {"dpfedavg_clip_norm": self.clip_norm}
         if not self.server_side_noising:
             additional_config[
                 "dpfedavg_noise_stddev"
             ] = self._calc_client_noise_stddev()
 
         client_instructions = self.strategy.configure_fit(
-            server_round, parameters, server, credential, strict,
+            server_round, parameters, server, credential,
         )
 
         for _, fit_ins in client_instructions:
             fit_ins.config.update(additional_config)
 
         return client_instructions
 
     def configure_evaluate(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         return self.strategy.configure_evaluate(
-            server_round, parameters, server, credential, strict,
+            server_round, parameters, server, credential,
         )
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
         failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
@@ -133,7 +131,12 @@
     ) -> Tuple[Optional[float], Dict[str, Scalar]]:
         return self.strategy.aggregate_evaluate(server_round, results, failures)
 
     def evaluate(
         self, server_round: int, parameters: Parameters
     ) -> Optional[Tuple[float, Dict[str, Scalar]]]:
         return self.strategy.evaluate(server_round, parameters)
+    
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        return
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 1,
         min_evaluate_clients: int = 1,
         min_available_clients: int = 1,
+        min_result: int = 1,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -60,17 +62,19 @@
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
     ) -> None:
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=True,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedadagrad.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedadagrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -106,17 +108,19 @@
             eta_l (float, optional): Client-side learning rate. Defaults to 1e-1.
             tau (float, optional): Controls the algorithm's degree of adaptability.
                 Defaults to 1e-9.
         """
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedadam.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedadam.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: float = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -109,17 +111,19 @@
             beta_2 (float, optional): Second moment parameter. Defaults to 0.99.
             tau (float, optional): Controls the algorithm's degree of adaptability.
                 Defaults to 1e-9.
         """
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedasync.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedasync.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
     CURRENT_ROUND,
-    NO_CREDENTIAL,
+    CurrentReturns,
+    CheckResults,
 )
 from daisyfl.common.logger import log
 from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg, fed_async_aggregate
 from .strategy import Strategy
@@ -55,17 +56,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         # NOTE:
         alpha: float = 0.9,
         staleness_fn: Callable = None,
         # NOTE:
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
@@ -121,17 +124,19 @@
             min_fit_clients > min_available_clients
             or min_evaluate_clients > min_available_clients
         ):
             log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
 
         self.fraction_fit = fraction_fit
         self.fraction_evaluate = fraction_evaluate
+        self.fraction_result = fraction_result
         self.min_fit_clients = min_fit_clients
         self.min_evaluate_clients = min_evaluate_clients
         self.min_available_clients = min_available_clients
+        self.min_result = min_result
         self.evaluate_fn = evaluate_fn
         self.on_fit_config_fn = on_fit_config_fn
         self.on_evaluate_config_fn = on_evaluate_config_fn
         self.accept_failures = accept_failures
         self.initial_parameters = initial_parameters
         self.fit_metrics_aggregation_fn = fit_metrics_aggregation_fn
         self.evaluate_metrics_aggregation_fn = evaluate_metrics_aggregation_fn
@@ -178,42 +183,40 @@
         return loss, metrics
 
     def configure_fit(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
         fit_ins = FitIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_fit_clients(
-            server.num_available()
+            server.num_available(credential=credential)
         )
-        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential, strict=strict,)
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # TODO: Client selection
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
     def configure_evaluate(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
         # Do not configure federated evaluation if fraction eval is 0.
         if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
@@ -221,17 +224,17 @@
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
         evaluate_ins = EvaluateIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_evaluation_clients(
-            server.num_available()
+            server.num_available(credential=credential)
         )
-        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential, strict=strict,)
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # TODO: Client selection
 
         # Return client/config pairs
         return [(client, evaluate_ins) for client in clients]
 
     def aggregate_fit(
@@ -301,7 +304,20 @@
             # Multiply accuracy of each client by number of examples used
             accuracies = [num_examples * m["accuracy"] for num_examples, m in eval_metrics]
             examples = [num_examples for num_examples, _ in eval_metrics]
             metrics_aggregated = {"accuracy": sum(accuracies) / sum(examples)}
 
         return loss_aggregated, metrics_aggregated
 
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        if current_returns is None:
+            return CheckResults.FAIL
+        if ((self.fraction_result * current_returns.selected <= current_returns.results_num) and \
+            (self.min_result <= current_returns.results_num)):
+            return CheckResults.OK
+        if ((self.fraction_result * current_returns.selected) <= (current_returns.selected - current_returns.failures_num)) \
+            and (self.min_result <= (current_returns.selected - current_returns.failures_num)):
+            return CheckResults.CONTINUE
+        return CheckResults.FAIL
+
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedavg.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedavg.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     FitRes,
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
-    NO_CREDENTIAL,
+    CheckResults,
+    CurrentReturns,
 )
 from daisyfl.common.logger import log
 from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg
 from .strategy import Strategy
@@ -54,17 +55,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 0.8,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -116,17 +119,19 @@
             min_fit_clients > min_available_clients
             or min_evaluate_clients > min_available_clients
         ):
             log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
 
         self.fraction_fit = fraction_fit
         self.fraction_evaluate = fraction_evaluate
+        self.fraction_result = fraction_result
         self.min_fit_clients = min_fit_clients
         self.min_evaluate_clients = min_evaluate_clients
         self.min_available_clients = min_available_clients
+        self.min_result = min_result
         self.evaluate_fn = evaluate_fn
         self.on_fit_config_fn = on_fit_config_fn
         self.on_evaluate_config_fn = on_evaluate_config_fn
         self.accept_failures = accept_failures
         self.initial_parameters = initial_parameters
         self.fit_metrics_aggregation_fn = fit_metrics_aggregation_fn
         self.evaluate_metrics_aggregation_fn = evaluate_metrics_aggregation_fn
@@ -169,41 +174,39 @@
         return loss, metrics
 
     def configure_fit(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
         fit_ins = FitIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_fit_clients(
-            server.num_available()
+            server.num_available(credential=credential)
         )
-        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential, strict=strict,)
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # TODO: Client selection
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
     def configure_evaluate(
         self, server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
         # Do not configure federated evaluation if fraction eval is 0.
         if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
@@ -211,17 +214,17 @@
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
         evaluate_ins = EvaluateIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_evaluation_clients(
-            server.num_available()
+            server.num_available(credential=credential)
         )
-        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential, strict=strict,)
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # TODO: Client selection
 
         # Return client/config pairs
         return [(client, evaluate_ins) for client in clients]
 
     def aggregate_fit(
@@ -284,7 +287,20 @@
             log(INFO, "Using default evaluate_metrics_aggregation_fn")
             # Multiply accuracy of each client by number of examples used
             accuracies = [num_examples * m["accuracy"] for num_examples, m in eval_metrics]
             examples = [num_examples for num_examples, _ in eval_metrics]
             metrics_aggregated = {"accuracy": sum(accuracies) / sum(examples)}
 
         return loss_aggregated, metrics_aggregated
+
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        if current_returns is None:
+            return CheckResults.FAIL
+        if ((self.fraction_result * current_returns.selected <= current_returns.results_num) and \
+            (self.min_result <= current_returns.results_num)):
+            return CheckResults.OK
+        if ((self.fraction_result * current_returns.selected) <= (current_returns.selected - current_returns.failures_num)) \
+            and (self.min_result <= (current_returns.selected - current_returns.failures_num)):
+            return CheckResults.CONTINUE
+        return CheckResults.FAIL
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedavg_android.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedavg_android.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     EvaluateRes,
     FitIns,
     FitRes,
     NDArray,
     NDArrays,
     Parameters,
     Scalar,
-    NO_CREDENTIAL,
+    CurrentReturns,
+    CheckResults,
 )
 from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg
 from .strategy import Strategy
 
@@ -46,17 +47,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -96,16 +99,18 @@
             containing failures. Defaults to True.
         initial_parameters : Optional[Parameters]
             Initial global model parameters.
         """
         super().__init__()
         self.min_fit_clients = min_fit_clients
         self.min_evaluate_clients = min_evaluate_clients
+        self.min_result = min_result
         self.fraction_fit = fraction_fit
         self.fraction_evaluate = fraction_evaluate
+        self.fraction_result = fraction_result
         self.min_available_clients = min_available_clients
         self.evaluate_fn = evaluate_fn
         self.on_fit_config_fn = on_fit_config_fn
         self.on_evaluate_config_fn = on_evaluate_config_fn
         self.accept_failures = accept_failures
         self.initial_parameters = initial_parameters
 
@@ -147,42 +152,40 @@
         return loss, metrics
 
     def configure_fit(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
         fit_ins = FitIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_fit_clients(
-            server.num_available()
+            server.num_available(credential=credential)
         )
-        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential, strict=strict,)
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # TODO: Client selection
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
     def configure_evaluate(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
         # Do not configure federated evaluation if fraction_evaluate is 0
         if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
@@ -190,17 +193,17 @@
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
         evaluate_ins = EvaluateIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_evaluation_clients(
-            server.num_available()
+            server.num_available(credential=credential)
         )
-        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential, strict=strict,)
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # TODO: Client selection
 
         # Return client/config pairs
         return [(client, evaluate_ins) for client in clients]
 
     def aggregate_fit(
@@ -257,7 +260,21 @@
         return ndarray.tobytes()
 
     # pylint: disable=R0201
     def bytes_to_ndarray(self, tensor: bytes) -> NDArray:
         """Deserialize NumPy array from bytes."""
         ndarray_deserialized = np.frombuffer(tensor, dtype=np.float32)  # type: ignore
         return cast(NDArray, ndarray_deserialized)
+
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        if current_returns is None:
+            return CheckResults.FAIL
+        if ((self.fraction_result * current_returns.selected <= current_returns.results_num) and \
+            (self.min_result <= current_returns.results_num)):
+            return CheckResults.OK
+        if ((self.fraction_result * current_returns.selected) <= (current_returns.selected - current_returns.failures_num)) \
+            and (self.min_result <= (current_returns.selected - current_returns.failures_num)):
+            return CheckResults.CONTINUE
+        return CheckResults.FAIL
+
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedavgm.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedavgm.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     FitRes,
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
-    NO_CREDENTIAL,
 )
 from daisyfl.common.logger import log
 from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate
 from .fedavg import FedAvg
@@ -51,17 +50,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -116,17 +117,19 @@
             or min_evaluate_clients > min_available_clients
         ):
             log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
 
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedopt.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedopt.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -101,17 +103,19 @@
         beta_2 (float, optional): Second moment parameter. Defaults to 0.0.
         tau (float, optional): Controls the algorithm's degree of adaptability.
             Defaults to 1e-9.
         """
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/fedyogi.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/fedyogi.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -109,17 +111,19 @@
             beta_2 (float, optional): Second moment parameter. Defaults to 0.99.
             tau (float, optional): Controls the algorithm's degree of adaptability.
                 Defaults to 1e-9.
         """
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/qfedavg.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/qfedavg.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     FitRes,
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
-    NO_CREDENTIAL,
 )
 from daisyfl.common.logger import log
 from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate_qffl, weighted_loss_avg
 from .fedavg import FedAvg
@@ -52,17 +51,19 @@
     def __init__(
         self,
         *,
         q_param: float = 0.2,
         qffl_learning_rate: float = 0.1,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 1,
         min_evaluate_clients: int = 1,
         min_available_clients: int = 1,
+        min_result: int = 1,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -71,17 +72,19 @@
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
     ) -> None:
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
@@ -119,45 +122,43 @@
         return max(num_clients, self.min_evaluate_clients), self.min_available_clients
 
     def configure_fit(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
         weights = parameters_to_ndarrays(parameters)
         self.pre_weights = weights
         parameters = ndarrays_to_parameters(weights)
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
         fit_ins = FitIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_fit_clients(
-            server.num_available()
+            server.num_available(credential=credential)
         )
-        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential, strict=strict,)
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # TODO: Client selection
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
     def configure_evaluate(
         self,
         server_round: int,
         parameters: Parameters,
         server: Server,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
         # Do not configure federated evaluation if fraction_evaluate is 0
         if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
@@ -165,17 +166,17 @@
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
         evaluate_ins = EvaluateIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_evaluation_clients(
-            server.num_available()
+            server.num_available(credential=credential)
         )
-        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential, strict=strict,)
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # TODO: Client selection
 
         # Return client/config pairs
         return [(client, evaluate_ins) for client in clients]
 
     def aggregate_fit(
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/strategy/strategy.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/strategy/strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 """Flower server strategy."""
 
 
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional, Tuple, Union
 
-from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar, NO_CREDENTIAL
+from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar, CheckResults, CurrentReturns
 from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 
 class Strategy(ABC):
     """Abstract base class for server strategy implementations."""
 
@@ -43,15 +43,15 @@
             If parameters are returned, then the server will treat these as the
             initial global model parameters.
         """
 
     @abstractmethod
     def configure_fit(
         self, server_round: int, parameters: Parameters, server: Server,
-        credential: str = NO_CREDENTIAL, strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training.
 
         Parameters
         ----------
         server_round : int
             The current round of federated learning.
@@ -105,15 +105,15 @@
             parameters, the updates received in this round are discarded, and
             the global model parameters remain the same.
         """
 
     @abstractmethod
     def configure_evaluate(
         self, server_round: int, parameters: Parameters, server: Server,
-        credential: str = NO_CREDENTIAL, strict: bool = True,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation.
 
         Parameters
         ----------
         server_round : int
             The current round of federated learning.
@@ -181,7 +181,18 @@
 
         Returns
         -------
         evaluation_result : Optional[Tuple[float, Dict[str, Scalar]]]
             The evaluation result, usually a Tuple containing loss and a
             dictionary containing task-specific metrics (e.g., accuracy).
         """
+    
+    @abstractmethod
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        """Check if there are enough results
+        Query CurrentReturns instance from Server
+        Call op_tools.wait_for_results
+        wait until this function returns CheckResults.OK or CheckResults.FAIL
+        """
+
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/utils/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .op_tools import get_configure_fit as get_configure_fit
 from .op_tools import get_configure_evaluate as get_configure_evaluate
 from .op_tools import aggregate_fit as aggregate_fit
 from .op_tools import aggregate_evaluate as aggregate_evaluate
 from .op_tools import generate_fit_report as generate_fit_report
 from .op_tools import generate_evaluate_report as generate_evaluate_report
-from .op_tools import get_results_from_queue as get_results_from_queue
+from .op_tools import wait_for_results as wait_for_results
 
 __all__ = [
     "get_configure_fit",
     "get_configure_evaluate",
     "aggregate_fit",
     "aggregate_evaluate",
     "generate_fit_report",
     "generate_evaluate_report",
     "wait_for_fit_sync",
     "wait_for_evaluate_sync",
     "aggregate_fit_async",
-    "get_results_from_queue",
+    "wait_for_results",
 ]
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/operator/utils/op_tools.py` & `daisyfl-0.4.1/src/py/daisyfl/operator/utils/op_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,23 @@
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
     Parameters,
     ReconnectIns,
     Scalar,
-    NO_CREDENTIAL,
+    CheckResults,
+    CurrentReturns,
 )
 from daisyfl.common.logger import log
 from daisyfl.common.typing import GetParametersIns
 from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 from daisyfl.operator.strategy import Strategy
+from threading import Condition
 
 FitResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, FitRes]],
     List[Union[Tuple[ClientProxy, FitRes], BaseException]],
 ]
 EvaluateResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, EvaluateRes]],
@@ -43,43 +45,39 @@
 
 def get_configure_fit(
     strategy: Strategy,
     server_round: int,
     parameters: Parameters,
     server: Server,
     config: Dict,
-    credential: str = NO_CREDENTIAL,
-    strict: bool = True,
+    credential: str,
 ) -> List[Tuple[ClientProxy, FitIns]]:
     client_instructions = strategy.configure_fit(
         server_round=server_round,
         parameters=parameters,
         server=server,
         credential=credential,
-        strict=strict,
     )
     for i in range(len(client_instructions)):
         client_instructions[i][1].config = config.copy()
     return client_instructions
 
 def get_configure_evaluate(
     strategy: Strategy,
     server_round: int,
     parameters: Parameters,
     server: Server,
     config: Dict,
-    credential: str = NO_CREDENTIAL,
-    strict: bool = True,
+    credential: str,
 ) -> List[Tuple[ClientProxy, EvaluateIns]]:
     client_instructions = strategy.configure_evaluate(
         server_round=server_round,
         parameters=parameters,
         server=server,
         credential=credential,
-        strict=strict,
     )
     for i in range(len(client_instructions)):
         client_instructions[i][1].config = config.copy()
     return client_instructions
 
 def aggregate_fit(
     strategy: Strategy,
@@ -148,15 +146,16 @@
     return Report(config={
         CURRENT_ROUND: server_round,
         LOSS: loss_aggregated,
         EVALUATE_SAMPLES: samples,
         METRICS: metrics_aggregated,
     })
 
-def get_results_from_queue(
-    returns_q: Queue,
-) -> List[Tuple[ClientProxy, EvaluateRes]]:
-    results = []
-    for i in range(returns_q.qsize()):
-        results.append(returns_q.get())
-    return results
-
+def wait_for_results(
+    strategy: Strategy, current_returns: CurrentReturns,
+) -> bool:
+    cnd = current_returns.cnd
+    with cnd:
+        cnd.wait_for(lambda: strategy.check_results(current_returns) in [CheckResults.OK, CheckResults.FAIL])
+    if strategy.check_results(current_returns) == CheckResults.OK:
+        return True
+    return False
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/proto/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/proto/transport_pb2.py` & `daisyfl-0.4.1/src/py/daisyfl/proto/transport_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flwr/proto/transport.proto
+# source: daisyfl/proto/transport.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='flwr/proto/transport.proto',
-  package='flwr.proto',
+  name='daisyfl/proto/transport.proto',
+  package='daisyfl.proto',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1a\x66lwr/proto/transport.proto\x12\nflwr.proto\"9\n\x06Status\x12\x1e\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x10.flwr.proto.Code\x12\x0f\n\x07message\x18\x02 \x01(\t\"2\n\nParameters\x12\x0f\n\x07tensors\x18\x01 \x03(\x0c\x12\x13\n\x0btensor_type\x18\x02 \x01(\t\"i\n\x06Scalar\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x42\x08\n\x06scalar\"4\n\tInnerList\x12\'\n\ninner_list\x18\x01 \x03(\x0b\x32\x13.flwr.proto.Element\"\x87\x01\n\x08InnerMap\x12\x35\n\tinner_map\x18\x01 \x03(\x0b\x32\".flwr.proto.InnerMap.InnerMapEntry\x1a\x44\n\rInnerMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.flwr.proto.Element:\x02\x38\x01\"\x97\x01\n\x0bInnerMapInt\x12?\n\rinner_map_int\x18\x01 \x03(\x0b\x32(.flwr.proto.InnerMapInt.InnerMapIntEntry\x1aG\n\x10InnerMapIntEntry\x12\x0b\n\x03key\x18\x01 \x01(\x03\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.flwr.proto.Element:\x02\x38\x01\"\xf5\x01\n\x07\x45lement\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x12)\n\tinner_map\x18\x10 \x01(\x0b\x32\x14.flwr.proto.InnerMapH\x00\x12\x30\n\rinner_map_int\x18\x11 \x01(\x0b\x32\x17.flwr.proto.InnerMapIntH\x00\x12+\n\ninner_list\x18\x12 \x01(\x0b\x32\x15.flwr.proto.InnerListH\x00\x42\t\n\x07\x65lement\"\xfd\x06\n\rServerMessage\x12?\n\rreconnect_ins\x18\x01 \x01(\x0b\x32&.flwr.proto.ServerMessage.ReconnectInsH\x00\x12H\n\x12get_properties_ins\x18\x02 \x01(\x0b\x32*.flwr.proto.ServerMessage.GetPropertiesInsH\x00\x12H\n\x12get_parameters_ins\x18\x03 \x01(\x0b\x32*.flwr.proto.ServerMessage.GetParametersInsH\x00\x12\x33\n\x07\x66it_ins\x18\x04 \x01(\x0b\x32 .flwr.proto.ServerMessage.FitInsH\x00\x12=\n\x0c\x65valuate_ins\x18\x05 \x01(\x0b\x32%.flwr.proto.ServerMessage.EvaluateInsH\x00\x1a\x1f\n\x0cReconnectIns\x12\x0f\n\x07seconds\x18\x01 \x01(\x03\x1a\x9d\x01\n\x10GetPropertiesIns\x12\x46\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x36.flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry\x1a\x41\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.flwr.proto.Scalar:\x02\x38\x01\x1a\x9d\x01\n\x10GetParametersIns\x12\x46\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x36.flwr.proto.ServerMessage.GetParametersIns.ConfigEntry\x1a\x41\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.flwr.proto.Scalar:\x02\x38\x01\x1aZ\n\x06\x46itIns\x12*\n\nparameters\x18\x01 \x01(\x0b\x32\x16.flwr.proto.Parameters\x12$\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x14.flwr.proto.InnerMap\x1a_\n\x0b\x45valuateIns\x12*\n\nparameters\x18\x01 \x01(\x0b\x32\x16.flwr.proto.Parameters\x12$\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x14.flwr.proto.InnerMapB\x05\n\x03msg\"\xa3\x07\n\rClientMessage\x12\x41\n\x0e\x64isconnect_res\x18\x01 \x01(\x0b\x32\'.flwr.proto.ClientMessage.DisconnectResH\x00\x12H\n\x12get_properties_res\x18\x02 \x01(\x0b\x32*.flwr.proto.ClientMessage.GetPropertiesResH\x00\x12H\n\x12get_parameters_res\x18\x03 \x01(\x0b\x32*.flwr.proto.ClientMessage.GetParametersResH\x00\x12\x33\n\x07\x66it_res\x18\x04 \x01(\x0b\x32 .flwr.proto.ClientMessage.FitResH\x00\x12=\n\x0c\x65valuate_res\x18\x05 \x01(\x0b\x32%.flwr.proto.ClientMessage.EvaluateResH\x00\x1a\x33\n\rDisconnectRes\x12\"\n\x06reason\x18\x01 \x01(\x0e\x32\x12.flwr.proto.Reason\x1a\xcd\x01\n\x10GetPropertiesRes\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.flwr.proto.Status\x12N\n\nproperties\x18\x02 \x03(\x0b\x32:.flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry\x1a\x45\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.flwr.proto.Scalar:\x02\x38\x01\x1a\x62\n\x10GetParametersRes\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.flwr.proto.Status\x12*\n\nparameters\x18\x02 \x01(\x0b\x32\x16.flwr.proto.Parameters\x1a~\n\x06\x46itRes\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.flwr.proto.Status\x12*\n\nparameters\x18\x02 \x01(\x0b\x32\x16.flwr.proto.Parameters\x12$\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x14.flwr.proto.InnerMap\x1aW\n\x0b\x45valuateRes\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.flwr.proto.Status\x12$\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x14.flwr.proto.InnerMapB\x05\n\x03msg*\x8d\x01\n\x04\x43ode\x12\x06\n\x02OK\x10\x00\x12\"\n\x1eGET_PROPERTIES_NOT_IMPLEMENTED\x10\x01\x12\"\n\x1eGET_PARAMETERS_NOT_IMPLEMENTED\x10\x02\x12\x17\n\x13\x46IT_NOT_IMPLEMENTED\x10\x03\x12\x1c\n\x18\x45VALUATE_NOT_IMPLEMENTED\x10\x04*[\n\x06Reason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tRECONNECT\x10\x01\x12\x16\n\x12POWER_DISCONNECTED\x10\x02\x12\x14\n\x10WIFI_UNAVAILABLE\x10\x03\x12\x07\n\x03\x41\x43K\x10\x04\x32S\n\rFlowerService\x12\x42\n\x04Join\x12\x19.flwr.proto.ClientMessage\x1a\x19.flwr.proto.ServerMessage\"\x00(\x01\x30\x01\x62\x06proto3'
+  serialized_pb=b'\n\x1d\x64\x61isyfl/proto/transport.proto\x12\rdaisyfl.proto\"<\n\x06Status\x12!\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x13.daisyfl.proto.Code\x12\x0f\n\x07message\x18\x02 \x01(\t\"2\n\nParameters\x12\x0f\n\x07tensors\x18\x01 \x03(\x0c\x12\x13\n\x0btensor_type\x18\x02 \x01(\t\"i\n\x06Scalar\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x42\x08\n\x06scalar\"7\n\tInnerList\x12*\n\ninner_list\x18\x01 \x03(\x0b\x32\x16.daisyfl.proto.Element\"\x8d\x01\n\x08InnerMap\x12\x38\n\tinner_map\x18\x01 \x03(\x0b\x32%.daisyfl.proto.InnerMap.InnerMapEntry\x1aG\n\rInnerMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.daisyfl.proto.Element:\x02\x38\x01\"\x9d\x01\n\x0bInnerMapInt\x12\x42\n\rinner_map_int\x18\x01 \x03(\x0b\x32+.daisyfl.proto.InnerMapInt.InnerMapIntEntry\x1aJ\n\x10InnerMapIntEntry\x12\x0b\n\x03key\x18\x01 \x01(\x03\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.daisyfl.proto.Element:\x02\x38\x01\"\xfe\x01\n\x07\x45lement\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x12,\n\tinner_map\x18\x10 \x01(\x0b\x32\x17.daisyfl.proto.InnerMapH\x00\x12\x33\n\rinner_map_int\x18\x11 \x01(\x0b\x32\x1a.daisyfl.proto.InnerMapIntH\x00\x12.\n\ninner_list\x18\x12 \x01(\x0b\x32\x18.daisyfl.proto.InnerListH\x00\x42\t\n\x07\x65lement\"\xb8\x08\n\rServerMessage\x12\x42\n\rreconnect_ins\x18\x01 \x01(\x0b\x32).daisyfl.proto.ServerMessage.ReconnectInsH\x00\x12K\n\x12get_properties_ins\x18\x02 \x01(\x0b\x32-.daisyfl.proto.ServerMessage.GetPropertiesInsH\x00\x12K\n\x12get_parameters_ins\x18\x03 \x01(\x0b\x32-.daisyfl.proto.ServerMessage.GetParametersInsH\x00\x12\x36\n\x07\x66it_ins\x18\x04 \x01(\x0b\x32#.daisyfl.proto.ServerMessage.FitInsH\x00\x12@\n\x0c\x65valuate_ins\x18\x05 \x01(\x0b\x32(.daisyfl.proto.ServerMessage.EvaluateInsH\x00\x12S\n\x16server_received_signal\x18\x06 \x01(\x0b\x32\x31.daisyfl.proto.ServerMessage.ServerReceivedSignalH\x00\x1a\x1f\n\x0cReconnectIns\x12\x0f\n\x07seconds\x18\x01 \x01(\x03\x1a\xa3\x01\n\x10GetPropertiesIns\x12I\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x39.daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry\x1a\x44\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1a\xa3\x01\n\x10GetParametersIns\x12I\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x39.daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry\x1a\x44\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1a`\n\x06\x46itIns\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x65\n\x0b\x45valuateIns\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a=\n\x14ServerReceivedSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.StatusB\x05\n\x03msg\"\xcc\t\n\rClientMessage\x12\x44\n\x0e\x64isconnect_res\x18\x01 \x01(\x0b\x32*.daisyfl.proto.ClientMessage.DisconnectResH\x00\x12K\n\x12get_properties_res\x18\x02 \x01(\x0b\x32-.daisyfl.proto.ClientMessage.GetPropertiesResH\x00\x12K\n\x12get_parameters_res\x18\x03 \x01(\x0b\x32-.daisyfl.proto.ClientMessage.GetParametersResH\x00\x12\x36\n\x07\x66it_res\x18\x04 \x01(\x0b\x32#.daisyfl.proto.ClientMessage.FitResH\x00\x12@\n\x0c\x65valuate_res\x18\x05 \x01(\x0b\x32(.daisyfl.proto.ClientMessage.EvaluateResH\x00\x12\x42\n\rclient_status\x18\x06 \x01(\x0b\x32).daisyfl.proto.ClientMessage.ClientStatusH\x00\x12S\n\x16\x63lient_received_signal\x18\x07 \x01(\x0b\x32\x31.daisyfl.proto.ClientMessage.ClientReceivedSignalH\x00\x1a\x36\n\rDisconnectRes\x12%\n\x06reason\x18\x01 \x01(\x0e\x32\x15.daisyfl.proto.Reason\x1a\xd6\x01\n\x10GetPropertiesRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12Q\n\nproperties\x18\x02 \x03(\x0b\x32=.daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry\x1aH\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1ah\n\x10GetParametersRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12-\n\nparameters\x18\x02 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x1a\x87\x01\n\x06\x46itRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12-\n\nparameters\x18\x02 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a]\n\x0b\x45valuateRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x1e\n\x0c\x43lientStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x1a=\n\x14\x43lientReceivedSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.StatusB\x05\n\x03msg*\x9f\x01\n\x04\x43ode\x12\x06\n\x02OK\x10\x00\x12\"\n\x1eGET_PROPERTIES_NOT_IMPLEMENTED\x10\x01\x12\"\n\x1eGET_PARAMETERS_NOT_IMPLEMENTED\x10\x02\x12\x17\n\x13\x46IT_NOT_IMPLEMENTED\x10\x03\x12\x1c\n\x18\x45VALUATE_NOT_IMPLEMENTED\x10\x04\x12\x10\n\x0cMESSAGE_LOST\x10\x05*[\n\x06Reason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tRECONNECT\x10\x01\x12\x16\n\x12POWER_DISCONNECTED\x10\x02\x12\x14\n\x10WIFI_UNAVAILABLE\x10\x03\x12\x07\n\x03\x41\x43K\x10\x04\x32Y\n\rFlowerService\x12H\n\x04Join\x12\x1c.daisyfl.proto.ClientMessage\x1a\x1c.daisyfl.proto.ServerMessage\"\x00(\x01\x30\x01\x62\x06proto3'
 )
 
 _CODE = _descriptor.EnumDescriptor(
   name='Code',
-  full_name='flwr.proto.Code',
+  full_name='daisyfl.proto.Code',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
       name='OK', index=0, number=0,
       serialized_options=None,
@@ -51,26 +51,31 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='EVALUATE_NOT_IMPLEMENTED', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='MESSAGE_LOST', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2685,
-  serialized_end=2826,
+  serialized_start=3202,
+  serialized_end=3361,
 )
 _sym_db.RegisterEnumDescriptor(_CODE)
 
 Code = enum_type_wrapper.EnumTypeWrapper(_CODE)
 _REASON = _descriptor.EnumDescriptor(
   name='Reason',
-  full_name='flwr.proto.Reason',
+  full_name='daisyfl.proto.Reason',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
       name='UNKNOWN', index=0, number=0,
       serialized_options=None,
@@ -95,50 +100,51 @@
       name='ACK', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2828,
-  serialized_end=2919,
+  serialized_start=3363,
+  serialized_end=3454,
 )
 _sym_db.RegisterEnumDescriptor(_REASON)
 
 Reason = enum_type_wrapper.EnumTypeWrapper(_REASON)
 OK = 0
 GET_PROPERTIES_NOT_IMPLEMENTED = 1
 GET_PARAMETERS_NOT_IMPLEMENTED = 2
 FIT_NOT_IMPLEMENTED = 3
 EVALUATE_NOT_IMPLEMENTED = 4
+MESSAGE_LOST = 5
 UNKNOWN = 0
 RECONNECT = 1
 POWER_DISCONNECTED = 2
 WIFI_UNAVAILABLE = 3
 ACK = 4
 
 
 
 _STATUS = _descriptor.Descriptor(
   name='Status',
-  full_name='flwr.proto.Status',
+  full_name='daisyfl.proto.Status',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='code', full_name='flwr.proto.Status.code', index=0,
+      name='code', full_name='daisyfl.proto.Status.code', index=0,
       number=1, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='message', full_name='flwr.proto.Status.message', index=1,
+      name='message', full_name='daisyfl.proto.Status.message', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -148,36 +154,36 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42,
-  serialized_end=99,
+  serialized_start=48,
+  serialized_end=108,
 )
 
 
 _PARAMETERS = _descriptor.Descriptor(
   name='Parameters',
-  full_name='flwr.proto.Parameters',
+  full_name='daisyfl.proto.Parameters',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='tensors', full_name='flwr.proto.Parameters.tensors', index=0,
+      name='tensors', full_name='daisyfl.proto.Parameters.tensors', index=0,
       number=1, type=12, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='tensor_type', full_name='flwr.proto.Parameters.tensor_type', index=1,
+      name='tensor_type', full_name='daisyfl.proto.Parameters.tensor_type', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -187,57 +193,57 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=101,
-  serialized_end=151,
+  serialized_start=110,
+  serialized_end=160,
 )
 
 
 _SCALAR = _descriptor.Descriptor(
   name='Scalar',
-  full_name='flwr.proto.Scalar',
+  full_name='daisyfl.proto.Scalar',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='double', full_name='flwr.proto.Scalar.double', index=0,
+      name='double', full_name='daisyfl.proto.Scalar.double', index=0,
       number=1, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sint64', full_name='flwr.proto.Scalar.sint64', index=1,
+      name='sint64', full_name='daisyfl.proto.Scalar.sint64', index=1,
       number=8, type=18, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bool', full_name='flwr.proto.Scalar.bool', index=2,
+      name='bool', full_name='daisyfl.proto.Scalar.bool', index=2,
       number=13, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='string', full_name='flwr.proto.Scalar.string', index=3,
+      name='string', full_name='daisyfl.proto.Scalar.string', index=3,
       number=14, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bytes', full_name='flwr.proto.Scalar.bytes', index=4,
+      name='bytes', full_name='daisyfl.proto.Scalar.bytes', index=4,
       number=15, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -247,34 +253,34 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
-      name='scalar', full_name='flwr.proto.Scalar.scalar',
+      name='scalar', full_name='daisyfl.proto.Scalar.scalar',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=153,
-  serialized_end=258,
+  serialized_start=162,
+  serialized_end=267,
 )
 
 
 _INNERLIST = _descriptor.Descriptor(
   name='InnerList',
-  full_name='flwr.proto.InnerList',
+  full_name='daisyfl.proto.InnerList',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='inner_list', full_name='flwr.proto.InnerList.inner_list', index=0,
+      name='inner_list', full_name='daisyfl.proto.InnerList.inner_list', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -284,36 +290,36 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=260,
-  serialized_end=312,
+  serialized_start=269,
+  serialized_end=324,
 )
 
 
 _INNERMAP_INNERMAPENTRY = _descriptor.Descriptor(
   name='InnerMapEntry',
-  full_name='flwr.proto.InnerMap.InnerMapEntry',
+  full_name='daisyfl.proto.InnerMap.InnerMapEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.InnerMap.InnerMapEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.InnerMap.InnerMapEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.InnerMap.InnerMapEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.InnerMap.InnerMapEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -323,28 +329,28 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=382,
-  serialized_end=450,
+  serialized_start=397,
+  serialized_end=468,
 )
 
 _INNERMAP = _descriptor.Descriptor(
   name='InnerMap',
-  full_name='flwr.proto.InnerMap',
+  full_name='daisyfl.proto.InnerMap',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='inner_map', full_name='flwr.proto.InnerMap.inner_map', index=0,
+      name='inner_map', full_name='daisyfl.proto.InnerMap.inner_map', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -354,36 +360,36 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=315,
-  serialized_end=450,
+  serialized_start=327,
+  serialized_end=468,
 )
 
 
 _INNERMAPINT_INNERMAPINTENTRY = _descriptor.Descriptor(
   name='InnerMapIntEntry',
-  full_name='flwr.proto.InnerMapInt.InnerMapIntEntry',
+  full_name='daisyfl.proto.InnerMapInt.InnerMapIntEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.InnerMapInt.InnerMapIntEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.InnerMapInt.InnerMapIntEntry.key', index=0,
       number=1, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.InnerMapInt.InnerMapIntEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.InnerMapInt.InnerMapIntEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -393,28 +399,28 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=533,
-  serialized_end=604,
+  serialized_start=554,
+  serialized_end=628,
 )
 
 _INNERMAPINT = _descriptor.Descriptor(
   name='InnerMapInt',
-  full_name='flwr.proto.InnerMapInt',
+  full_name='daisyfl.proto.InnerMapInt',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='inner_map_int', full_name='flwr.proto.InnerMapInt.inner_map_int', index=0,
+      name='inner_map_int', full_name='daisyfl.proto.InnerMapInt.inner_map_int', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -424,78 +430,78 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=453,
-  serialized_end=604,
+  serialized_start=471,
+  serialized_end=628,
 )
 
 
 _ELEMENT = _descriptor.Descriptor(
   name='Element',
-  full_name='flwr.proto.Element',
+  full_name='daisyfl.proto.Element',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='double', full_name='flwr.proto.Element.double', index=0,
+      name='double', full_name='daisyfl.proto.Element.double', index=0,
       number=1, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sint64', full_name='flwr.proto.Element.sint64', index=1,
+      name='sint64', full_name='daisyfl.proto.Element.sint64', index=1,
       number=8, type=18, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bool', full_name='flwr.proto.Element.bool', index=2,
+      name='bool', full_name='daisyfl.proto.Element.bool', index=2,
       number=13, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='string', full_name='flwr.proto.Element.string', index=3,
+      name='string', full_name='daisyfl.proto.Element.string', index=3,
       number=14, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bytes', full_name='flwr.proto.Element.bytes', index=4,
+      name='bytes', full_name='daisyfl.proto.Element.bytes', index=4,
       number=15, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='inner_map', full_name='flwr.proto.Element.inner_map', index=5,
+      name='inner_map', full_name='daisyfl.proto.Element.inner_map', index=5,
       number=16, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='inner_map_int', full_name='flwr.proto.Element.inner_map_int', index=6,
+      name='inner_map_int', full_name='daisyfl.proto.Element.inner_map_int', index=6,
       number=17, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='inner_list', full_name='flwr.proto.Element.inner_list', index=7,
+      name='inner_list', full_name='daisyfl.proto.Element.inner_list', index=7,
       number=18, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -505,34 +511,34 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
-      name='element', full_name='flwr.proto.Element.element',
+      name='element', full_name='daisyfl.proto.Element.element',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=607,
-  serialized_end=852,
+  serialized_start=631,
+  serialized_end=885,
 )
 
 
 _SERVERMESSAGE_RECONNECTINS = _descriptor.Descriptor(
   name='ReconnectIns',
-  full_name='flwr.proto.ServerMessage.ReconnectIns',
+  full_name='daisyfl.proto.ServerMessage.ReconnectIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='seconds', full_name='flwr.proto.ServerMessage.ReconnectIns.seconds', index=0,
+      name='seconds', full_name='daisyfl.proto.ServerMessage.ReconnectIns.seconds', index=0,
       number=1, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -542,35 +548,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1201,
-  serialized_end=1232,
+  serialized_start=1334,
+  serialized_end=1365,
 )
 
 _SERVERMESSAGE_GETPROPERTIESINS_CONFIGENTRY = _descriptor.Descriptor(
   name='ConfigEntry',
-  full_name='flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry',
+  full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -580,28 +586,28 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1327,
-  serialized_end=1392,
+  serialized_start=1463,
+  serialized_end=1531,
 )
 
 _SERVERMESSAGE_GETPROPERTIESINS = _descriptor.Descriptor(
   name='GetPropertiesIns',
-  full_name='flwr.proto.ServerMessage.GetPropertiesIns',
+  full_name='daisyfl.proto.ServerMessage.GetPropertiesIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ServerMessage.GetPropertiesIns.config', index=0,
+      name='config', full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.config', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -611,35 +617,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1235,
-  serialized_end=1392,
+  serialized_start=1368,
+  serialized_end=1531,
 )
 
 _SERVERMESSAGE_GETPARAMETERSINS_CONFIGENTRY = _descriptor.Descriptor(
   name='ConfigEntry',
-  full_name='flwr.proto.ServerMessage.GetParametersIns.ConfigEntry',
+  full_name='daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.ServerMessage.GetParametersIns.ConfigEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.ServerMessage.GetParametersIns.ConfigEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -649,28 +655,28 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1327,
-  serialized_end=1392,
+  serialized_start=1463,
+  serialized_end=1531,
 )
 
 _SERVERMESSAGE_GETPARAMETERSINS = _descriptor.Descriptor(
   name='GetParametersIns',
-  full_name='flwr.proto.ServerMessage.GetParametersIns',
+  full_name='daisyfl.proto.ServerMessage.GetParametersIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ServerMessage.GetParametersIns.config', index=0,
+      name='config', full_name='daisyfl.proto.ServerMessage.GetParametersIns.config', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -680,35 +686,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1395,
-  serialized_end=1552,
+  serialized_start=1534,
+  serialized_end=1697,
 )
 
 _SERVERMESSAGE_FITINS = _descriptor.Descriptor(
   name='FitIns',
-  full_name='flwr.proto.ServerMessage.FitIns',
+  full_name='daisyfl.proto.ServerMessage.FitIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='parameters', full_name='flwr.proto.ServerMessage.FitIns.parameters', index=0,
+      name='parameters', full_name='daisyfl.proto.ServerMessage.FitIns.parameters', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ServerMessage.FitIns.config', index=1,
+      name='config', full_name='daisyfl.proto.ServerMessage.FitIns.config', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -718,35 +724,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1554,
-  serialized_end=1644,
+  serialized_start=1699,
+  serialized_end=1795,
 )
 
 _SERVERMESSAGE_EVALUATEINS = _descriptor.Descriptor(
   name='EvaluateIns',
-  full_name='flwr.proto.ServerMessage.EvaluateIns',
+  full_name='daisyfl.proto.ServerMessage.EvaluateIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='parameters', full_name='flwr.proto.ServerMessage.EvaluateIns.parameters', index=0,
+      name='parameters', full_name='daisyfl.proto.ServerMessage.EvaluateIns.parameters', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ServerMessage.EvaluateIns.config', index=1,
+      name='config', full_name='daisyfl.proto.ServerMessage.EvaluateIns.config', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -756,93 +762,131 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1646,
-  serialized_end=1741,
+  serialized_start=1797,
+  serialized_end=1898,
+)
+
+_SERVERMESSAGE_SERVERRECEIVEDSIGNAL = _descriptor.Descriptor(
+  name='ServerReceivedSignal',
+  full_name='daisyfl.proto.ServerMessage.ServerReceivedSignal',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ServerMessage.ServerReceivedSignal.status', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1900,
+  serialized_end=1961,
 )
 
 _SERVERMESSAGE = _descriptor.Descriptor(
   name='ServerMessage',
-  full_name='flwr.proto.ServerMessage',
+  full_name='daisyfl.proto.ServerMessage',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='reconnect_ins', full_name='flwr.proto.ServerMessage.reconnect_ins', index=0,
+      name='reconnect_ins', full_name='daisyfl.proto.ServerMessage.reconnect_ins', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='get_properties_ins', full_name='flwr.proto.ServerMessage.get_properties_ins', index=1,
+      name='get_properties_ins', full_name='daisyfl.proto.ServerMessage.get_properties_ins', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='get_parameters_ins', full_name='flwr.proto.ServerMessage.get_parameters_ins', index=2,
+      name='get_parameters_ins', full_name='daisyfl.proto.ServerMessage.get_parameters_ins', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='fit_ins', full_name='flwr.proto.ServerMessage.fit_ins', index=3,
+      name='fit_ins', full_name='daisyfl.proto.ServerMessage.fit_ins', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='evaluate_ins', full_name='flwr.proto.ServerMessage.evaluate_ins', index=4,
+      name='evaluate_ins', full_name='daisyfl.proto.ServerMessage.evaluate_ins', index=4,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='server_received_signal', full_name='daisyfl.proto.ServerMessage.server_received_signal', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_SERVERMESSAGE_RECONNECTINS, _SERVERMESSAGE_GETPROPERTIESINS, _SERVERMESSAGE_GETPARAMETERSINS, _SERVERMESSAGE_FITINS, _SERVERMESSAGE_EVALUATEINS, ],
+  nested_types=[_SERVERMESSAGE_RECONNECTINS, _SERVERMESSAGE_GETPROPERTIESINS, _SERVERMESSAGE_GETPARAMETERSINS, _SERVERMESSAGE_FITINS, _SERVERMESSAGE_EVALUATEINS, _SERVERMESSAGE_SERVERRECEIVEDSIGNAL, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
-      name='msg', full_name='flwr.proto.ServerMessage.msg',
+      name='msg', full_name='daisyfl.proto.ServerMessage.msg',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=855,
-  serialized_end=1748,
+  serialized_start=888,
+  serialized_end=1968,
 )
 
 
 _CLIENTMESSAGE_DISCONNECTRES = _descriptor.Descriptor(
   name='DisconnectRes',
-  full_name='flwr.proto.ClientMessage.DisconnectRes',
+  full_name='daisyfl.proto.ClientMessage.DisconnectRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='reason', full_name='flwr.proto.ClientMessage.DisconnectRes.reason', index=0,
+      name='reason', full_name='daisyfl.proto.ClientMessage.DisconnectRes.reason', index=0,
       number=1, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -852,35 +896,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2099,
-  serialized_end=2150,
+  serialized_start=2487,
+  serialized_end=2541,
 )
 
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
-  full_name='flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry',
+  full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -890,35 +934,35 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2289,
-  serialized_end=2358,
+  serialized_start=2686,
+  serialized_end=2758,
 )
 
 _CLIENTMESSAGE_GETPROPERTIESRES = _descriptor.Descriptor(
   name='GetPropertiesRes',
-  full_name='flwr.proto.ClientMessage.GetPropertiesRes',
+  full_name='daisyfl.proto.ClientMessage.GetPropertiesRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='status', full_name='flwr.proto.ClientMessage.GetPropertiesRes.status', index=0,
+      name='status', full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.status', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='properties', full_name='flwr.proto.ClientMessage.GetPropertiesRes.properties', index=1,
+      name='properties', full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.properties', index=1,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -928,35 +972,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2153,
-  serialized_end=2358,
+  serialized_start=2544,
+  serialized_end=2758,
 )
 
 _CLIENTMESSAGE_GETPARAMETERSRES = _descriptor.Descriptor(
   name='GetParametersRes',
-  full_name='flwr.proto.ClientMessage.GetParametersRes',
+  full_name='daisyfl.proto.ClientMessage.GetParametersRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='status', full_name='flwr.proto.ClientMessage.GetParametersRes.status', index=0,
+      name='status', full_name='daisyfl.proto.ClientMessage.GetParametersRes.status', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='parameters', full_name='flwr.proto.ClientMessage.GetParametersRes.parameters', index=1,
+      name='parameters', full_name='daisyfl.proto.ClientMessage.GetParametersRes.parameters', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -966,42 +1010,42 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2360,
-  serialized_end=2458,
+  serialized_start=2760,
+  serialized_end=2864,
 )
 
 _CLIENTMESSAGE_FITRES = _descriptor.Descriptor(
   name='FitRes',
-  full_name='flwr.proto.ClientMessage.FitRes',
+  full_name='daisyfl.proto.ClientMessage.FitRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='status', full_name='flwr.proto.ClientMessage.FitRes.status', index=0,
+      name='status', full_name='daisyfl.proto.ClientMessage.FitRes.status', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='parameters', full_name='flwr.proto.ClientMessage.FitRes.parameters', index=1,
+      name='parameters', full_name='daisyfl.proto.ClientMessage.FitRes.parameters', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ClientMessage.FitRes.config', index=2,
+      name='config', full_name='daisyfl.proto.ClientMessage.FitRes.config', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -1011,35 +1055,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2460,
-  serialized_end=2586,
+  serialized_start=2867,
+  serialized_end=3002,
 )
 
 _CLIENTMESSAGE_EVALUATERES = _descriptor.Descriptor(
   name='EvaluateRes',
-  full_name='flwr.proto.ClientMessage.EvaluateRes',
+  full_name='daisyfl.proto.ClientMessage.EvaluateRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='status', full_name='flwr.proto.ClientMessage.EvaluateRes.status', index=0,
+      name='status', full_name='daisyfl.proto.ClientMessage.EvaluateRes.status', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ClientMessage.EvaluateRes.config', index=1,
+      name='config', full_name='daisyfl.proto.ClientMessage.EvaluateRes.config', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -1049,80 +1093,156 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2588,
-  serialized_end=2675,
+  serialized_start=3004,
+  serialized_end=3097,
+)
+
+_CLIENTMESSAGE_CLIENTSTATUS = _descriptor.Descriptor(
+  name='ClientStatus',
+  full_name='daisyfl.proto.ClientMessage.ClientStatus',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ClientMessage.ClientStatus.status', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3099,
+  serialized_end=3129,
+)
+
+_CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL = _descriptor.Descriptor(
+  name='ClientReceivedSignal',
+  full_name='daisyfl.proto.ClientMessage.ClientReceivedSignal',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ClientMessage.ClientReceivedSignal.status', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3131,
+  serialized_end=3192,
 )
 
 _CLIENTMESSAGE = _descriptor.Descriptor(
   name='ClientMessage',
-  full_name='flwr.proto.ClientMessage',
+  full_name='daisyfl.proto.ClientMessage',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='disconnect_res', full_name='flwr.proto.ClientMessage.disconnect_res', index=0,
+      name='disconnect_res', full_name='daisyfl.proto.ClientMessage.disconnect_res', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='get_properties_res', full_name='flwr.proto.ClientMessage.get_properties_res', index=1,
+      name='get_properties_res', full_name='daisyfl.proto.ClientMessage.get_properties_res', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='get_parameters_res', full_name='flwr.proto.ClientMessage.get_parameters_res', index=2,
+      name='get_parameters_res', full_name='daisyfl.proto.ClientMessage.get_parameters_res', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='fit_res', full_name='flwr.proto.ClientMessage.fit_res', index=3,
+      name='fit_res', full_name='daisyfl.proto.ClientMessage.fit_res', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='evaluate_res', full_name='flwr.proto.ClientMessage.evaluate_res', index=4,
+      name='evaluate_res', full_name='daisyfl.proto.ClientMessage.evaluate_res', index=4,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='client_status', full_name='daisyfl.proto.ClientMessage.client_status', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='client_received_signal', full_name='daisyfl.proto.ClientMessage.client_received_signal', index=6,
+      number=7, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_CLIENTMESSAGE_DISCONNECTRES, _CLIENTMESSAGE_GETPROPERTIESRES, _CLIENTMESSAGE_GETPARAMETERSRES, _CLIENTMESSAGE_FITRES, _CLIENTMESSAGE_EVALUATERES, ],
+  nested_types=[_CLIENTMESSAGE_DISCONNECTRES, _CLIENTMESSAGE_GETPROPERTIESRES, _CLIENTMESSAGE_GETPARAMETERSRES, _CLIENTMESSAGE_FITRES, _CLIENTMESSAGE_EVALUATERES, _CLIENTMESSAGE_CLIENTSTATUS, _CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
-      name='msg', full_name='flwr.proto.ClientMessage.msg',
+      name='msg', full_name='daisyfl.proto.ClientMessage.msg',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=1751,
-  serialized_end=2682,
+  serialized_start=1971,
+  serialized_end=3199,
 )
 
 _STATUS.fields_by_name['code'].enum_type = _CODE
 _SCALAR.oneofs_by_name['scalar'].fields.append(
   _SCALAR.fields_by_name['double'])
 _SCALAR.fields_by_name['double'].containing_oneof = _SCALAR.oneofs_by_name['scalar']
 _SCALAR.oneofs_by_name['scalar'].fields.append(
@@ -1182,19 +1302,22 @@
 _SERVERMESSAGE_GETPARAMETERSINS.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE_FITINS.fields_by_name['parameters'].message_type = _PARAMETERS
 _SERVERMESSAGE_FITINS.fields_by_name['config'].message_type = _INNERMAP
 _SERVERMESSAGE_FITINS.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE_EVALUATEINS.fields_by_name['parameters'].message_type = _PARAMETERS
 _SERVERMESSAGE_EVALUATEINS.fields_by_name['config'].message_type = _INNERMAP
 _SERVERMESSAGE_EVALUATEINS.containing_type = _SERVERMESSAGE
+_SERVERMESSAGE_SERVERRECEIVEDSIGNAL.fields_by_name['status'].message_type = _STATUS
+_SERVERMESSAGE_SERVERRECEIVEDSIGNAL.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE.fields_by_name['reconnect_ins'].message_type = _SERVERMESSAGE_RECONNECTINS
 _SERVERMESSAGE.fields_by_name['get_properties_ins'].message_type = _SERVERMESSAGE_GETPROPERTIESINS
 _SERVERMESSAGE.fields_by_name['get_parameters_ins'].message_type = _SERVERMESSAGE_GETPARAMETERSINS
 _SERVERMESSAGE.fields_by_name['fit_ins'].message_type = _SERVERMESSAGE_FITINS
 _SERVERMESSAGE.fields_by_name['evaluate_ins'].message_type = _SERVERMESSAGE_EVALUATEINS
+_SERVERMESSAGE.fields_by_name['server_received_signal'].message_type = _SERVERMESSAGE_SERVERRECEIVEDSIGNAL
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['reconnect_ins'])
 _SERVERMESSAGE.fields_by_name['reconnect_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['get_properties_ins'])
 _SERVERMESSAGE.fields_by_name['get_properties_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
@@ -1202,14 +1325,17 @@
 _SERVERMESSAGE.fields_by_name['get_parameters_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['fit_ins'])
 _SERVERMESSAGE.fields_by_name['fit_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['evaluate_ins'])
 _SERVERMESSAGE.fields_by_name['evaluate_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
+_SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
+  _SERVERMESSAGE.fields_by_name['server_received_signal'])
+_SERVERMESSAGE.fields_by_name['server_received_signal'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE_DISCONNECTRES.fields_by_name['reason'].enum_type = _REASON
 _CLIENTMESSAGE_DISCONNECTRES.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY.fields_by_name['value'].message_type = _SCALAR
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY.containing_type = _CLIENTMESSAGE_GETPROPERTIESRES
 _CLIENTMESSAGE_GETPROPERTIESRES.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_GETPROPERTIESRES.fields_by_name['properties'].message_type = _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY
 _CLIENTMESSAGE_GETPROPERTIESRES.containing_type = _CLIENTMESSAGE
@@ -1219,19 +1345,24 @@
 _CLIENTMESSAGE_FITRES.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_FITRES.fields_by_name['parameters'].message_type = _PARAMETERS
 _CLIENTMESSAGE_FITRES.fields_by_name['config'].message_type = _INNERMAP
 _CLIENTMESSAGE_FITRES.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE_EVALUATERES.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_EVALUATERES.fields_by_name['config'].message_type = _INNERMAP
 _CLIENTMESSAGE_EVALUATERES.containing_type = _CLIENTMESSAGE
+_CLIENTMESSAGE_CLIENTSTATUS.containing_type = _CLIENTMESSAGE
+_CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL.fields_by_name['status'].message_type = _STATUS
+_CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE.fields_by_name['disconnect_res'].message_type = _CLIENTMESSAGE_DISCONNECTRES
 _CLIENTMESSAGE.fields_by_name['get_properties_res'].message_type = _CLIENTMESSAGE_GETPROPERTIESRES
 _CLIENTMESSAGE.fields_by_name['get_parameters_res'].message_type = _CLIENTMESSAGE_GETPARAMETERSRES
 _CLIENTMESSAGE.fields_by_name['fit_res'].message_type = _CLIENTMESSAGE_FITRES
 _CLIENTMESSAGE.fields_by_name['evaluate_res'].message_type = _CLIENTMESSAGE_EVALUATERES
+_CLIENTMESSAGE.fields_by_name['client_status'].message_type = _CLIENTMESSAGE_CLIENTSTATUS
+_CLIENTMESSAGE.fields_by_name['client_received_signal'].message_type = _CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['disconnect_res'])
 _CLIENTMESSAGE.fields_by_name['disconnect_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['get_properties_res'])
 _CLIENTMESSAGE.fields_by_name['get_properties_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
@@ -1239,14 +1370,20 @@
 _CLIENTMESSAGE.fields_by_name['get_parameters_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['fit_res'])
 _CLIENTMESSAGE.fields_by_name['fit_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['evaluate_res'])
 _CLIENTMESSAGE.fields_by_name['evaluate_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
+_CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
+  _CLIENTMESSAGE.fields_by_name['client_status'])
+_CLIENTMESSAGE.fields_by_name['client_status'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
+_CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
+  _CLIENTMESSAGE.fields_by_name['client_received_signal'])
+_CLIENTMESSAGE.fields_by_name['client_received_signal'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 DESCRIPTOR.message_types_by_name['Status'] = _STATUS
 DESCRIPTOR.message_types_by_name['Parameters'] = _PARAMETERS
 DESCRIPTOR.message_types_by_name['Scalar'] = _SCALAR
 DESCRIPTOR.message_types_by_name['InnerList'] = _INNERLIST
 DESCRIPTOR.message_types_by_name['InnerMap'] = _INNERMAP
 DESCRIPTOR.message_types_by_name['InnerMapInt'] = _INNERMAPINT
 DESCRIPTOR.message_types_by_name['Element'] = _ELEMENT
@@ -1254,215 +1391,239 @@
 DESCRIPTOR.message_types_by_name['ClientMessage'] = _CLIENTMESSAGE
 DESCRIPTOR.enum_types_by_name['Code'] = _CODE
 DESCRIPTOR.enum_types_by_name['Reason'] = _REASON
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Status = _reflection.GeneratedProtocolMessageType('Status', (_message.Message,), {
   'DESCRIPTOR' : _STATUS,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.Status)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.Status)
   })
 _sym_db.RegisterMessage(Status)
 
 Parameters = _reflection.GeneratedProtocolMessageType('Parameters', (_message.Message,), {
   'DESCRIPTOR' : _PARAMETERS,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.Parameters)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.Parameters)
   })
 _sym_db.RegisterMessage(Parameters)
 
 Scalar = _reflection.GeneratedProtocolMessageType('Scalar', (_message.Message,), {
   'DESCRIPTOR' : _SCALAR,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.Scalar)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.Scalar)
   })
 _sym_db.RegisterMessage(Scalar)
 
 InnerList = _reflection.GeneratedProtocolMessageType('InnerList', (_message.Message,), {
   'DESCRIPTOR' : _INNERLIST,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.InnerList)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerList)
   })
 _sym_db.RegisterMessage(InnerList)
 
 InnerMap = _reflection.GeneratedProtocolMessageType('InnerMap', (_message.Message,), {
 
   'InnerMapEntry' : _reflection.GeneratedProtocolMessageType('InnerMapEntry', (_message.Message,), {
     'DESCRIPTOR' : _INNERMAP_INNERMAPENTRY,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.InnerMap.InnerMapEntry)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerMap.InnerMapEntry)
     })
   ,
   'DESCRIPTOR' : _INNERMAP,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.InnerMap)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerMap)
   })
 _sym_db.RegisterMessage(InnerMap)
 _sym_db.RegisterMessage(InnerMap.InnerMapEntry)
 
 InnerMapInt = _reflection.GeneratedProtocolMessageType('InnerMapInt', (_message.Message,), {
 
   'InnerMapIntEntry' : _reflection.GeneratedProtocolMessageType('InnerMapIntEntry', (_message.Message,), {
     'DESCRIPTOR' : _INNERMAPINT_INNERMAPINTENTRY,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.InnerMapInt.InnerMapIntEntry)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerMapInt.InnerMapIntEntry)
     })
   ,
   'DESCRIPTOR' : _INNERMAPINT,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.InnerMapInt)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerMapInt)
   })
 _sym_db.RegisterMessage(InnerMapInt)
 _sym_db.RegisterMessage(InnerMapInt.InnerMapIntEntry)
 
 Element = _reflection.GeneratedProtocolMessageType('Element', (_message.Message,), {
   'DESCRIPTOR' : _ELEMENT,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.Element)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.Element)
   })
 _sym_db.RegisterMessage(Element)
 
 ServerMessage = _reflection.GeneratedProtocolMessageType('ServerMessage', (_message.Message,), {
 
   'ReconnectIns' : _reflection.GeneratedProtocolMessageType('ReconnectIns', (_message.Message,), {
     'DESCRIPTOR' : _SERVERMESSAGE_RECONNECTINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.ReconnectIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.ReconnectIns)
     })
   ,
 
   'GetPropertiesIns' : _reflection.GeneratedProtocolMessageType('GetPropertiesIns', (_message.Message,), {
 
     'ConfigEntry' : _reflection.GeneratedProtocolMessageType('ConfigEntry', (_message.Message,), {
       'DESCRIPTOR' : _SERVERMESSAGE_GETPROPERTIESINS_CONFIGENTRY,
-      '__module__' : 'flwr.proto.transport_pb2'
-      # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry)
+      '__module__' : 'daisyfl.proto.transport_pb2'
+      # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry)
       })
     ,
     'DESCRIPTOR' : _SERVERMESSAGE_GETPROPERTIESINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.GetPropertiesIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.GetPropertiesIns)
     })
   ,
 
   'GetParametersIns' : _reflection.GeneratedProtocolMessageType('GetParametersIns', (_message.Message,), {
 
     'ConfigEntry' : _reflection.GeneratedProtocolMessageType('ConfigEntry', (_message.Message,), {
       'DESCRIPTOR' : _SERVERMESSAGE_GETPARAMETERSINS_CONFIGENTRY,
-      '__module__' : 'flwr.proto.transport_pb2'
-      # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.GetParametersIns.ConfigEntry)
+      '__module__' : 'daisyfl.proto.transport_pb2'
+      # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry)
       })
     ,
     'DESCRIPTOR' : _SERVERMESSAGE_GETPARAMETERSINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.GetParametersIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.GetParametersIns)
     })
   ,
 
   'FitIns' : _reflection.GeneratedProtocolMessageType('FitIns', (_message.Message,), {
     'DESCRIPTOR' : _SERVERMESSAGE_FITINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.FitIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.FitIns)
     })
   ,
 
   'EvaluateIns' : _reflection.GeneratedProtocolMessageType('EvaluateIns', (_message.Message,), {
     'DESCRIPTOR' : _SERVERMESSAGE_EVALUATEINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.EvaluateIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.EvaluateIns)
+    })
+  ,
+
+  'ServerReceivedSignal' : _reflection.GeneratedProtocolMessageType('ServerReceivedSignal', (_message.Message,), {
+    'DESCRIPTOR' : _SERVERMESSAGE_SERVERRECEIVEDSIGNAL,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.ServerReceivedSignal)
     })
   ,
   'DESCRIPTOR' : _SERVERMESSAGE,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage)
   })
 _sym_db.RegisterMessage(ServerMessage)
 _sym_db.RegisterMessage(ServerMessage.ReconnectIns)
 _sym_db.RegisterMessage(ServerMessage.GetPropertiesIns)
 _sym_db.RegisterMessage(ServerMessage.GetPropertiesIns.ConfigEntry)
 _sym_db.RegisterMessage(ServerMessage.GetParametersIns)
 _sym_db.RegisterMessage(ServerMessage.GetParametersIns.ConfigEntry)
 _sym_db.RegisterMessage(ServerMessage.FitIns)
 _sym_db.RegisterMessage(ServerMessage.EvaluateIns)
+_sym_db.RegisterMessage(ServerMessage.ServerReceivedSignal)
 
 ClientMessage = _reflection.GeneratedProtocolMessageType('ClientMessage', (_message.Message,), {
 
   'DisconnectRes' : _reflection.GeneratedProtocolMessageType('DisconnectRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_DISCONNECTRES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.DisconnectRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.DisconnectRes)
     })
   ,
 
   'GetPropertiesRes' : _reflection.GeneratedProtocolMessageType('GetPropertiesRes', (_message.Message,), {
 
     'PropertiesEntry' : _reflection.GeneratedProtocolMessageType('PropertiesEntry', (_message.Message,), {
       'DESCRIPTOR' : _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY,
-      '__module__' : 'flwr.proto.transport_pb2'
-      # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry)
+      '__module__' : 'daisyfl.proto.transport_pb2'
+      # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry)
       })
     ,
     'DESCRIPTOR' : _CLIENTMESSAGE_GETPROPERTIESRES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.GetPropertiesRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.GetPropertiesRes)
     })
   ,
 
   'GetParametersRes' : _reflection.GeneratedProtocolMessageType('GetParametersRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_GETPARAMETERSRES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.GetParametersRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.GetParametersRes)
     })
   ,
 
   'FitRes' : _reflection.GeneratedProtocolMessageType('FitRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_FITRES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.FitRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.FitRes)
     })
   ,
 
   'EvaluateRes' : _reflection.GeneratedProtocolMessageType('EvaluateRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_EVALUATERES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.EvaluateRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.EvaluateRes)
+    })
+  ,
+
+  'ClientStatus' : _reflection.GeneratedProtocolMessageType('ClientStatus', (_message.Message,), {
+    'DESCRIPTOR' : _CLIENTMESSAGE_CLIENTSTATUS,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.ClientStatus)
+    })
+  ,
+
+  'ClientReceivedSignal' : _reflection.GeneratedProtocolMessageType('ClientReceivedSignal', (_message.Message,), {
+    'DESCRIPTOR' : _CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.ClientReceivedSignal)
     })
   ,
   'DESCRIPTOR' : _CLIENTMESSAGE,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage)
   })
 _sym_db.RegisterMessage(ClientMessage)
 _sym_db.RegisterMessage(ClientMessage.DisconnectRes)
 _sym_db.RegisterMessage(ClientMessage.GetPropertiesRes)
 _sym_db.RegisterMessage(ClientMessage.GetPropertiesRes.PropertiesEntry)
 _sym_db.RegisterMessage(ClientMessage.GetParametersRes)
 _sym_db.RegisterMessage(ClientMessage.FitRes)
 _sym_db.RegisterMessage(ClientMessage.EvaluateRes)
+_sym_db.RegisterMessage(ClientMessage.ClientStatus)
+_sym_db.RegisterMessage(ClientMessage.ClientReceivedSignal)
 
 
 _INNERMAP_INNERMAPENTRY._options = None
 _INNERMAPINT_INNERMAPINTENTRY._options = None
 _SERVERMESSAGE_GETPROPERTIESINS_CONFIGENTRY._options = None
 _SERVERMESSAGE_GETPARAMETERSINS_CONFIGENTRY._options = None
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY._options = None
 
 _FLOWERSERVICE = _descriptor.ServiceDescriptor(
   name='FlowerService',
-  full_name='flwr.proto.FlowerService',
+  full_name='daisyfl.proto.FlowerService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=2921,
-  serialized_end=3004,
+  serialized_start=3456,
+  serialized_end=3545,
   methods=[
   _descriptor.MethodDescriptor(
     name='Join',
-    full_name='flwr.proto.FlowerService.Join',
+    full_name='daisyfl.proto.FlowerService.Join',
     index=0,
     containing_service=None,
     input_type=_CLIENTMESSAGE,
     output_type=_SERVERMESSAGE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/proto/transport_pb2.pyi` & `daisyfl-0.4.1/src/py/daisyfl/proto/transport_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 class _CodeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Code.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     OK: _Code.ValueType  # 0
     GET_PROPERTIES_NOT_IMPLEMENTED: _Code.ValueType  # 1
     GET_PARAMETERS_NOT_IMPLEMENTED: _Code.ValueType  # 2
     FIT_NOT_IMPLEMENTED: _Code.ValueType  # 3
     EVALUATE_NOT_IMPLEMENTED: _Code.ValueType  # 4
+    MESSAGE_LOST: _Code.ValueType  # 5
 class Code(_Code, metaclass=_CodeEnumTypeWrapper):
     pass
 
 OK: Code.ValueType  # 0
 GET_PROPERTIES_NOT_IMPLEMENTED: Code.ValueType  # 1
 GET_PARAMETERS_NOT_IMPLEMENTED: Code.ValueType  # 2
 FIT_NOT_IMPLEMENTED: Code.ValueType  # 3
 EVALUATE_NOT_IMPLEMENTED: Code.ValueType  # 4
+MESSAGE_LOST: Code.ValueType  # 5
 global___Code = Code
 
 
 class _Reason:
     ValueType = typing.NewType('ValueType', builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 class _ReasonEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Reason.ValueType], builtins.type):
@@ -331,40 +333,56 @@
             *,
             parameters: typing.Optional[global___Parameters] = ...,
             config: typing.Optional[global___InnerMap] = ...,
             ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["config",b"config","parameters",b"parameters"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["config",b"config","parameters",b"parameters"]) -> None: ...
 
+    class ServerReceivedSignal(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        @property
+        def status(self) -> global___Status: ...
+        def __init__(self,
+            *,
+            status: typing.Optional[global___Status] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["status",b"status"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
     RECONNECT_INS_FIELD_NUMBER: builtins.int
     GET_PROPERTIES_INS_FIELD_NUMBER: builtins.int
     GET_PARAMETERS_INS_FIELD_NUMBER: builtins.int
     FIT_INS_FIELD_NUMBER: builtins.int
     EVALUATE_INS_FIELD_NUMBER: builtins.int
+    SERVER_RECEIVED_SIGNAL_FIELD_NUMBER: builtins.int
     @property
     def reconnect_ins(self) -> global___ServerMessage.ReconnectIns: ...
     @property
     def get_properties_ins(self) -> global___ServerMessage.GetPropertiesIns: ...
     @property
     def get_parameters_ins(self) -> global___ServerMessage.GetParametersIns: ...
     @property
     def fit_ins(self) -> global___ServerMessage.FitIns: ...
     @property
     def evaluate_ins(self) -> global___ServerMessage.EvaluateIns: ...
+    @property
+    def server_received_signal(self) -> global___ServerMessage.ServerReceivedSignal: ...
     def __init__(self,
         *,
         reconnect_ins: typing.Optional[global___ServerMessage.ReconnectIns] = ...,
         get_properties_ins: typing.Optional[global___ServerMessage.GetPropertiesIns] = ...,
         get_parameters_ins: typing.Optional[global___ServerMessage.GetParametersIns] = ...,
         fit_ins: typing.Optional[global___ServerMessage.FitIns] = ...,
         evaluate_ins: typing.Optional[global___ServerMessage.EvaluateIns] = ...,
+        server_received_signal: typing.Optional[global___ServerMessage.ServerReceivedSignal] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["reconnect_ins","get_properties_ins","get_parameters_ins","fit_ins","evaluate_ins"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins","server_received_signal",b"server_received_signal"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins","server_received_signal",b"server_received_signal"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["reconnect_ins","get_properties_ins","get_parameters_ins","fit_ins","evaluate_ins","server_received_signal"]]: ...
 global___ServerMessage = ServerMessage
 
 class ClientMessage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     class DisconnectRes(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
         REASON_FIELD_NUMBER: builtins.int
@@ -454,34 +472,64 @@
             *,
             status: typing.Optional[global___Status] = ...,
             config: typing.Optional[global___InnerMap] = ...,
             ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["config",b"config","status",b"status"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["config",b"config","status",b"status"]) -> None: ...
 
+    class ClientStatus(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        status: typing.Text
+        def __init__(self,
+            *,
+            status: typing.Text = ...,
+            ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
+    class ClientReceivedSignal(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        @property
+        def status(self) -> global___Status: ...
+        def __init__(self,
+            *,
+            status: typing.Optional[global___Status] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["status",b"status"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
     DISCONNECT_RES_FIELD_NUMBER: builtins.int
     GET_PROPERTIES_RES_FIELD_NUMBER: builtins.int
     GET_PARAMETERS_RES_FIELD_NUMBER: builtins.int
     FIT_RES_FIELD_NUMBER: builtins.int
     EVALUATE_RES_FIELD_NUMBER: builtins.int
+    CLIENT_STATUS_FIELD_NUMBER: builtins.int
+    CLIENT_RECEIVED_SIGNAL_FIELD_NUMBER: builtins.int
     @property
     def disconnect_res(self) -> global___ClientMessage.DisconnectRes: ...
     @property
     def get_properties_res(self) -> global___ClientMessage.GetPropertiesRes: ...
     @property
     def get_parameters_res(self) -> global___ClientMessage.GetParametersRes: ...
     @property
     def fit_res(self) -> global___ClientMessage.FitRes: ...
     @property
     def evaluate_res(self) -> global___ClientMessage.EvaluateRes: ...
+    @property
+    def client_status(self) -> global___ClientMessage.ClientStatus: ...
+    @property
+    def client_received_signal(self) -> global___ClientMessage.ClientReceivedSignal: ...
     def __init__(self,
         *,
         disconnect_res: typing.Optional[global___ClientMessage.DisconnectRes] = ...,
         get_properties_res: typing.Optional[global___ClientMessage.GetPropertiesRes] = ...,
         get_parameters_res: typing.Optional[global___ClientMessage.GetParametersRes] = ...,
         fit_res: typing.Optional[global___ClientMessage.FitRes] = ...,
         evaluate_res: typing.Optional[global___ClientMessage.EvaluateRes] = ...,
+        client_status: typing.Optional[global___ClientMessage.ClientStatus] = ...,
+        client_received_signal: typing.Optional[global___ClientMessage.ClientReceivedSignal] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["disconnect_res","get_properties_res","get_parameters_res","fit_res","evaluate_res"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["client_received_signal",b"client_received_signal","client_status",b"client_status","disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_received_signal",b"client_received_signal","client_status",b"client_status","disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["disconnect_res","get_properties_res","get_parameters_res","fit_res","evaluate_res","client_status","client_received_signal"]]: ...
 global___ClientMessage = ClientMessage
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/proto/transport_pb2_grpc.py` & `daisyfl-0.4.1/src/py/daisyfl/proto/transport_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from daisyfl.proto import transport_pb2 as flwr_dot_proto_dot_transport__pb2
+from daisyfl.proto import transport_pb2 as daisyfl_dot_proto_dot_transport__pb2
 
 
 class FlowerServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Join = channel.stream_stream(
-                '/flwr.proto.FlowerService/Join',
-                request_serializer=flwr_dot_proto_dot_transport__pb2.ClientMessage.SerializeToString,
-                response_deserializer=flwr_dot_proto_dot_transport__pb2.ServerMessage.FromString,
+                '/daisyfl.proto.FlowerService/Join',
+                request_serializer=daisyfl_dot_proto_dot_transport__pb2.ClientMessage.SerializeToString,
+                response_deserializer=daisyfl_dot_proto_dot_transport__pb2.ServerMessage.FromString,
                 )
 
 
 class FlowerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Join(self, request_iterator, context):
@@ -31,20 +31,20 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_FlowerServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Join': grpc.stream_stream_rpc_method_handler(
                     servicer.Join,
-                    request_deserializer=flwr_dot_proto_dot_transport__pb2.ClientMessage.FromString,
-                    response_serializer=flwr_dot_proto_dot_transport__pb2.ServerMessage.SerializeToString,
+                    request_deserializer=daisyfl_dot_proto_dot_transport__pb2.ClientMessage.FromString,
+                    response_serializer=daisyfl_dot_proto_dot_transport__pb2.ServerMessage.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'flwr.proto.FlowerService', rpc_method_handlers)
+            'daisyfl.proto.FlowerService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class FlowerService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -55,12 +55,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/flwr.proto.FlowerService/Join',
-            flwr_dot_proto_dot_transport__pb2.ClientMessage.SerializeToString,
-            flwr_dot_proto_dot_transport__pb2.ServerMessage.FromString,
+        return grpc.experimental.stream_stream(request_iterator, target, '/daisyfl.proto.FlowerService/Join',
+            daisyfl_dot_proto_dot_transport__pb2.ClientMessage.SerializeToString,
+            daisyfl_dot_proto_dot_transport__pb2.ServerMessage.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/proto/transport_pb2_grpc.pyi` & `daisyfl-0.4.1/src/py/daisyfl/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/app.py` & `daisyfl-0.4.1/src/py/daisyfl/server/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,20 +28,22 @@
     generic_create_grpc_server,
     start_grpc_server,
 )
 from daisyfl.server.history import History
 from daisyfl.server.server import Server
 from daisyfl.server.server_operator_manager import ServerOperatorManager
 from daisyfl.server.task_manager import TaskManager
-from daisyfl.server.server_api_handler import listening
+from daisyfl.server.server_api_handler import ServerListener
+from daisyfl.client.zone_client import ZoneClient
 
 import threading
 import time
 
 DEFAULT_SERVER_ADDRESS = "[::]:8887"
+_cnd_stop: threading.Condition = threading.Condition()
 
 def start_server(  # pylint: disable=too-many-arguments
     *,
     # task manager
     zone: bool = False,
     parent_address: str = "",
     # server
@@ -50,19 +52,17 @@
     api_ip: str = None,
     api_port: int = None,
     # grpc
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     certificates: Optional[Tuple[bytes, bytes, bytes]] = None,
 ) -> None:
     # Initialize server and task manager
-    initialized_server, initialized_task_manager = _init_defaults(
-        # task manager
+    initialized_server: Server = _init_defaults(
         zone=zone,
         parent_address=parent_address,
-        # api_handler
         api_ip=api_ip,
         api_port=api_port,
     )
     log(INFO, "Starting Flower server",)
 
     # Start gRPC server
     grpc_server = start_grpc_server(
@@ -73,64 +73,76 @@
     )
     log(
         INFO,
         "Flower ECE: gRPC server running , SSL is %s",
         "enabled" if certificates is not None else "disabled",
     )
 
-    # Wait until shutdown    
-    with initialized_task_manager._cnd_stop:
-        initialized_task_manager._cnd_stop.wait()
-    initialized_server.disconnect_all_clients(timeout=None)
+    # Wait until shutdown
+    with _cnd_stop:
+        _cnd_stop.wait()
     # Stop the gRPC server
     grpc_server.stop(grace=1)
+    initialized_server.get_client_manager().unregister_all()
     log(INFO, "Daisy server shutdown")
     exit(0)
 
 
 def _init_defaults(
-    # task manager
     zone: bool,
     parent_address: Optional[str],
-    # api_handler
     api_ip: str = None,
     api_port: int = None,
 ) -> Tuple[Server, TaskManager]:
     # client_manager
     client_manager = SimpleClientManager()       
     # server
     server = Server(client_manager=client_manager)
     # server_operator_manager
     server_operator_manager = ServerOperatorManager(server=server)
-    # task_manager
-    ## zone or master
+    # zone or master
     manager_type = Type.ZONE if zone else Type.MASTER
+    # task_manager
     task_manager = TaskManager(
         server_operator_manager=server_operator_manager,
         manager_type=manager_type,
-        parent_address=parent_address,
     )
-    # api_handler
-    start_api_handler(api_ip=api_ip, api_port=api_port, task_manager=task_manager)
+    # for master: start ServerListener
+    if manager_type == Type.MASTER:
+        start_server_listener(api_ip=api_ip, api_port=api_port, task_manager=task_manager)
+    # for zone: start ZoneClient
+    elif manager_type == Type.ZONE:
+        start_zone_client(parent_address, api_ip, api_port, task_manager)
+    else:
+        log(ERROR, "Use undefined node type.")
+        exit(1)
     
-    return server, task_manager
+    return server
 
-# api_handler
-def start_api_handler(api_ip: str, api_port: int, task_manager: TaskManager) -> bool:
+# server_listener
+def start_server_listener(api_ip: str, api_port: int, task_manager: TaskManager) -> bool:
     if isinstance(api_ip, str) and isinstance(api_port, int):
-        listener = threading.Thread(target=listening, args=(api_ip, api_port, task_manager))
-        listener.setDaemon(True)
-        listener.start()
+        listener = ServerListener(api_ip, api_port, task_manager, _cnd_stop)
+        listener_thread = threading.Thread(target=listener.run, args=())
+        listener_thread.setDaemon(True)
+        listener_thread.start()
         time.sleep(1)
-        if not listener.is_alive():
-            log(
-                ERROR,
-                "client_api_handler failed",
-            )
+        if not listener_thread.is_alive():
+            log(ERROR, "ServerListner failed")
             exit(1)
     else:
         log(
             ERROR,
             "Please check api_ip is string and api_port is integer.",
         )
         exit(1)
     return True
+
+# zone_client
+def start_zone_client(parent_address: str,  api_ip: str, api_port: int, task_manager: TaskManager):
+    zc = threading.Thread(target=ZoneClient, args=(parent_address, api_ip, api_port, task_manager, _cnd_stop))
+    zc.setDaemon(True)
+    zc.start()
+    threading.Event().wait(timeout=1)
+    if not zc.is_alive():
+        log(ERROR, "ZoneClient failed")
+        exit(1)
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/client_manager.py` & `daisyfl-0.4.1/src/py/daisyfl/server/client_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 """Flower ClientManager."""
 
 
 import random
 import threading
 from abc import ABC, abstractmethod
 from logging import INFO
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Callable
 
 from daisyfl.common.logger import log
-from daisyfl.common import CREDENTIAL, NO_CREDENTIAL, ZONE_CREDENTIAL
+from daisyfl.common import CREDENTIAL, IS_ZONE
 
 from .client_proxy import ClientProxy
 
 
 class ClientManager(ABC):
     """Abstract base class for managing Flower clients."""
 
@@ -43,140 +43,166 @@
         """
 
     @abstractmethod
     def unregister(self, client: ClientProxy) -> None:
         """Unregister Flower ClientProxy instance."""
 
     @abstractmethod
+    def unregister_all(self,) -> None:
+        """Unregister all Flower ClientProxy instances."""
+    
+    @abstractmethod
     def all(self) -> Dict[str, ClientProxy]:
         """Return all available clients."""
 
     @abstractmethod
     def wait_for(self, num_clients: int, timeout: int) -> bool:
         """Wait until at least `num_clients` are available."""
 
     @abstractmethod
     def get_available_clients(
         self,
         min_num_clients: int = 2,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: Optional[str] = None,
     ) -> List[ClientProxy]:
         """get all available Daisy ClientProxy instances."""
 
+    @abstractmethod
+    def set_submit_subtask_fn(self, submit_subtask: Callable) -> None:
+        """
+        Server set this callback function.
+        ClientProxy call this callback function to submit a result.
+        """
+
+    
+
 
 class SimpleClientManager(ClientManager):
     """Provides a pool of available clients."""
 
     def __init__(self) -> None:
-        self.clients: Dict[str, Dict[str, ClientProxy]] = {
-            NO_CREDENTIAL: {},
-            ZONE_CREDENTIAL: {},
-        }
+        self.zones: Dict[str, ClientProxy] = {}
+        self.clients: Dict[str, Dict[str, ClientProxy]] = {}
         self._cv = threading.Condition()
+        self.submit_subtask: Callable = None
 
     def __len__(self,) -> int:
-        return len(self.clients)
+        count = 0
+        for key in self.clients.keys():
+            count = count + len(self.clients[key])
+        count = count + len(self.zones)
+        return count
 
-    def wait_for(self, num_clients: int, credential: str = NO_CREDENTIAL, strict: bool = True, timeout: int = 86400) -> bool:
+    def wait_for(self, num_clients: int, credential: Optional[str], timeout: int = 86400) -> bool:
         """Block until at least `num_clients` are available or until a timeout
         is reached.
 
         Current timeout default: 1 day.
         """
-        if credential not in self.clients:
-            self.clients[credential] = {}
-
         with self._cv:
             return self._cv.wait_for(
-                lambda: self.num_available(credential, strict) >= num_clients, timeout=timeout
+                lambda: self.num_available(credential) >= num_clients, timeout=timeout
             )
 
-    def num_available(self, credential, strict=True,) -> int:
+    def num_available(self, credential: Optional[str]) -> int:
         """Return the number of available clients."""
-        if credential not in self.clients:
+        if credential is None:
+            return len(self.zones.values())
+        
+        if not self.clients.__contains__(credential):
             self.clients[credential] = {}
 
-        nums = len(self.clients[credential])
-        if credential != ZONE_CREDENTIAL:
-            nums = nums + len(self.clients[ZONE_CREDENTIAL])
-        if (not strict) and (credential != NO_CREDENTIAL):
-            nums = nums + len(self.clients[NO_CREDENTIAL])
-
+        nums = 0
+        for client in self.clients[credential].values():
+            if client.bridge.client_available():
+                nums = nums + 1
+        for client in self.zones.values():
+            if client.bridge.client_available():
+                nums = nums + 1
         return nums
 
-    def register(self, client: ClientProxy) -> bool:
+    def register(self, client: ClientProxy, is_zone: bool) -> bool:
         """Register Flower ClientProxy instance.
 
         Returns:
             bool: Indicating if registration was successful. False if ClientProxy is
                 already registered or can not be registered for any reason
         """
-        if client.cid in self.clients:
+        # check cid
+        for credential_key in self.clients:
+            if client.cid in self.clients[credential_key].keys():
+                return False
+        if client.cid in self.zones.keys():
             return False
-        if hasattr(client, "metadata_dict"):
-            metadata_dict = getattr(client, "metadata_dict")
-            if ZONE_CREDENTIAL in metadata_dict:
-                self.clients[ZONE_CREDENTIAL][client.cid] = client
-            elif CREDENTIAL in metadata_dict:
-                credential = metadata_dict[CREDENTIAL]
-                if credential not in self.clients:
-                    self.clients[credential] = {}
-                self.clients[credential][client.cid] = client
-            else:
-                self.clients[NO_CREDENTIAL][client.cid] = client
+        client.set_submit_subtask_fn(self.submit_subtask)
+        # register a zone
+        if is_zone:
+            self.zones[client.cid] = client
         else:
-            self.clients[NO_CREDENTIAL][client.cid] = client
+            credential = client.metadata_dict[CREDENTIAL]
+            if not self.clients.__contains__(credential):
+                self.clients[credential] = {}
+            self.clients[credential][client.cid] = client
         
         with self._cv:
             self._cv.notify_all()
 
         return True
 
     def unregister(self, client: ClientProxy) -> None:
         """Unregister Flower ClientProxy instance.
 
         This method is idempotent.
         """
-        if hasattr(client, "metadata_dict"):
-            metadata_dict = getattr(client, "metadata_dict")
-            if ZONE_CREDENTIAL in metadata_dict:
-                credential = ZONE_CREDENTIAL
-            elif CREDENTIAL in metadata_dict:
-                credential = metadata_dict[CREDENTIAL]
-            else:
-                credential = NO_CREDENTIAL
-        else:
-            credential = NO_CREDENTIAL
-        
-        if credential in self.clients:
-            if client.cid in self.clients[credential]:
-                del self.clients[credential][client.cid]
-                with self._cv:
-                    self._cv.notify_all()
+        if self.zones.__contains__(client.cid):
+            del self.zones[client.cid]
+        for credential_key in self.clients.keys():
+            if self.clients[credential_key].__contains__(client.cid):
+                del self.clients[credential_key][client.cid]
+
+        with self._cv:
+            self._cv.notify_all()
+
+    def unregister_all(self,) -> None:
+        clients = self.all()
+        for client in clients:
+            client.bridge.close()
+            self.unregister(client)
 
-    def all(self) -> Dict[str, Dict[str, ClientProxy]]:
+    def all(self) -> List[ClientProxy]:
         """Return all available clients."""
-        return self.clients
+        def get_values(d):
+            values = []
+            for v in d.values():
+                if isinstance(v, dict):
+                    values.extend(get_values(v))
+                else:
+                    values.append(v)
+            return values
+        
+        client_list = get_values(self.clients)
+        client_list = client_list + list(self.zones.values())
+        return client_list
 
     def get_available_clients(
         self,
         min_num_clients: int = 2,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: Optional[str] = None,
     ) -> List[ClientProxy]:
         """get all available Daisy ClientProxy instances."""
         # Block until at least num_clients are connected.
-        self.wait_for(min_num_clients, credential, strict)
-        available_cids = list(self.clients[credential])
-        available_cids_zone_credential = list(self.clients[ZONE_CREDENTIAL])
-        available_cids_no_credential = list(self.clients[NO_CREDENTIAL]) \
-            if (credential == NO_CREDENTIAL) or strict else []
-        
-        clients = [self.clients[credential][cid] for cid in available_cids]
-        clients_zone_credential = [self.clients[ZONE_CREDENTIAL][cid] for cid in available_cids_zone_credential]
-        clients_no_credential = [self.clients[NO_CREDENTIAL][cid] for cid in available_cids_no_credential]
-        clients = clients + clients_zone_credential + clients_no_credential
-        return clients
+        self.wait_for(min_num_clients, credential)
 
-# TODO: 多個Task共用Clients如何確保Client availability
-# TODO: 多個Task共用Clients如何確定選中Clients (其他Task不能來搶)
+        if credential is None:
+            return list(self.zones.values())
+        
+        client_list = []
+        for client in self.clients[credential].values():
+            if client.bridge.client_available():
+                client_list.append(client)
+        for client in self.zones.values():
+            if client.bridge.client_available():
+                client_list.append(client)
+        return client_list
+    
+    def set_submit_subtask_fn(self, submit_subtask: Callable) -> None:
+        self.submit_subtask = submit_subtask
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/client_proxy.py` & `daisyfl-0.4.1/src/py/daisyfl/server/client_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,70 +12,77 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client (abstract base class)."""
 
 
 from abc import ABC, abstractmethod
-from typing import Optional
+from typing import Optional, Union, Callable
 
 from daisyfl.common import (
     DisconnectRes,
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
     GetParametersIns,
     GetParametersRes,
     GetPropertiesIns,
     GetPropertiesRes,
     Properties,
     ReconnectIns,
 )
+from daisyfl.proto.transport_pb2 import ClientMessage
 
 
 class ClientProxy(ABC):
     """Abstract base class for Flower client proxies."""
 
     def __init__(self, cid: str):
         self.cid = cid
         self.properties: Properties = {}
 
     @abstractmethod
     def get_properties(
         self,
         ins: GetPropertiesIns,
-        timeout: Optional[float],
-    ) -> GetPropertiesRes:
+    ) -> None:
         """Returns the client's properties."""
 
     @abstractmethod
     def get_parameters(
         self,
         ins: GetParametersIns,
-        timeout: Optional[float],
-    ) -> GetParametersRes:
+    ) -> None:
         """Return the current local model parameters."""
 
     @abstractmethod
     def fit(
         self,
         ins: FitIns,
-        timeout: Optional[float],
-    ) -> FitRes:
+    ) -> None:
         """Refine the provided parameters using the locally held dataset."""
 
     @abstractmethod
     def evaluate(
         self,
         ins: EvaluateIns,
-        timeout: Optional[float],
-    ) -> EvaluateRes:
+    ) -> None:
         """Evaluate the provided parameters using the locally held dataset."""
 
     @abstractmethod
     def reconnect(
         self,
         ins: ReconnectIns,
-        timeout: Optional[float],
-    ) -> DisconnectRes:
+    ) -> None:
         """Disconnect and (optionally) reconnect later."""
+    
+    @abstractmethod
+    def submit_client_message(
+        self,
+        client_message: ClientMessage,
+    ) -> None:
+        """Receive, deserialize, and submit"""
+
+    @abstractmethod
+    def set_submit_subtask_fn(self, submit_subtask: Callable) -> None:
+        """Set callback function"""
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/server/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/grpc_bridge.py` & `daisyfl-0.4.1/src/py/daisyfl/server/grpc_server/grpc_bridge.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,64 +13,50 @@
 # limitations under the License.
 # ==============================================================================
 """Provides class GRPCBridge."""
 
 from dataclasses import dataclass
 from enum import Enum
 from threading import Condition
-from typing import Iterator, Optional
+from typing import Iterator, Optional, Tuple, Callable
 
 from daisyfl.proto.transport_pb2 import ClientMessage, ServerMessage
 
 
-@dataclass
-class InsWrapper:
-    """Instruction wrapper class for a single server message."""
-
-    server_message: ServerMessage
-    timeout: Optional[float]
-
-
-@dataclass
-class ResWrapper:
-    """Result wrapper class for a single client message."""
-
-    client_message: ClientMessage
-
-
 class GRPCBridgeClosed(Exception):
     """Error signaling that GRPCBridge is closed."""
 
 
 class Status(Enum):
     """Status through which the bridge can transition."""
 
-    AWAITING_INS_WRAPPER = 1
-    INS_WRAPPER_AVAILABLE = 2
-    AWAITING_RES_WRAPPER = 3
-    RES_WRAPPER_AVAILABLE = 4
+    AWAITING_SERVER_MESSAGE = 1
+    SERVER_MESSAGE_AVAILABLE = 2
+    AWAITING_CLIENT_MESSAGE = 3
+    CLIENT_MESSAGE_AVAILABLE = 4
     CLOSED = 5
 
 
 class GRPCBridge:
-    """GRPCBridge holding res_wrapper and ins_wrapper.
+    """GRPCBridge holding ServerMessage and ClientMessage.
 
     For understanding this class it is recommended to understand how
     the threading.Condition class works. See here:
     - https://docs.python.org/3/library/threading.html#condition-objects
     """
 
-    def __init__(self) -> None:
+    def __init__(self, client_idling: bool = True) -> None:
         """Init bridge."""
         # Disable all unsubscriptable-object violations in __init__ method
         # pylint: disable=unsubscriptable-object
         self._cv = Condition()  # cv stands for condition variable
-        self._status = Status.AWAITING_INS_WRAPPER
-        self._ins_wrapper: Optional[InsWrapper] = None
-        self._res_wrapper: Optional[ResWrapper] = None
+        self._status = Status.AWAITING_SERVER_MESSAGE if client_idling else Status.AWAITING_CLIENT_MESSAGE
+        self._server_message: Optional[ServerMessage] = None
+        self._client_message: Optional[ClientMessage] = None
+        self.submit_client_message = None
 
     def _is_closed(self) -> bool:
         """Return True if closed and False otherwise."""
         return self._status == Status.CLOSED
 
     def _raise_if_closed(self) -> None:
         if self._status == Status.CLOSED:
@@ -81,106 +67,115 @@
 
         The caller of the transition method will have to aquire
         conditional variable.
         """
         if next_status == Status.CLOSED:
             self._status = next_status
         elif (
-            self._status == Status.AWAITING_INS_WRAPPER
-            and next_status == Status.INS_WRAPPER_AVAILABLE
-            and self._ins_wrapper is not None
-            and self._res_wrapper is None
+            self._status == Status.AWAITING_SERVER_MESSAGE
+            and next_status == Status.SERVER_MESSAGE_AVAILABLE
+            and self._server_message is not None
+            and self._client_message is None
         ):
             self._status = next_status
         elif (
-            self._status == Status.INS_WRAPPER_AVAILABLE
-            and next_status == Status.AWAITING_RES_WRAPPER
-            and self._ins_wrapper is None
-            and self._res_wrapper is None
+            self._status == Status.SERVER_MESSAGE_AVAILABLE
+            and next_status == Status.AWAITING_CLIENT_MESSAGE
+            and self._server_message is None
+            and self._client_message is None
         ):
             self._status = next_status
         elif (
-            self._status == Status.AWAITING_RES_WRAPPER
-            and next_status == Status.RES_WRAPPER_AVAILABLE
-            and self._ins_wrapper is None
-            and self._res_wrapper is not None
+            self._status == Status.AWAITING_CLIENT_MESSAGE
+            and next_status == Status.CLIENT_MESSAGE_AVAILABLE
+            and self._server_message is None
+            and self._client_message is not None
         ):
             self._status = next_status
         elif (
-            self._status == Status.RES_WRAPPER_AVAILABLE
-            and next_status == Status.AWAITING_INS_WRAPPER
-            and self._ins_wrapper is None
-            and self._res_wrapper is None
+            self._status == Status.CLIENT_MESSAGE_AVAILABLE
+            and next_status == Status.AWAITING_SERVER_MESSAGE
+            and self._server_message is None
+            and self._client_message is None
         ):
             self._status = next_status
         else:
             raise Exception(f"Invalid transition: {self._status} to {next_status}")
 
         self._cv.notify_all()
 
     def close(self) -> None:
         """Set bridge status to closed."""
         with self._cv:
             self._transition(Status.CLOSED)
 
-    def request(self, ins_wrapper: InsWrapper) -> ResWrapper:
-        """Set ins_wrapper and wait for res_wrapper."""
-        # Set ins_wrapper and transition to INS_WRAPPER_AVAILABLE
+    def request(self, server_message: ServerMessage) -> None:
+        """Set server_message."""
+        # Set ServerMessage and transition to SERVER_MESSAGE_AVAILABLE
         with self._cv:
             self._raise_if_closed()
 
-            if self._status != Status.AWAITING_INS_WRAPPER:
+            if self._status != Status.AWAITING_SERVER_MESSAGE:
                 raise Exception("This should not happen")
 
-            self._ins_wrapper = ins_wrapper  # Write
-            self._transition(Status.INS_WRAPPER_AVAILABLE)
+            self._server_message = server_message  # Write
+            self._transition(Status.SERVER_MESSAGE_AVAILABLE)
+            return
 
-        # Read res_wrapper and transition to AWAITING_INS_WRAPPER
-        with self._cv:
-            self._cv.wait_for(
-                lambda: self._status in [Status.CLOSED, Status.RES_WRAPPER_AVAILABLE]
-            )
-
-            self._raise_if_closed()
-            res_wrapper = self._res_wrapper  # Read
-            self._res_wrapper = None  # Reset
-            self._transition(Status.AWAITING_INS_WRAPPER)
-
-        if res_wrapper is None:
-            raise Exception("ResWrapper can not be None")
-
-        return res_wrapper
-
-    def ins_wrapper_iterator(self) -> Iterator[InsWrapper]:
-        """Return iterator over ins_wrapper objects."""
+    def server_message_iterator(self) -> Iterator[ServerMessage]:
+        """Return iterator over server_message objects."""
         while not self._is_closed():
             with self._cv:
                 self._cv.wait_for(
                     lambda: self._status
-                    in [Status.CLOSED, Status.INS_WRAPPER_AVAILABLE]
+                    in [Status.CLOSED, Status.SERVER_MESSAGE_AVAILABLE]
                 )
 
                 self._raise_if_closed()
 
-                ins_wrapper = self._ins_wrapper  # Read
-                self._ins_wrapper = None  # Reset
+                server_message = self._server_message  # Read
+                self._server_message = None  # Reset
 
                 # Transition before yielding as after the yield the execution of this
                 # function is paused and will resume when next is called again.
                 # Also release condition variable by exiting the context
-                self._transition(Status.AWAITING_RES_WRAPPER)
+                self._transition(Status.AWAITING_CLIENT_MESSAGE)
 
-            if ins_wrapper is None:
-                raise Exception("InsWrapper can not be None")
+            if server_message is None:
+                raise Exception("server_message can not be None")
 
-            yield ins_wrapper
+            yield server_message
 
-    def set_res_wrapper(self, res_wrapper: ResWrapper) -> None:
-        """Set res_wrapper for consumption."""
+    def set_client_message(self, client_message: ClientMessage) -> None:
+        """Set client_message for consumption."""
         with self._cv:
             self._raise_if_closed()
 
-            if self._status != Status.AWAITING_RES_WRAPPER:
+            if self._status != Status.AWAITING_CLIENT_MESSAGE:
                 raise Exception("This should not happen")
 
-            self._res_wrapper = res_wrapper  # Write
-            self._transition(Status.RES_WRAPPER_AVAILABLE)
+            self._client_message = client_message  # Write
+
+            self._transition(Status.CLIENT_MESSAGE_AVAILABLE)
+
+        with self._cv:
+            self._cv.wait_for(
+                lambda: self._status in [Status.CLOSED, Status.CLIENT_MESSAGE_AVAILABLE]
+            )
+
+            self._raise_if_closed()
+            client_message = self._client_message  # Read
+            self._client_message = None  # Reset
+            self._transition(Status.AWAITING_SERVER_MESSAGE)
+
+        if client_message is None:
+            raise Exception("client_message can not be None")
+        
+        self.submit_client_message(client_message)
+
+    def client_available(self,) -> bool:
+        if self._status == Status.AWAITING_SERVER_MESSAGE:
+            return True
+        return False
+    
+    def set_submit_client_message_fn(self, submit_client_message: Callable) -> None:
+        self.submit_client_message = submit_client_message
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py` & `daisyfl-0.4.1/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,118 +8,126 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""gRPC-based Flower ClientProxy implementation."""
+"""Ray-based Flower ClientProxy implementation."""
 
-from typing import Optional
+
+from typing import Callable, Dict, Optional, cast
+
+import ray
 
 from daisyfl import common
-from daisyfl.common import serde
-from daisyfl.proto.transport_pb2 import ClientMessage, ServerMessage
+from daisyfl.client import Client, ClientLike, to_client
 from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.server.grpc_server.grpc_bridge import GRPCBridge, InsWrapper, ResWrapper
+
+ClientFn = Callable[[str], ClientLike]
 
 
-class GrpcClientProxy(ClientProxy):
-    """Flower client proxy which delegates over the network using gRPC."""
+class RayClientProxy(ClientProxy):
+    """Flower client proxy which delegates work using Ray."""
 
-    def __init__(
-        self,
-        cid: str,
-        bridge: GRPCBridge,
-    ):
+    def __init__(self, client_fn: ClientFn, cid: str, resources: Dict[str, int]):
         super().__init__(cid)
-        self.bridge = bridge
+        self.client_fn = client_fn
+        self.resources = resources
 
     def get_properties(
-        self,
-        ins: common.GetPropertiesIns,
-        timeout: Optional[float],
+        self, ins: common.GetPropertiesIns, timeout: Optional[float]
     ) -> common.GetPropertiesRes:
-        """Requests client's set of internal properties."""
-        get_properties_msg = serde.get_properties_ins_to_proto(ins)
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(get_properties_ins=get_properties_msg),
-                timeout=timeout,
-            )
+        """Returns client's properties."""
+        future_get_properties_res = launch_and_get_properties.options(  # type: ignore
+            **self.resources,
+        ).remote(self.client_fn, self.cid, ins)
+        res = ray.get(future_get_properties_res, timeout=timeout)
+        return cast(
+            common.GetPropertiesRes,
+            res,
         )
-        client_msg: ClientMessage = res_wrapper.client_message
-        get_properties_res = serde.get_properties_res_from_proto(
-            client_msg.get_properties_res
-        )
-        return get_properties_res
 
     def get_parameters(
-        self,
-        ins: common.GetParametersIns,
-        timeout: Optional[float],
+        self, ins: common.GetParametersIns, timeout: Optional[float]
     ) -> common.GetParametersRes:
         """Return the current local model parameters."""
-        get_parameters_msg = serde.get_parameters_ins_to_proto(ins)
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(get_parameters_ins=get_parameters_msg),
-                timeout=timeout,
-            )
-        )
-        client_msg: ClientMessage = res_wrapper.client_message
-        get_parameters_res = serde.get_parameters_res_from_proto(
-            client_msg.get_parameters_res
+        future_paramseters_res = launch_and_get_parameters.options(  # type: ignore
+            **self.resources,
+        ).remote(self.client_fn, self.cid, ins)
+        res = ray.get(future_paramseters_res, timeout=timeout)
+        return cast(
+            common.GetParametersRes,
+            res,
+        )
+
+    def fit(self, ins: common.FitIns, timeout: Optional[float]) -> common.FitRes:
+        """Train model parameters on the locally held dataset."""
+        future_fit_res = launch_and_fit.options(  # type: ignore
+            **self.resources,
+        ).remote(self.client_fn, self.cid, ins)
+        res = ray.get(future_fit_res, timeout=timeout)
+        return cast(
+            common.FitRes,
+            res,
         )
-        return get_parameters_res
-
-    def fit(
-        self,
-        ins: common.FitIns,
-        timeout: Optional[float],
-    ) -> common.FitRes:
-        """Refine the provided parameters using the locally held dataset."""
-        fit_ins_msg = serde.fit_ins_to_proto(ins)
-
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(fit_ins=fit_ins_msg),
-                timeout=timeout,
-            )
-        )
-        client_msg: ClientMessage = res_wrapper.client_message
-        fit_res = serde.fit_res_from_proto(client_msg.fit_res)
-        return fit_res
 
     def evaluate(
-        self,
-        ins: common.EvaluateIns,
-        timeout: Optional[float],
+        self, ins: common.EvaluateIns, timeout: Optional[float]
     ) -> common.EvaluateRes:
-        """Evaluate the provided parameters using the locally held dataset."""
-        evaluate_msg = serde.evaluate_ins_to_proto(ins)
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(evaluate_ins=evaluate_msg),
-                timeout=timeout,
-            )
+        """Evaluate model parameters on the locally held dataset."""
+        future_evaluate_res = launch_and_evaluate.options(  # type: ignore
+            **self.resources,
+        ).remote(self.client_fn, self.cid, ins)
+        res = ray.get(future_evaluate_res, timeout=timeout)
+        return cast(
+            common.EvaluateRes,
+            res,
         )
-        client_msg: ClientMessage = res_wrapper.client_message
-        evaluate_res = serde.evaluate_res_from_proto(client_msg.evaluate_res)
-        return evaluate_res
 
     def reconnect(
-        self,
-        ins: common.ReconnectIns,
-        timeout: Optional[float],
+        self, ins: common.ReconnectIns, timeout: Optional[float]
     ) -> common.DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
-        reconnect_ins_msg = serde.reconnect_ins_to_proto(ins)
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(reconnect_ins=reconnect_ins_msg),
-                timeout=timeout,
-            )
-        )
-        client_msg: ClientMessage = res_wrapper.client_message
-        disconnect = serde.disconnect_res_from_proto(client_msg.disconnect_res)
-        return disconnect
+        return common.DisconnectRes(reason="")  # Nothing to do here (yet)
+
+
+@ray.remote
+def launch_and_get_properties(
+    client_fn: ClientFn, cid: str, get_properties_ins: common.GetPropertiesIns
+) -> common.GetPropertiesRes:
+    """Exectue get_properties remotely."""
+    client: Client = _create_client(client_fn, cid)
+    return client.get_properties(get_properties_ins)
+
+
+@ray.remote
+def launch_and_get_parameters(
+    client_fn: ClientFn, cid: str, get_parameters_ins: common.GetParametersIns
+) -> common.GetParametersRes:
+    """Exectue get_parameters remotely."""
+    client: Client = _create_client(client_fn, cid)
+    return client.get_parameters(get_parameters_ins)
+
+
+@ray.remote
+def launch_and_fit(
+    client_fn: ClientFn, cid: str, fit_ins: common.FitIns
+) -> common.FitRes:
+    """Exectue fit remotely."""
+    client: Client = _create_client(client_fn, cid)
+    return client.fit(fit_ins)
+
+
+@ray.remote
+def launch_and_evaluate(
+    client_fn: ClientFn, cid: str, evaluate_ins: common.EvaluateIns
+) -> common.EvaluateRes:
+    """Exectue evaluate remotely."""
+    client: Client = _create_client(client_fn, cid)
+    return client.evaluate(evaluate_ins)
+
+
+def _create_client(client_fn: ClientFn, cid: str) -> Client:
+    """Create a client instance."""
+    client_like: ClientLike = client_fn(cid)
+    return to_client(client_like=client_like)
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/grpc_server/grpc_server.py` & `daisyfl-0.4.1/src/py/daisyfl/server/grpc_server/grpc_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     >>>         Path("/crts/root.pem").read_bytes(),
     >>>         Path("/crts/localhost.crt").read_bytes(),
     >>>         Path("/crts/localhost.key").read_bytes(),
     >>>     ),
     >>> )
     """
 
-    servicer = FlowerServiceServicer(client_manager)
+    servicer = FlowerServiceServicer(client_manager, server_address)
     add_servicer_to_server_fn = add_FlowerServiceServicer_to_server
 
     server = generic_create_grpc_server(
         servicer_and_add_fn=(servicer, add_servicer_to_server_fn),
         server_address=server_address,
         max_concurrent_workers=max_concurrent_workers,
         max_message_length=max_message_length,
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/history.py` & `daisyfl-0.4.1/src/py/daisyfl/server/history.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/server.py` & `daisyfl-0.4.1/src/py/daisyfl/server/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Flower server."""
 
 
 import concurrent.futures
 import timeit
-from threading import Event, Condition
+from threading import Event, Condition, Lock, Timer
 from queue import Queue
 from logging import DEBUG, INFO
 from typing import Dict, List, Optional, Tuple, Union, Callable
 
 from daisyfl.common import (
     Task,
     Report,
@@ -37,15 +37,15 @@
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
     Parameters,
     ReconnectIns,
     Scalar,
-    NO_CREDENTIAL,
+    CurrentReturns,
 )
 from daisyfl.common.logger import log
 from daisyfl.common.typing import GetParametersIns
 from daisyfl.server.client_manager import ClientManager
 from daisyfl.server.client_proxy import ClientProxy
 from daisyfl.server.history import History
 
@@ -57,29 +57,116 @@
     List[Tuple[ClientProxy, EvaluateRes]],
     List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]],
 ]
 ReconnectResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, DisconnectRes]],
     List[Union[Tuple[ClientProxy, DisconnectRes], BaseException]],
 ]
-EVENT_SET = "EVENT_SET"
-FAILURES_NUM = "FAILURES_NUM"
-RESULTS_NUM = "RESULTS_NUM"
-SELECTED_NUM = "SELECTED_NUM"    
+
+# TODO: get results from server (server: queue to result)
+# TODO: Server:   cnd = Condition()
+# TODO: CurrentReturns = self.server.query_status(ticket)
+# TODO: self.server.query_returns(subtask_id)
+# TODO: self.server.stop_subtask(subtask_id)
+
+class SubtaskManager:
+    def __init__(self,) -> None:
+        self.subtasks: Dict[int, CurrentReturns] = {}
+        self.queues: Dict[int, Queue] = {}
+        self.client_previous_subtask: Dict[str, int] = {}
+        self._lock: Lock = Lock()
+        self._subtask_num = 0
+    
+    def subtask_id_generator(self,) -> int:
+        with self._lock:
+            tmp = self._subtask_num
+            self._subtask_num += 1
+        return tmp
+    
+    def register_subtask(
+        self, subtask_id: int, 
+        client_instructions: List[Tuple[ClientProxy, FitIns]],
+        timeout: int,
+    ) -> None:
+        # CurrentReturns
+        self.subtasks[subtask_id]: CurrentReturns = CurrentReturns(
+            selected=len(client_instructions),
+            results_num=0,
+            failures_num=0,
+            cnd=Condition(),
+        )
+        # queue
+        self.queues[subtask_id] = Queue()
+        # update client_previoud_subtask
+        for item in client_instructions:
+            cid = item[0].cid
+            if self.client_previous_subtask.__contains__(cid):
+                pre_subtask = self.client_previous_subtask[cid]
+                self.subtasks[pre_subtask].failures_num += 1
+                del self.client_previous_subtask[cid]
+                self.subtasks[pre_subtask].cnd.notify_all()
+            self.client_previous_subtask[cid] = subtask_id
+        # timeout
+        Timer(timeout, self.subtask_timeout, subtask_id)
+
+    def unregister_subtask(self, subtask_id: int) -> None:
+        del self.subtasks[subtask_id]
+        del self.queues[subtask_id]
+        cid_list = self.client_previous_subtask.keys()
+        for cid in cid_list:
+            if self.client_previous_subtask[cid] == subtask_id:
+                del self.client_previous_subtask[cid]
+        return
+
+    def submit_subtask(
+        self, result: Tuple[ClientProxy, Union[FitRes, EvaluateRes]],
+    ) -> None:
+        client_proxy, res = result
+        if (not self.client_previous_subtask.__contains__(client_proxy.cid)):
+            return
+        subtask_id = self.client_previous_subtask[client_proxy.cid]
+        if (not self.subtasks.__contains__(subtask_id)):
+            return
+        # Check result status code
+        if res.status.code == Code.OK:
+            self.subtasks[subtask_id].results_num += 1
+            self.queues[subtask_id].put(result)
+        # Not successful, client returned a result where the status code is not OK
+        else:
+            self.subtasks[subtask_id].failures_num += 1
+        del self.client_previous_subtask[client_proxy.cid]
+        with self.subtasks[subtask_id].cnd:
+            self.subtasks[subtask_id].cnd.notify_all()
+        return
+        
+    def get_current_returns(self, subtask_id: int) -> CurrentReturns:
+        return self.subtasks[subtask_id]
+    
+    def get_results(self, subtask_id: int) -> List[Tuple[ClientProxy, Union[FitRes, EvaluateRes]]]:
+        results = []
+        q = self.queues[subtask_id]
+        for _ in range(q.qsize()):
+            results.append(q.get())
+        return results
+      
+    def subtask_timeout(self, substask_id: int,) -> None:
+        if self.subtasks.__contains__(substask_id):
+            self.unregister_subtask(substask_id)
+
 
 class Server:
     """Flower server."""
-
     def __init__(
         self, *, 
         client_manager: ClientManager,
     ) -> None:
         self._client_manager: ClientManager = client_manager
         self._max_workers: Optional[int] = None
-        self.tickets = {}
+        self._subtask_manager: SubtaskManager = SubtaskManager()
+        self._client_manager.set_submit_subtask_fn(self._subtask_manager.submit_subtask)
 
     # set Server attributes
     def set_max_workers(self, max_workers: Optional[int]) -> None:
         """Set the max_workers used by ThreadPoolExecutor."""
         self._max_workers = max_workers
 
     # get Server attributes
@@ -87,117 +174,87 @@
         """Return ClientManager."""
         return self._client_manager
 
     def get_max_workers(self) -> Optional[int]:
         """Return max_workers."""
         return self._max_workers
     
-    # ClientManager APIs 
-    def num_available(self, credential: str = NO_CREDENTIAL, strict: bool = True,) -> int:
-        return self._client_manager.num_available(credential=credential, strict=strict)
+    # NOTE: ClientManager APIs 
+    def num_available(self, credential: Optional[str] = None) -> int:
+        return self._client_manager.num_available(credential=credential)
         
     def get_available_clients(
         self,
         min_num_clients: int = 2,
-        credential: str = NO_CREDENTIAL,
-        strict: bool = True,
+        credential: Optional[str] = None,
     ) -> List[ClientProxy]:
         return self._client_manager.get_available_clients(
             min_num_clients=min_num_clients,
             credential=credential,
-            strict=strict,
         )
 
+    # NOTE: SubtaskManager APIs
+    def finish_subtask(self, subtask_id: int) -> None:
+        self._subtask_manager.unregister_subtask(subtask_id)
+
+    def get_current_returns(self, subtask_id: int) -> CurrentReturns:
+        return self._subtask_manager.get_current_returns(subtask_id)
+    
+    def get_results(self, subtask_id: int) -> List[Tuple[ClientProxy, Union[FitRes, EvaluateRes]]]:
+        return self._subtask_manager.get_results(subtask_id)
+
     # TODO:
-    def disconnect_all_clients(self, timeout: Optional[float]) -> None:
+    def disconnect_all_clients(self,) -> None:
         """Send shutdown signal to all clients."""
-        all_clients = self.get_client_manager().all()
-        clients = [all_clients[k] for k in all_clients.keys()]
+        clients = self.get_client_manager().all() 
         instruction = ReconnectIns(seconds=None)
         client_instructions = [(client_proxy, instruction) for client_proxy in clients]
         _ = self._reconnect_clients(
             client_instructions=client_instructions,
             max_workers=self.get_max_workers(),
-            timeout=timeout,
         )
 
     def fit_clients(
         self,
         client_instructions: List[Tuple[ClientProxy, FitIns]],
         max_workers: Optional[int],
         timeout: Optional[float],
-        returns_q: Queue,
-        ticket: int,
-    ) -> None:
-        event = Event()
-        self.tickets[ticket] = {
-            EVENT_SET: event.set,
-            SELECTED_NUM: len(client_instructions),
-            RESULTS_NUM: 0,
-            FAILURES_NUM: 0,
-        }
-        return self._fit_clients(
+    ) -> int:
+        subtask_id = self._subtask_manager.subtask_id_generator()
+        self._subtask_manager.register_subtask(subtask_id, client_instructions, timeout)
+        self._fit_clients(
             client_instructions=client_instructions,
             max_workers=max_workers,
-            timeout=timeout,
-            returns_q=returns_q,
-            event=event,
-            ticket=ticket,
         )
+        return subtask_id
     
     def evaluate_clients(
         self,
         client_instructions: List[Tuple[ClientProxy, EvaluateIns]],
         max_workers: Optional[int],
         timeout: Optional[float],
-        returns_q: Queue,
-        ticket: int,
-    ) -> None:
-        event = Event()
-        self.tickets[ticket] = {
-            EVENT_SET: event.set,
-            SELECTED_NUM: len(client_instructions),
-            RESULTS_NUM: 0,
-            FAILURES_NUM: 0,
-        }
-        return self._evaluate_clients(
+    ) -> int:
+        subtask_id = self._subtask_manager.subtask_id_generator()
+        self._subtask_manager.register_subtask(subtask_id, client_instructions, timeout)
+        self._evaluate_clients(
             client_instructions=client_instructions,
             max_workers=max_workers,
-            timeout=timeout,
-            returns_q=returns_q,
-            event=event,
-            ticket=ticket,
         )
+        return subtask_id
 
-    def stop_return(self, ticket: int) -> bool:
-        if self.check_ticket(ticket):
-            self.tickets[ticket][EVENT_SET]()
-            del self.tickets[ticket]
-            return True
-        return False
-
-    def query_status(self, ticket: int,) -> Tuple[int, int, int]:
-        if self.check_ticket(ticket):
-            return self.tickets[ticket][SELECTED_NUM], self.tickets[ticket][RESULTS_NUM], self.tickets[ticket][FAILURES_NUM]
-    
-    def check_ticket(self, ticket) -> bool:
-        if ticket in self.tickets:
-            return True
-        return False
 
     def _reconnect_clients(
         self,
         client_instructions: List[Tuple[ClientProxy, ReconnectIns]],
         max_workers: Optional[int],
-        timeout: Optional[float],
     ) -> ReconnectResultsAndFailures:
         """Instruct clients to disconnect and never reconnect."""
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             submitted_fs = {
-                executor.submit(self._reconnect_client, self, client_proxy, ins, timeout)
+                executor.submit(self._reconnect_client, self, client_proxy, ins,)
                 for client_proxy, ins in client_instructions
             }
             finished_fs, _ = concurrent.futures.wait(
                 fs=submitted_fs,
                 timeout=None,  # Handled in the respective communication stack
             )
 
@@ -228,100 +285,28 @@
         return client, disconnect
 
 
     def _fit_clients(
         self,
         client_instructions: List[Tuple[ClientProxy, FitIns]],
         max_workers: Optional[int],
-        timeout: Optional[float],
-        returns_q: Queue,
-        event: Event,
-        ticket: int,
     ) -> None:
         """Refine parameters concurrently on all selected clients."""
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
-            submitted_fs = {
-                executor.submit(self._fit_client, client_proxy, ins, timeout)
+            {
+                executor.submit(client_proxy.fit, ins,)
                 for client_proxy, ins in client_instructions
             }
-            
-            for f in submitted_fs:
-                f.add_done_callback(self._get_future_callback_fn(returns_q=returns_q, event=event, ticket=ticket))
-            return 
-
-
-    def _fit_client(
-        self, client: ClientProxy, ins: FitIns, timeout: Optional[float]
-    ) -> Tuple[ClientProxy, FitRes]:
-        """Refine parameters on a single client."""
-        fit_res = client.fit(ins, timeout=timeout)
-        return client, fit_res
 
 
     def _evaluate_clients(
         self,
         client_instructions: List[Tuple[ClientProxy, EvaluateIns]],
         max_workers: Optional[int],
-        timeout: Optional[float],
-        returns_q: Queue,
-        event: Event,
-        ticket: int,
     ) -> None:
         """Evaluate parameters concurrently on all selected clients."""
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
-            submitted_fs = {
-                executor.submit(self._evaluate_client, client_proxy, ins, timeout)
+            {
+                executor.submit(client_proxy.evaluate, ins,)
                 for client_proxy, ins in client_instructions
             }
 
-            for f in submitted_fs:
-                f.add_done_callback(self._get_future_callback_fn(returns_q=returns_q, event=event, ticket=ticket))
-            return
-
-
-    def _evaluate_client(
-        self,
-        client: ClientProxy,
-        ins: EvaluateIns,
-        timeout: Optional[float],
-    ) -> Tuple[ClientProxy, EvaluateRes]:
-        """Evaluate parameters on a single client."""
-        evaluate_res = client.evaluate(ins, timeout=timeout)
-        return client, evaluate_res
-
-
-    def _get_future_callback_fn(
-        self,
-        returns_q: Queue,
-        event: Event,
-        ticket: int,
-    ) -> None:
-        """Convert finished future into either a result or a failure."""
-        def future_callback_fn(future: concurrent.futures.Future):
-            # Expired
-            if event.is_set():
-                return
-            self._handle_future(future, returns_q, ticket)
-        return future_callback_fn
-
-    # TODO: results and failures to job
-    def _handle_future(self, future, returns_q: Queue, ticket: int) -> None:
-        # Check if there was an exception
-        failure: Union[Tuple[ClientProxy, EvaluateRes], BaseException] = future.exception()
-        if failure is not None:
-            self.tickets[ticket][FAILURES_NUM] = self.tickets[ticket][FAILURES_NUM] + 1
-            return
-        
-        # Successfully received a result from a client
-        result: Tuple[ClientProxy, FitRes] = future.result()
-        _, res = result
-
-        # Check result status code
-        if res.status.code == Code.OK:
-            self.tickets[ticket][RESULTS_NUM] = self.tickets[ticket][RESULTS_NUM] + 1
-            returns_q.put(result)
-            return
-        
-        # Not successful, client returned a result where the status code is not OK
-        self.tickets[ticket][FAILURES_NUM] = self.tickets[ticket][FAILURES_NUM] + 1
-        return
-
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/server_operator_manager.py` & `daisyfl-0.4.1/src/py/daisyfl/server/server_operator_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,33 +11,26 @@
     Report,
     TID,
     REMOVE_OPERATOR,
     OPERATORS,
     STRATEGIES,
 )
 from daisyfl.server.server import Server
+from threading import Lock
 @dataclass
 class TaskOperator:
     tid: str
     operator_path: List[str]
     strategy_path: List[str]
     operator: ServerLogic
-    returns_fit: Queue
-    returns_evaluate: Queue
 
 class ServerOperatorManager:
     def __init__(self, server: Server):
         self.server: Server = server
         self.operators: List[TaskOperator] = []
-        # ticket(job id)
-        self._ticket_num: int = 0
-    
-    def disconnect_all_clients(self, timeout: int) -> None:
-        # TODO:
-        self.server.disconnect_all_clients(timeout)
     
     def fit_round(self, parameters: Parameters, task: Task) -> Tuple[Parameters, Report]:
         task_operator = self._get_task_operator(tid=task.config[TID])
         if not task_operator:
             self._register_operator(
                 tid=task.config[TID],
                 operator_path=task.config[OPERATORS][self.operator_key],
@@ -49,15 +42,15 @@
             log(WARNING, "Operator changed.")
             self._unregister_operator(tid=task.config[TID])
             self._register_operator(
                 tid=task.config[TID],
                 operator_path=task.config[OPERATORS][self.operator_key],
                 strategy_path=task.config[STRATEGIES][self.strategy_key],
             )
-        parameters, report = task_operator.operator.fit_round(parameters, task, task_operator.returns_fit,)
+        parameters, report = task_operator.operator.fit_round(parameters, task,)
         if task.config.__contains__(REMOVE_OPERATOR):
             if task.config[REMOVE_OPERATOR]:
                 self._unregister_operator(tid=task.config[TID])
         
         return parameters, report
 
 
@@ -75,26 +68,21 @@
             log(WARNING, "Operator changed.")
             self._unregister_operator(tid=task.config[TID])
             self._register_operator(
                 tid=task.config[TID],
                 operator_path=task.config[OPERATORS][self.operator_key],
                 strategy_path=task.config[STRATEGIES][self.strategy_key],
             )
-        report = task_operator.operator.evaluate_round(parameters, task, task_operator.returns_evaluate)
+        report = task_operator.operator.evaluate_round(parameters, task,)
         if task.config.__contains__(REMOVE_OPERATOR):
             if task.config[REMOVE_OPERATOR]:
                 self._unregister_operator(tid=task.config[TID])
         
         return report
     
-    # job_id
-    def ticket_dispenser(self,) -> int:
-        tmp = self._ticket_num
-        self._ticket_num = self._ticket_num + 1
-        return tmp
 
     # called by task_manager
     def set_operator_key(self, keys: List[str]) -> None:
         self.operator_key = keys[0]
         self.strategy_key = keys[1]
 
     def _get_task_operator(self, tid: str) -> TaskOperator:
@@ -112,17 +100,15 @@
             return False
         operator: ServerLogic = dynamic_load(operator_path[0], operator_path[1])
         strategy = dynamic_load(strategy_path[0], strategy_path[1])
         self.operators.append(TaskOperator(
             tid=tid,
             operator_path=operator_path,
             strategy_path=strategy_path,
-            operator=operator(server=self.server, strategy=strategy(), ticket_dispenser=self.ticket_dispenser),
-            returns_fit=Queue(),
-            returns_evaluate=Queue(),
+            operator=operator(server=self.server, strategy=strategy(),),
         ))
         return True
     
     def _unregister_operator(self, tid: str) -> bool:
         for i in range(len(self.operators)):
             if self.operators[i].tid == tid:
                 del self.operators[i]
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/server/task_manager.py` & `daisyfl-0.4.1/src/py/daisyfl/server/task_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import timeit
 from logging import DEBUG, INFO, ERROR, WARNING
 from typing import Dict, List, Optional, Tuple, Union, Callable, TypedDict
-import time
 
 from daisyfl.common import (
     NUM_ROUNDS,
     CURRENT_ROUND,
     EVALUATE,
     TIMEOUT,
     FIT_SAMPLES,
@@ -63,42 +62,26 @@
 class TaskManager():
     """Task manager."""
 
     def __init__(
         self,
         server_operator_manager: ServerOperatorManager,
         manager_type: Type,
-        parent_address: str,
     ) -> None:
         self.start_times: List[(int, float)] = []
         self.server_operator_manager: ServerOperatorManager = server_operator_manager
         self.type: Type = manager_type
         if self.type == Type.MASTER:
             operator_key = [MASTER_SERVER_OPERATOR, MASTER_STRATEGY] 
         else:
             operator_key = [ZONE_SERVER_OPERATOR, ZONE_STRATEGY]
         self.server_operator_manager.set_operator_key(operator_key)
 
         # MetaTask
         self.meta_tasks: List[MetaTask] = []
-        
-        # for zones: wait for receiving tasks sent from master
-        self._cnd_stop = threading.Condition()
-
-        # zone_client
-        self.zc_thread = threading.Thread(target=ZoneClient, args=(self, parent_address, _set_zone_client)) \
-            if self.type == Type.ZONE else None
-        if self.zc_thread:
-            self.zc_thread.start()
-            time.sleep(1)
-            if not self.zc_thread.is_alive():
-                log(ERROR,
-                    "ZoneClient failed",
-                )
-                exit(1)
 
     def receive_task(
         self, task_config: TypedDict, parameters: Optional[Parameters] = None
     )-> Tuple[Parameters, Report]:
         # MetaTask
         if parameters is None:
             parameters: Parameters = _initialize_parameters(model_path=task_config[MODEL_PATH])
@@ -333,25 +316,14 @@
 
     def task_complete(self, tid: str) -> bool:
         if not _pop_meta_task(task_manager=self, tid=tid):
             log(WARNING, "Can't delete MetaTask")
             return False
         return True
 
-    # receive commands from API Handler
-    def reconnect_to_parent(self, address: str = None, sleep_duration: int = None):
-        self.zone_client.reconnect(address, sleep_duration)
-    
-    def disconnect_clients(self, address: str = None, sleep_duration: int = None):
-        self.server_operator_manager.disconnect_all_clients(timeout=None)
-        
-    def shutdown(self,) -> None:
-        with self._cnd_stop:
-            self._cnd_stop.notify()
-
 
 # initial parameters
 def _initialize_parameters(model_path: str) -> Parameters:
     # FL Starting
     log(INFO, "Initializing global parameters")
     return ndarrays_to_parameters(list(np.load(model_path, allow_pickle=True)))
 
@@ -370,10 +342,7 @@
 
 def _pop_meta_task(task_manager: TaskManager, tid: str) -> bool:
     for i in range(len(task_manager.meta_tasks)):
         if task_manager.meta_tasks[i].tid == tid:
             task_manager.meta_tasks.pop(i)
             return True
     return False
-
-def _set_zone_client(task_manager: TaskManager, zone_client: ZoneClient) -> None:
-    task_manager.zone_client: ZoneClient = zone_client
```

### Comparing `daisyfl-0.2.0/src/py/daisyfl/simulation/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/simulation/ray_transport/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/src/py/daisyfl/utils/__init__.py` & `daisyfl-0.4.1/src/py/daisyfl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.2.0/setup.py` & `daisyfl-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
  'simulation': ['ray[default]>=2.0.0,<2.1.0']}
 
 setup_kwargs = {
     'name': 'daisyfl',
-    'version': '0.2.0',
+    'version': '0.4.1',
     'description': 'Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing',
     'long_description': "# Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing\n\n## dev mode\n1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n2. build up environment\n```\ndocker run -it -v <daisy_source_code>:/root/daisy tcfwbper/daisyfl-dev:<version_tag> /bin/bash\n```\n3. develop<br>\n4. setup examples<br>\ndon't overwrite daisyfl dependency in this step.<br>\n```\ndocker attach <container_id>\n```\n```\ncd <example_path> && conda activate daisy\npip install <pkgs_for_your_example>\n```\n5. run examples\n\n## user mode\n1. install daisyfl\n```\npip install <daisyfl_version>\n```\n2. setup examples\n```\npip install <pkgs_for_your_example>\n```\n3. run examples",
     'author': 'tcfwbper',
     'author_email': 'b05208031@ntu.edu.tw',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Intelligent-Systems-Lab/daisy',
```

### Comparing `daisyfl-0.2.0/PKG-INFO` & `daisyfl-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daisyfl
-Version: 0.2.0
+Version: 0.4.1
 Summary: Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing
 Home-page: https://github.com/Intelligent-Systems-Lab/daisy
 License: Apache-2.0
 Author: tcfwbper
 Author-email: b05208031@ntu.edu.tw
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

