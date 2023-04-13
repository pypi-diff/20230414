# Comparing `tmp/caikit-0.1.1.tar.gz` & `tmp/caikit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.1.1.tar", last modified: Wed Apr 12 22:28:30 2023, max compression
+gzip compressed data, was "caikit-0.1.2.tar", last modified: Thu Apr 13 23:42:59 2023, max compression
```

## Comparing `caikit-0.1.1.tar` & `caikit-0.1.2.tar`

### file list

```diff
@@ -1,299 +1,300 @@
--rw-r--r--   0        0        0       60 2023-04-12 22:28:23.919434 caikit-0.1.1/.coveragerc
--rw-r--r--   0        0        0      676 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0     1272 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-04-12 22:28:23.919434 caikit-0.1.1/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      191 2023-04-12 22:28:23.919434 caikit-0.1.1/.gitignore
--rw-r--r--   0        0        0      299 2023-04-12 22:28:23.919434 caikit-0.1.1/.isort.cfg
--rw-r--r--   0        0        0      370 2023-04-12 22:28:23.919434 caikit-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-04-12 22:28:23.919434 caikit-0.1.1/.prettierignore
--rw-r--r--   0        0        0       12 2023-04-12 22:28:23.919434 caikit-0.1.1/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-04-12 22:28:23.919434 caikit-0.1.1/.pylintrc
--rw-r--r--   0        0        0       78 2023-04-12 22:28:23.923434 caikit-0.1.1/.whitesource
--rw-r--r--   0        0        0     3358 2023-04-12 22:28:23.923434 caikit-0.1.1/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     6510 2023-04-12 22:28:23.923434 caikit-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-04-12 22:28:23.923434 caikit-0.1.1/LICENSE
--rw-r--r--   0        0        0       18 2023-04-12 22:28:23.923434 caikit-0.1.1/OWNERS
--rw-r--r--   0        0        0     5206 2023-04-12 22:28:23.923434 caikit-0.1.1/README.md
--rw-r--r--   0        0        0    44878 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit-overview.png
--rw-r--r--   0        0        0      323 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/__init__.py
--rw-r--r--   0        0        0     1861 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1104 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/config/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/config/config.py
--rw-r--r--   0        0        0     1010 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/config/config.yml
--rw-r--r--   0        0        0      962 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    29225 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    12141 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     5340 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1471 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40187 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    20773 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/model_manager.py
--rw-r--r--   0        0        0    51860 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module.py
--rw-r--r--   0        0        0     7643 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     1786 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     1493 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5493 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/module_meta.py
--rw-r--r--   0        0        0      709 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/resources/base.py
--rw-r--r--   0        0        0     1110 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0     1787 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/config_utils.py
--rw-r--r--   0        0        0      637 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    18275 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     5439 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/extension_utils.py
--rw-r--r--   0        0        0     4935 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1864 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0      630 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/json_test_data.py
--rw-r--r--   0        0        0     4278 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/performance.py
--rw-r--r--   0        0        0     1013 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/test_data.py
--rw-r--r--   0        0        0     1476 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance/text_test_data.py
--rw-r--r--   0        0        0      950 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/performance_metrics.py
--rw-r--r--   0        0        0    32214 2023-04-12 22:28:23.923434 caikit-0.1.1/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9298 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     5379 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/config/config.yml
--rw-r--r--   0        0        0     1716 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    13853 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4703 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0     2370 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/metrics/throughput.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     6068 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12138 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4194 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1587 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    17113 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     2947 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5611 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12289 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     5750 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0     9693 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/serializers.py
--rw-r--r--   0        0        0      666 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    11398 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4850 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     7128 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    12326 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    14525 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10554 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1696 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4223 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/config_parser.py
--rw-r--r--   0        0        0     6692 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0     1686 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/log_config.py
--rw-r--r--   0        0        0    17900 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-04-12 22:28:23.927434 caikit-0.1.1/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      837 2023-04-12 22:28:23.931434 caikit-0.1.1/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     1069 2023-04-12 22:28:26.883463 caikit-0.1.1/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-04-12 22:28:23.931434 caikit-0.1.1/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-04-12 22:28:23.931434 caikit-0.1.1/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3783 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/base.py
--rw-r--r--   0        0        0     8909 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    12705 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26028 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13070 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    11977 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     2909 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     3080 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_config.py
--rw-r--r--   0        0        0      521 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_imports.py
--rw-r--r--   0        0        0    18331 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    17316 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_module.py
--rw-r--r--   0        0        0     4751 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8440 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     1038 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7967 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0     1953 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_config_utils.py
--rw-r--r--   0        0        0    14999 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4408 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_extension_utils.py
--rw-r--r--   0        0        0     4972 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    15632 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5655 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0       27 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      106 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-04-12 22:28:23.931434 caikit-0.1.1/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      176 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1852 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      616 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2411 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1404 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2498 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      202 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/config.py
--rw-r--r--   0        0        0      141 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0      859 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1763 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      933 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/fixtures/studio_models/studio_block
--rw-r--r--   0        0        0        0 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0     6439 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/metrics/test_throughput.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14115 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    11774 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    18079 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5053 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     4762 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3295 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18350 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     1387 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9667 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    12985 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3533 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7386 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4180 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    29820 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0     5570 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     3891 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/utils/test_configs.py
--rw-r--r--   0        0        0     5047 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26472 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-04-12 22:28:23.935434 caikit-0.1.1/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1025 2023-04-12 22:28:23.935434 caikit-0.1.1/tox.ini
--rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 caikit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-04-13 23:42:51.860106 caikit-0.1.2/.coveragerc
+-rw-r--r--   0        0        0      676 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0     1272 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      191 2023-04-13 23:42:51.860106 caikit-0.1.2/.gitignore
+-rw-r--r--   0        0        0      310 2023-04-13 23:42:51.860106 caikit-0.1.2/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-04-13 23:42:51.860106 caikit-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-04-13 23:42:51.860106 caikit-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       12 2023-04-13 23:42:51.860106 caikit-0.1.2/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-04-13 23:42:51.860106 caikit-0.1.2/.pylintrc
+-rw-r--r--   0        0        0       78 2023-04-13 23:42:51.860106 caikit-0.1.2/.whitesource
+-rw-r--r--   0        0        0     3358 2023-04-13 23:42:51.860106 caikit-0.1.2/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     6510 2023-04-13 23:42:51.860106 caikit-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-04-13 23:42:51.860106 caikit-0.1.2/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-13 23:42:51.860106 caikit-0.1.2/OWNERS
+-rw-r--r--   0        0        0     3757 2023-04-13 23:42:51.860106 caikit-0.1.2/README.md
+-rw-r--r--   0        0        0    44878 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit-overview.png
+-rw-r--r--   0        0        0      323 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/__init__.py
+-rw-r--r--   0        0        0     1861 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0     1104 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/config/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/config/config.py
+-rw-r--r--   0        0        0     1010 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/config/config.yml
+-rw-r--r--   0        0        0      962 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    29207 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    13676 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     5340 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1471 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40187 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    20773 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    51860 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/module.py
+-rw-r--r--   0        0        0     7643 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     1786 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     1493 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5493 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_meta.py
+-rw-r--r--   0        0        0      709 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     1110 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0     1787 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/config_utils.py
+-rw-r--r--   0        0        0      637 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    18275 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     5439 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/extension_utils.py
+-rw-r--r--   0        0        0     4935 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1864 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0      630 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/__init__.py
+-rw-r--r--   0        0        0     1459 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/json_test_data.py
+-rw-r--r--   0        0        0     4278 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/performance.py
+-rw-r--r--   0        0        0     1013 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/test_data.py
+-rw-r--r--   0        0        0     1476 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/text_test_data.py
+-rw-r--r--   0        0        0      950 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance_metrics.py
+-rw-r--r--   0        0        0    32214 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9298 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     5379 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/config/config.yml
+-rw-r--r--   0        0        0     1716 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    13853 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4703 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0     2370 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/metrics/throughput.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     6068 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12138 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4194 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1587 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    17157 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5611 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    12289 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     5768 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    10121 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/serializers.py
+-rw-r--r--   0        0        0      666 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10301 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4911 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8296 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    12326 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    14523 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10554 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1696 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4223 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/config_parser.py
+-rw-r--r--   0        0        0     6692 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0     1686 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/log_config.py
+-rw-r--r--   0        0        0    17900 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      837 2023-04-13 23:42:51.868106 caikit-0.1.2/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     1154 2023-04-13 23:42:55.448182 caikit-0.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-04-13 23:42:51.868106 caikit-0.1.2/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-04-13 23:42:51.868106 caikit-0.1.2/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3783 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/base.py
+-rw-r--r--   0        0        0     8909 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    12691 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26013 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13070 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    13533 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     2909 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     3080 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/test_config.py
+-rw-r--r--   0        0        0      521 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/test_imports.py
+-rw-r--r--   0        0        0    18331 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    17317 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/test_module.py
+-rw-r--r--   0        0        0     4751 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8441 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     1038 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7967 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0     1953 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_config_utils.py
+-rw-r--r--   0        0        0    14999 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4408 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_extension_utils.py
+-rw-r--r--   0        0        0     4972 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    15618 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5655 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      106 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      176 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1852 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      616 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2411 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1404 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2498 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      202 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/config.py
+-rw-r--r--   0        0        0      141 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1763 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      933 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/studio_models/studio_block
+-rw-r--r--   0        0        0        0 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0     6439 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/metrics/test_throughput.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14115 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    11774 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    18079 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5053 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     1654 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     3326 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3280 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18350 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     1372 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9610 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    12985 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3533 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7386 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4180 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    29936 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0     5570 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     3891 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/utils/test_configs.py
+-rw-r--r--   0        0        0     5041 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26086 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1025 2023-04-13 23:42:51.876106 caikit-0.1.2/tox.ini
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 caikit-0.1.2/PKG-INFO
```

### Comparing `caikit-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.1.2/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/.github/workflows/build-library.yml` & `caikit-0.1.2/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/.github/workflows/lint-code.yml` & `caikit-0.1.2/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/.github/workflows/publish-library.yml` & `caikit-0.1.2/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/.pylintrc` & `caikit-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/CODE-OF-CONDUCT.md` & `caikit-0.1.2/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/CONTRIBUTING.md` & `caikit-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/LICENSE` & `caikit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit-overview.png` & `caikit-0.1.2/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/__init__.py` & `caikit-0.1.2/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/augmentors/__init__.py` & `caikit-0.1.2/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/augmentors/base.py` & `caikit-0.1.2/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.1.2/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.1.2/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/augmentors/schemes/base.py` & `caikit-0.1.2/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.1.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.1.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/blocks/__init__.py` & `caikit-0.1.2/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/blocks/base.py` & `caikit-0.1.2/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/config/__init__.py` & `caikit-0.1.2/caikit/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/config/config.py` & `caikit-0.1.2/caikit/core/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/config/config.yml` & `caikit-0.1.2/caikit/core/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/__init__.py` & `caikit-0.1.2/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/base.py` & `caikit-0.1.2/caikit/core/data_model/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,16 +747,14 @@
 
         Args:
             class_name (str)
                 The name of the class either as a fully-qualified protobuf name
                 or as the unqualified class name
 
         Returns:
