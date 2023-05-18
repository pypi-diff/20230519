# Comparing `tmp/caikit-0.4.3.tar.gz` & `tmp/caikit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.4.3.tar` & `caikit-0.4.4.tar`

### file list

```diff
@@ -1,315 +1,320 @@
--rw-r--r--   0        0        0       60 2023-05-17 19:45:34.757668 caikit-0.4.3/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1272 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      212 2023-05-17 19:45:34.757668 caikit-0.4.3/.gitignore
--rw-r--r--   0        0        0      324 2023-05-17 19:45:34.757668 caikit-0.4.3/.isort.cfg
--rw-r--r--   0        0        0      370 2023-05-17 19:45:34.757668 caikit-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-05-17 19:45:34.757668 caikit-0.4.3/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-17 19:45:34.757668 caikit-0.4.3/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-05-17 19:45:34.757668 caikit-0.4.3/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-17 19:45:34.757668 caikit-0.4.3/.whitesource
--rw-r--r--   0        0        0      368 2023-05-17 19:45:34.757668 caikit-0.4.3/CODEOWNERS
--rw-r--r--   0        0        0     7165 2023-05-17 19:45:34.757668 caikit-0.4.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-17 19:45:34.757668 caikit-0.4.3/LICENSE
--rw-r--r--   0        0        0     3626 2023-05-17 19:45:34.757668 caikit-0.4.3/README.md
--rw-r--r--   0        0        0      152 2023-05-17 19:45:34.757668 caikit-0.4.3/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit-overview.png
--rw-r--r--   0        0        0      419 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/config/__init__.py
--rw-r--r--   0        0        0     6052 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/config/config.py
--rw-r--r--   0        0        0     6554 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/config/config.yml
--rw-r--r--   0        0        0     1838 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1586 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1026 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    28986 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    12390 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4858 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1564 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40248 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21916 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/model_manager.py
--rw-r--r--   0        0        0    41505 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module.py
--rw-r--r--   0        0        0     6062 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4716 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2769 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     6293 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_meta.py
--rw-r--r--   0        0        0    14929 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_type.py
--rw-r--r--   0        0        0      709 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/resources/base.py
--rw-r--r--   0        0        0     5391 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32204 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9332 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14200 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    16693 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5845 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13249 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    12818 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0      666 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10744 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4794 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8232 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9473 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    15316 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6797 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17900 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      169 2023-05-17 19:45:34.765668 caikit-0.4.3/code-of-conduct.md
--rw-r--r--   0        0        0     1610 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/architecture_club/README.md
--rw-r--r--   0        0        0      837 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1425 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      671 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      742 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      643 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3061 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py
--rw-r--r--   0        0        0     1157 2023-05-17 19:45:37.989673 caikit-0.4.3/pyproject.toml
--rwxr-xr-x   0        0        0      639 2023-05-17 19:45:34.769668 caikit-0.4.3/scripts/check_deps.sh
--rwxr-xr-x   0        0        0      720 2023-05-17 19:45:34.769668 caikit-0.4.3/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-05-17 19:45:34.769668 caikit-0.4.3/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0     3572 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/base.py
--rw-r--r--   0        0        0        0 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/config/test_configs.py
--rw-r--r--   0        0        0     9171 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    11661 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26454 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13147 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    19621 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     1104 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4291 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0      521 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_imports.py
--rw-r--r--   0        0        0    21985 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    13348 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_module.py
--rw-r--r--   0        0        0     6950 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8080 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     3773 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_module_type.py
--rw-r--r--   0        0        0     1038 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     2456 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_task.py
--rw-r--r--   0        0        0     7967 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4972 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    14622 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5542 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      647 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      337 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1875 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      646 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2456 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1306 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2713 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      410 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1717 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0        0 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14146 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10454 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17908 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     5398 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8668 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3768 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18431 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1716 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1372 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7848 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    15426 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    30097 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    11070 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26122 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1301 2023-05-17 19:45:34.773668 caikit-0.4.3/tox.ini
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 caikit-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-18 22:23:26.587025 caikit-0.4.4/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1272 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-05-18 22:23:26.587025 caikit-0.4.4/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      261 2023-05-18 22:23:26.587025 caikit-0.4.4/.gitignore
+-rw-r--r--   0        0        0      324 2023-05-18 22:23:26.587025 caikit-0.4.4/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-05-18 22:23:26.587025 caikit-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-05-18 22:23:26.587025 caikit-0.4.4/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-18 22:23:26.587025 caikit-0.4.4/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-05-18 22:23:26.587025 caikit-0.4.4/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-18 22:23:26.587025 caikit-0.4.4/.whitesource
+-rw-r--r--   0        0        0      368 2023-05-18 22:23:26.587025 caikit-0.4.4/CODEOWNERS
+-rw-r--r--   0        0        0     7165 2023-05-18 22:23:26.587025 caikit-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-18 22:23:26.587025 caikit-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3626 2023-05-18 22:23:26.587025 caikit-0.4.4/README.md
+-rw-r--r--   0        0        0      152 2023-05-18 22:23:26.587025 caikit-0.4.4/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit-overview.png
+-rw-r--r--   0        0        0      419 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/config/config.py
+-rw-r--r--   0        0        0     6554 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/config/config.yml
+-rw-r--r--   0        0        0     1838 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1586 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0     1026 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    35512 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4050 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    13826 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4858 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1564 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40248 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21916 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    41505 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module.py
+-rw-r--r--   0        0        0     6062 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4716 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2769 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6293 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_meta.py
+-rw-r--r--   0        0        0    14929 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/module_type.py
+-rw-r--r--   0        0        0      709 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     5391 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/task.py
+-rw-r--r--   0        0        0     1001 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-05-18 22:23:26.591025 caikit-0.4.4/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32204 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9332 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1827 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14200 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    16693 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5845 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13914 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7155 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    12818 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0      666 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10744 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4794 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8232 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9473 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    15316 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-05-18 22:23:26.595025 caikit-0.4.4/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6797 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17900 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-05-18 22:23:26.599025 caikit-0.4.4/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      169 2023-05-18 22:23:26.599025 caikit-0.4.4/code-of-conduct.md
+-rw-r--r--   0        0        0       68 2023-05-18 22:23:26.599025 caikit-0.4.4/docs-requirements.txt
+-rw-r--r--   0        0        0      634 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/Makefile
+-rw-r--r--   0        0        0     1610 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/architecture_club/README.md
+-rw-r--r--   0        0        0     2660 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/conf.py
+-rw-r--r--   0        0        0      225 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-18 22:23:26.599025 caikit-0.4.4/docs/make.bat
+-rw-r--r--   0        0        0      837 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1425 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      671 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      643 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3061 2023-05-18 22:23:26.599025 caikit-0.4.4/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py
+-rw-r--r--   0        0        0     1157 2023-05-18 22:23:30.587056 caikit-0.4.4/pyproject.toml
+-rwxr-xr-x   0        0        0      639 2023-05-18 22:23:26.599025 caikit-0.4.4/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-05-18 22:23:26.599025 caikit-0.4.4/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-05-18 22:23:26.599025 caikit-0.4.4/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     3572 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/base.py
+-rw-r--r--   0        0        0        0 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/config/test_configs.py
+-rw-r--r--   0        0        0     9171 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    11661 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5033 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26454 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16232 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    18410 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     1104 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4291 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0      521 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21985 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    13348 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_module.py
+-rw-r--r--   0        0        0     6950 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8080 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     3773 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_module_type.py
+-rw-r--r--   0        0        0     1038 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     2456 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/test_task.py
+-rw-r--r--   0        0        0     7967 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4972 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.599025 caikit-0.4.4/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    14622 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     6782 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      337 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1875 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      646 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2456 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1306 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2713 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      410 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1717 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14146 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10454 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17908 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     5398 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8668 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3768 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18431 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1716 2023-05-18 22:23:26.603025 caikit-0.4.4/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1372 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7848 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    15426 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    30097 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    11070 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26122 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-05-18 22:23:26.607025 caikit-0.4.4/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2115 2023-05-18 22:23:26.607025 caikit-0.4.4/tox.ini
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 caikit-0.4.4/PKG-INFO
```

### Comparing `caikit-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.4.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.4.4/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/.github/workflows/build-library.yml` & `caikit-0.4.4/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/.github/workflows/lint-code.yml` & `caikit-0.4.4/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/.github/workflows/publish-library.yml` & `caikit-0.4.4/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/.pylintrc` & `caikit-0.4.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/CONTRIBUTING.md` & `caikit-0.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/LICENSE` & `caikit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/README.md` & `caikit-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit-overview.png` & `caikit-0.4.4/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/config/__init__.py` & `caikit-0.4.4/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/config/config.py` & `caikit-0.4.4/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/config/config.yml` & `caikit-0.4.4/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/__init__.py` & `caikit-0.4.4/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/augmentors/__init__.py` & `caikit-0.4.4/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/augmentors/base.py` & `caikit-0.4.4/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.4.4/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.4.4/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/augmentors/schemes/base.py` & `caikit-0.4.4/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.4.4/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.4.4/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/blocks/__init__.py` & `caikit-0.4.4/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/blocks/base.py` & `caikit-0.4.4/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/__init__.py` & `caikit-0.4.4/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/base.py` & `caikit-0.4.4/caikit/core/data_model/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 """
 
 # metaclass-generated field members cannot be detected by pylint
 # pylint: disable=no-member
 
 # Standard
 from enum import Enum
