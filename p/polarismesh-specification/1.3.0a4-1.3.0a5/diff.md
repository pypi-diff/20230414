# Comparing `tmp/polarismesh_specification-1.3.0a4.tar.gz` & `tmp/polarismesh_specification-1.3.0a5.tar.gz`

## Comparing `polarismesh_specification-1.3.0a4.tar` & `polarismesh_specification-1.3.0a5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    15838 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0     4864 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/pyproject.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a4/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    15838 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0     4864 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/pyproject.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/PKG-INFO
```

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/code_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from ..service_manage import service_pb2 as service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fheartbeat.proto\x12\x02v1\x1a\rservice.proto\"\xc0\x01\n\x0fHeartbeatRecord\x12\x1f\n\ninstanceId\x18\x01 \x01(\tR\x0binstance_id\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12\x12\n\x04host\x18\x04 \x01(\tR\x04host\x12\x12\n\x04port\x18\x05 \x01(\rR\x04port\x12,\n\x10lastHeartbeatSec\x18\x06 \x01(\x03R\x12last_heartbeat_sec\":\n\nHeartbeats\x12,\n\nheartbeats\x18\x01 \x03(\x0b\x32\x0c.v1.InstanceR\nheartbeats\"9\n\x14GetHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"F\n\x15GetHeartbeatsResponse\x12-\n\x07records\x18\x01 \x03(\x0b\x32\x13.v1.HeartbeatRecordR\x07records\"9\n\x14\x44\x65lHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"3\n\x15\x44\x65lHeartbeatsResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\r\x12\x0c\n\x04info\x18\x02 \x01(\tB\x7f\n7com.tencent.polaris.specification.api.v1.service.manageZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fheartbeat.proto\x12\x02v1\x1a\rservice.proto\"\xd6\x01\n\x0fHeartbeatRecord\x12\x1f\n\ninstanceId\x18\x01 \x01(\tR\x0binstance_id\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12\x12\n\x04host\x18\x04 \x01(\tR\x04host\x12\x12\n\x04port\x18\x05 \x01(\rR\x04port\x12,\n\x10lastHeartbeatSec\x18\x06 \x01(\x03R\x12last_heartbeat_sec\x12\x14\n\x05\x65xist\x18\x07 \x01(\x08R\x05\x65xist\":\n\nHeartbeats\x12,\n\nheartbeats\x18\x01 \x03(\x0b\x32\x0c.v1.InstanceR\nheartbeats\"9\n\x14GetHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"F\n\x15GetHeartbeatsResponse\x12-\n\x07records\x18\x01 \x03(\x0b\x32\x13.v1.HeartbeatRecordR\x07records\"9\n\x14\x44\x65lHeartbeatsRequest\x12!\n\x0binstanceIds\x18\x01 \x03(\tR\x0cinstance_ids\"3\n\x15\x44\x65lHeartbeatsResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\r\x12\x0c\n\x04info\x18\x02 \x01(\tB\x7f\n7com.tencent.polaris.specification.api.v1.service.manageZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'heartbeat_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
   _HEARTBEATRECORD._serialized_start=39
-  _HEARTBEATRECORD._serialized_end=231
-  _HEARTBEATS._serialized_start=233
-  _HEARTBEATS._serialized_end=291
-  _GETHEARTBEATSREQUEST._serialized_start=293
-  _GETHEARTBEATSREQUEST._serialized_end=350
-  _GETHEARTBEATSRESPONSE._serialized_start=352
-  _GETHEARTBEATSRESPONSE._serialized_end=422
-  _DELHEARTBEATSREQUEST._serialized_start=424
-  _DELHEARTBEATSREQUEST._serialized_end=481
-  _DELHEARTBEATSRESPONSE._serialized_start=483
-  _DELHEARTBEATSRESPONSE._serialized_end=534
+  _HEARTBEATRECORD._serialized_end=253
+  _HEARTBEATS._serialized_start=255
+  _HEARTBEATS._serialized_end=313
+  _GETHEARTBEATSREQUEST._serialized_start=315
+  _GETHEARTBEATSREQUEST._serialized_end=372
+  _GETHEARTBEATSRESPONSE._serialized_start=374
+  _GETHEARTBEATSRESPONSE._serialized_end=444
+  _DELHEARTBEATSREQUEST._serialized_start=446
+  _DELHEARTBEATSREQUEST._serialized_end=503
+  _DELHEARTBEATSRESPONSE._serialized_start=505
+  _DELHEARTBEATSRESPONSE._serialized_end=556
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -29,27 +29,29 @@
 class GetHeartbeatsResponse(_message.Message):
     __slots__ = ["records"]
     RECORDS_FIELD_NUMBER: _ClassVar[int]
     records: _containers.RepeatedCompositeFieldContainer[HeartbeatRecord]
     def __init__(self, records: _Optional[_Iterable[_Union[HeartbeatRecord, _Mapping]]] = ...) -> None: ...
 
 class HeartbeatRecord(_message.Message):
-    __slots__ = ["host", "instanceId", "lastHeartbeatSec", "namespace", "port", "service"]
+    __slots__ = ["exist", "host", "instanceId", "lastHeartbeatSec", "namespace", "port", "service"]
+    EXIST_FIELD_NUMBER: _ClassVar[int]
     HOST_FIELD_NUMBER: _ClassVar[int]
     INSTANCEID_FIELD_NUMBER: _ClassVar[int]
     LASTHEARTBEATSEC_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     PORT_FIELD_NUMBER: _ClassVar[int]
     SERVICE_FIELD_NUMBER: _ClassVar[int]
+    exist: bool
     host: str
     instanceId: str
     lastHeartbeatSec: int
     namespace: str
     port: int
     service: str
-    def __init__(self, instanceId: _Optional[str] = ..., service: _Optional[str] = ..., namespace: _Optional[str] = ..., host: _Optional[str] = ..., port: _Optional[int] = ..., lastHeartbeatSec: _Optional[int] = ...) -> None: ...
+    def __init__(self, instanceId: _Optional[str] = ..., service: _Optional[str] = ..., namespace: _Optional[str] = ..., host: _Optional[str] = ..., port: _Optional[int] = ..., lastHeartbeatSec: _Optional[int] = ..., exist: bool = ...) -> None: ...
 
 class Heartbeats(_message.Message):
     __slots__ = ["heartbeats"]
     HEARTBEATS_FIELD_NUMBER: _ClassVar[int]
     heartbeats: _containers.RepeatedCompositeFieldContainer[_service_pb2.Instance]
     def __init__(self, heartbeats: _Optional[_Iterable[_Union[_service_pb2.Instance, _Mapping]]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/LICENSE.txt` & `polarismesh_specification-1.3.0a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/README.md` & `polarismesh_specification-1.3.0a5/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/pyproject.toml` & `polarismesh_specification-1.3.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a4/PKG-INFO` & `polarismesh_specification-1.3.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarismesh-specification
-Version: 1.3.0a4
+Version: 1.3.0a5
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