-
-        Returns:
             dm_class (Type[DataBase])
                 The data model class corresponding to the given protobuf
         """
         dm_class = _DataBaseMetaClass.class_registry.get(class_name)
         if dm_class is not None:
             return dm_class
         matching_classes = [
```

### Comparing `caikit-0.1.1/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.1.2/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/data_backends/base.py` & `caikit-0.1.2/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.1.2/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/dataobject.py` & `caikit-0.1.2/caikit/core/data_model/dataobject.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from datetime import datetime
 from functools import update_wrapper
 from types import ModuleType
 from typing import Callable, Dict, List, Type, Union
 import importlib
 import sys
 import types
+import typing
 
 # Third Party
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal.enum_type_wrapper import EnumTypeWrapper
 
 # First Party
@@ -37,14 +38,15 @@
 import alog
 import jtd_to_proto
 
 # Local
 from ..toolkit.errors import error_handler
 from . import enums
 from .base import DataBase, _DataBaseMetaClass
+from .streams.data_stream import DataStream
 
 ## Globals #####################################################################
 
 log = alog.use_channel("SCHEMA")
 error = error_handler.get(log)
 
 # Type defs for input schemas to a dataobject
@@ -232,20 +234,24 @@
 
 class _EnumBaseSentinel:
     """This base class is used to provide a common base class for enum warpper
     classes so that they can be identified generically
     """
 
 
-def _to_jtd_schema(input_schema: _SCHEMA_DEF_TYPE) -> _JTD_DEF_TYPE:
+# pylint: disable=too-many-return-statements
+def _to_jtd_schema(
+    input_schema: _SCHEMA_DEF_TYPE, is_inside_properties_dict: bool = False
+) -> _JTD_DEF_TYPE:
     """Recursive helper that will convert an input schema to a fully fleshed out
     JTD schema
     """
-
     try:
+        # Unwrap optional to base type if applicable
+        input_schema = _unwrap_optional_type(input_schema)
 
         # If it's a reference to an EnumBase, de-alias to that enum's EnumDescriptor
         # NOTE: This must come before the check for dict since EnumBase instances
         #   are themselves dicts
         if isinstance(input_schema, enums.EnumBase) or (
             isinstance(input_schema, type)
             and issubclass(input_schema, _EnumBaseSentinel)
@@ -256,38 +262,65 @@
             # If this dict is already a JTD schema, return it as is
             if is_valid_jtd(input_schema, valid_types=JTD_TO_PROTO_TYPES.keys()):
                 return input_schema
 
             # If the dict is structured as a JTD element already, recurse on the
             # values
             if any(keyword in input_schema for keyword in _JTD_KEYWORDS):
-                return {k: _to_jtd_schema(v) for k, v in input_schema.items()}
+                return {
+                    k: _to_jtd_schema(v, "properties" in k.lower())
+                    for k, v in input_schema.items()
+                }
 
             # If not, assume it's a flat properties dict
-            return {
-                "properties": {k: _to_jtd_schema(v) for k, v in input_schema.items()}
-            }
+            # Check to make sure we don't re-wrap *properties
+            translated_dict = {k: _to_jtd_schema(v) for k, v in input_schema.items()}
+            return (
+                {"properties": translated_dict}
+                if not is_inside_properties_dict
+                else translated_dict
+            )
 
         # If it's a reference to another data model object, de-alias to that
         # object's underlying proto descriptor
         if isinstance(input_schema, type) and issubclass(input_schema, DataBase):
             return {"type": input_schema.get_proto_class().DESCRIPTOR}
 
         # If it's a native type, wrap it as a "type" element
         if input_schema in _NATIVE_TYPE_TO_JTD:
             return {"type": _NATIVE_TYPE_TO_JTD[input_schema]}
 
+        # If it's a list or data stream, wrap it with "elements":
+        if typing.get_origin(input_schema) in [list, DataStream]:
+            # type_ could be caikit.core.data_model.streams.data_stream.DataStream[int]
+            return {"elements": _to_jtd_schema(typing.get_args(input_schema)[0])}
+
         # All other cases are invalid!
         raise ValueError(f"Invalid input schema: {input_schema}")
 
     except ValueError:
         log.error("Invalid schema: %s", input_schema)
         raise
 
 
+def _unwrap_optional_type(type_: typing.Any) -> typing.Any:
+    """Unwrap an Optional[T] type, or return the type as-is if it is not an optional
+    NB: Optional[T] is expressed as Union[T, None]
+    This function checks for Unions of [T, None] and returns T, or raises if the union
+    contains more types, as those need to be handled differently (and are not yet supported)
+    """
+    if typing.get_origin(type_) != Union:
+        return type_
+    possible_types = set(typing.get_args(type_))
+    possible_types.discard(type(None))
+    if len(possible_types) == 1:
+        return list(possible_types)[0]
+    raise ValueError(f"Invalid input schema, cannot handle unions yet: {type_}")
+
+
 def _get_all_enums(
     proto_class: Union[_message.Message, EnumTypeWrapper],
 ) -> List[EnumTypeWrapper]:
     """Given a generated proto class, recursively extract all enums"""
     all_enums = []
     if isinstance(proto_class, EnumTypeWrapper):
         all_enums.append(proto_class)
```

### Comparing `caikit-0.1.1/caikit/core/data_model/enums.py` & `caikit-0.1.2/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/producer.py` & `caikit-0.1.2/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.1.2/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/streams/__init__.py` & `caikit-0.1.2/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/streams/converter.py` & `caikit-0.1.2/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.1.2/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/streams/data_stream.py` & `caikit-0.1.2/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/streams/resolver.py` & `caikit-0.1.2/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/data_model/streams/validator.py` & `caikit-0.1.2/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/model_manager.py` & `caikit-0.1.2/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/module.py` & `caikit-0.1.2/caikit/core/module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/module_backend_config.py` & `caikit-0.1.2/caikit/core/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/module_backends/__init__.py` & `caikit-0.1.2/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/module_backends/backend_types.py` & `caikit-0.1.2/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/module_backends/base.py` & `caikit-0.1.2/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/module_backends/local_backend.py` & `caikit-0.1.2/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/module_config.py` & `caikit-0.1.2/caikit/core/module_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/module_meta.py` & `caikit-0.1.2/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/resources/__init__.py` & `caikit-0.1.2/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/resources/base.py` & `caikit-0.1.2/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/__init__.py` & `caikit-0.1.2/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/compatibility.py` & `caikit-0.1.2/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/config_utils.py` & `caikit-0.1.2/caikit/core/toolkit/config_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/errors/__init__.py` & `caikit-0.1.2/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.1.2/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.1.2/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/extension_utils.py` & `caikit-0.1.2/caikit/core/toolkit/extension_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/fileio.py` & `caikit-0.1.2/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/isa.py` & `caikit-0.1.2/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/logging.py` & `caikit-0.1.2/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/performance/__init__.py` & `caikit-0.1.2/caikit/core/toolkit/performance/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/performance/json_test_data.py` & `caikit-0.1.2/caikit/core/toolkit/performance/json_test_data.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/performance/performance.py` & `caikit-0.1.2/caikit/core/toolkit/performance/performance.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/performance/test_data.py` & `caikit-0.1.2/caikit/core/toolkit/performance/test_data.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/performance/text_test_data.py` & `caikit-0.1.2/caikit/core/toolkit/performance/text_test_data.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/performance_metrics.py` & `caikit-0.1.2/caikit/core/toolkit/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.1.2/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/serializers.py` & `caikit-0.1.2/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/toolkit/wip_decorator.py` & `caikit-0.1.2/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/workflows/__init__.py` & `caikit-0.1.2/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/core/workflows/base.py` & `caikit-0.1.2/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/interfaces/__init__.py` & `caikit-0.1.2/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/interfaces/common/__init__.py` & `caikit-0.1.2/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.1.2/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/interfaces/common/data_model/producer.py` & `caikit-0.1.2/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/interfaces/runtime/__init__.py` & `caikit-0.1.2/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.1.2/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.1.2/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/__init__.py` & `caikit-0.1.2/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/config/config.yml` & `caikit-0.1.2/caikit/runtime/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/dump_services.py` & `caikit-0.1.2/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/grpc_server.py` & `caikit-0.1.2/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/interceptors/__init__.py` & `caikit-0.1.2/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.1.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/metrics/__init__.py` & `caikit-0.1.2/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.1.2/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/metrics/throughput.py` & `caikit-0.1.2/caikit/runtime/metrics/throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/model_management/__init__.py` & `caikit-0.1.2/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/model_management/batcher.py` & `caikit-0.1.2/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/model_management/loaded_model.py` & `caikit-0.1.2/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/model_management/model_loader.py` & `caikit-0.1.2/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/model_management/model_manager.py` & `caikit-0.1.2/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/model_management/model_sizer.py` & `caikit-0.1.2/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/model_management/training_manager.py` & `caikit-0.1.2/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/__init__.py` & `caikit-0.1.2/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.1.2/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.1.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.1.2/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.1.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.1.2/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.1.2/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.1.2/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.1.2/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.1.2/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/service_factory.py` & `caikit-0.1.2/caikit/runtime/service_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module is responsible for creating service objects for the runtime to consume"""
 # Standard
 from enum import Enum
 from types import ModuleType
-from typing import Callable, Dict, List, Type, Union
+from typing import Callable, Dict, List, Type
 import dataclasses
 import inspect
-import typing
 
 # Third Party
 import google.protobuf.descriptor
 import google.protobuf.service
 import grpc
 
 # First Party
@@ -32,15 +31,14 @@
     service_descriptor_to_server_registration_function,
     service_descriptor_to_service,
 )
 import alog
 
 # Local
 from caikit.core import dataobject
