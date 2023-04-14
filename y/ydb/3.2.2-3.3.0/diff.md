# Comparing `tmp/ydb-3.2.2.tar.gz` & `tmp/ydb-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydb-3.2.2.tar", last modified: Thu Apr  6 11:52:04 2023, max compression
+gzip compressed data, was "ydb-3.3.0.tar", last modified: Fri Apr 14 17:36:18 2023, max compression
```

## Comparing `ydb-3.2.2.tar` & `ydb-3.3.0.tar`

### file list

```diff
@@ -1,248 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.444212 ydb-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-06 11:51:54.000000 ydb-3.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-06 11:51:54.000000 ydb-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 11:51:54.000000 ydb-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-06 11:52:04.444212 ydb-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-06 11:51:54.000000 ydb-3.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-06 11:51:54.000000 ydb-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-06 11:51:54.000000 ydb-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 11:52:04.444212 ydb-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-06 11:51:57.000000 ydb-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.444212 ydb-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-06 11:51:54.000000 ydb-3.2.2/tests/test_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.420212 ydb-3.2.2/ydb/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.420212 ydb-3.2.2/ydb/_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.420212 ydb-3.2.2/ydb/_grpc/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.420212 ydb-3.2.2/ydb/_grpc/grpcwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/grpcwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/grpcwrapper/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/grpcwrapper/ydb_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    42335 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/grpcwrapper/ydb_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/grpcwrapper/ydb_topic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.424212 ydb-3.2.2/ydb/_grpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.428212 ydb-3.2.2/ydb/_grpc/v3/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.428212 ydb-3.2.2/ydb/_grpc/v3/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-06 11:51:54.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.432212 ydb-3.2.2/ydb/_grpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.436212 ydb-3.2.2/ydb/_grpc/v4/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.436212 ydb-3.2.2/ydb/_grpc/v4/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_session_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14424 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_sp_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.436212 ydb-3.2.2/ydb/_topic_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_common/common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_common/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.440212 ydb-3.2.2/ydb/_topic_reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_reader/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_reader/datatypes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_reader/topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22781 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_reader/topic_reader_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    46742 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_reader/topic_reader_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_reader/topic_reader_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.440212 ydb-3.2.2/ydb/_topic_writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_writer/topic_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23229 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_writer/topic_writer_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_writer/topic_writer_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_writer/topic_writer_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_topic_writer/topic_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_tx_ctx_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/_utilities_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.440212 ydb-3.2.2/ydb/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/aio/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/auth_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.444212 ydb-3.2.2/ydb/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/dbapi/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/dbapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/default_pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.444212 ydb-3.2.2/ydb/iam/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/iam/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/import_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/scheme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.444212 ydb-3.2.2/ydb/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/sqlalchemy/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-04-06 11:51:55.000000 ydb-3.2.2/ydb/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-06 11:51:57.000000 ydb-3.2.2/ydb/ydb_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:52:04.444212 ydb-3.2.2/ydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-06 11:52:04.000000 ydb-3.2.2/ydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-06 11:52:04.000000 ydb-3.2.2/ydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:52:04.000000 ydb-3.2.2/ydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-06 11:52:04.000000 ydb-3.2.2/ydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-06 11:52:04.000000 ydb-3.2.2/ydb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-14 17:36:08.000000 ydb-3.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-14 17:36:08.000000 ydb-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 17:36:08.000000 ydb-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 17:36:18.365202 ydb-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-14 17:36:08.000000 ydb-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 17:36:08.000000 ydb-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 17:36:08.000000 ydb-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:36:18.365202 ydb-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 17:36:11.000000 ydb-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.313202 ydb-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.313202 ydb-3.3.0/tests/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_async_iter_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_session_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/aio/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/session_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.313202 ydb-3.3.0/tests/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/ssl/test_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.313202 ydb-3.3.0/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/table/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/table/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.317202 ydb-3.3.0/tests/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/topics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/topics/test_control_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/topics/test_topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-04-14 17:36:08.000000 ydb-3.3.0/tests/topics/test_topic_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.321202 ydb-3.3.0/ydb/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.325202 ydb-3.3.0/ydb/_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.325202 ydb-3.3.0/ydb/_grpc/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.325202 ydb-3.3.0/ydb/_grpc/grpcwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42486 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.329202 ydb-3.3.0/ydb/_grpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.341202 ydb-3.3.0/ydb/_grpc/v3/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.341202 ydb-3.3.0/ydb/_grpc/v3/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.349202 ydb-3.3.0/ydb/_grpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.357202 ydb-3.3.0/ydb/_grpc/v4/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.357202 ydb-3.3.0/ydb/_grpc/v4/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_session_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_sp_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.357202 ydb-3.3.0/ydb/_topic_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_common/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_common/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.361202 ydb-3.3.0/ydb/_topic_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/datatypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/topic_reader_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/topic_reader_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_reader/topic_reader_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.361202 ydb-3.3.0/ydb/_topic_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_topic_writer/topic_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_tx_ctx_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/_utilities_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/aio/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/auth_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/dbapi/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/dbapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/default_pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/iam/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/import_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/scheme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/sqlalchemy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-04-14 17:36:08.000000 ydb-3.3.0/ydb/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 17:36:11.000000 ydb-3.3.0/ydb/ydb_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:36:18.365202 ydb-3.3.0/ydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 17:36:18.000000 ydb-3.3.0/ydb.egg-info/top_level.txt
```

### Comparing `ydb-3.2.2/LICENSE` & `ydb-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/PKG-INFO` & `ydb-3.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.2.2
+Version: 3.3.0
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.2.2/README.md` & `ydb-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/setup.py` & `ydb-3.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for line in r.readlines():
         line = line.strip()
         if line != "":
             requirements.append(line)
 
 setuptools.setup(
     name="ydb",
-    version="3.2.2",  # AUTOVERSION
+    version="3.3.0",  # AUTOVERSION
     description="YDB Python SDK",
     author="Yandex LLC",
     author_email="ydb@yandex-team.ru",
     url="http://github.com/ydb-platform/ydb-python-sdk",
     license="Apache 2.0",
     package_dir={"": "."},
     long_description=long_description,
```

### Comparing `ydb-3.2.2/tests/test_errors.py` & `ydb-3.3.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/__init__.py` & `ydb-3.3.0/ydb/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from pkgutil import extend_path
+
+__path__ = extend_path(__path__, __name__)
+
 from .credentials import *  # noqa
 from .driver import *  # noqa
 from .global_settings import *  # noqa
 from .table import *  # noqa
 from .issues import *  # noqa
 from .types import *  # noqa
 from .scheme import *  # noqa
```

### Comparing `ydb-3.2.2/ydb/_apis.py` & `ydb-3.3.0/ydb/_apis.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_errors.py` & `ydb-3.3.0/ydb/_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/common/__init__.py` & `ydb-3.3.0/ydb/_grpc/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/grpcwrapper/common_utils.py` & `ydb-3.3.0/ydb/_grpc/grpcwrapper/common_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,22 +270,23 @@
 
     loop = asyncio.get_running_loop()
     ctx = contextvars.copy_context()
     func_call = functools.partial(ctx.run, func, *args, **kwargs)
     return await loop.run_in_executor(None, func_call)
 
 
-def proto_duration_from_timedelta(t: Optional[datetime.timedelta]) -> ProtoDuration:
+def proto_duration_from_timedelta(t: Optional[datetime.timedelta]) -> Optional[ProtoDuration]:
     if t is None:
         return None
+
     res = ProtoDuration()
     res.FromTimedelta(t)
 
 
-def proto_timestamp_from_datetime(t: Optional[datetime.datetime]) -> ProtoTimeStamp:
+def proto_timestamp_from_datetime(t: Optional[datetime.datetime]) -> Optional[ProtoTimeStamp]:
     if t is None:
         return None
 
     res = ProtoTimeStamp()
     res.FromDatetime(t)
```

### Comparing `ydb-3.2.2/ydb/_grpc/grpcwrapper/ydb_scheme.py` & `ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/grpcwrapper/ydb_topic.py` & `ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,25 +406,31 @@
                 res.topics_read_settings.append(settings.to_proto())
             return res
 
         @dataclass
         class TopicReadSettings(IToProto):
             path: str
             partition_ids: List[int] = field(default_factory=list)
-            max_lag_seconds: Union[datetime.timedelta, None] = None
-            read_from: Union[int, float, datetime.datetime, None] = None
+            max_lag: Optional[datetime.timedelta] = None
+            read_from: Optional[datetime.datetime] = None
 
             def to_proto(
                 self,
             ) -> ydb_topic_pb2.StreamReadMessage.InitRequest.TopicReadSettings:
                 res = ydb_topic_pb2.StreamReadMessage.InitRequest.TopicReadSettings()
                 res.path = self.path
                 res.partition_ids.extend(self.partition_ids)
-                if self.max_lag_seconds is not None:
-                    res.max_lag = proto_duration_from_timedelta(self.max_lag_seconds)
+                max_lag = proto_duration_from_timedelta(self.max_lag)
+                if max_lag is not None:
+                    res.max_lag = max_lag
+
+                read_from = proto_timestamp_from_datetime(self.read_from)
+                if read_from is not None:
+                    res.read_from = read_from
+
                 return res
 
     @dataclass
     class InitResponse(IFromProto):
         session_id: str
 
         @staticmethod
```

### Comparing `ydb-3.2.2/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py` & `ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/grpcwrapper/ydb_topic_test.py` & `ydb-3.3.0/ydb/_grpc/grpcwrapper/ydb_topic_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/annotations/validation_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_auth_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_cms_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_common_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_coordination_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_discovery_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_export_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_formats_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_import_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_operation_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_scheme_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_scripting_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_table_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_topic_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/protos/ydb_value_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_auth_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_cms_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_coordination_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_discovery_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_export_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_import_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_operation_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_scheme_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_scripting_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_table_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_topic_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/annotations/validation_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_auth_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_cms_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_common_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_coordination_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_discovery_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_export_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_formats_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_import_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_operation_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_scheme_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_scripting_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_table_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_topic_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/protos/ydb_value_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_auth_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_cms_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_coordination_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_discovery_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_export_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_import_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_operation_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_scheme_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_scripting_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_table_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_topic_v1_pb2.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.0/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_session_impl.py` & `ydb-3.3.0/ydb/_session_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_sp_impl.py` & `ydb-3.3.0/ydb/_sp_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -331,14 +331,18 @@
             # current status of the session
         except issues.Error:
             self._destroy(session, "keep-alive-error")
         except Exception:
             self._destroy(session, "keep-alive-error")
 
     def acquire(self, blocking=True, timeout=None):
+        if self._should_stop.is_set():
+            self._logger.error("Take session from closed session pool")
+            raise ValueError("Take session from closed session pool.")
+
         waiter = self.subscribe()
         has_result = False
         if blocking:
             tracing.trace(self.tracer, {"acquire.blocking": True})
             try:
                 tracing.trace(self.tracer, {"acquire.blocking.wait": True})
                 session = waiter.result(timeout=timeout)
```

### Comparing `ydb-3.2.2/ydb/_topic_common/common.py` & `ydb-3.3.0/ydb/_topic_common/common.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_common/common_test.py` & `ydb-3.3.0/ydb/_topic_common/common_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_common/test_helpers.py` & `ydb-3.3.0/ydb/_topic_common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_reader/datatypes.py` & `ydb-3.3.0/ydb/_topic_reader/datatypes.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_reader/datatypes_test.py` & `ydb-3.3.0/ydb/_topic_reader/datatypes_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_reader/topic_reader.py` & `ydb-3.3.0/ydb/_topic_reader/topic_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,45 +10,76 @@
     Callable,
 )
 
 from ..table import RetrySettings
 from .._grpc.grpcwrapper.ydb_topic import StreamReadMessage, OffsetsRange
 
 