-from typing import Optional, Type, Union
+from typing import Any, Dict, Optional, Type, Union
 import base64
 import json
 
 # Third Party
 from google.protobuf import json_format
 from google.protobuf.descriptor import Descriptor
+from google.protobuf.internal import type_checkers as proto_type_checkers
 from google.protobuf.message import Message as ProtoMessageType
 
 # First Party
 import alog
 
 # Local
 from ..toolkit.errors import error_handler
@@ -55,87 +56,95 @@
     _MISSING_ATTRIBUTE = "missing attribute"
 
     # Special attribute used to communicate that the proto fields are forward
     # declared and will be populated after the metaclass has completed
     # construction.
     _FWD_DECL_FIELDS = "__fwd_decl_fields__"
 
+    # Special instance attributes that an instance of a class derived from
+    # DataBase may have. These are added to __slots__.
+    _BACKEND_ATTR = "_backend"
+    _WHICH_ONEOF_ATTR = "_which_oneof"
+
     def __new__(mcs, name, bases, attrs):
         """When constructing a new data model class, we set the 'fields' class variable from the
         protobufs descriptor and then set the '__slots__' magic class attribute to fields.  This
         provides two benefits: (a) performance is improved since the classes only need to know
         about these attributes (b) it helps to enforce that all member variables in these classes
         are described in the protobufs.
 
         Note:  If you want to add a variable for internal use that is not described in the
         protobufs, it can be named in the tuple class variable _private_slots and will
         automatically be added to __slots__.
         """
-        # Get all fields in protobufs with same name as class,
-        # except for DataBase, which has no matching protobufs
-        fields = ()
 
-        # Protobufs fields can be divided into these categories, which are used to automatically
-        # determine appropriate behavior in a number of methods
-        fields_enum_map = {}
-        fields_enum_rev = {}
-        _fields_message = ()
-        _fields_message_repeated = ()
-        _fields_enum = ()
-        _fields_enum_repeated = ()
-        _fields_primitive = ()
-        _fields_primitive_repeated = ()
-        _fields_map = ()
+        # Protobufs fields can be divided into these categories, which are used
+        # to automatically determine appropriate behavior in a number of methods
+        attrs["full_name"] = name
+        attrs["fields_enum_map"] = {}
+        attrs["fields_enum_rev"] = {}
+        attrs["_fields_oneofs_map"] = {}
+        attrs["_fields_to_oneof"] = {}
+        attrs["_fields_map"] = ()
+        attrs["_fields_message"] = ()
+        attrs["_fields_message_repeated"] = ()
+        attrs["_fields_enum"] = ()
+        attrs["_fields_enum_repeated"] = ()
+        attrs["_fields_primitive"] = ()
+        attrs["_fields_primitive_repeated"] = ()
+
+        # Look for the set of fields either from a predefined protobuf class or
+        # from a forward declaration from @dataobject
+        fields = ()
         proto_class = None
-        full_name = name
         if name not in ["DataBase", "DataObjectBase"]:
             # Look for a precompiled proto class and if found, parse its
             # descriptor
             proto_class = attrs.get("_proto_class")
             if proto_class is not None:
-                fields = tuple(proto_class.DESCRIPTOR.fields_by_name)
+                all_oneof_fields = [
+                    field.name
+                    for oneof in proto_class.DESCRIPTOR.oneofs
+                    for field in oneof.fields
+                ]
+                fields = tuple(
+                    (
+                        field
+                        for field in proto_class.DESCRIPTOR.fields_by_name
+                        if field not in all_oneof_fields
+                    )
+                ) + tuple(proto_class.DESCRIPTOR.oneofs_by_name)
 
             # Otherwise, we need to get the fields from a "special" attribute
             else:
                 fields = attrs.pop(mcs._FWD_DECL_FIELDS, None)
                 log.debug4(
                     "Using dataclass forward declaration fields %s for %s", fields, name
                 )
                 error.value_check(
                     "<COR49310991E>",
                     fields is not None,
                     "No proto class found for {}",
                     name,
                 )
+        attrs["fields"] = fields
+        attrs["_proto_class"] = proto_class
 
         # Look if any private slots are declared as class variables
         private_slots = attrs.setdefault("_private_slots", ())
 
         # Class slots are fields + private slots, this prevents other
         # member attributes from being set and also improves performance
         attrs["__slots__"] = tuple(
-            [f"_{field}" for field in fields] + list(private_slots) + ["_backend"]
+            [f"_{field}" for field in fields]
+            + list(private_slots)
+            + [mcs._BACKEND_ATTR, mcs._WHICH_ONEOF_ATTR]
         )
 
-        # Set fields class variable for reference
-        # these are valuable for validating attributes and
-        # also for recursively converting to and from protobufs
-        attrs["full_name"] = full_name
-        attrs["fields"] = fields
-        attrs["fields_enum_map"] = fields_enum_map
-        attrs["fields_enum_rev"] = fields_enum_rev
-        attrs["_fields_map"] = _fields_map
-        attrs["_fields_message"] = _fields_message
-        attrs["_fields_message_repeated"] = _fields_message_repeated
-        attrs["_fields_enum"] = _fields_enum
-        attrs["_fields_enum_repeated"] = _fields_enum_repeated
-        attrs["_fields_primitive"] = _fields_primitive
-        attrs["_fields_primitive_repeated"] = _fields_primitive_repeated
-        attrs["_proto_class"] = proto_class
-
+        # Create the instance of the type
         instance = super().__new__(mcs, name, bases, attrs)
 
         # If there's a valid proto class, perform proto descriptor parsing
         if proto_class is not None:
             mcs.parse_proto_descriptor(instance)
 
         # Return the constructed class instance
@@ -150,14 +159,15 @@
 
         # use the fully qualified protobuf name to avoid conflicts with
         # nested messages that have matching names
         cls.full_name = cls._proto_class.DESCRIPTOR.full_name
 
         # preserve old fields for _make_property_getter later
         old_fields = cls.fields