-from caikit.core.data_model import DataStream
 from caikit.core.data_model.base import DataBase
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
 )
 from caikit.runtime import service_generation
 from caikit.runtime.service_generation.serializers import (
@@ -241,40 +239,46 @@
                 ),
                 stub_class=service_descriptor_to_client_stub(service_descriptor),
                 messages=client_module,
             )
 
     # Implementation details for pure python service packages #
     @staticmethod
-    def _fix_lists(type_: Type) -> Union[Dict, Type]:
-        if typing.get_origin(type_) in [list, DataStream]:
-            # type_ could be caikit.core.data_model.streams.data_stream.DataStream[int]
-            return {"elements": typing.get_args(type_)[0]}
-        return type_
-
-    @staticmethod
     def _create_request_message_types(
         rpcs_list: List[RPCSerializerBase],
         package_name: str,
     ) -> List[Type[DataBase]]:
         """Dynamically create data model classes for the inputs to these RPCs"""
         data_model_classes = []
         for task in rpcs_list:
-            schema = {
+            properties = {
                 # triple e.g. ('caikit.interfaces.common.ProducerPriority', 'producer_id', 1)
                 # This does not take care of nested descriptors
-                triple[1]: ServicePackageFactory._fix_lists(triple[0])
+                triple[1]: triple[0]
+                for triple in task.request.triples
+                if triple[1] not in task.request.default_set
+            }
+            optional_properties = {
+                triple[1]: triple[0]
                 for triple in task.request.triples
+                if triple[1] in task.request.default_set
+            }
+            schema = {
+                "properties": properties,
+                "optionalProperties": optional_properties,
             }
 
             if not schema:
                 # hacky hack hack: make sure we actually have a schema to generate
                 continue
 
-            decorator = dataobject(schema=schema, package=package_name)
+            decorator = dataobject(
+                schema=schema,
+                package=package_name,
+            )
             cls_ = type(task.request.name, (object,), {})
             decorated_cls = decorator(cls_)
             data_model_classes.append(decorated_cls)
 
         return data_model_classes
 
     @staticmethod
```

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.1.2/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.1.2/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     The logic here assumes one of several conventions is followed for the Module
     1. The Module is declared in a python module named
         `<library>.<block/workflow>.<module type>`
     2. The module derives from a base class that itself derives from one of the
         known type-hierarchy derived from `ModuleBase`.
     """
+    # NOTE: all of this assumes <library> has no .
     # Use the library name to qualify the module type in case there are
     # collisions across domains (e.g. classification in nlp and cv)
     py_mod_name_parts = ck_module.__module__.split(".")
     lib_name = py_mod_name_parts[0]
 
     # First, look for the python module naming convention
     if len(py_mod_name_parts) >= 3:
@@ -60,15 +61,18 @@
             module_kind,
             ck_module,
         )
         return ModuleInfo(library=lib_name, kind=module_kind, type=module_type)
 
     # Look for a base class that meets our expectations
     for parent in ck_module.__mro__[1:]:
-        if parent.__module__.partition(".")[0] != "caikit.core":
+        if not (
+            parent.__module__.partition(".")[0] == "caikit"
+            and parent.__module__.partition(".")[1] == "core"
+        ):
             module_parts = parent.__module__.split(".")
             module_kind = module_parts[1]
             module_type = module_parts[-1]
             log.debug3(
                 "Using parent module type %s and module kind %s for Module %s",
                 module_type,
                 module_kind,
```

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/create_service.py` & `caikit-0.1.2/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.1.2/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/primitives.py` & `caikit-0.1.2/caikit/runtime/service_generation/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
     Returns True is arg_type is in PROTO_TYPE_MAP(float, int, bool, str, bytes)
     Or if it's an imported Caikit library primitive.
     Or if it's a Union of at least one primitive.
     Or if it's a List of primitives.
     False otherwise"""
     lib_dm_primitives = _get_library_dm_primitives(primitive_data_model_types)
     primitive_set = list(PROTO_TYPE_MAP.keys()) + lib_dm_primitives
+
     if arg_type in primitive_set:
         return True
     if typing.get_origin(arg_type) == list:
         log.debug2("Arg is List")
         # check that list is not nested
         if len(typing.get_args(arg_type)) == 1:
             return typing.get_args(arg_type)[0] in primitive_set
@@ -153,7 +154,8 @@
     log.debug3("DM Primitives: %s", lib_dm_primitives)
     return lib_dm_primitives
 
 
 def _is_optional_type(arg_type: Type):
     if typing.get_origin(arg_type) == Union and type(None) in typing.get_args(arg_type):
         return True
+    return False
```

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/serializers.py` & `caikit-0.1.2/caikit/runtime/service_generation/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """
 This package has classes that will serialize a python interface to a protocol buffer interface.
 
 Typically used for `caikit.core.module`s that expose .train and .run functions.
 """
 # Standard
-from typing import Dict, List, Optional, Tuple, Type, get_args
+from typing import Dict, List, Optional, Set, Tuple, Type, get_args
 import abc
 
 # First Party
 import alog
 
 # Local
 from . import primitives, type_helpers
@@ -72,15 +72,17 @@
         # Compute the mapping from argument name to type for the module's run
         log.debug3("Param Dict: %s", self._method.parameters)
         log.debug3("Return Type: %s", self._method.return_type)
 
         # Store the input and output protobuf message types for this RPC
         self.return_type = self._method.return_type
         self._req = _RequestMessage(
-            self._module_class_to_req_name(), self._method.parameters
+            self._module_class_to_req_name(),
+            self._method.parameters,
+            self._method.default_parameters,
         )
 
     @property
     def module_list(self) -> List[Type[ModuleBase]]:
         """Returns a list containing the single caikit.core.module type that this RPC is for"""
         return [self.clz]
 
@@ -167,27 +169,33 @@
         """
         self.task = task
         self._module_list = [method.module for method in method_signatures]
         self._method_signatures = method_signatures
 
         # Aggregate the argument signature types into a single parameters_dict
         parameters_dict = {}
+        default_parameters = set()
         for method in method_signatures:
+            default_parameters.update(method.default_parameters)
             primitive_arg_dict = primitives.to_primitive_signature(
                 method.parameters, primitive_data_model_types
             )
             for arg_name, arg_type in primitive_arg_dict.items():
                 current_val = parameters_dict.get(arg_name, arg_type)
+                # TODO: raise runtime error here instead of assert!
+                # TODO: need to resolve Optional[T] vs. T - if both come in, use Optional[T]
                 assert (
                     current_val == arg_type
                 ), f"Conflicting value types for arg {arg_name}: {current_val} != {arg_type}"
 
                 parameters_dict[arg_name] = arg_type
 
-        self._req = _RequestMessage(self._task_to_req_name(), parameters_dict)
+        self._req = _RequestMessage(
+            self._task_to_req_name(), parameters_dict, default_parameters
+        )
 
         # Validate that the return_type of all modules in the grouping matches
         return_types = {method.return_type for method in method_signatures}
         assert len(return_types) == 1, f"Found multiple return types for task [{task}]"
         return_type = list(return_types)[0]
         self.return_type = return_type
 
@@ -224,20 +232,21 @@
 
 class _RequestMessage:
     """Helper class to create the input request message that wraps up the inputs
     for a given function. The request Contains N named data-model or primitive
     objects.
     """
 
-    def __init__(self, msg_name: str, params: Dict[str, Type]):
+    def __init__(self, msg_name: str, params: Dict[str, Type], default_set: Set[str]):
         """Initialize with the module class and the parsed parameters to the run
         function.
         """
         self.name = msg_name
         self.triples = []
+        self.default_set = default_set
 
         existing_fields = ApiFieldNames.get_fields_for_message(self.name)
 
         if len(existing_fields) > 0:
             last_used_number = max(existing_fields.values())
         else:
             last_used_number = 0
```

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,63 +11,58 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This package handles all the gorp of finding types from docstrings given our custom
 conventions"""
 
 # Standard
-from types import FunctionType
-from typing import Dict, List, Optional, Tuple, Type, Union
+from typing import Callable, Dict, List, Optional, Tuple, Type, Union
 import builtins
 import sys
 
 # Third Party
-# Third party
 import docstring_parser
 
 # First Party
-# First party
 import alog
 
 # Local
-from caikit.core import ModuleBase
+from caikit.core.data_model.base import DataBase
 import caikit.core
 
 log = alog.use_channel("DOCSTRINGS")
 
 
-def get_return_type(module_class: Type[ModuleBase], fn: FunctionType) -> Optional[Type]:
+def get_return_type(fn: Callable) -> Optional[Type]:
     """
     Grabs the return type off the docstring, if possible
     Args:
-        module_class: The type of the caikit.core.module that fn is defined on
-            e.g. my_caikit_library.blocks.classification.Transformer
         fn: The function to get the return value of
             e.g. my_caikit_library.blocks.classification.Transformer.run
 
     Returns:
         The return type of `fn`, if it can be parsed from the docstring. Otherwise, None
     """
     docstring = docstring_parser.parse(fn.__doc__)
     if not docstring:
-        log.warning("Failed to parse the docstring for %s", module_class)
+        log.warning("Failed to parse the docstring")
         return None
 
     type_names, desc_names = _get_candidate_type_names_from_docstring(docstring.returns)
 
-    return_type = _get_docstring_type(module_class, type_names)
+    return_type = _get_docstring_type(type_names)
     if return_type:
         return return_type
 
-    return _get_docstring_type(module_class, desc_names)
+    return _get_docstring_type(desc_names)
 
 
-def is_optional(fn: FunctionType, arg_name: str) -> bool:
+def is_optional(fn: Callable, arg_name: str) -> bool:
     """
-    Checks if the `argname` param from `fn`s docstring is optional
+    Checks if the `arg_name` param from `fn`s docstring is optional
     by checking if param description starts with "an optional"
     or "optional".
 
     Args:
         fn: The function to get the type of a parameter from
             e.g.  my_caikit_library.blocks.classification.Transformer.run
         arg_name: The name of the parameter that we should try to get the type of
@@ -91,53 +86,45 @@
                 ) or description_line.lower().startswith("an optional"):
                     log.debug2("Optional parameter found: %s", ds_param)
                     return True
 
         return False
 
 
-def get_arg_type(
-    module_class: ModuleBase.__class__, fn: FunctionType, arg_name: str
-) -> Optional[Type]:
+def get_arg_type(fn: Callable, arg_name: str) -> Optional[Type]:
     """
-    Grabs the type of the `argname` param from `fn`s docstring, if possible
+    Grabs the type of the `arg_name` param from `fn`s docstring, if possible
     Args:
-        module_class: The type of the caikit.core.module that fn is defined on
-            e.g. my_caikit_library.blocks.classification.Transformer
         fn: The function to get the type of a parameter from
             e.g. my_caikit_library.blocks.classification.Transformer.run
         arg_name: The name of the parameter that we should try to get the type of
             e.g. "raw_document"
     Returns:
         The return type of `fn`, if it can be parsed from the docstring. Otherwise, None
     """
 
     docstring = docstring_parser.parse(fn.__doc__)
     if not docstring:
-        log.warning(
-            "Failed to parse the docstring for %s:%s", module_class, fn.__name__
-        )
+        log.warning("Failed to parse the docstring for function %s", fn.__name__)
         return None
 
     ds_param = [param for param in docstring.params if param.arg_name == arg_name]
     if ds_param:
         if len(ds_param) > 1:
             log.warning("Docstring has multiple args with the same name! %s", arg_name)
         ds_param = ds_param[0]
         type_names, desc_names = _get_candidate_type_names_from_docstring(ds_param)
-        docstring_type = _get_docstring_type(module_class, type_names)
+        docstring_type = _get_docstring_type(type_names)
         if not docstring_type:
-            docstring_type = _get_docstring_type(module_class, desc_names)
+            docstring_type = _get_docstring_type(desc_names)
         if docstring_type is not None:
             log.debug2("Found type from docstring for %s: %s", arg_name, docstring_type)
             return docstring_type
     else:
-        log.warning(
-            "Found no parameter named %s in %s:%s", arg_name, module_class, fn.__name__
-        )
+        log.warning("Found no parameter named %s:%s", arg_name, fn.__name__)
     return None
 
 
 def _get_candidate_type_names_from_docstring(
     param: Optional[docstring_parser.common.DocstringParam],
 ) -> Tuple[List[str], List[str]]:
     if param is None:
@@ -165,15 +152,14 @@
         candidate_types_from_description,
     )
 
     return candidate_type_names, candidate_types_from_description
 
 
 def _get_docstring_type(
-    module_class: Type[ModuleBase],
     candidate_type_names: List[str],
 ) -> Optional[Type]:
     """Given a parsed docstring parameter, look in all of the possible places
     for the actual type
     """
 
     log.debug2(
@@ -193,98 +179,86 @@
         if builtin_type is not None:
             valid_candidates.append(builtin_type)
             log.debug2(f"Found valid candidate type: {builtin_type}")
             continue
 
         # Try to find things like "list(str)"
         # List[str]???
-        nested_type = _extract_nested_type(module_class, type_name)
+        nested_type = _extract_nested_type(type_name)
         if nested_type is not None:
             valid_candidates.append(nested_type)
             log.debug2(f"Found valid nested type: {nested_type}")
             continue
 
         # Try to spelunk down `sys.modules` for the type. This should work if it is fully qualified
-        candidate_type = _extract_type_from_pymodule(
-            sys.modules, module_class, type_name
-        )
+        candidate_type = _extract_type_from_pymodule(sys.modules, type_name)
         if candidate_type is not None:
             valid_candidates.append(candidate_type)
             log.debug2(f"Found valid candidate type on sys.modules: {candidate_type}")
             continue
 
         # If the type was not fully qualified (like a `RawDocument`), look in a couple well known
         # places - the caikit core data model itself
         candidate_type = _extract_type_from_pymodule(
-            caikit.interfaces.common.data_model, module_class, type_name
+            caikit.interfaces.common.data_model, type_name
         )
         if candidate_type is not None:
             valid_candidates.append(candidate_type)
             log.debug2(
                 # pylint: disable=line-too-long
                 f"Found valid candidate type on caikit.interfaces.common.data_model: {candidate_type}"
             )
             continue
-        # ...And the containing library's data model
-        lib_base = sys.modules[module_class.__module__.partition(".")[0]]
-        if hasattr(lib_base, "data_model"):
-            candidate_type = _extract_type_from_pymodule(
-                lib_base.data_model, module_class, type_name
-            )
+        # ...And the data model within the interfaces, including those defined in library
+        try:
+            candidate_type = DataBase.get_class_for_name(type_name)
+        except ValueError:
+            log.debug2(f"Data model match failed on {candidate_type}, continuing")
+            continue
         if candidate_type is not None:
             valid_candidates.append(candidate_type)
-            log.debug2(
-                f"Found valid candidate type on {lib_base.data_model}: {candidate_type}"
-            )
+            log.debug2(f"Found valid data model candidate type: {candidate_type}")
             continue
 
     log.debug3("valid candidates %s", valid_candidates)
 
     # If valid candidates were found, return either the single or a Union
     if valid_candidates:
         if len(valid_candidates) == 1:
             return valid_candidates[0]
 
         # pylint: disable=unnecessary-dunder-call
         return Union.__getitem__(tuple(valid_candidates))
     log.debug2(
-        "Unable to pull type name [%s] from module %s",
+        "Unable to pull type name [%s]",
         candidate_type_names,
-        module_class.__module__,
     )
 
 
-def _extract_nested_type(
-    module_class: Type[ModuleBase], type_name: str
-) -> Optional[Type]:
+def _extract_nested_type(type_name: str) -> Optional[Type]:
     type_name = type_name.replace("[", "(").replace("]", ")")
     is_a_list = type_name.lower().startswith("list")
     if is_a_list:
         start_child_type_name = type_name.find("(") + 1
         end_child_type_name = type_name.rfind(")")
         child_type_name = type_name[start_child_type_name:end_child_type_name]
 
-        child_type = _get_docstring_type(
-            module_class=module_class, candidate_type_names=[child_type_name]
-        )
+        child_type = _get_docstring_type(candidate_type_names=[child_type_name])
         if child_type:
             return List[child_type]
 
 
 def _extract_type_from_pymodule(
-    py_module: Union[Type, Dict], module_class: Type[ModuleBase], type_name: str
+    py_module: Union[Type, Dict], type_name: str
 ) -> Optional[Type]:
     """This walks down a type hierarchy to try to find the concrete type given an input string name
 
     Args:
         py_module: Type | Dict
             A python module, or dictionary of modules, to start walking to find "type_name"
-        module_class: Type[ModuleBase]
-            The containing class of the function which has an argument of type "type_name".
-            Used for logging.
         type_name: str
             The name of the type that we're trying to find. e.g. "caikit.core.data_model.ProducerId"
 
     Returns:
         Optional[Type]
             The type of "type_name", or None if it cannot be found
     """
@@ -299,15 +273,14 @@
         if isinstance(output_type, dict):
             output_type = output_type.get(part, None)
         else:
             output_type = getattr(output_type, part, None)
         if output_type is None:
             if not isinstance(py_module, dict):
                 log.debug2(
-                    "Couldn't find type name [%s] as an attribute on [%s] for module %s",
+                    "Couldn't find type name [%s] as an attribute on [%s]",
                     type_name,
                     py_module,
-                    module_class.__module__,
                 )
             return None
     if output_type not in [None, py_module]:
         return output_type
```

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 name, return type and input parameters.
 
 This encapsulates a lot of custom logic used to parse input/output parameters, especially when it
 comes to the caikit core common data model.
 """
 
 # Standard
-from typing import Dict, Optional, Type
+from typing import Dict, Optional, Set, Type
 import inspect
 
 # First Party
 import alog
 
 # Local
 from . import parsers
@@ -58,33 +58,29 @@
 
     def __init__(self, caikit_core_module: Type[ModuleBase], method_name: str):
         self._module = caikit_core_module
         self._method_name = method_name
 
         try:
             self._method_pointer = getattr(self._module, self._method_name)
+            self._default_set = parsers.get_args_with_defaults(self._method_pointer)
             method_signature = inspect.signature(self._method_pointer)
             self._return_type = parsers.get_output_type_name(
                 self._module, method_signature, self._method_pointer
             )
 
-            self._parameters = {
-                name: parsers.get_argument_type(
-                    param, self._module, self._method_pointer
-                )
-                for name, param in method_signature.parameters.items()
-                if name not in ["self", "args", "kwargs", "_"]
-            }
+            self._parameters = parsers.get_argument_types(self._method_pointer)
         except AttributeError:
             log.warning(
                 "Could not find method [%s] in this module",
                 self.method_name,
             )
             self._return_type = None
             self._parameters = None
+            self._default_set = set()
 
     @property
     def module(self) -> Type[ModuleBase]:
         """The concrete caikit.core.ModuleBase type"""
         return self._module
 
     @property
@@ -99,14 +95,19 @@
 
     @property
     def parameters(self) -> Optional[Dict[str, Type]]:
         """A dictionary of the parameter names to their types, or None if the method does not
         exist"""
         return self._parameters
 
+    @property
+    def default_parameters(self) -> Set[str]:
+        """A set of all parameter names which have default values"""
+        return self._default_set
+
 
 class CustomSignature(CaikitCoreModuleMethodSignature):
     """(TBD on new class)? Need something to hold an intentionally mutated representation of a
     method signature. This represents the extra indirection that lives in the runtime, between the
     service API and the actual method. For example: .train functions return a fully constructed
     module, but the runtime will invoke .train asynchronously and instead return some handle that
     can be used to check training status."""
```

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Contains functions that attempt to parse the I/O types of member methods on `caikit.core.module`s
 """
 # Standard
-from types import FunctionType
-from typing import List, Optional, Type
+from typing import Callable, Dict, List, Optional, Set, Type
 import inspect
 
 # First Party
 import alog
 
 # Local
 from . import docstrings
@@ -39,15 +38,15 @@
 KNOWN_OUTPUT_TYPES = {}
 
 
 @alog.logged_function(log.debug2)
 def get_output_type_name(
     module_class: ModuleBase.__class__,
     fn_signature: inspect.Signature,
-    fn: FunctionType,
+    fn: Callable,
 ) -> Type:
     """Get the type for a return type based on the name of the module class and
     the Caikit library naming convention.
     """
     extra_candidate_names = []
     log.debug(fn_signature)
     # Check type annotation first
@@ -67,60 +66,93 @@
                 fn_signature.return_annotation,
             )
             extra_candidate_names.append(fn_signature.return_annotation)
         else:
             return fn_signature.return_annotation
 
     # Check the docstring