-class Selector:
+@dataclass
+class PublicTopicSelector:
     path: str
-    partitions: Union[None, int, List[int]]
-    read_from_timestamp_ms: Optional[int]
-    max_time_lag_ms: Optional[int]
-
-    def __init__(self, path, *, partitions: Union[None, int, List[int]] = None):
-        self.path = path
-        self.partitions = partitions
+    partitions: Optional[Union[int, List[int]]] = None
+    read_from: Optional[datetime.datetime] = None
+    max_lag: Optional[datetime.timedelta] = None
+
+    def _to_topic_read_settings(self) -> StreamReadMessage.InitRequest.TopicReadSettings:
+        partitions = self.partitions
+        if partitions is None:
+            partitions = []
+
+        elif not isinstance(partitions, list):
+            partitions = [partitions]
+
+        return StreamReadMessage.InitRequest.TopicReadSettings(
+            path=self.path,
+            partition_ids=partitions,
+            max_lag=self.max_lag,
+            read_from=self.read_from,
+        )
+
+
+TopicSelectorTypes = Union[str, PublicTopicSelector, List[Union[str, PublicTopicSelector]]]
 
 
 @dataclass
 class PublicReaderSettings:
     consumer: str
-    topic: str
+    topic: TopicSelectorTypes
     buffer_size_bytes: int = 50 * 1024 * 1024
 
     decoders: Union[Mapping[int, Callable[[bytes], bytes]], None] = None
     """decoders: map[codec_code] func(encoded_bytes)->decoded_bytes"""
 
     # decoder_executor, must be set for handle non raw messages
     decoder_executor: Optional[concurrent.futures.Executor] = None
     update_token_interval: Union[int, float] = 3600
 