+
         # overwrite to only have proto-specific fields present
         cls.fields = tuple(cls._proto_class.DESCRIPTOR.fields_by_name)
 
         # map from all enum fields to their enum classes
         # note: enums are also primitives, these overlap
         cls.fields_enum_map = {
             field.name: getattr(enums, field.enum_type.name)
@@ -167,14 +177,29 @@
 
         cls.fields_enum_rev = {
             field.name: getattr(enums, field.enum_type.name + "Rev")
             for field in cls._proto_class.DESCRIPTOR.fields
             if field.enum_type is not None
         }
 
+        # mapping of all oneofs and the fields that are part of them
+        # NOTE: protobuf makes an interesting use of oneof to wrap types that
+        #   should be explicitly optional. We don't want to consider these
+        #   oneofs in the general oneof handling.
+        cls._fields_oneofs_map = {
+            oneof_name: [field.name for field in oneof.fields]
+            for oneof_name, oneof in cls._proto_class.DESCRIPTOR.oneofs_by_name.items()
+            if len(oneof.fields) != 1 or oneof.name != f"_{oneof.fields[0].name}"
+        }
+        cls._fields_to_oneof = {
+            field_name: oneof_name
+            for (oneof_name, oneof_fields) in cls._fields_oneofs_map.items()
+            for field_name in oneof_fields
+        }
+
         # all repeated fields
         fields_repeated = tuple(
             field.name
             for field in cls._proto_class.DESCRIPTOR.fields
             if field.label == field.LABEL_REPEATED
         )
 
@@ -211,16 +236,18 @@
         cls._fields_message = frozenset(_fields_message_all).difference(fields_repeated)
 
         # messages that are repeated
         cls._fields_message_repeated = frozenset(fields_repeated).intersection(
             _fields_message_all
         )
 
+        # enums that are not repeated
         cls._fields_enum = frozenset(_fields_enum_all).difference(fields_repeated)
 
+        # enums that are repeated
         cls._fields_enum_repeated = frozenset(_fields_enum_all).intersection(
             fields_repeated
         )
 
         # primitives that are not repeated
         cls._fields_primitive = frozenset(_fields_primitive_all).difference(
             fields_repeated
@@ -232,55 +259,81 @@
         )
 
         # Update the global class and proto registries
         # NOTE: Explicitly not respecting metaclass inheritance so single
         #   registry shared for all
         _DataBaseMetaClass.class_registry[cls.full_name] = cls
 
-        # Add properties that use the underlying backend
-        # also add fields that existed in old_fields
-        # for supporting oneofs
+        # Add properties that use the underlying backend. Also add fields that
+        # existed in old_fields for supporting oneofs
         # see https://github.com/caikit/caikit/pull/107 for details
         for field in set(cls.fields + tuple(old_fields)):
-            setattr(cls, field, mcs._make_property_getter(field))
+
+            # If the field is the name of a field within a oneof and it was not
+            # in the old fields, the data is held under the oneof's name if this
+            # is the set value for the oneof
+            if oneof_name := cls._fields_to_oneof.get(field):
+                setattr(cls, field, mcs._make_property_getter(field, oneof_name))
+
+            # If the field is a plain field or the name of a oneof, it will be
+            # accessed directly
+            else:
+                setattr(cls, field, mcs._make_property_getter(field))
 
         # If there is not already an __init__ function defined, make one
         current_init = cls.__init__
         if current_init is None or current_init is DataBase.__init__:
             setattr(cls, "__init__", mcs._make_init(cls.fields))
 
     @classmethod
-    def _make_property_getter(mcs, field):
+    def _make_property_getter(mcs, field, oneof_name=None):
         """This helper creates an @property attribute getter for the given field
 
         NOTE: This needs to live as a standalone function in order for the given
             field name to be properly bound to the closure for the attrs
         """
-        private_name = f"_{field}"
+        private_name = f"_{field}" if oneof_name is None else oneof_name
 
-        @property
         def _property_getter(self):
             # Check to see if the private name is defined and just return it if
             # it is
             current = getattr(self, private_name, mcs._MISSING_ATTRIBUTE)
             if current is not mcs._MISSING_ATTRIBUTE:
                 return current
 
             # If not currently set, delegate to the backend
-            attr_val = self._backend.get_attribute(self.__class__, field)
+            backend = self.backend
+            if backend is None:
+                error(
+                    "<COR66616239E>",
+                    AttributeError(
+                        f"{type(self)} missing attribute {field} and no backend set"
+                    ),
+                )
+            attr_val = backend.get_attribute(self.__class__, field)
 
             # If the backend says that this attribute should be cached, set it
             # as an attribute on the class
-            if self._backend.cache_attribute(field, attr_val):
-                setattr(self, private_name, attr_val)
+            if backend.cache_attribute(field, attr_val):
+                setattr(self, field, attr_val)
 
             # Return the value found by the backend
             return attr_val
 
-        return _property_getter
+        # If this is a oneof, add an extra layer of wrapping to check
+        # which_oneof before returning a valid result
+        if oneof_name:
+
+            def _oneof_property_getter(self):
+                if self.which_oneof(oneof_name) == field:
+                    return _property_getter(self)
+
+            return property(_oneof_property_getter)
+
+        return property(_property_getter)
 
     @staticmethod
     def _make_init(fields):
         """This helper creates an __init__ function for a class which has the
         arguments for all the fields and just sets them as instance attributes.
         """
 
@@ -294,44 +347,62 @@
 
         def __init__(self, *args, **kwargs):
             num_args = len(args)
             num_kwargs = len(kwargs)
             num_fields = len(fields)
             used_fields = []
 
+            # If the proto has oneofs, set up which_oneof
+            which_oneof = {}
+            cls = self.__class__
+            if cls._fields_oneofs_map:
+                setattr(self, _DataBaseMetaClass._WHICH_ONEOF_ATTR, which_oneof)
+
             if num_args + num_kwargs > num_fields:
                 error(
                     "<COR71444420E>",
                     TypeError(f"Too many arguments given. Args are: {fields}"),
                 )
 
             if num_args > 0:  # Do a quick check for performance reason
                 for i, field_val in enumerate(args):
                     field_name = fields[i]
                     setattr(self, field_name, field_val)
                     used_fields.append(field_name)
 
             if num_kwargs > 0:  # Do a quick check for performance reason
                 for field_name, field_val in kwargs.items():
-                    if field_name not in fields:
+
+                    # If this is a oneof field, alias to the oneof name
+                    if oneof_name := cls._fields_to_oneof.get(field_name):
+                        which_oneof[oneof_name] = field_name
+                        field_name = oneof_name
+
+                    if (
+                        field_name not in fields
+                        and field_name not in cls._fields_oneofs_map
+                    ):
                         error(
                             "<COR71444421E>", TypeError(f"Unknown field {field_name}")
                         )
                     elif field_name in used_fields:
                         error(
                             "<COR71444422E>",
                             TypeError(f"Got multiple values for field {field_name}"),
                         )
                     setattr(self, field_name, field_val)
                     used_fields.append(field_name)
 
             # Default all unspecified fields to None
             if num_fields > 0:  # Do a quick check for performance reason
                 for field_name in fields:
-                    if field_name not in used_fields:
+                    if (
+                        field_name not in used_fields
+                        and field_name not in cls._fields_to_oneof
+                    ):
                         setattr(self, field_name, None)
 
         # Set docstring to the method explicitly
         setattr(__init__, "__doc__", docstring)
         return __init__
 
 
@@ -340,18 +411,30 @@
 
     Notes:
         All leaves in the hierarchy of derived classes should have a corresponding protobufs class
         defined in the interface definitions.  If not, an exception will be thrown at runtime.
     """
 
     def __setattr__(self, name, val):
-        """If attempting to set one of the named fields, instead set the
-        "private" version of the attribute.
+        """Handle attribute setting for oneofs and named fields with delegation
+        to backends as needed
         """
-        if name in self.__class__.fields:
+        # If setting a oneof directly, remove any oneof information
+        cls = self.__class__
+        if name in cls._fields_oneofs_map:
+            self._get_which_oneof_dict().pop(name, None)
+
+        # If this is the name of a oneof field, set the oneof itself
+        if oneof_name := cls._fields_to_oneof.get(name):
+            self._get_which_oneof_dict()[oneof_name] = name
+            name = oneof_name
+
+        # If attempting to set one of the named fields or a oneof, instead set
+        # the private version of the attribute.
+        if name in cls.fields or name in cls._fields_oneofs_map:
             super().__setattr__(f"_{name}", val)
         else:
             super().__setattr__(name, val)
 
     @classmethod
     def get_proto_class(cls) -> Type[ProtoMessageType]:
         return cls._proto_class
@@ -379,17 +462,93 @@
                 cls.get_proto_class().DESCRIPTOR.fields_by_name[field_name].message_type
             )
         return None
 
     @classmethod
     def from_backend(cls, backend):
         instance = cls.__new__(cls)
-        setattr(instance, "_backend", backend)
+        setattr(instance, _DataBaseMetaClass._BACKEND_ATTR, backend)
         return instance
 
+    @property
+    def backend(self) -> Optional["DataModelBackendBase"]:
+        return getattr(self, _DataBaseMetaClass._BACKEND_ATTR, None)
+
+    def which_oneof(self, oneof_name: str) -> Optional[str]:
+        """Get the name of the oneof field set for the given oneof or None if no
+        field is set
+        """
+        # If the internal dict is already set, use that information
+        which_oneof = self._get_which_oneof_dict()
+        if current_val := which_oneof.get(oneof_name):
+            return current_val
+
+        # Get the current value for the oneof and introspect which field its
+        # type matches
+        oneof_val = getattr(self, oneof_name)
+        which_field = self._infer_which_oneof(oneof_name, oneof_val)
+        if which_field is not None:
+            which_oneof[oneof_name] = which_field
+        return which_field
+
+    @classmethod
+    def _infer_which_oneof(cls, oneof_name: str, oneof_val: Any) -> Optional[str]:
+        """Check each candidate field within the oneof to see if it's a type
+        match
+
+        NOTE: In the case where fields within a oneof have the same type, the
+          first field whose type matches will be used!
+        """
+        for field_name in cls._fields_oneofs_map.get(oneof_name, []):
+            if cls._is_valid_type_for_field(field_name, oneof_val):
+                return field_name
+
+    def _get_which_oneof_dict(self) -> Dict[str, str]:
+        which_oneof = getattr(self, _DataBaseMetaClass._WHICH_ONEOF_ATTR, None)
+        if which_oneof is None:
+            super().__setattr__(_DataBaseMetaClass._WHICH_ONEOF_ATTR, {})
+            which_oneof = getattr(self, _DataBaseMetaClass._WHICH_ONEOF_ATTR)
+        return which_oneof
+
+    @classmethod
+    def _is_valid_type_for_field(cls, field_name: str, val: Any) -> bool:
+        """Check whether the given value is valid for the given field"""
+        field_descriptor = cls._proto_class.DESCRIPTOR.fields_by_name[field_name]
+
+        if val is None:
+            return False
+
+        # If it's a data object or an enum and the descriptors match, it's a
+        # good type
+        if (
+            isinstance(val, DataBase)
+            and field_descriptor.message_type == val.get_proto_class().DESCRIPTOR
+        ) or (
+            isinstance(val, Enum)
+            and field_descriptor.enum_type == val.get_proto_class().DESCRIPTOR
+        ):
+            return True
+
+        # If it's a data object or an enum and the descriptors don't match, it's
+        # a bad type
+        if field_descriptor.type in [
+            field_descriptor.TYPE_MESSAGE,
+            field_descriptor.TYPE_ENUM,
+        ]:
+            return False
+
+        # If it's a primitive, use protobuf type checkers
+        checker = proto_type_checkers.GetTypeChecker(field_descriptor)
+        try:
+            checker.CheckValue(val)
+            return True
+        except TypeError:
+            pass
+        return False
+
     @classmethod
     def from_binary_buffer(cls, buf):
         """Builds the data model object out of the binary string
 
         Args:
             buf: The binary buffer containing a serialized protobufs message
 
@@ -409,20 +568,20 @@
             proto:
                 A protocol buffer to serialize from.
 
         Returns:
             protobufs
                 A DataBase object.
         """
-        if cls.__name__ != proto.DESCRIPTOR.name:
+        if cls._proto_class.DESCRIPTOR.name != proto.DESCRIPTOR.name:
             error(
                 "<COR71783894E>",
                 ValueError(
                     "class name `{}` does not match protobufs name `{}`".format(
-                        cls.__name__, proto.DESCRIPTOR.name
+                        cls._proto_class.DESCRIPTOR.name, proto.DESCRIPTOR.name
                     )
                 ),
             )
 
         kwargs = {}
         for field in cls.fields:
             try:
```

### Comparing `caikit-0.4.3/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.4.4/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/data_backends/base.py` & `caikit-0.4.4/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.4.4/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,15 +59,18 @@
         """
 
         # NOTE: We do not type-check the args here for efficiency. This method
         #   should only be called by the DataBase class, so we can assume it's
         #   being used correctly.
 
         # Make sure the name is a valid field on the given class
-        if name not in data_model_class.fields:
+        if (
+            name not in data_model_class.fields
+            and name not in data_model_class._fields_oneofs_map
+        ):
             error(
                 "<COR85037211E>",
                 AttributeError(
                     f"No such attribute [{name}] on [{data_model_class.__name__}]"
                 ),
             )
```

### Comparing `caikit-0.4.3/caikit/core/data_model/dataobject.py` & `caikit-0.4.4/caikit/core/data_model/dataobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,24 +63,19 @@
         """When instantiating a new DataObject class, the proto class will not
         yet have been generated, but the set of fields will be known since the
         class will be the raw input representation of a @dataclass
         """
 
         # Get the annotations that will go into the dataclass
         if name != "DataObjectBase":
-            raw_field_names = attrs.get("__annotations__")
-            if raw_field_names is None:
+            field_names = attrs.get("__annotations__")
+            if field_names is None:
                 raise TypeError(
                     "All DataObjectBase classes must follow dataclass syntax"
                 )
-
-            # TODO: Sort out oneof field names
-            field_names = list(raw_field_names.keys())
-
-            # Add the forward declaration
             attrs[_DataBaseMetaClass._FWD_DECL_FIELDS] = field_names
 
         # Delegate to the base metaclass
         return super().__new__(mcs, name, bases, attrs)
 
 
 class DataObjectBase(DataBase, metaclass=_DataObjectBaseMetaClass):
@@ -125,55 +120,35 @@
             "{} must inherit from DataObjectBase/Enum when using @dataobject",
             cls.__name__,
         )
 
         # Add the package to the kwargs
         kwargs.setdefault("package", package)
 
-        # If there's a schema in the keyword args, use jtd_to_proto
-        schema = kwargs.pop("schema", None)
-        if schema is not None:
-            log.debug("Using JTD To Proto")
-            kwargs.setdefault("validate_jtd", True)
-            descriptor = py_to_proto.jtd_to_proto(
-                name=cls.__name__,
-                jtd_def=schema,
-                **kwargs,
-            )
-        # If it's already a dataclass, convert it directly
-        else:
-            log.debug("Using dataclass/enum to proto on dataclass")
-
-            # If it's not an enum, fill in any missing field defaults as None
-            # and make sure it's a dataclass
-            if not issubclass(cls, Enum):
-                log.debug2("Wrapping data class %s", cls)
-                user_defined_defaults = {}
-                for annotation in getattr(cls, "__annotations__", {}):
-                    user_defined_default = getattr(cls, annotation, dataclasses.MISSING)
-                    if user_defined_default == dataclasses.MISSING:
-                        log.debug3("Filling in None default for %s.%s", cls, annotation)
-                        setattr(cls, annotation, None)
-                    else:
-                        user_defined_defaults[annotation] = user_defined_default
-                # If the current __init__ is auto-generated by dataclass, remove
-                # it so that a new one is created with the new defaults. This is
-                # a little hard to detect across different python versions, so
-                # the most reliable way is to assume that the only place
-                # __annotations__ are added to the __init__ function itself are
-                # in dataclass. If cls is either not a dataclass or is a
-                # dataclass with a non-default __init__, there will not be
-                # annotations
-                if getattr(cls.__init__, "__annotations__", None):
-                    log.debug3("Resetting default dataclass init")
-                    delattr(cls, "__init__")
-                cls = dataclasses.dataclass(cls)
-                setattr(cls, _USER_DEFINED_DEFAULTS, user_defined_defaults)
+        # If it's not an enum, fill in any missing field defaults as None
+        # and make sure it's a dataclass
+        if not issubclass(cls, Enum):
+            log.debug2("Wrapping data class %s", cls)
+            user_defined_defaults = {}
+            for annotation in getattr(cls, "__annotations__", {}):
+                user_defined_default = getattr(cls, annotation, dataclasses.MISSING)
+                if user_defined_default == dataclasses.MISSING:
+                    log.debug3("Filling in None default for %s.%s", cls, annotation)
+                    setattr(cls, annotation, None)
+                else:
+                    user_defined_defaults[annotation] = user_defined_default
+            # If the current __init__ is auto-generated by dataclass, remove
+            # it so that a new one is created with the new defaults
+            if _has_dataclass_init(cls):
+                log.debug3("Resetting default dataclass init")
+                delattr(cls, "__init__")
+            cls = dataclasses.dataclass(cls)
+            setattr(cls, _USER_DEFINED_DEFAULTS, user_defined_defaults)
 
-            descriptor = _dataobject_to_proto(dataclass_=cls, **kwargs)
+        descriptor = _dataobject_to_proto(dataclass_=cls, **kwargs)
 
         # Create the message class from the dataclass
         proto_class = py_to_proto.descriptor_to_message_class(descriptor)
         _AUTO_GEN_PROTO_CLASSES.append(proto_class)
 
         # Add enums to the global enums module
         for enum_class in _get_all_enums(proto_class):
@@ -181,14 +156,21 @@
             enums.import_enum(enum_class)
 
         # Declare the merged class that binds DataBase to the wrapped class with
         # this generated proto class
         if isinstance(proto_class, type):
             setattr(cls, "_proto_class", proto_class)
             cls = _make_data_model_class(proto_class, cls)
+
+            # If this was a default-generated dataclass __init__ and there are
+            # any oneofs, we need to augment the __init__ to support kwargs for
+            # the individual fields
+            if _has_dataclass_init(cls) and cls._fields_oneofs_map:
+                setattr(cls, "__init__", _make_oneof_init(cls))
+
         else:
             enums.import_enum(proto_class, cls)
             setattr(cls, "_proto_enum", proto_class)
 
         # Return the decorated class
         return cls
 
@@ -317,7 +299,69 @@
         setattr(
             cls,
             nested_enum_descriptor.name,
             getattr(enums, nested_enum_descriptor.name),
         )
 
     return cls
+
+
+def _make_oneof_init(cls):
+    """Helper to augment a defaulted dataclass __init__ to support kwargs for
+    oneof fields
+    """
+    original_init = cls.__init__
+    fields_to_oneofs = cls._fields_to_oneof
+    oneofs_to_fields = cls._fields_oneofs_map
+
+    def __init__(self, *args, **kwargs):
+        new_kwargs = {}
+        to_remove = []
+        which_oneof = {}
+        for field_name, val in kwargs.items():
+            if oneof_name := fields_to_oneofs.get(field_name):
+                oneof_pos_idx = list(cls.__dataclass_fields__.keys()).index(oneof_name)
+                has_pos_val = len(args) > oneof_pos_idx
+                if has_pos_val:
+                    error(
+                        "<COR09282193E>",
+                        TypeError(
+                            "Received conflicting oneof args/kwargs for {}/{}".format(
+                                oneof_name,
+                                field_name,
+                            )
+                        ),
+                    )
+
+                other_oneof_fields = (
+                    field
+                    for field in [oneof_name] + oneofs_to_fields[oneof_name]
+                    if field != field_name
+                )
+                if any(field in kwargs for field in other_oneof_fields):
+                    error(
+                        "<COR59933157E>",
+                        TypeError(
+                            "Received multiple keyword arguments for oneof {}".format(
+                                oneof_name,
+                            )
+                        ),
+                    )
+                new_kwargs[oneof_name] = val
+                to_remove.append(field_name)
+                which_oneof[oneof_name] = field_name
+
+        for kwarg in to_remove:
+            del kwargs[kwarg]
+        kwargs.update(new_kwargs)
+        original_init(self, *args, **kwargs)
+        setattr(self, _DataBaseMetaClass._WHICH_ONEOF_ATTR, which_oneof)
+
+    return __init__
+
+
+def _has_dataclass_init(cls) -> bool:
+    """When the dataclass decorator adds an __init__ to a class, it adds
+    __annotations__ to the init function itself. This function uses that fact to
+    detect if the class's __init__ function was generated by @dataclass
+    """
+    return bool(getattr(cls.__init__, "__annotations__", None))
```

### Comparing `caikit-0.4.3/caikit/core/data_model/enums.py` & `caikit-0.4.4/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/producer.py` & `caikit-0.4.4/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.4.4/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/streams/__init__.py` & `caikit-0.4.4/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/streams/converter.py` & `caikit-0.4.4/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.4.4/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/streams/data_stream.py` & `caikit-0.4.4/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/streams/resolver.py` & `caikit-0.4.4/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/data_model/streams/validator.py` & `caikit-0.4.4/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/model_manager.py` & `caikit-0.4.4/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module.py` & `caikit-0.4.4/caikit/core/module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module_backend_config.py` & `caikit-0.4.4/caikit/core/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module_backends/__init__.py` & `caikit-0.4.4/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module_backends/backend_types.py` & `caikit-0.4.4/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module_backends/base.py` & `caikit-0.4.4/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module_backends/local_backend.py` & `caikit-0.4.4/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module_config.py` & `caikit-0.4.4/caikit/core/module_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module_meta.py` & `caikit-0.4.4/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/module_type.py` & `caikit-0.4.4/caikit/core/module_type.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/resources/__init__.py` & `caikit-0.4.4/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/resources/base.py` & `caikit-0.4.4/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/task.py` & `caikit-0.4.4/caikit/core/task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/__init__.py` & `caikit-0.4.4/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/compatibility.py` & `caikit-0.4.4/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/errors/__init__.py` & `caikit-0.4.4/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.4.4/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.4.4/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/fileio.py` & `caikit-0.4.4/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/isa.py` & `caikit-0.4.4/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/logging.py` & `caikit-0.4.4/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.4.4/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/serializers.py` & `caikit-0.4.4/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/toolkit/wip_decorator.py` & `caikit-0.4.4/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/workflows/__init__.py` & `caikit-0.4.4/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/core/workflows/base.py` & `caikit-0.4.4/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/interfaces/__init__.py` & `caikit-0.4.4/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/interfaces/common/__init__.py` & `caikit-0.4.4/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.4.4/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/interfaces/common/data_model/producer.py` & `caikit-0.4.4/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/interfaces/runtime/__init__.py` & `caikit-0.4.4/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.4.4/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.4.4/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/__init__.py` & `caikit-0.4.4/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/dump_services.py` & `caikit-0.4.4/caikit/runtime/dump_services.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 # Standard
 import sys
 
 # Local
 from ..core.data_model import render_dataobject_protos
 from .service_factory import ServicePackageFactory
+import caikit
 
 
 def dump_services(output_dir: str):
     """
     Utility for rendering the all generated interfaces to proto files
     """
     inf_svc = ServicePackageFactory.get_service_package(
@@ -42,8 +43,11 @@
     train_svc.service.write_proto_file(output_dir)
     train_mgt_svc.service.write_proto_file(output_dir)
 
 
 if __name__ == "__main__":
     assert len(sys.argv) == 2, f"Usage: {sys.argv[0]} <output_dir>"
     out_dir = sys.argv[1]
+    # Set up logging so users can set LOG_LEVEL etc
+    caikit.core.toolkit.logging.configure()
+
     dump_services(out_dir)
```

### Comparing `caikit-0.4.3/caikit/runtime/grpc_server.py` & `caikit-0.4.4/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/interceptors/__init__.py` & `caikit-0.4.4/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.4.4/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/metrics/__init__.py` & `caikit-0.4.4/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.4.4/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/model_management/__init__.py` & `caikit-0.4.4/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/model_management/batcher.py` & `caikit-0.4.4/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/model_management/loaded_model.py` & `caikit-0.4.4/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/model_management/model_loader.py` & `caikit-0.4.4/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/model_management/model_manager.py` & `caikit-0.4.4/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/model_management/model_sizer.py` & `caikit-0.4.4/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/model_management/training_manager.py` & `caikit-0.4.4/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/__init__.py` & `caikit-0.4.4/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.4.4/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.4.4/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.4.4/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.4.4/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.4.4/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.4.4/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.4.4/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.4.4/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.4.4/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_factory.py` & `caikit-0.4.4/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.4.4/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.4.4/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/create_service.py` & `caikit-0.4.4/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.4.4/caikit/runtime/service_generation/data_stream_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 from datetime import datetime
 from glob import glob
-from typing import Any, Optional, Type
+from typing import Any, List, Optional, Type, Union
 import os
 import sys
 
 # Third Party
 from google.protobuf.message import Message as ProtoMessageType
 import grpc
 
 # First Party
+from py_to_proto.dataclass_to_proto import Annotated, OneofField
 import alog
 
 # Local
 from caikit.core.data_model.base import DataBase
 from caikit.core.data_model.dataobject import (
     DataObjectBase,
     _DataObjectBaseMetaClass,
+    _make_oneof_init,
     dataobject,
 )
 from caikit.core.data_model.streams.data_stream import DataStream
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 import caikit
 
 # This global holds the mapping of element types to their respective
@@ -59,24 +61,14 @@
     """This base class acts as a sentinel so that dynamically generated data
     stream source classes can be identified programmatically.
     """
 
     def __init__(self):
         """Validate oneof semantics"""
         super().__init__(lambda: self.to_data_stream().generator_func())
-        self._set_fields = {
-            f.name: getattr(self, f.name)
-            for f in self.get_proto_class().DESCRIPTOR.oneofs[0].fields
-            if getattr(self, f.name) is not None
-        }
-        if len(self._set_fields) > 1:
-            raise CaikitRuntimeException(
-                grpc.StatusCode.INVALID_ARGUMENT,
-                f"Multiple oneof fields set: {self._set_fields.keys()}",
-            )
 
     def __getstate__(self) -> bytes:
         """A DataStreamSource is pickled by serializing its source
         representation. This is particularly useful when sharing data streams
         across subprocesses to run training in an isolated process.
         """
         return self.to_binary_buffer()
@@ -84,19 +76,15 @@
     def __setstate__(self, pickle_bytes: bytes):
         """Unpickling a DataStreamSource basically involves unpacking the
         serialized source representation. The catch is that the oneof is
         represented strangely in __dict__, so we need to explicitly set all
         oneof members.
         """
         new_inst = self.__class__.from_binary_buffer(pickle_bytes)
-        new_inst_dict = new_inst.__dict__
-        self.__dict__.update(new_inst_dict)
-        for field_descriptor in self.get_proto_class().DESCRIPTOR.oneofs[0].fields:
-            field_name = field_descriptor.name
-            setattr(self, field_name, getattr(new_inst, field_name))
+        setattr(self, new_inst.which_oneof("data_stream"), new_inst.data_stream)
 
     # pylint: disable=too-many-return-statements
     def to_data_stream(self) -> DataStream:
         """Convert to the target data stream type based on the source type"""
 
         # Determine which of the value types is set
         set_field = None
@@ -212,90 +200,122 @@
     """Dynamically create a data stream source message type that supports
     pulling an iterable of the given type from all valid data stream sources
     """
     log.debug2("Looking for DataStreamSource[%s]", data_element_type)
     if data_element_type not in _DATA_STREAM_SOURCE_TYPES:
         cls_name = _make_data_stream_source_type_name(data_element_type)
         log.debug("Creating DataStreamSource[%s] -> %s", data_element_type, cls_name)
-        element_type = (
-            data_element_type.get_proto_class().DESCRIPTOR
-            if isinstance(data_element_type, type)
-            and issubclass(data_element_type, DataBase)
-            else _NATIVE_TYPE_TO_JTD[data_element_type]
+
+        # Set up the "sub classes." In python, this is the same as creating a
+        # standalone class with a __qualname__ that nests it under a parent
+        # class. We do this outside the declaration of the parent class so that
+        # these classes can be referenced within the Union annotation for the
+        # outer class itself.
+        package = "caikit_data_model.runtime"
+        JsonData = dataobject(package=package, name=f"{cls_name}JsonData")(
+            _DataObjectBaseMetaClass.__new__(
+                _DataObjectBaseMetaClass,
+                name="JsonData",
+                bases=(DataObjectBase,),
+                attrs={
+                    "__annotations__": {"data": List[data_element_type]},
+                    "__qualname__": f"{cls_name}.JsonData",
+                },
+            ),
         )
-        schema = {
-            "properties": {
-                "data_stream": {
-                    "discriminator": "data_reference_type",
-                    "mapping": {
-                        "JsonData": {
-                            "properties": {
-                                "data": {
-                                    "elements": {"type": element_type},
-                                },
-                            },
-                        },
-                        "File": {"properties": {"filename": {"type": "string"}}},
-                        "ListOfFiles": {
-                            "properties": {
-                                "files": {
-                                    "elements": {"type": "string"},
-                                },
-                            },
-                        },
-                        "Directory": {
-                            "properties": {
-                                "dirname": {"type": "string"},
-                                "extension": {"type": "string"},
-                            }
-                        },
+        File = dataobject(package=package, name=f"{cls_name}File")(
+            _DataObjectBaseMetaClass.__new__(
+                _DataObjectBaseMetaClass,
+                name="File",
+                bases=(DataObjectBase,),
+                attrs={
+                    "__annotations__": {"filename": str},
+                    "__qualname__": f"{cls_name}.File",
+                },
+            ),
+        )
+        ListOfFiles = dataobject(package=package, name=f"{cls_name}ListOfFiles")(
+            _DataObjectBaseMetaClass.__new__(
+                _DataObjectBaseMetaClass,
+                name="ListOfFiles",
+                bases=(DataObjectBase,),
+                attrs={
+                    "__annotations__": {"files": List[str]},
+                    "__qualname__": f"{cls_name}.ListOfFiles",
+                },
+            ),
+        )
+        Directory = dataobject(package=package, name=f"{cls_name}Directory")(
+            _DataObjectBaseMetaClass.__new__(
+                _DataObjectBaseMetaClass,
+                name="Directory",
+                bases=(DataObjectBase,),
+                attrs={
+                    "__annotations__": {
+                        "dirname": str,
+                        "extension": str,
                     },
-                }
-            }
-        }
-        # TODO: Once full oneof support is implemented, this can move to using
-        #   the proper @dataclass style. In the meantime, the "schema" version
-        #   that uses JTD is still supported so that this oneof can be
-        #   dynamically declared. In order to make this work, the
-        #   _DataObjectBaseMetaClass needs to pre-know the right set of field
-        #   names for the oneof fields as if this were a dataclass. The values
-        #   of these annotations are unused since this will never be made into a
-        #   true @dataclass.
-        annotations = {
-            name.lower(): None
-            for name in schema["properties"]["data_stream"]["mapping"]
-        }
-        data_object = dataobject(schema=schema, package="caikit_data_model.runtime",)(
+                    "__qualname__": f"{cls_name}.Directory",
+                },
+            ),
+        )
+
+        # Create the outer class that encapsulates the Union (oneof) or the
+        # various types of input sources
+        data_object = dataobject(package=package)(
             _DataObjectBaseMetaClass.__new__(
                 _DataObjectBaseMetaClass,
                 name=cls_name,
                 bases=(DataObjectBase, DataStreamSourceBase),
                 attrs={
                     "ELEMENT_TYPE": data_element_type,
-                    "__annotations__": annotations,
+                    JsonData.__name__: JsonData,
+                    File.__name__: File,
+                    ListOfFiles.__name__: ListOfFiles,
+                    Directory.__name__: Directory,
+                    "__annotations__": {
+                        "data_stream": Union[
+                            Annotated[JsonData, OneofField(JsonData.__name__.lower())],
+                            Annotated[File, OneofField(File.__name__.lower())],
+                            Annotated[
+                                ListOfFiles, OneofField(ListOfFiles.__name__.lower())
+                            ],
+                            Annotated[
+                                Directory, OneofField(Directory.__name__.lower())
+                            ],
+                        ],
+                    },
                 },
             )
         )
+
+        # Add this data stream source to the common data model and the module
+        # where it was declared
         setattr(
             caikit.interfaces.common.data_model,
             cls_name,
             data_object,
         )
         setattr(
             sys.modules[data_object.__module__],
             cls_name,
             data_object,
         )
 
         # Add an init that sequences the initialization so that
         # DataStreamSourceBase is initialized after DataBase
-        orig_init = _DataObjectBaseMetaClass._make_init(data_object.fields)
+        orig_init = _make_oneof_init(data_object)
 
         def __init__(self, *args, **kwargs):
-            orig_init(self, *args, **kwargs)
+            try:
+                orig_init(self, *args, **kwargs)
+            except TypeError as err:
+                raise CaikitRuntimeException(
+                    grpc.StatusCode.INVALID_ARGUMENT, str(err)
+                ) from err
             DataStreamSourceBase.__init__(self)
 
         setattr(data_object, "__init__", __init__)
 
         _DATA_STREAM_SOURCE_TYPES[data_element_type] = data_object
 
     # Return the global stream source object for this element type
```

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/primitives.py` & `caikit-0.4.4/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/rpcs.py` & `caikit-0.4.4/caikit/runtime/service_generation/rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.4.4/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.4.4/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/servicers/__init__.py` & `caikit-0.4.4/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.4.4/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.4.4/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.4.4/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.4.4/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.4.4/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/types/__init__.py` & `caikit-0.4.4/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/types/aborted_exception.py` & `caikit-0.4.4/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.4.4/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.4.4/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/utils/__init__.py` & `caikit-0.4.4/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/utils/import_util.py` & `caikit-0.4.4/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/utils/servicer_util.py` & `caikit-0.4.4/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/work_management/__init__.py` & `caikit-0.4.4/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/work_management/abortable_action.py` & `caikit-0.4.4/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/work_management/call_aborter.py` & `caikit-0.4.4/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.4.4/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/docs/adrs/010-data-model-definition.md` & `caikit-0.4.4/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/docs/adrs/015-runtime-service-generation.md` & `caikit-0.4.4/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/docs/adrs/018-shared-backends.md` & `caikit-0.4.4/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/docs/adrs/019-loader-stack.md` & `caikit-0.4.4/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/docs/architecture_club/04-25-23.md` & `caikit-0.4.4/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/start_runtime_with_sample_lib.py` & `caikit-0.4.4/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/README.md` & `caikit-0.4.4/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/client.py` & `caikit-0.4.4/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.4.4/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/start_runtime.py` & `caikit-0.4.4/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.4.4/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.4.4/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.4.4/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.4.4/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.4.4/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py` & `caikit-0.4.4/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/pyproject.toml` & `caikit-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.4.3"
+version = "0.4.4"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `caikit-0.4.3/scripts/check_deps.sh` & `caikit-0.4.4/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/scripts/fmt.sh` & `caikit-0.4.4/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/__init__.py` & `caikit-0.4.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/base.py` & `caikit-0.4.4/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/config/test_configs.py` & `caikit-0.4.4/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/conftest.py` & `caikit-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.4.4/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.4.4/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/blocks/__init__.py` & `caikit-0.4.4/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/blocks/test_base.py` & `caikit-0.4.4/tests/core/blocks/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.4.4/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,14 +124,27 @@
         sub_msg1, sub_msg2 = sub_msgs
         assert sub_msg1.foo == data_dict["some_foos"][0]["foo"]
         assert sub_msg1.bar == data_dict["some_foos"][0]["bar"]
         assert sub_msg2.foo == data_dict["some_foos"][1]["foo"]
         assert sub_msg2.bar == data_dict["some_foos"][1]["bar"]
 
 
+def test_dict_backend_oneof():
+    """Make sure that a oneof can be correctly accessed from a backend"""
+    with temp_data_model(make_proto_def({"Foo": {"foo": "Union[str, int]"}})) as dm:
+        assert hasattr(dm, "Foo")
+        assert issubclass(dm.Foo, DataBase)
+
+        data_dict = {"foo": "asdf"}
+        backend = DictBackend(data_dict)
+        msg = dm.Foo.from_backend(backend)
+        assert msg.foo == "asdf"
+        assert msg.which_oneof("foo") == "foostr"
+
+
 def test_dict_backend_invalid_field_error():
     """Make sure that an AttributeError is raised if an invalid field is
     requested
     """
     with temp_data_model(
         make_proto_def(
             {
```

### Comparing `caikit-0.4.3/tests/core/data_model/streams/test_converter.py` & `caikit-0.4.4/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.4.4/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.4.4/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/data_model/streams/test_resolver.py` & `caikit-0.4.4/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/data_model/streams/test_validator.py` & `caikit-0.4.4/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/data_model/test_base.py` & `caikit-0.4.4/tests/core/data_model/test_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 # Third Party
 import pytest
 
 # Local
 from caikit.core.data_model.base import DataBase
 from caikit.core.data_model.data_backends.base import DataModelBackendBase
+from caikit.core.data_model.dataobject import DataObjectBase
 from tests.data_model_helpers import (
     justify_script_string,
     make_proto_def,
     temp_data_model,
     temp_module,
 )
 
@@ -126,14 +127,16 @@
         ) as handle:
             handle.write(
                 justify_script_string(
                     """
                     class FakeDescriptor:
                         fields = []
                         fields_by_name = {}