-    # TODO: NOOOOOOOO need the real function
-    type_from_docstring = docstrings.get_return_type(module_class, fn)
+    type_from_docstring = docstrings.get_return_type(fn)
     if type_from_docstring:
         return type_from_docstring
 
     # Check based on naming conventions and then known output types
     module_parts = module_class.__module__.split(".")
     log.debug3("Parent module parts for %s: %s", module_class.__name__, module_parts)
 
-    # TODO: Why the F doesn't this work with docstrings?
-    # please test lol
-
+    # TODO: this part needs a test (or consider deleting and say user needs to specify output type)
     class_name = _snake_to_camel(module_parts[2]) + "Prediction"
     return _get_dm_type_from_name(class_name) or _get_dm_type_from_name(
         KNOWN_OUTPUT_TYPES.get(class_name)
     )
 
 
+def get_argument_types(module_method: Callable) -> Dict[str, Type]:
+    """Get the python types for each parameter to this method, returned in a dict.
+    This does more than simply looking at inspect.Signature, see _get_argument_type
+
+    Args:
+        module_method (Callable): A pointer to a method
+
+    Returns:
+        Dict[str, Type]: A dictionary of parameter name to parameter type
+    """
+    method_signature = inspect.signature(module_method)
+    return {
+        name: _get_argument_type(param, module_method)
+        for name, param in method_signature.parameters.items()
+        if name not in ["self", "args", "kwargs", "_", "__"]
+    }
+
+
+def get_args_with_defaults(module_method: Callable) -> Set[str]:
+    """Get the names of all arguments that have a default value supplied.
+    Args:
+        module_method (Callable): A pointer to a method
+
+    Returns:
+        Set[str]: A set of all parameter names which have a default value.
+            Empty if none have defaults or no parameters exist.
+    """
+    method_signature = inspect.signature(module_method)
+    return {
+        param.name
+        for param in method_signature.parameters.values()
+        if param.default != inspect.Parameter.empty
+    }
+
+
 # pylint: disable=too-many-return-statements
 @alog.logged_function(log.debug2)