+    def __post_init__(self):
+        # check possible create init message
+        _ = self._init_message()
+
     def _init_message(self) -> StreamReadMessage.InitRequest:
+        if not isinstance(self.consumer, str):
+            raise TypeError("Unsupported type for customer field: '%s'" % type(self.consumer))
+
+        if isinstance(self.topic, list):
+            selectors = self.topic
+        else:
+            selectors = [self.topic]
+
+        for index, selector in enumerate(selectors):
+            if isinstance(selector, str):
+                selectors[index] = PublicTopicSelector(path=selector)
+            elif isinstance(selector, PublicTopicSelector):
+                pass
+            else:
+                raise TypeError("Unsupported type for topic field: '%s'" % type(selector))
+
         return StreamReadMessage.InitRequest(
-            topics_read_settings=[
-                StreamReadMessage.InitRequest.TopicReadSettings(
-                    path=self.topic,
-                )
-            ],
+            topics_read_settings=list(map(PublicTopicSelector._to_topic_read_settings, selectors)),  # type: ignore
             consumer=self.consumer,
         )
 
     def _retry_settings(self) -> RetrySettings:
         return RetrySettings(idempotent=True)
```

### Comparing `ydb-3.2.2/ydb/_topic_reader/topic_reader_asyncio.py` & `ydb-3.3.0/ydb/_topic_reader/topic_reader_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         attempt = 0
         while True:
             try:
                 self._stream_reader = await ReaderStream.create(self._id, self._driver, self._settings)
                 attempt = 0
                 self._state_changed.set()
                 await self._stream_reader.wait_error()