+                        oneofs_by_name = {}
+                        oneofs = []
                         name = "Baz"
                         full_name = "foo.bar.Baz"
 
                     class Object:
                         DESCRIPTOR = FakeDescriptor
                     """
                 )
@@ -157,14 +160,94 @@
         # Make sure the import succeeds and that the data model class has the
         # right inheritance
         lib = importlib.import_module(".".join([mod_name, "object"]))
         assert hasattr(lib, "Object")
         assert issubclass(lib.Object, DataBase)
 
 
+def test_compiled_proto_init():
+    """Make sure that support for 'compiled' protos works cleanly without using
+    the dataobject wrapper
+    """
+    # pylint: disable=duplicate-code
+    with temp_data_model(
+        make_proto_def(
+            {
+                "ThingOne": {
+                    "foo": str,
+                    "bar": int,
+                }
+            },
+            mock_compiled=True,
+        )
+    ) as dm:
+        assert isinstance(dm.ThingOne, type)
+        assert issubclass(dm.ThingOne, DataBase)
+        assert not issubclass(dm.ThingOne, DataObjectBase)
+        assert dm.ThingOne.fields == ("foo", "bar")
+
+        # Test construction with positional args
+        inst = dm.ThingOne("foo", 1)
+        assert inst.foo == "foo"
+        assert inst.bar == 1
+
+        # Test construction with keyword args
+        inst = dm.ThingOne(foo="foo", bar=1)
+        assert inst.foo == "foo"
+        assert inst.bar == 1
+
+        # Test defaulting to None
+        inst = dm.ThingOne()
+        assert inst.foo is None
+        assert inst.bar is None
+
+        # Test error cases for construction
+        with pytest.raises(TypeError):
+            dm.ThingOne("foo", foo="bar")
+        with pytest.raises(TypeError):
+            dm.ThingOne(widget="qewr")
+        with pytest.raises(TypeError):
+            dm.ThingOne("foo", 1, 2)
+
+
+def test_compiled_proto_oneof():
+    """Make sure that support for 'compiled' protos works cleanly without using
+    the dataobject wrapper
+    """
+    # pylint: disable=duplicate-code
+    with temp_data_model(
+        make_proto_def(
+            {
+                "ThingOne": {
+                    "foo": "Union[str, int]",
+                }
+            },
+            mock_compiled=True,
+        )
+    ) as dm:
+        assert isinstance(dm.ThingOne, type)
+        assert issubclass(dm.ThingOne, DataBase)
+        assert not issubclass(dm.ThingOne, DataObjectBase)
+        assert set(dm.ThingOne.fields) == {"foostr", "fooint"}
+
+        # Construct with the oneof name
+        inst = dm.ThingOne(foo=1)
+        assert inst.foo == 1
+        assert inst.which_oneof("foo") == "fooint"
+
+        # Construct with field name
+        inst = dm.ThingOne(foostr="asdf")
+        assert inst.foo == "asdf"
+        assert inst.which_oneof("foo") == "foostr"
+
+        # Conflicting args
+        with pytest.raises(TypeError):
+            dm.ThingOne(foo=1, fooster="asdf")
+
+
 ##################
 ## Data Backend ##
 ##################
 
 
 def test_cached_backend():
     """Make sure that a data model object will cache the result of get_attribute