-def get_argument_type(
+def _get_argument_type(
     arg: inspect.Parameter,
-    module_class: ModuleBase.__class__,
-    module_method: FunctionType,
+    module_method: Callable,
 ) -> Type:
     """Get the python type for a named argument to a Module's given method. This
     is where the heuristics for determining types are implemented:
 
     * Look for a known type mapping based on the name of the argument
     * Look for python type annotations
     * Look for a default value and check its type
     * Parse the docstring
     * Look for a data model object whose name matches the argument name
     """
-    # Check docstring for optional arg
-    optional_arg = docstrings.is_optional(module_method, arg.name)
+    # TODO: KNOWN_ARG_TYPES should be configurable
 
     # Use known arg types first
     # This avoids cases where docstrings are very obviously flubbed, such as
     #   `raw_document` being annotated as a `str` only in caikit.interfaces.nlp
     dm_type_from_known_arg_types = _get_dm_type_from_name(KNOWN_ARG_TYPES.get(arg.name))
     if dm_type_from_known_arg_types:
         # Not checking if this is optional: These known types should never be optional (maybe...?)
         # This could totally be incorrect!
         return dm_type_from_known_arg_types
 
+    # Check docstring for optional arg
+    optional_arg = docstrings.is_optional(module_method, arg.name)
+
     # Look for a type annotation
     if arg.annotation != inspect.Parameter.empty:
         log.debug("Found annotation for %s", arg.name)
         if optional_arg:
             return Optional[arg.annotation]
         return arg.annotation
 
@@ -129,15 +161,15 @@
     # Check for a default argument and return its type
     default_type = _get_default_type(arg)
     if default_type:
         return default_type
 
     # Parse docstring
 
-    type_from_docstring = docstrings.get_arg_type(module_class, module_method, arg.name)
+    type_from_docstring = docstrings.get_arg_type(module_method, arg.name)
     if type_from_docstring:
         if optional_arg:
             return Optional[type_from_docstring]
         return type_from_docstring
 
     # Look for a data model object whose name matches the argument name and fall
     # back to the KNOWN_ARG_TYPES dict
```

### Comparing `caikit-0.1.1/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.1.2/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/servicers/__init__.py` & `caikit-0.1.2/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.1.2/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.1.2/caikit/runtime/servicers/global_train_servicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             log_dict = {
                 "log_code": "<RUN49049070W>",
                 "message": repr(e),
                 "stack_trace": traceback.format_exc(),
             }
             log.warning(log_dict)
             raise CaikitRuntimeException(
-                StatusCode.INTERNAL, "Unhandled exception during prediction"
+                StatusCode.INTERNAL, "Unhandled exception during training"
             ) from e
 
     def run_training_job(
         self,
         request,
         model,
         training_id,
```

### Comparing `caikit-0.1.1/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.1.2/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.1.2/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.1.2/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/types/__init__.py` & `caikit-0.1.2/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/types/aborted_exception.py` & `caikit-0.1.2/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.1.2/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.1.2/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/utils/__init__.py` & `caikit-0.1.2/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/utils/config_parser.py` & `caikit-0.1.2/caikit/runtime/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/utils/import_util.py` & `caikit-0.1.2/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/utils/log_config.py` & `caikit-0.1.2/caikit/runtime/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/utils/servicer_util.py` & `caikit-0.1.2/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/work_management/__init__.py` & `caikit-0.1.2/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/work_management/abortable_action.py` & `caikit-0.1.2/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/work_management/call_aborter.py` & `caikit-0.1.2/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.1.2/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/examples/start_runtime_with_sample_lib.py` & `caikit-0.1.2/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/pyproject.toml` & `caikit-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.1.1"
+version = "0.1.2"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
-repository = "https://github.com/caikit/caikit"
 requires-python = "~=3.8"
+classifiers=[
+    "License :: OSI Approved :: Apache Software License"
+]
 dependencies = [
     "alchemy-config>=1.0.0",
     "alchemy-logging>=1.0.4",
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1",
     "grpcio-health-checking>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0",
@@ -25,10 +27,13 @@
     "py-grpc-prometheus>=0.7.0,<0.8",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
     "semver>=2.13.0,<3.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
     "wheel>=0.37.0",
-    "jtd-to-proto>=0.11.4,<0.12.0",
+    "jtd-to-proto>=0.12.1,<0.13.0",
     "import-tracker>=3.1.5,<4",
 ]
+
+[project.urls]
+Source = "https://github.com/caikit/caikit"
```

### Comparing `caikit-0.1.1/scripts/fmt.sh` & `caikit-0.1.2/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/__init__.py` & `caikit-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/base.py` & `caikit-0.1.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/conftest.py` & `caikit-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.1.2/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.1.2/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/blocks/__init__.py` & `caikit-0.1.2/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/blocks/test_base.py` & `caikit-0.1.2/tests/core/blocks/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,24 @@
 # limitations under the License.
 
 # Standard
 import os
 import shutil
 import tempfile
 
-# Third Party
-# pylint: disable=import-error
-from sample_lib.blocks.sample_task import SampleBlock
-from sample_lib.data_model.sample import SampleInputType
-
 # Local
 from caikit.core.blocks import block
 from caikit.core.blocks.base import BlockSaver
 from caikit.core.config import lib_config
 from caikit.core.toolkit.serializers import JSONSerializer
 
+# pylint: disable=import-error
+from sample_lib.blocks.sample_task import SampleBlock
+from sample_lib.data_model.sample import SampleInputType
+
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 import caikit.core
 
 
 class TestBlockBase(TestCaseBase):
     @classmethod
```

### Comparing `caikit-0.1.1/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.1.2/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/data_model/streams/test_converter.py` & `caikit-0.1.2/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.1.2/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.1.2/tests/core/data_model/streams/test_data_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 import os
 
-# Third Party
-from sample_lib.blocks.sample_task.sample_implementation import SampleBlock
-from sample_lib.data_model.sample import SampleInputType, SampleOutputType
-
 # Local
 from caikit.core import data_model as core_dm
 from caikit.core.augmentors import AugmentorBase
+from sample_lib.blocks.sample_task.sample_implementation import SampleBlock
+from sample_lib.data_model.sample import SampleInputType, SampleOutputType
 
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 import caikit.core
 
 
 def build_test_augmentor(produces_none):
```

### Comparing `caikit-0.1.1/tests/core/data_model/streams/test_resolver.py` & `caikit-0.1.2/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/data_model/streams/test_validator.py` & `caikit-0.1.2/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/data_model/test_base.py` & `caikit-0.1.2/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/data_model/test_dataobject.py` & `caikit-0.1.2/tests/core/data_model/test_dataobject.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for the @dataobject decorator"""
 
 # Standard
+from typing import Optional
 import json
 import os
 import tempfile
 
 # Third Party
 from google.protobuf import descriptor_pool, message
 import pytest
@@ -217,14 +218,72 @@
         FooBar.get_proto_class(), "bar", BarEnum._proto_enum.DESCRIPTOR
     )
     assert check_field_enum_type(
         FooBar.get_proto_class(), "bare_bar", BarEnum._proto_enum.DESCRIPTOR
     )
 
 
+def test_dataobject_obj_refs_with_optional_types():
+    """Make sure that references to other data objects and enums work as
+    expected
+    """
+
+    @dataobject({"enum": ["EXAM", "METAL"]})
+    class BarEnum:
+        pass
+
+    @dataobject({"foo": str})
+    class Foo:
+        pass
+
+    # The dataobject in question: includes Optional[T]
+    @dataobject(
+        schema={
+            "foo": Foo,
+            "optionalFoo": Optional[Foo],
+            "bar": BarEnum,
+            "optionalBar": Optional[BarEnum],
+        }
+    )
+    class FooBar:
+        pass
+
+    assert check_field_type(FooBar._proto_class, "foo", "TYPE_MESSAGE")
+    for field in ["foo", "optionalFoo"]:
+        assert check_field_message_type(
+            FooBar._proto_class, field, Foo._proto_class.DESCRIPTOR
+        )
+    for field in ["bar", "optionalBar"]:
+        assert check_field_enum_type(
+            FooBar._proto_class, field, BarEnum._proto_enum.DESCRIPTOR
+        )
+
+
+def test_dataobject_properties_needs_jtd_translation():
+    """Make sure shorthand get recognized as still needing jtd translation
+    when inside properties or optionalProperties
+    """
+
+    @dataobject(
+        schema={
+            "properties": {
+                "foo": int,
+            },
+            "optionalProperties": {
+                "bar": bool,
+            },
+        }
+    )
+    class FooBar:
+        pass
+
+    assert check_field_type(FooBar.get_proto_class(), "foo", "TYPE_INT64")
+    assert check_field_type(FooBar.get_proto_class(), "bar", "TYPE_BOOL")
+
+
 def test_dataobject_invalid_schema():
     """Make sure that a ValueError is raised on an invalid schema"""
     with pytest.raises(ValueError):
         # pylint: disable=unused-variable
         @dataobject("Foo")
         class Foo:
             pass
```

### Comparing `caikit-0.1.1/tests/core/helpers.py` & `caikit-0.1.2/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/module_backends/test_backend_types.py` & `caikit-0.1.2/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/test_config.py` & `caikit-0.1.2/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/test_imports.py` & `caikit-0.1.2/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/test_model_manager.py` & `caikit-0.1.2/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/test_module.py` & `caikit-0.1.2/tests/core/test_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,28 @@
 import abc
 import io
 import os
 import tempfile
 import uuid
 
 # Third Party
-# pylint: disable=import-error
-from sample_lib.blocks.sample_task import SampleBlock
-from sample_lib.data_model.sample import SampleInputType
 import pytest
 
 # First Party
 import aconfig
 
 # Local
 from caikit.core import ModuleConfig, module
 from caikit.core.module_backend_config import get_backend
 from caikit.core.module_backends import backend_types
 
+# pylint: disable=import-error
+from sample_lib.blocks.sample_task import SampleBlock
+from sample_lib.data_model.sample import SampleInputType
+
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 
 # NOTE: We do need to import `reset_backend_types` and `reset_module_distribution_registry` for `reset_globals` to work
 from tests.core.helpers import *
 import caikit.core
```

### Comparing `caikit-0.1.1/tests/core/test_module_backend_config.py` & `caikit-0.1.2/tests/core/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/test_module_metadata.py` & `caikit-0.1.2/tests/core/test_module_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 
 # Standard
 from typing import Any, Dict, Set
 import os
 import tempfile
 
 # Third Party
+import pytest
+
+# Local
+from caikit.core import toolkit
+
 # pylint: disable=import-error
 from sample_lib.blocks.sample_task import SampleBlock
 
 # pylint: disable=import-error
 from sample_lib.workflows.sample_task import SampleWorkflow
-import pytest
-
-# Local
-from caikit.core import toolkit
 
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 import caikit.core
 
 # scratch:
 # - might want to support like a `saved` date?
```

### Comparing `caikit-0.1.1/tests/core/test_no_write_permissions.py` & `caikit-0.1.2/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/toolkit/test_compatibility.py` & `caikit-0.1.2/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/toolkit/test_config_utils.py` & `caikit-0.1.2/tests/core/toolkit/test_config_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/toolkit/test_error_handler.py` & `caikit-0.1.2/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/toolkit/test_extension_utils.py` & `caikit-0.1.2/tests/core/toolkit/test_extension_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/toolkit/test_fileio.py` & `caikit-0.1.2/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.1.2/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/toolkit/test_serializers.py` & `caikit-0.1.2/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.1.2/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/workflows/__init__.py` & `caikit-0.1.2/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/core/workflows/test_base.py` & `caikit-0.1.2/tests/core/workflows/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 import os
 import tempfile
 
-# Third Party
-# pylint: disable=import-error
-from sample_lib.blocks.sample_task import SampleBlock
-from sample_lib.data_model.sample import SampleInputType
-from sample_lib.workflows.sample_task import SampleWorkflow
-
 # Local
 from caikit.core.config import lib_config
 from caikit.core.workflows import workflow
 from caikit.core.workflows.base import WorkflowLoader, WorkflowSaver
 
+# pylint: disable=import-error
+from sample_lib.blocks.sample_task import SampleBlock
+from sample_lib.data_model.sample import SampleInputType
+from sample_lib.workflows.sample_task import SampleWorkflow
+
 # Unit Test Infrastructure
 from tests.base import TestCaseBase
 import caikit.core
 
 
 class SampleWorkflowLoader(caikit.core.module.ModuleLoader):
     pass
```

### Comparing `caikit-0.1.1/tests/data_model_helpers.py` & `caikit-0.1.2/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/dummy_block.zip` & `caikit-0.1.2/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/dummy_block/config.yml` & `caikit-0.1.2/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.1.2/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/dummy_resource.zip` & `caikit-0.1.2/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/dummy_workflow.zip` & `caikit-0.1.2/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.1.2/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/fixtures.py` & `caikit-0.1.2/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/invalid.zip` & `caikit-0.1.2/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/linux.txt` & `caikit-0.1.2/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/primitive_party.proto` & `caikit-0.1.2/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.1.2/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.1.2/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.1.2/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.1.2/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/fixtures/studio_models/studio_block` & `caikit-0.1.2/tests/fixtures/studio_models/studio_block`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/generated/__init__.py` & `caikit-0.1.2/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/metrics/__init__.py` & `caikit-0.1.2/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.1.2/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/metrics/test_throughput.py` & `caikit-0.1.2/tests/runtime/metrics/test_throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/model_management/__init__.py` & `caikit-0.1.2/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/model_management/test_batcher.py` & `caikit-0.1.2/tests/runtime/model_management/test_batcher.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 # Standard
 import os
 import queue
 import threading
 import time
 
 # Third Party
-from sample_lib.data_model import SampleOutputType
 import pytest
 
 # First Party
 import alog
 
 # Local
 from caikit.runtime.model_management.batcher import Batcher
+from sample_lib.data_model import SampleOutputType
 import caikit.core
 
 ## Helpers #####################################################################
 
 log = alog.use_channel("TEST")
 
 DUMMY_MODEL = os.path.realpath(
```

### Comparing `caikit-0.1.1/tests/runtime/model_management/test_model_loader.py` & `caikit-0.1.2/tests/runtime/model_management/test_model_loader.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 from contextlib import contextmanager
 import copy
 import tempfile
 import unittest
 import uuid
 
 # Third Party
-from sample_lib.blocks.sample_task import SampleBlock
-from sample_lib.data_model import SampleInputType, SampleOutputType
 import grpc
 import pytest
 
 # Local
 from caikit.core import ModuleConfig
 from caikit.core.blocks import base, block
 from caikit.core.module_backend_config import _CONFIGURED_BACKENDS, configure
 from caikit.core.module_backends import BackendBase, backend_types
 from caikit.core.module_backends.backend_types import register_backend_type
 from caikit.runtime.model_management.batcher import Batcher
 from caikit.runtime.model_management.model_loader import ModelLoader
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.config_parser import ConfigParser
+from sample_lib.blocks.sample_task import SampleBlock
+from sample_lib.data_model import SampleInputType, SampleOutputType
 from tests.conftest import temp_config_parser
 from tests.fixtures import Fixtures
 
 ## Helpers #####################################################################
 
 
 def _random_test_id():
```

### Comparing `caikit-0.1.1/tests/runtime/model_management/test_model_manager.py` & `caikit-0.1.2/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.1.2/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/model_management/test_training_manager.py` & `caikit-0.1.2/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.1.2/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/service_generation/test_create_service.py` & `caikit-0.1.2/tests/runtime/service_generation/test_create_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# Third Party
-import sample_lib
-
 # Local
 from caikit.runtime.service_generation.create_service import (
     create_inference_rpcs,
     create_training_rpcs,
 )
+import sample_lib
 
 ## Setup ########################################################################
 
 widget_class = sample_lib.blocks.sample_task.SampleBlock
 untrainable_module_class = sample_lib.blocks.sample_task.SamplePrimitiveBlock
 
 ## Tests ########################################################################
```

### Comparing `caikit-0.1.1/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.1.2/tests/runtime/service_generation/test_data_stream_source.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from typing import List
 import json
 import os
 import pickle
 import tempfile
 
 # Third Party
-from sample_lib.data_model.sample import SampleTrainingType
 import pytest
 
 # Local
 from caikit.core.data_model.streams.data_stream import DataStream
 from caikit.runtime.service_generation.data_stream_source import (
     DataStreamSourceBase,
     _make_data_stream_source_type_name,
     get_data_stream_source,
     make_data_stream_source,
 )
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
+from sample_lib.data_model.sample import SampleTrainingType
 from tests.conftest import temp_config_parser
 import caikit
 
 ################################################
 # Fixtures
```

### Comparing `caikit-0.1.1/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.1.2/tests/runtime/service_generation/test_type_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 from typing import List, Optional, Union
 
-# Third Party
-import sample_lib
-
 # Local
 from caikit.core.data_model import DataStream
 from caikit.runtime.service_generation.type_helpers import (
     get_data_stream_type,
     has_data_stream,
     is_model_type,
 )
+import sample_lib
 
 
 def test_data_stream_helpers():
     assert has_data_stream(DataStream[int])
     assert has_data_stream(Optional[DataStream[int]])
     assert has_data_stream(Union[List[DataStream[int]], str])
```

### Comparing `caikit-0.1.1/tests/runtime/servicers/__init__.py` & `caikit-0.1.2/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.1.2/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,24 @@
 import os
 import tempfile
 import threading
 import time
 import uuid
 
 # Third Party
-from sample_lib.blocks.sample_task import SampleBlock
-from sample_lib.data_model import SampleInputType, SampleOutputType
 import grpc
 import pytest
-import sample_lib
 
 # Local
 from caikit.runtime.servicers.global_predict_servicer import GlobalPredictServicer
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
+from sample_lib.blocks.sample_task import SampleBlock
+from sample_lib.data_model import SampleInputType, SampleOutputType
 from tests.fixtures import Fixtures
-from tests.fixtures.protobufs import primitive_party_pb2
+import sample_lib
 
 
 def _random_test_id():
     return "test-any-model-" + str(uuid.uuid4())
 
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
```

### Comparing `caikit-0.1.1/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.1.2/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 # Standard
 from tempfile import TemporaryDirectory
 import time
 import uuid
 
 # Third Party
-from sample_lib.blocks.sample_task.sample_implementation import SampleBlock
-from sample_lib.data_model.sample import (
-    SampleInputType,
-    SampleOutputType,
-    SampleTrainingType,
-)
 import pytest
 
 # Local
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.servicers.global_train_servicer import GlobalTrainServicer
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
+from sample_lib.blocks.sample_task.sample_implementation import SampleBlock
+from sample_lib.data_model.sample import (
+    SampleInputType,
+    SampleOutputType,
+    SampleTrainingType,
+)
 from tests.conftest import temp_config_parser
 from tests.fixtures import Fixtures
 from tests.fixtures.protobufs import primitive_party_pb2
 import caikit.core
 
 ## Helpers #####################################################################
```

### Comparing `caikit-0.1.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.1.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.1.2/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 import os
 import tempfile
 import uuid
 
 # Third Party
 import grpc
 import pytest
-import sample_lib
 
 # Local
 from caikit.interfaces.runtime.data_model import TrainingStatus
 from caikit.runtime.protobufs import process_pb2
 from caikit.runtime.servicers.model_train_servicer import ModelTrainServicerImpl
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from tests.conftest import temp_config_parser
+import sample_lib
 
 
 @pytest.fixture
 def sample_model_train_servicer(sample_train_service) -> ModelTrainServicerImpl:
     servicer = ModelTrainServicerImpl(training_service=sample_train_service)
     yield servicer
```

### Comparing `caikit-0.1.1/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.1.2/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/test_grpc_server.py` & `caikit-0.1.2/tests/runtime/test_grpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,38 +14,29 @@
 # Have pylint ignore Class XXXX has no YYYY member so that we can use gRPC enums.
 # pylint: disable=E1101
 # Standard
 from dataclasses import dataclass
 from unittest import mock
 import json
 import os
-import tempfile
 import threading
 import time
 import uuid
 
 # Third Party
 from grpc_health.v1 import health_pb2, health_pb2_grpc
-from sample_lib.data_model import (
-    OtherOutputType,
-    SampleInputType,
-    SampleOutputType,
-    SampleTrainingType,
-)
 import grpc
 import pytest
-import sample_lib
 import tls_test_tools
 
 # First Party
 import alog
 
 # Local
 from caikit.interfaces.runtime.data_model import (
-    ModelPointer,
     TrainingInfoRequest,
     TrainingInfoResponse,
     TrainingJob,
     TrainingStatus,
 )
 from caikit.runtime.grpc_server import RuntimeGRPCServer
 from caikit.runtime.model_management.model_manager import ModelManager
@@ -54,17 +45,24 @@
     model_runtime_pb2,
     model_runtime_pb2_grpc,
     process_pb2,
     process_pb2_grpc,
 )
 from caikit.runtime.service_factory import ServicePackage, ServicePackageFactory
 from caikit.runtime.utils.config_parser import ConfigParser
+from sample_lib.data_model import (
+    OtherOutputType,
+    SampleInputType,
+    SampleOutputType,
+    SampleTrainingType,
+)
 from tests.conftest import temp_config_parser
 from tests.fixtures import Fixtures
 import caikit
+import sample_lib
 
 log = alog.use_channel("TEST-SERVE-I")
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
 HAPPY_PATH_RESPONSE = SampleOutputType(greeting="Hello Gabe").to_proto()
 HAPPY_PATH_TRAIN_RESPONSE = TrainingJob(
     model_name="dummy name", training_id="dummy id"
@@ -74,33 +72,37 @@
 def is_good_train_response(actual_response, expected, model_name):
     assert dir(actual_response) == dir(expected)
     assert actual_response.training_id is not None
     assert isinstance(actual_response.training_id, str)
     assert actual_response.model_name == model_name
 
 
-# TODO: Fix this with optional fields support - https://github.com/IBM/jtd-to-proto/issues/34
-@pytest.mark.skip("Waiting for optional fields support")
 def test_model_train(runtime_grpc_server):
     """Test model train's RUN function"""
     model_train_stub = process_pb2_grpc.ProcessStub(
         runtime_grpc_server.make_local_channel()
     )
     training_id = str(uuid.uuid4())
     model_train_request = process_pb2.ProcessRequest(
         trainingID=training_id,
         customTrainingID=str(uuid.uuid4()),
         request_dict={
             "train_module": "00110203-0405-0607-0809-0a0b02dd0e0f",
             "training_params": json.dumps(
                 {
                     "model_name": "abc",
-                    "training_data": [
-                        sample_lib.data_model.SampleTrainingType(number=1).to_dict()
-                    ],
+                    "training_data": {
+                        "jsondata": {
+                            "data": [
+                                sample_lib.data_model.SampleTrainingType(
+                                    number=1
+                                ).to_dict()
+                            ]
+                        },
+                    },
                 }
             ),
         },
         training_input_dir="training_input_dir",
         training_output_dir=os.path.join("test", "training_output", training_id),
     )
     training_response = model_train_stub.Run(model_train_request)
@@ -128,22 +130,24 @@
 
     # MT training is sync, so it should be COMPLETE immediately
     response: TrainingInfoResponse = TrainingInfoResponse.from_proto(
         training_management_stub.GetTrainingStatus(training_info_request)
     )
     assert response.status == TrainingStatus.COMPLETED
 
-    # make sure we wait for training to finish
+    # Make sure we wait for training to finish
     result = TrainingManager.get_instance().training_futures[training_id].result()
 
-    assert result.batch_size == 64
     assert (
         result.BLOCK_CLASS
         == "sample_lib.blocks.sample_task.sample_implementation.SampleBlock"
     )
+    # Fields with defaults have expected values
+    assert result.batch_size == 64
+    assert result.learning_rate == 0.0015
 
 
 def test_predict_fake_block_ok_response(
     loaded_model_id, runtime_grpc_server, sample_inference_service
 ):
     """Test RPC CaikitRuntime.WidgetPredict successful response"""
     stub = sample_inference_service.stub_class(runtime_grpc_server.make_local_channel())
```

### Comparing `caikit-0.1.1/tests/runtime/test_service_factory.py` & `caikit-0.1.2/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/utils/__init__.py` & `caikit-0.1.2/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/utils/test_configs.py` & `caikit-0.1.2/tests/runtime/utils/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/utils/test_import_util.py` & `caikit-0.1.2/tests/runtime/utils/test_import_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     mock_config = SimpleNamespace(**{"caikit_library": "sys"})
     data_model = get_data_model(mock_config)
     assert isinstance(data_model, UnifiedDataModel)
 
 
 def test_get_data_model_is_accessible():
     """get_data_model should return the stuff in the `sample_lib.data_model` package"""
-    # Third Party
+    # Local
     import sample_lib
 
     cdm = get_data_model()
     attrs_match = [
         (hasattr(cdm, attr_name) and getattr(cdm, attr_name) == attr_val)
         for attr_name, attr_val in vars(sample_lib.data_model).items()
         if not attr_name.startswith("_")
```

### Comparing `caikit-0.1.1/tests/runtime/utils/test_servicer_util.py` & `caikit-0.1.2/tests/runtime/utils/test_servicer_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,35 +13,35 @@
 # limitations under the License.
 
 # Standard
 import os
 import tempfile
 
 # Third Party
-from sample_lib.data_model import SampleInputType, SampleTrainingType
 import pytest
-import sample_lib
 
 # Local
 from caikit.runtime.protobufs import model_runtime_pb2
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import get_data_model
 from caikit.runtime.utils.servicer_util import (
     build_caikit_library_request_dict,
     build_proto_response,
     get_metadata,
     is_protobuf_primitive_field,
     validate_caikit_library_class_exists,
     validate_caikit_library_class_method_exists,
     validate_data_model,
 )
+from sample_lib.data_model import SampleInputType
 from tests.fixtures import Fixtures
 from tests.fixtures.protobufs import primitive_party_pb2
 import caikit.core
 import caikit.interfaces
+import sample_lib
 
 
 # ---------------- Tests for validate_caikit_library_class_exists --------------------
 def test_servicer_util_validate_caikit_library_class_exists_returns_caikit_class():
     """Test that validate_caikit_library_class_exists returns a caikit class object"""
     validated_class = validate_caikit_library_class_exists(
         get_data_model(), "TrainingInfoResponse"
@@ -217,18 +217,16 @@
     request_dict = build_caikit_library_request_dict(
         sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT
         ),
         sample_lib.blocks.sample_task.SampleBlock().run,
     )
 
-    expected_arguments = set(
-        sample_lib.blocks.sample_task.SampleBlock().run.__code__.co_varnames
-    )
-    expected_arguments.remove("self")
+    # No self or "throw", throw was not set and the throw parameter contains a default value
+    expected_arguments = {"sample_input"}
 
     assert expected_arguments == set(request_dict.keys())
     assert isinstance(request_dict["sample_input"], SampleInputType)
 
 
 def test_global_predict_build_caikit_library_request_dict_strips_invalid_run_kwargs_from_request(
     sample_inference_service,
@@ -238,18 +236,15 @@
     request_dict = build_caikit_library_request_dict(
         sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT, int_type=5, bool_type=True
         ),
         sample_lib.blocks.sample_task.SampleBlock().run,
     )
 
-    expected_arguments = set(
-        sample_lib.blocks.sample_task.SampleBlock().run.__code__.co_varnames
-    )
-    expected_arguments.remove("self")
+    expected_arguments = {"sample_input"}
     assert expected_arguments == set(request_dict.keys())
     assert "int_type" not in request_dict.keys()
 
 
 def test_global_predict_build_caikit_library_request_dict_strips_empty_list_from_request(
     sample_inference_service,
 ):
@@ -352,25 +347,23 @@
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.blocks.sample_task.SampleBlock().train,
     )
 
-    expected_arguments = set(
-        sample_lib.blocks.sample_task.SampleBlock().train.__code__.co_varnames
-    )
-    expected_arguments.remove("cls")
+    expected_arguments = {"training_data"}
 
-    # assert that even though not passed in, caikit.core_request now has both batch_size and training_data
+    # assert that even though not passed in, caikit.core_request now has training_data
+    # because empty stream types get an empty steam initialized
+    # TODO: will need additional tests for list arguments
     assert expected_arguments == set(caikit.core_request.keys())
     assert isinstance(
         caikit.core_request["training_data"], caikit.core.data_model.DataStream
     )
-    assert caikit.core_request["batch_size"] == 0
 
 
 def test_global_train_build_caikit_library_request_dict_strips_empty_list_from_request(
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict strips empty list from request"""
     # NOTE: not sure this test is relevant anymore, since nothing effectively gets removed?
@@ -384,18 +377,16 @@
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.blocks.sample_task.SampleBlock().train,
     )
 
-    expected_arguments = set(
-        sample_lib.blocks.sample_task.SampleBlock().train.__code__.co_varnames
-    )
-    expected_arguments.remove("cls")
+    # model_name is not expected to be passed through
+    expected_arguments = {"training_data"}
 
     assert expected_arguments == set(caikit.core_request.keys())
 
 
 def test_global_train_build_caikit_library_request_dict_works_for_repeated_fields(
     sample_train_service,
 ):
@@ -410,21 +401,19 @@
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.blocks.sample_task.ListBlock().train,
     )
 
-    expected_arguments = set(
-        sample_lib.blocks.sample_task.ListBlock().train.__code__.co_varnames
-    )
-    expected_arguments.remove("cls")
+    # model_name is not expected to be passed through
+    expected_arguments = {"training_data", "poison_pills"}
 
     assert expected_arguments == set(caikit.core_request.keys())
-    assert len(caikit.core_request.keys()) == 3
+    assert len(caikit.core_request.keys()) == 2
     assert "poison_pills" in caikit.core_request
     assert isinstance(caikit.core_request["poison_pills"], list)
 
 
 def test_global_train_build_caikit_library_request_dict_ok_with_DataStreamSourceInt_with_inline_json(
     sample_train_service,
 ):
@@ -466,18 +455,16 @@
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.blocks.sample_task.SampleBlock().train,
     )
 
-    expected_arguments = set(
-        sample_lib.blocks.sample_task.SampleBlock().train.__code__.co_varnames
-    )
-    expected_arguments.remove("cls")
+    # model_name is not expected to be passed through
+    expected_arguments = {"training_data"}
 
     assert expected_arguments == set(caikit.core_request.keys())
 
 
 def test_global_train_build_caikit_library_request_dict_ok_with_training_data_as_list_of_files(
     sample_train_service, sample_csv_file, sample_json_file
 ):
@@ -493,21 +480,19 @@
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.blocks.sample_task.ListBlock().train,
     )
 
-    expected_arguments = set(
-        sample_lib.blocks.sample_task.ListBlock().train.__code__.co_varnames
-    )
-    expected_arguments.remove("cls")
+    # model_name is not expected to be passed through
+    expected_arguments = {"training_data", "poison_pills"}
 
     assert expected_arguments == set(caikit.core_request.keys())
-    assert len(caikit.core_request.keys()) == 3
+    assert len(caikit.core_request.keys()) == 2
     assert "training_data" in caikit.core_request
 
 
 def test_build_caikit_library_request_dict_works_when_data_stream_directory_includes_mixed_types(
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict works when mixed supported types are present"""
```

### Comparing `caikit-0.1.1/tests/runtime/work_management/__init__.py` & `caikit-0.1.2/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.1.2/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.1.2/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.1.2/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/tox.ini` & `caikit-0.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.1.1/PKG-INFO` & `caikit-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.1.1
+Version: 0.1.2
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.0.0
 Requires-Dist: alchemy-logging>=1.0.4
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: ijson>=3.1.4,<3.2.0
@@ -17,140 +18,64 @@
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<3.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
 Requires-Dist: wheel>=0.37.0
-Requires-Dist: jtd-to-proto>=0.11.4,<0.12.0
+Requires-Dist: jtd-to-proto>=0.12.1,<0.13.0
 Requires-Dist: import-tracker>=3.1.5,<4
+Project-URL: Source, https://github.com/caikit/caikit
 
 # Caikit
 
-Caikit is an AI toolkit that enables users to manage AI models through a set of developer friendly APIs. It provides a consistent format for AI model deployment, consumption and evolution.
+Caikit is an AI toolkit that enables users to manage models through a set of developer friendly APIs. It provides a consistent format for creating and using AI models against a wide variety of data domains and tasks.
 
 ![Caikit Overview](https://raw.githubusercontent.com/caikit/caikit/main/caikit-overview.png)
 
 ## Capabilities
 
-Caikit streamlines the management of AI models for application usage. Think of it as REST API for applications to AI models.
+Caikit streamlines the management of AI models for application usage by letting AI model authors focus on solving well known problems with novel technology. With a set of model implementations based on Caikit, you can:
 
-- Hosts AI models for inference and training so that models can be accessed through APIs
-- Provides access to the different training techniques as supported by a model
-- Supports models from different AI communities like HuggingFace ...
-- Allows applications to change model versions without any code changes
-- Compatability with other AI model runtimes
+- Run training jobs to create models from your data
+- Run model inference using data APIs that represent data as structures rather than tensors
+- Implement the right training techniques to fit the model, from static regexes to multi-GPU distribution
+- Merge models from diverse AI communities into a common API (e.g. `transformers`, `tensorflow`, `sklearn`, etc...)
+- Update applications to newer models for a given task without client-side changes
 
-## What Differentiates Caikit to Other AI Model Runtimes?
+## What Differentiates Caikit from Other AI Model Runtimes?
 
-Developers who write applications that consume AI models are not necessarily AI experts who understand the intricate details of the AI model that they use. Some would like to treat it as a "black box" where they give it input and it returns the output. This is similar in cloud computing whereby some users would like to deploy their applications to the cloud without detailed knowledge of the cloud infrastructure. The value for them is in their application and that is what is of most interest to them.
+Developers who write applications that consume AI models are not necessarily AI experts who understand the intricate details of the AI models that they use. Some would like to treat AI as a "black box function" where they give it input and it returns the output. This is similar in cloud computing whereby some users would like to deploy their applications to the cloud without detailed knowledge of the cloud infrastructure. The value for them is in their application and that is what is of most interest to them.
 
-Caikit provides an abstraction layer for application developers where they can consume an AI model through APIs independent of understanding the data form of the model. In other words, the input and output to the model is in a format which is easily programmable and does not require data transformations. This facilitates the model and the application to evolve independently of each other.
+Caikit provides an abstraction layer for application developers where they can consume AI models through APIs independent of understanding the data form of the model. In other words, the input and output to the model is in a format which is easily programmable and does not require data transformations. This facilitates the model and the application to evolve independently of each other.
 
-Does this matter when you just want to load 1 or 2 models? No. The benefits are when consuming 10s or hundreds of AI model. Caikit simplifies the scaling and maintainence of such integrations compared to other runtimes. This is because other runtimes require an AI centric view of the model (for example, the common interface of “tensor in, tensor out”) which means having to code different data tranformations into the application for each model. Additionally, the data form of the model may change from version to version.
+When deploying a small handful of models, this benefit is minimal. The benefits are generally realized when consuming 10s or hundreds of AI models, or maintaining an application over time as AI technology evolves. Caikit simplifies the scaling and maintenance of such integrations compared to other runtimes. This is because other runtimes require an AI centric view of the model (for example, the common interface of “tensor in, tensor out”) which means having to code different data transformations into the application for each model. Additionally, the data form of the model may change from version to version.
 
 ## User Profiles
 
 There are 2 user profiles who leverage Caikit:
 
 - AI Model Author:
   - Model Authors build and train AI models for data analysis
-  - They bring data and tuning params to a pre-existing model and creates a new model using APIs provided by Caikit
+  - They bring data and tuning params to a pre-existing model architecture and create a new concrete model using APIs provided by Caikit
   - Examples of model authors are machine learning engineers, data scientists, and AI developers
 - AI Model Operator:
-  - Model operators request analysis of a data set by operating on it with a trained AI model (Inference)
+  - Model operators use an existing AI model to perform a specific function within the context of an application
   - They take trained models, deploy them, and then infer the models in applications through APIs provided by Caikit
-  - Examples of operators are application developers, and AI model authors
+  - Examples of operators are cloud and embedded application developers whose applications need analysis of unstructured data
 
-## Quick Start
+## AI Model Operator Quick Start
 
-**TODO: Need to redesign this section**
+**UNDER CONSTRUCTION**
 
-<strike>
+At this point, Caikit does not publish any pre-defined task implementations that can be readily consumed. Stay tuned!
 
-### Prerequisitive
+## AI Model Author Quick Start
 
-Install Caikit toolkit:
+**UNDER CONSTRUCTION**
 
-```console
-pip install caikit
-pip install caikit-nlp
-
-# TODO: import the libraries to enable the sample code to run
-```
-
-### Preprocessing
-
-Start by loading training data from Consumer Financial complaint database:
-
-**TODO: show how to preprocess sample training data**
-
-```python
-
-```
-
-### Training
-
-Train an TF-IDF SVM classifier model on the training data:
-
-```python
-import caikit_nlp
-
-syntax_model = caikit.load('syntax_izumo_en_stock'))
-
-tfidf_classification_model = caikit_nlp.workflows.classification.base_classifier.tfidf_svm.TFidfSvm.train(
-    training_data=training_data,
-    syntax_model=syntax_model, 
-    tfidf_svm_epochs=1,
-    multi_label=True
-)
-```
-
-### Inference
-
-Use the trained model for prediction on new data:
-
-```python
-tfidf_svm_preds = tfidf_classification_model.run(text)
-```
-
-## Start the runtime with the sample_lib! 
-
-Useful for interacting with the runtime with the sample_lib and playing around with it.
-
-### Start the server
-In one terminal, run the script that starts the server:
-
-```
-python3 -m examples.start_runtime_with_sample_lib
-```
-
-### Start training a sample block
-
-This script will also create `protos`. In order to interact with the `sample_lib`, in another terminal, go inside that directory:
-
-```
-cd protos
-```
-then
-
-```
-grpcurl -plaintext -proto samplelibtrainingservice.proto -d '{"model_name": "my_model", "training_data": {"file": {"filename": "protos/sample.json"}}}' localhost:8085 caikit.runtime.SampleLib.SampleLibTrainingService/BlocksSampleTaskSampleBlockTrain
-```
-### Fetch status through training management API
-
-```
-grpcurl -plaintext -proto trainingmanagement.proto -d '{
-    "training_id": "<training_id_from_above_response>"
-}' localhost:8085 caikit.runtime.training.TrainingManagement/GetTrainingStatus
-```
-### Run prediction on trained block
-```
-grpcurl -plaintext -proto samplelibservice.proto -d '{"sample_input": {"name": "blah"}}' -H 'mm-model-id: my_model' localhost:8085 caikit.runtime.SampleLib.SampleLibService/SampleTaskPredict
-```
-
-</strike>
+We're getting a slim example ready, so stay tuned!
 
 ## Code of conduct
 
 Participation in the Caikit community is governed by the [Code of Conduct](CODE-OF-CONDUCT.md).
```