-            except issues.Error as err:
+            except BaseException as err:
                 retry_info = check_retriable_error(err, self._settings._retry_settings(), attempt)
                 if not retry_info.is_retriable:
                     self._set_first_error(err)
                     return
                 await asyncio.sleep(retry_info.sleep_timeout_seconds)
 
                 attempt += 1
```

### Comparing `ydb-3.2.2/ydb/_topic_reader/topic_reader_asyncio_test.py` & `ydb-3.3.0/ydb/_topic_reader/topic_reader_asyncio_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,15 +572,15 @@
         reader = ReaderStream(self.default_reader_reconnector_id, default_reader_settings)
         init_message = StreamReadMessage.InitRequest(
             consumer="test-consumer",
             topics_read_settings=[
                 StreamReadMessage.InitRequest.TopicReadSettings(
                     path="/local/test-topic",
                     partition_ids=[],
-                    max_lag_seconds=None,
+                    max_lag=None,
                     read_from=None,
                 )
             ],
         )
         start_task = asyncio.create_task(reader._start(stream, init_message))
 
         sent_message = await wait_for_fast(stream.from_client.get())
@@ -1135,21 +1135,25 @@
 
         async def wait_error():
             raise test_error
 
         reader_stream_mock_with_error = mock.Mock(ReaderStream)
         reader_stream_mock_with_error.wait_error = mock.AsyncMock(side_effect=wait_error)
 