@@ -220,14 +303,34 @@
         msg.bar
         msg.bar
         msg.bar
         assert backend.access_count("foo") == 2
         assert backend.access_count("bar") == 3
 
 
+def test_invalid_attribute_no_backend():
+    """Make sure that when created without a backend and without proper
+    initialization, an AttributeError is raised
+    """
+    # pylint: disable=duplicate-code
+    with temp_data_model(
+        make_proto_def(
+            {
+                "ThingOne": {
+                    "foo": str,
+                    "bar": int,
+                }
+            }
+        )
+    ) as dm:
+        msg = dm.ThingOne.__new__(dm.ThingOne)
+        with pytest.raises(AttributeError):
+            msg.foo
+
+
 ##################
 ## Default Init ##
 ##################
 
 
 def test_default_init_valid_args():
     """Make sure that valid ways of using the default __init__ all work as
```

### Comparing `caikit-0.4.3/tests/core/data_model/test_dataobject.py` & `caikit-0.4.4/tests/core/data_model/test_dataobject.py`

 * *Files 7% similar despite different names*

```diff
@@ -109,30 +109,14 @@
     assert inst.foo == "test"
     assert inst.bar == 1
     inst = Foo()
     assert inst.foo is None
     assert inst.bar is None
 
 
-def test_dataobject_jtd():
-    """Make sure that a simple usage of dataobject using a full JTD schema works
-    as expected
-    """
-
-    @dataobject(schema={"properties": {"foo": {"type": "string"}}})
-    class Foo(DataObjectBase):
-        foo: str
-
-    assert check_field_type(Foo.get_proto_class(), "foo", "TYPE_STRING")
-    inst = Foo(foo="test")
-    assert inst.foo == "test"
-    inst = Foo()
-    assert inst.foo is None
-
-
 def test_dataobject_nested_objects():
     """Make sure that nested objects are handled correctly"""
 
     @dataobject
     class Foo(DataObjectBase):
         @dataobject
         class Bar(DataObjectBase):
@@ -275,23 +259,14 @@
         )
     for field in ["bar", "optionalBar"]:
         assert check_field_enum_type(
             FooBar._proto_class, field, BarEnum._proto_enum.DESCRIPTOR
         )
 
 
-def test_dataobject_invalid_schema():
-    """Make sure that a ValueError is raised on an invalid schema"""
-    with pytest.raises(ValueError):
-        # pylint: disable=unused-variable
-        @dataobject(schema="Foo")
-        class Foo:
-            pass
-
-
 def test_dataobject_additional_methods():
     """Make sure that additional methods on wrapped classes (for messages and
     enums) are preserved
     """
 
     @dataobject
     class Foo(Enum):
@@ -368,137 +343,122 @@
         assert rendered_files == {
             BarEnum._proto_enum.DESCRIPTOR.file.name,
             Foo.get_proto_class().DESCRIPTOR.file.name,
             FooBar.get_proto_class().DESCRIPTOR.file.name,
         }
 
 
-def test_dataobject_with_discriminator():
-    """Make sure that adding a discriminator works as expected"""
-
-    @dataobject(
-        schema={
-            "properties": {
-                "data_stream": {
-                    "discriminator": "data_reference_type",
-                    "mapping": {
-                        "Foo": {
-                            "properties": {
-                                "data": {
-                                    "elements": {"type": "string"},
-                                },
-                            },
-                        },
-                        "Bar": {"properties": {"data": {"type": "string"}}},
-                        "Baz": {
-                            "properties": {
-                                "data": {
-                                    "elements": {"type": "string"},
-                                },
-                            },
-                        },
-                        "Bat": {
-                            "properties": {
-                                "data1": {"type": "string"},
-                                "data2": {"type": "string"},
-                            }
-                        },
-                    },
-                }
-            }
-        }
-    )
-    class BazObj(DataObjectBase):
-        foo: str
-        bar: str
-        baz: str
-        bat: str
-
-    # proto tests
-    foo1 = BazObj(foo=BazObj.Foo(data=["hello"]))
-    proto_repr_foo = foo1.to_proto()
-    assert proto_repr_foo.foo.data == ["hello"]
-    assert BazObj.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
-
-    bar1 = BazObj(foo=BazObj.Foo(data=["hello"]), bar=BazObj.Bar(data="world"))
-    proto_repr_bar = bar1.to_proto()
-    assert proto_repr_bar.bar.data == "world"
-
-    # json tests
-    foo1 = BazObj(foo=BazObj.Foo(data=["hello"]))
-    json_repr_foo = foo1.to_json()
-    assert json.loads(json_repr_foo) == {
-        "foo": {"data": ["hello"]},
-        "bar": None,
-        "baz": None,
-        "bat": None,
-    }
-
-
 def test_dataobject_with_oneof():
     """Make sure that using a Union to create a oneof works as expected"""
 
     @dataobject
     class BazObj(DataObjectBase):
-        _private_slots = ("_which_oneof_datastream",)
-
         @dataobject
         class Foo(DataObjectBase):
             data: List[str]
 
         @dataobject
         class Bar(DataObjectBase):
             data: str
 
         data_stream: Union[
             Annotated[Foo, FieldNumber(1), OneofField("foo")],
             Annotated[Bar, FieldNumber(2), OneofField("bar")],
         ]
 
-        def __getattr__(self, name):
-            if name == "data_stream":
-                if self._which_oneof_datastream == "foo":
-                    return self.foo
-                elif self._which_oneof_datastream == "bar":
-                    return self.bar
-                return None
-            if name == "_foo":
-                if self._which_oneof_datastream == "foo":
-                    return self._data_stream
-            if name == "_bar":
-                if self._which_oneof_datastream == "bar":
-                    return self._data_stream
-
-        def __init__(self, *args, **kwargs):
-            if "foo" in kwargs:
-                self._which_oneof_datastream = "foo"
-                self._data_stream = kwargs["foo"]
-            if "bar" in kwargs:
-                self._which_oneof_datastream = "bar"
-                self._data_stream = kwargs["bar"]
-
-    # proto tests
+    # Construct with oneof field name
     foo1 = BazObj(foo=BazObj.Foo(data=["hello"]))
     assert isinstance(foo1.data_stream, BazObj.Foo)
+    assert foo1.which_oneof("data_stream") == "foo"
+    assert foo1.foo is foo1.data_stream
+    assert foo1.bar is None
+
+    # Test other oneof field name
+    bar1 = BazObj(bar=BazObj.Bar(data="world"))
+    assert isinstance(bar1.data_stream, BazObj.Bar)
+    assert bar1.which_oneof("data_stream") == "bar"
+    assert bar1.bar is bar1.data_stream
+    assert bar1.foo is None
+
+    # Test proto round trip
     proto_repr_foo = foo1.to_proto()
     assert proto_repr_foo.foo.data == ["hello"]
     assert BazObj.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
-
-    bar1 = BazObj(foo=BazObj.Foo(data=["hello"]), bar=BazObj.Bar(data="world"))
-    assert isinstance(bar1.data_stream, BazObj.Bar)
     proto_repr_bar = bar1.to_proto()
     assert proto_repr_bar.bar.data == "world"
 
-    # json tests
-    foo1 = BazObj(foo=BazObj.Foo(data=["hello"]))
+    # Test json round trip
     json_repr_foo = foo1.to_json()
     assert json.loads(json_repr_foo) == {
         "foo": {"data": ["hello"]},
         "bar": None,
     }
+    assert BazObj.from_json(json_repr_foo) == foo1
+
+    # Test setattr
+    foo1.bar = BazObj.Bar(data="it's a bar")
+    assert foo1.which_oneof("data_stream") == "bar"
+    assert foo1.data_stream is foo1.bar
+    assert foo1.foo is None
+
+    # Construct with oneof name
+    foo2 = BazObj(data_stream=BazObj.Foo(data=["some", "foo"]))
+    assert foo2.data_stream.data == ["some", "foo"]
+    assert foo2.bar is None
+    assert foo2.foo is foo2.data_stream
+    assert foo2.which_oneof("data_stream") == "foo"
+
+    # Assign with oneof name
+    foo2.data_stream = BazObj.Bar(data="asdf")
+    assert foo2.foo is None
+    assert foo2.bar is foo2.data_stream
+    assert foo2.which_oneof("data_stream") == "bar"
+
+    # Construct with positional oneof name
+    foo2 = BazObj(BazObj.Foo(data=["some", "foo"]))
+    assert foo2.data_stream.data == ["some", "foo"]
+    assert foo2.bar is None
+    assert foo2.foo is foo2.data_stream
+    assert foo2.which_oneof("data_stream") == "foo"
+
+    foo3 = BazObj()
+    assert foo3.foo is None
+    assert foo3.bar is None
+    assert foo3.data_stream is None
+    assert foo3.which_oneof("data_stream") == None
+    # Invalid constructors
+    with pytest.raises(TypeError):
+        BazObj(BazObj.Foo(), foo=BazObj.Foo())
+    with pytest.raises(TypeError):
+        BazObj(data_stream=BazObj.Foo(), foo=BazObj.Foo())
+    with pytest.raises(TypeError):
+        BazObj(foo=BazObj.Foo(), bar=BazObj.Bar())
+
+
+def test_dataobject_with_same_type_of_oneof():
+    """Make sure that using a Union to create a oneof with the same types works as expected"""
+
+    @dataobject
+    class Foo(DataObjectBase):
+        foo: Union[
+            Annotated[bool, FieldNumber(10), OneofField("foo_bool1")],
+            Annotated[bool, FieldNumber(20), OneofField("foo_bool2")],
+        ]
+
+    # if the fields are of the same type, then by default the first one is set
+    foo1 = Foo(True)
+    assert foo1.which_oneof("foo") == "foo_bool1"
+    assert foo1.foo_bool1
+    assert foo1.foo_bool2 == None
+
+    # unless set explicitly
+    foo2 = Foo(foo_bool2=True)
+    assert foo2.which_oneof("foo") == "foo_bool2"
+    assert foo2.foo_bool1 == None
+    assert foo2.foo_bool2
 
 
 def test_dataobject_round_trip_json():
     """Make sure that a dataobject class can serialize to/from json"""
 
     @dataobject
     class BazObj(DataObjectBase):
```

### Comparing `caikit-0.4.3/tests/core/data_model/test_enums.py` & `caikit-0.4.4/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/data_model/test_producer.py` & `caikit-0.4.4/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/helpers.py` & `caikit-0.4.4/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/module_backends/test_backend_types.py` & `caikit-0.4.4/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/test_imports.py` & `caikit-0.4.4/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/test_model_manager.py` & `caikit-0.4.4/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/test_module.py` & `caikit-0.4.4/tests/core/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/test_module_backend_config.py` & `caikit-0.4.4/tests/core/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/test_module_metadata.py` & `caikit-0.4.4/tests/core/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/test_module_type.py` & `caikit-0.4.4/tests/core/test_module_type.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/test_no_write_permissions.py` & `caikit-0.4.4/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/test_task.py` & `caikit-0.4.4/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/toolkit/test_compatibility.py` & `caikit-0.4.4/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/toolkit/test_error_handler.py` & `caikit-0.4.4/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/toolkit/test_fileio.py` & `caikit-0.4.4/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.4.4/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/toolkit/test_serializers.py` & `caikit-0.4.4/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.4.4/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/workflows/__init__.py` & `caikit-0.4.4/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/core/workflows/test_base.py` & `caikit-0.4.4/tests/core/workflows/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/data_model_helpers.py` & `caikit-0.4.4/tests/data_model_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -143,28 +143,65 @@
         return field_val.__name__
     if isinstance(field_val, list):
         assert len(field_val) == 1
         return f"List[{_get_proto_val_name(field_val[0])}]"
     raise RuntimeError(f"Invalid field type specifier: {field_val}")
 
 
-def make_proto_def(message_specs: Dict[str, dict], pkg_suffix: str = None) -> str:
+def make_proto_def(
+    message_specs: Dict[str, dict],
+    pkg_suffix: str = None,
+    mock_compiled: bool = False,
+) -> str:
     """Helper for writing a syntatically correct protobufs file"""
     if pkg_suffix is None:
         pkg_suffix = _random_package_suffix()
     package_name = f"{caikit.core.data_model.CAIKIT_DATA_MODEL}.{pkg_suffix}"
     out = justify_script_string(
         """