-        async def wait_messages():
+        async def wait_messages_with_error():
             raise test_error
 
-        reader_stream_mock_with_error.wait_messages = mock.AsyncMock(side_effect=wait_messages)
+        reader_stream_mock_with_error.wait_messages = mock.AsyncMock(side_effect=wait_messages_with_error)
+
+        async def wait_forever():
+            f = asyncio.Future()
+            await f
 
         reader_stream_with_messages = mock.Mock(ReaderStream)
-        reader_stream_with_messages.wait_error.return_value = asyncio.Future()
+        reader_stream_with_messages.wait_error = mock.AsyncMock(side_effect=wait_forever)
         reader_stream_with_messages.wait_messages.return_value = None
 
         stream_index = 0
 
         async def stream_create(
             reader_reconnector_id: int,
             driver: SupportedDriverType,
```

### Comparing `ydb-3.2.2/ydb/_topic_reader/topic_reader_sync.py` & `ydb-3.3.0/ydb/_topic_reader/topic_reader_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_writer/topic_writer.py` & `ydb-3.3.0/ydb/_topic_writer/topic_writer.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_writer/topic_writer_asyncio.py` & `ydb-3.3.0/ydb/_topic_writer/topic_writer_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,34 +362,33 @@
                 self._stream_connected.set()
 
                 send_loop = asyncio.create_task(self._send_loop(stream_writer), name="writer send loop")
                 receive_loop = asyncio.create_task(self._read_loop(stream_writer), name="writer receive loop")
 
                 tasks = [send_loop, receive_loop]
                 done, _ = await asyncio.wait([send_loop, receive_loop], return_when=asyncio.FIRST_COMPLETED)
-                await stream_writer.close()
-                done.pop().result()
+                done.pop().result()  # need for raise exception - reason of stop task
             except issues.Error as err:
                 err_info = check_retriable_error(err, retry_settings, attempt)
                 if not err_info.is_retriable:
                     self._stop(err)
                     return
 
                 await asyncio.sleep(err_info.sleep_timeout_seconds)
 
             except (asyncio.CancelledError, Exception) as err:
                 self._stop(err)
                 return
             finally:
-                if stream_writer:
-                    await stream_writer.close()
                 for task in tasks:
                     task.cancel()
                 if tasks:
                     await asyncio.wait(tasks)
+                if stream_writer:
+                    await stream_writer.close()
 
     async def _encode_loop(self):
         try:
             while True:
                 messages = await self._messages_for_encode.get()
                 while not self._messages_for_encode.empty():
                     messages.extend(self._messages_for_encode.get_nowait())
```

### Comparing `ydb-3.2.2/ydb/_topic_writer/topic_writer_asyncio_test.py` & `ydb-3.3.0/ydb/_topic_writer/topic_writer_asyncio_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_writer/topic_writer_sync.py` & `ydb-3.3.0/ydb/_topic_writer/topic_writer_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_topic_writer/topic_writer_test.py` & `ydb-3.3.0/ydb/_topic_writer/topic_writer_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/_tx_ctx_impl.py` & `ydb-3.3.0/ydb/_tx_ctx_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,11 +155,9 @@
 @reset_tx_id_handler
 @not_found_handler
 def wrap_result_and_tx_id(rpc_state, response_pb, session_state, tx_state, query):
     session_state.complete_query()
     issues._process_response(response_pb.operation)
     message = _apis.ydb_table.ExecuteQueryResult()
     response_pb.operation.result.Unpack(message)
-    if message.query_meta.id:
-        session_state.keep(query, message.query_meta.id)
     tx_state.tx_id = None if not message.tx_meta.id else message.tx_meta.id
     return convert.ResultSets(message.result_sets, session_state.table_client_settings)
```

### Comparing `ydb-3.2.2/ydb/_utilities.py` & `ydb-3.3.0/ydb/_utilities.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/aio/connection.py` & `ydb-3.3.0/ydb/aio/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/aio/credentials.py` & `ydb-3.3.0/ydb/aio/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/aio/driver.py` & `ydb-3.3.0/ydb/aio/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/aio/iam.py` & `ydb-3.3.0/ydb/aio/iam.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/aio/pool.py` & `ydb-3.3.0/ydb/aio/pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/aio/resolver.py` & `ydb-3.3.0/ydb/aio/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/aio/scheme.py` & `ydb-3.3.0/ydb/aio/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/aio/table.py` & `ydb-3.3.0/ydb/aio/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,16 +337,16 @@
             return self._create()
         _, session = task_wait.result()
         return session
 
     async def acquire(self, timeout: float = None, retry_timeout: float = None, retry_num: int = None) -> ydb.ISession:
 
         if self._should_stop.is_set():
-            self._logger.debug("Acquired not inited session")
-            return self._create()
+            self._logger.error("Take session from closed session pool")
+            raise ValueError("Take session from closed session pool.")
 
         if retry_timeout is None:
             retry_timeout = timeout
 
         try:
             _, session = self._active_queue.get_nowait()
             self._logger.debug("Acquired active session from queue: %s", session.session_id)
```

### Comparing `ydb-3.2.2/ydb/connection.py` & `ydb-3.3.0/ydb/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/convert.py` & `ydb-3.3.0/ydb/convert.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/credentials.py` & `ydb-3.3.0/ydb/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/dbapi/__init__.py` & `ydb-3.3.0/ydb/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/dbapi/connection.py` & `ydb-3.3.0/ydb/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/dbapi/cursor.py` & `ydb-3.3.0/ydb/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/dbapi/errors.py` & `ydb-3.3.0/ydb/dbapi/errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/default_pem.py` & `ydb-3.3.0/ydb/default_pem.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/driver.py` & `ydb-3.3.0/ydb/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/export.py` & `ydb-3.3.0/ydb/export.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/global_settings.py` & `ydb-3.3.0/ydb/global_settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/iam/auth.py` & `ydb-3.3.0/ydb/iam/auth.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/import_client.py` & `ydb-3.3.0/ydb/import_client.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/interceptor.py` & `ydb-3.3.0/ydb/interceptor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/issues.py` & `ydb-3.3.0/ydb/issues.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/operation.py` & `ydb-3.3.0/ydb/operation.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/pool.py` & `ydb-3.3.0/ydb/pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/resolver.py` & `ydb-3.3.0/ydb/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/scheme.py` & `ydb-3.3.0/ydb/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/scheme_test.py` & `ydb-3.3.0/ydb/scheme_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/scripting.py` & `ydb-3.3.0/ydb/scripting.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/settings.py` & `ydb-3.3.0/ydb/settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/sqlalchemy/__init__.py` & `ydb-3.3.0/ydb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/sqlalchemy/types.py` & `ydb-3.3.0/ydb/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/table.py` & `ydb-3.3.0/ydb/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/table_test.py` & `ydb-3.3.0/ydb/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/topic.py` & `ydb-3.3.0/ydb/topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,21 @@
     "TopicCodec",
     "TopicConsumer",
     "TopicDescription",
     "TopicError",
     "TopicMeteringMode",
     "TopicReader",
     "TopicReaderAsyncIO",
+    "TopicReaderSelector",
     "TopicReaderSettings",
     "TopicStatWindow",
+    "TopicWriteResult",
     "TopicWriter",
     "TopicWriterAsyncIO",
+    "TopicWriterInitInfo",
     "TopicWriterMessage",
     "TopicWriterSettings",
 ]
 
 import concurrent.futures
 import datetime
 from dataclasses import dataclass