-        from typing import Dict, List
-        from caikit.core.data_model import DataObjectBase, dataobject
-
+        from typing import Dict, List, Union
         """
     )
-    for message_name, message_spec in message_specs.items():
-        msg_str = (
-            f'\n@dataobject("{package_name}")\nclass {message_name}(DataObjectBase):\n'
+    if mock_compiled:
+        out += justify_script_string(
+            """
+            from caikit.core.data_model import DataBase
+            from py_to_proto import dataclass_to_proto, descriptor_to_message_class
+            from dataclasses import dataclass
+            """
         )
+    else:
+        out += "\nfrom caikit.core.data_model import DataObjectBase, dataobject\n"
+    for message_name, message_spec in message_specs.items():
+        type_annotations = ""
         for field_name, field_type in message_spec.items():
-            msg_str += f"    {field_name}: {_get_proto_val_name(field_type)}\n"
-        msg_str += "\n"
+            type_annotations += f"    {field_name}: {_get_proto_val_name(field_type)}\n"
+
+        # Manually create the proto class and use the precompiled proto style
+        if mock_compiled:
+            dataclass_name = f"_{message_name}"
+            proto_name = f"{dataclass_name}_proto"
+            msg_str = f"\n@dataclass\nclass {dataclass_name}:\n"
+            msg_str += type_annotations
+            msg_str += justify_script_string(
+                f"""
+
+                {proto_name} = descriptor_to_message_class(
+                    dataclass_to_proto(
+                        dataclass_={dataclass_name},
+                        package="{package_name}",
+                        name="{message_name}",
+                    )
+                )
+
+                class {message_name}(DataBase):
+                    _proto_class = {proto_name}
+                """
+            )
+
+        # Add as a dataobject
+        else:
+            msg_str = f'\n@dataobject("{package_name}")\nclass {message_name}(DataObjectBase):\n'
+            msg_str += type_annotations
+
         out += msg_str
     return out
```

### Comparing `caikit-0.4.3/tests/fixtures/config/config.yml` & `caikit-0.4.4/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.4.4/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/dummy_block.zip` & `caikit-0.4.4/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/dummy_block/config.yml` & `caikit-0.4.4/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.4.4/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/dummy_resource.zip` & `caikit-0.4.4/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/dummy_workflow.zip` & `caikit-0.4.4/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.4.4/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/fixtures.py` & `caikit-0.4.4/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/invalid.zip` & `caikit-0.4.4/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/linux.txt` & `caikit-0.4.4/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/primitive_party.proto` & `caikit-0.4.4/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.4.4/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.4.4/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.4.4/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.4.4/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.4.4/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.4.4/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/generated/__init__.py` & `caikit-0.4.4/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/metrics/__init__.py` & `caikit-0.4.4/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.4.4/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/model_management/__init__.py` & `caikit-0.4.4/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/model_management/test_batcher.py` & `caikit-0.4.4/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/model_management/test_model_loader.py` & `caikit-0.4.4/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/model_management/test_model_manager.py` & `caikit-0.4.4/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.4.4/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/model_management/test_training_manager.py` & `caikit-0.4.4/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.4.4/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.4.4/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.4.4/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/service_generation/test_create_service.py` & `caikit-0.4.4/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.4.4/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/service_generation/test_primitives.py` & `caikit-0.4.4/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.4.4/tests/runtime/service_generation/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.4.4/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/servicers/__init__.py` & `caikit-0.4.4/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.4.4/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.4.4/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.4.4/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.4.4/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.4.4/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/test_grpc_server.py` & `caikit-0.4.4/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/test_service_factory.py` & `caikit-0.4.4/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/utils/__init__.py` & `caikit-0.4.4/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/utils/test_import_util.py` & `caikit-0.4.4/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/utils/test_servicer_util.py` & `caikit-0.4.4/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/work_management/__init__.py` & `caikit-0.4.4/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.4.4/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.4.4/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.4.4/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.3/tox.ini` & `caikit-0.4.4/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,45 @@
 commands = pytest --cov=caikit --cov-report=html {posargs:tests}
 
 ; Unclear: We probably want to test wheel packaging
 ; But! tox will fail when this is set and _any_ interpreter is missing
 ; Without this, sdist packaging is tested so that's a start.
 package=wheel
 
+[testenv:docs]
+recreate = True
+deps = 
+    -r {toxinidir}/docs-requirements.txt
+    alchemy-config>=1.1.1,<2.0.0
+    alchemy-logging>=1.0.4,<2.0.0
+    anytree>=2.7.0,<3.0
+    docstring-parser>=0.14.1,<0.16.0
+    grpcio-health-checking>=1.35.0,<2.0
+    grpcio>=1.35.0,<2.0
+    ijson>=3.1.4,<3.3.0
+    munch>=2.5.0,<4.0
+    protobuf>=3.19.0,<5
+    prometheus_client>=0.12.0,<1.0
+    py-grpc-prometheus>=0.7.0,<0.8
+    PyYAML>=6.0,<7.0
+    requests>=2.26.0,<3.0
+    semver>=2.13.0,<4.0
+    six>=1.16.0,<2.0.0
+    tqdm>=4.59.0,<5.0.0
+    py-to-proto>=0.2.0,<0.3.0
+    import-tracker>=3.1.5,<4
+changedir = docs
+
+; Disabled '-W' flag as warnings in the files
+; TOTO: Add back in once build warnings fixed
+commands =
+  sphinx-apidoc -f -o api/ ../caikit
+  sphinx-build -E -a -b html -T . _build/html
+skip_install = True
+
 [testenv:fmt]
 description = format with pre-commit
 deps = pre-commit>=3.0.4,<4.0
 commands = ./scripts/fmt.sh
 allowlist_externals = ./scripts/fmt.sh
 skip_install = True # Skip package install since fmt doesn't need to execute code, for ⚡⚡⚡
```

### Comparing `caikit-0.4.3/PKG-INFO` & `caikit-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.4.3
+Version: 0.4.4
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
```