@@ -26,26 +29,29 @@
 
 from . import aio, Credentials, _apis, issues
 
 from . import driver
 
 from ._topic_reader.topic_reader import (
     PublicReaderSettings as TopicReaderSettings,
+    PublicTopicSelector as TopicReaderSelector,
 )
 
 from ._topic_reader.topic_reader_sync import TopicReaderSync as TopicReader
 
 from ._topic_reader.topic_reader_asyncio import (
     PublicAsyncIOReader as TopicReaderAsyncIO,
 )
 
 from ._topic_writer.topic_writer import (  # noqa: F401
     PublicWriterSettings as TopicWriterSettings,
     PublicMessage as TopicWriterMessage,
     RetryPolicy as TopicWriterRetryPolicy,
+    PublicWriterInitInfo as TopicWriterInitInfo,
+    PublicWriteResult as TopicWriteResult,
 )
 
 from ydb._topic_writer.topic_writer_asyncio import WriterAsyncIO as TopicWriterAsyncIO
 from ._topic_writer.topic_writer_sync import WriterSync as TopicWriter
 
 from ._topic_common.common import (
     wrap_operation as _wrap_operation,
@@ -147,15 +153,15 @@
             _apis.TopicService.Stub,
             _apis.TopicService.DropTopic,
             _wrap_operation,
         )
 
     def reader(
         self,
-        topic: str,
+        topic: Union[str, TopicReaderSelector, List[Union[str, TopicReaderSelector]]],
         consumer: str,
         buffer_size_bytes: int = 50 * 1024 * 1024,
         # decoders: map[codec_code] func(encoded_bytes)->decoded_bytes
         decoders: Union[Mapping[int, Callable[[bytes], bytes]], None] = None,
         decoder_executor: Optional[concurrent.futures.Executor] = None,  # default shared client executor pool
     ) -> TopicReaderAsyncIO:
 
@@ -296,15 +302,15 @@
             _apis.TopicService.Stub,
             _apis.TopicService.DropTopic,
             _wrap_operation,
         )
 
     def reader(
         self,
-        topic: str,
+        topic: Union[str, TopicReaderSelector, List[Union[str, TopicReaderSelector]]],
         consumer: str,
         buffer_size_bytes: int = 50 * 1024 * 1024,
         # decoders: map[codec_code] func(encoded_bytes)->decoded_bytes
         decoders: Union[Mapping[int, Callable[[bytes], bytes]], None] = None,
         decoder_executor: Optional[concurrent.futures.Executor] = None,  # default shared client executor pool
     ) -> TopicReader:
         if not decoder_executor:
```

### Comparing `ydb-3.2.2/ydb/tracing.py` & `ydb-3.3.0/ydb/tracing.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb/types.py` & `ydb-3.3.0/ydb/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.2.2/ydb.egg-info/PKG-INFO` & `ydb-3.3.0/ydb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.2.2
+Version: 3.3.0
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.2.2/ydb.egg-info/SOURCES.txt` & `ydb-3.3.0/ydb.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
+./tests/__init__.py
+./tests/conftest.py
+./tests/session_pool.py
+./tests/test_errors.py
+./tests/aio/__init__.py
+./tests/aio/test_async_iter_stream.py
+./tests/aio/test_connection.py
+./tests/aio/test_connection_pool.py
+./tests/aio/test_session_pool.py
+./tests/aio/test_table.py
+./tests/aio/test_tx.py
+./tests/aio/test_types.py
+./tests/ssl/__init__.py
+./tests/ssl/test_ssl.py
+./tests/table/__init__.py
+./tests/table/table_test.py
+./tests/table/test_tx.py
+./tests/topics/__init__.py
+./tests/topics/test_control_plane.py
+./tests/topics/test_topic_reader.py
+./tests/topics/test_topic_writer.py
 ./ydb/__init__.py
 ./ydb/_apis.py
 ./ydb/_errors.py
 ./ydb/_session_impl.py
 ./ydb/_sp_impl.py
 ./ydb/_tx_ctx_impl.py
 ./ydb/_utilities.py
```

